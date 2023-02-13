---
content-type: api
navigation-topic: api-navigation-topic
title: 事件訂閱憑證
description: 事件訂閱憑證
author: Becky
feature: Workfront API
source-git-commit: 53ef8f4fda22c912c274841d07ad865aa04141c8
workflow-type: tm+mt
source-wordcount: '330'
ht-degree: 0%

---

# 為事件訂閱配置客戶端TLS

<!--Configuring Client TLS for Event Subscription
Steps to Verify Workfront's Client Certificate
Examples for Server configuration
NGINX
Apache
Certificate to Environment Mapping
Certificates
Production
Preview
Sandbox 1
Sandbox 2
-->

用戶端TLS可讓您驗證您收到的事件訂閱訊息是否實際來自Adobe Workfront。 若要啟用此功能，您的伺服器必須設定為要求及驗證Workfront的x509憑證。


## 驗證Workfront的用戶端憑證

此過程假設您的伺服器已配置為接受TLS連接。 Workfront不支援自行簽署的憑證。

一般而言，開啟伺服器的用戶端驗證所需的步驟如下：

1. 下載DigiCert全域根CA憑證的PEM版本。
1. 開啟客戶端證書驗證。

   將步驟1的CA憑證指定為受信任。

1. 將驗證深度設為2，因為我們的憑證實際上是由DigiCert SHA2 Secure Server CA簽署，該CA是DigiCert Global Root CA下的中間CA。
1. 檢查其主旨網域名稱，以確認用戶端憑證是否實際來自Workfront。

## 伺服器配置範例

### NGINX

```
server {

    listen 443 ssl default_server;
    # ... existing SSL configuration for server authentication ...

    ssl_verify_client on;
    ssl_client_certificate /path/to/DigiCert_Global_Root_CA.pem;
    ssl_verify_depth 2;

        # ... existing location configuration ...
    }
}
```

如需詳細資訊，請參閱 [ngx_http_ssl_module的NGiNX文檔](http://nginx.org/en/docs/http/ngx_http_ssl_module.html).

### Apache

```
Listen 443
<VirtualHost *:443>
    # ... existing SSL configuration for server authentication ...

    SSLVerifyClient require
    SSLCACertificateFile "/path/to/DigiCert_Global_Root_CA.pem"
    SSLVerifyDepth 2
</VirtualHost>

<Directory /var/www/>
    Require expr "%{SSL_CLIENT_S_DN_CN} == <>"

    # ... existing directory configuration ...
</Directory>
```

如需詳細資訊，請參閱

* [客戶端驗證和訪問控制](https://httpd.apache.org/docs/2.4/ssl/ssl_howto.html#accesscontrol)
* [Apache模組mod_ssl](https://httpd.apache.org/docs/2.4/mod/mod_ssl.html)
 

## 憑證與環境的對應

| WF環境 |證書公用名 |證書主體(DN) | | — | — | — | |生產 | *.prod.eventsubscriptions.workfront.com | subject= /C=US/ST=Utah/L=Lehi/O=Workfront, Inc./CN=*.prod.eventsubscriptions.workfront.com| |預覽 | *.preview.eventsubscriptions.workfront.com | subject= /C=US/ST=Utah/L=Lehi/O=Workfront, Inc./CN=*.preview.eventsubscriptions.workfront.com | |沙箱1 | *.sandbox.eventsubscriptions.workfront.com | subject= /C=US/ST=Utah/L=Lehi/O=Workfront, Inc./CN=*.sandbox.eventsubscriptions.workfront.com | |沙箱2 | *.sandbox.eventsubscriptions.workfront.com | subject= /C=US/ST=Utah/L=Lehi/O=Workfront, Inc./CN=*.sandbox.eventsubscriptions.workfront.com |

## 下載憑證

按一下以下連結以下載用戶端憑證。

* [用戶端憑證 — 生產環境](https://cdn.experience.workfront.com/Documentation/Event+Subscriptions/event_subscription_dec_2022_production.crt)
* [客戶端證書 — 預覽環境](https://cdn.experience.workfront.com/Documentation/Event+Subscriptions/event_subscription_dec_2022_preview.crt)
* [用戶端憑證 — 沙箱環境](https://cdn.experience.workfront.com/Documentation/Event+Subscriptions/event_subscription_dec_2022_sandboxes.crt)

>[!NOTE]
>
>您可以對兩個沙箱環境使用相同的用戶端憑證。

