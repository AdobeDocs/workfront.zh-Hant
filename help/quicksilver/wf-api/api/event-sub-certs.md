---
content-type: api
navigation-topic: api-navigation-topic
title: 事件訂閱憑證
description: 事件訂閱憑證
author: Becky
feature: Workfront API
role: Developer
exl-id: 3606b6c3-b373-47ea-9cb5-813bd3af8da7
source-git-commit: 0921cc0e45a0a845404df90fc8789efc764f5790
workflow-type: tm+mt
source-wordcount: '320'
ht-degree: 3%

---

# 設定事件訂閱的使用者端TLS

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

使用者端TLS可讓您驗證您收到的事件訂閱訊息是否實際來自Adobe Workfront。 若要啟用此功能，您的伺服器必須設定為請求及驗證Workfront的x509憑證。


>[!NOTE]
>
>如果事件訂閱將事件傳送至的伺服器支援1.3版，則事件訂閱會使用TLS 1.3版。如果連線的伺服器不支援1.3版，則事件訂閱會使用TLS 1.2版。



## 驗證Workfront的使用者端憑證

此程式假設您的伺服器已設定為接受TLS連線。 Workfront不支援自我簽署憑證。

一般而言，開啟伺服器使用者端驗證所需的步驟如下：

1. 下載DigiCert全域根CA憑證的PEM版本。
1. 開啟使用者端憑證驗證。

   將步驟1中的CA憑證指定為受信任。

1. 將驗證深度設定為2，因為我們的憑證實際是由DigiCert SHA2 Secure Server CA簽署，而此CA是DigiCert全域根CA下的中間CA。
1. 透過檢查其主體網域名稱來驗證使用者端憑證是否確實來自Workfront。

## 伺服器設定範例

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

如需詳細資訊，請參閱ngx_http_ssl_module[的](https://nginx.org/en/docs/http/ngx_http_ssl_module.html)NGiNX檔案。

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

* [使用者端驗證與存取控制](https://httpd.apache.org/docs/2.4/ssl/ssl_howto.html#accesscontrol)
* [Apache模組mod_ssl](https://httpd.apache.org/docs/2.4/mod/mod_ssl.html)
 

## 憑證與環境對應

| WF環境 | 憑證一般名稱 | 憑證主體(DN) |
| -- | -- | -- |
| 生產 | *.prod.eventsubscriptions.workfront.com | subject= /C=US/ST=Utah/L=Lehi/O=Workfront， Inc./CN=*.prod.eventsubscriptions.workfront.com |
| 預覽 | *.preview.eventsubscriptions.workfront.com | subject= /C=US/ST=Utah/L=Lehi/O=Workfront， Inc./CN=*.preview.eventsubscriptions.workfront.com |
| 沙箱 1 | *.sandbox.eventsubscriptions.workfront.com | subject= /C=US/ST=Utah/L=Lehi/O=Workfront， Inc./CN=*.sandbox.eventsubscriptions.workfront.com |
| 沙箱 2 | *.sandbox.eventsubscriptions.workfront.com | subject= /C=US/ST=Utah/L=Lehi/O=Workfront， Inc./CN=*.sandbox.eventsubscriptions.workfront.com |

## 下載憑證

按一下下列連結以下載使用者端憑證。

* [使用者端憑證 — 生產環境](assets/prod-ES-client-cert-oct25.crt)
* [使用者端憑證 — 預覽環境](assets/preview-ES-client-cert-oct25.crt)
* [使用者端憑證 — 沙箱環境](assets/sandbox-ES-client-cert-oct25.crt)

>[!NOTE]
>
>您可以對兩個沙箱環境使用相同的使用者端憑證。
