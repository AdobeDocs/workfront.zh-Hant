---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: 檔案Webhook的驗證
description: 檔案Webhook的驗證
author: Becky
feature: Workfront API
role: Developer
exl-id: 2303c202-27c7-4922-a613-e9824910504c
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '438'
ht-degree: 0%

---

# 檔案Webhook的驗證

## 驗證

Adobe Workfront檔案webhook支援兩種不同的驗證形式： OAuth2和ApiKey。 在這兩種情況下，Workfront都會在進行API呼叫時在標題中傳遞驗證權杖。

### OAuth2

OAuth2可讓Workfront代表使用者向webhook提供者發出授權的API呼叫。 在執行此操作之前，使用者必須將其外部檔案提供者帳戶連線至Workfront並授予Workfront

代表他們行事的存取權。 此握手程式只會針對每位使用者進行一次。 以下是運作方式：

1. 使用者開始將webhook整合連線至其帳戶。 目前，若要這麼做，請按一下「新增檔案」下拉式清單>「新增服務」>自訂整合名稱。
1. Workfront會導覽使用者驗證URL，這可能會提示使用者登入外部檔案提供者。 此頁面由webhook提供者或外部檔案管理系統託管。 Workfront這麼做時，會將「state」引數新增至驗證URL。 必須在下列步驟中，將相同的值附加至Workfront傳回URI，將此值傳回Workfront。
1. 登入外部系統後（或如果使用者已登入），使用者將被帶到「驗證」頁面，此頁面說明Workfront正在請求存取權，以代表使用者執行一組動作。
1. 如果使用者按一下「允許」按鈕，瀏覽器會重新導向至Workfront重新導向URI ，並將「code=`<code>`」新增至querystring。 根據OAuth2規格，此代號只會短暫有效。 查詢字串也必須具有下列「state=`<sent_by_workfront>`」。
1. Workfront處理此要求，並使用授權代碼對權杖端點URL進行API呼叫。
1. 權杖端點URL會傳回重新整理權杖和存取權杖。
1. Workfront會儲存這些Token並完整布建此使用者的webhook整合。
1. 從現在開始，Workfront將能夠向webhook提供者發出授權的API呼叫。 進行這些呼叫時，Workfront會在HTTP請求標頭中傳送存取權杖，如下所示：

   ```
   -------------------------------  
   Authorization: Bearer [access_token] ­­­­­­­­­­­­­­­­­­­­­­­­­­  
   -------------------------------
   ```

1. 如果存取權杖已過期，Workfront會呼叫權杖端點URL以擷取新的存取權杖，然後使用新的存取權杖再次嘗試授權API呼叫。

### ApiKey

使用ApiKey向webhook提供者發出授權API呼叫比OAuth2簡單得多。 進行API呼叫時，Workfront只會在HTTP請求標頭中傳遞ApiKey和Workfront使用者名稱： 

```
-------------------------------

apiKey: 12345

username: johndoe@foo.com

-------------------------------
```

Webhook提供者可以使用使用者名稱來套用使用者特定的許可權。 當兩個系統都使用單一登入(SSO)連線到LDAP時，這個方法會發揮最佳效果。

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h3>Adding Request Headers (optional)</h3>
<p>In addition to using either OAuth2 tokens or an ApiKey for authentication, Workfront can send a predefined set of headers to the webhook provider for every API call. A Workfront admin can setup set this up when&nbsp;registering or editing a Webook Integration, as described in the section above. See Registering a Webhook Integration.</p>
<p>For example, this can be used for Basic Authentication. To do this, the Workfront administrator would add the following Request Header information in the Custom Integration dialog:</p>
<p>&nbsp; &nbsp; &nbsp;Authorization Basic QWxhZGRpbjpvcGVuIHNlc2FtZQ==</p>
<p>where QWxhZGRpbjpvcGVuIHNlc2FtZQ== is a base-64 encoded string of "username:password". See Basic Authentication . Provided that this added, Workfront will pass this in the HTTP request header, in addition to other request headers:&nbsp;</p>
<p>-------------------------------</p>
<p>apiKey: 12345</p>
<p>username: johndoe@foo.com</p>
<p>Authorization: Basic QWxhZGRpbjpvcGVuIHNlc2FtZQ== ­­­­­­­­­­­­­­­­­­­­­­­­­­</p>
<p>-------------------------------</p>
</div>
-->
