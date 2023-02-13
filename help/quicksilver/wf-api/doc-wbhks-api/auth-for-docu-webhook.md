---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: 文檔Webhook的驗證
description: 文檔Webhook的驗證
author: John
feature: Workfront API
exl-id: 2303c202-27c7-4922-a613-e9824910504c
source-git-commit: a849ecaf6097dcdc924aaab2867f37bf57d5bc09
workflow-type: tm+mt
source-wordcount: '438'
ht-degree: 0%

---

# 文檔Webhook的驗證

## 驗證

Adobe Workfront document webhook支援兩種不同的驗證形式：OAuth2和ApiKey。 在這兩種情況下，Workfront會在進行API呼叫時，在標題中傳遞驗證Token。

### OAuth2

OAuth2可讓Workfront代表使用者向網頁連結提供者發出授權API呼叫。 在執行此動作之前，使用者必須將其外部檔案提供者帳戶連線至Workfront，並授與Workfront

有權代表他們採取行動。 此握手過程僅對每個用戶進行一次。 其運作方式如下：

1. 使用者開始將Webhook整合連線至其帳戶。 目前，您可以按一下「新增檔案」下拉式清單>「新增服務」>「自訂整合名稱」來完成此作業。
1. Workfront會導覽使用者驗證URL，這可能會提示使用者登入外部檔案提供者。 此頁由Webhook提供程式或外部文檔管理系統托管。 這麼做時，Workfront會將「state」參數新增至驗證URL。 您必須在下列步驟中，將相同的值附加至Workfront傳回URI，以將此值傳回Workfront。
1. 登入外部系統後（或如果使用者已登入），會將使用者帶入「驗證」頁面，說明Workfront正在代表使用者要求存取以執行一組動作。
1. 如果使用者按一下「允許」按鈕，瀏覽器會重新導向至Workfront重新導向URI ，並新增「code=`<code>`&quot;到查詢字串。 根據OAuth2規格，此代號是短期的。 查詢字串也必須具備下列項目： &quot;state=`<sent_by_workfront>`」。
1. Workfront會處理此要求，並使用授權程式碼對Token端點URL進行API呼叫。
1. Token端點URL會傳回重新整理Token和存取Token。
1. Workfront會儲存這些代號，並為此使用者完全布建webhook整合。
1. 此後，Workfront將能夠向Webhook提供者發出授權API呼叫。 進行這些呼叫時，Workfront會在HTTP要求標題中傳送存取權杖，如下所示：

   ```
   -------------------------------  
   Authorization: Bearer [access_token] ­­­­­­­­­­­­­­­­­­­­­­­­­­  
   -------------------------------
   ```

1. 如果存取權杖已過期，Workfront會呼叫權杖端點URL以擷取新的存取權杖，然後使用新的存取權杖再次嘗試授權API呼叫。

### ApiKey

使用ApiKey向網頁連結提供者發出授權API呼叫比OAuth2簡單得多。 發出API呼叫時，Workfront只會在HTTP要求標題中傳遞ApiKey和Workfront使用者名稱： 

```
-------------------------------

apiKey: 12345

username: johndoe@foo.com

-------------------------------
```

Webhook提供者可使用使用者名稱來套用使用者專屬權限。 當兩個系統都使用單一登入(SSO)連接到LDAP時，這種方法效果最佳。

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h3>Adding Request Headers (optional)</h3>
<p>In addition to using either OAuth2 tokens or an ApiKey for authentication, Workfront can send a predefined set of headers to the webhook provider for every API call. A Workfront admin can setup set this up when&nbsp;registering or editing a Webook Integration, as described in the section above. See Registering a Webhook Integration.</p>
<p>For example, this can be used for Basic Authentication. To do this, the Workfront administrator would add the following Request Header information in the Custom Integration dialog:</p>
<p>&nbsp; &nbsp; &nbsp;Authorization Basic QWxhZGRpbjpvcGVuIHNlc2FtZQ==</p>
<p>where QWxhZGRpbjpvcGVuIHNlc2FtZQ== is a base-64 encoded string of “username:password”. See Basic Authentication . Provided that this added, Workfront will pass this in the HTTP request header, in addition to other request headers:&nbsp;</p>
<p>-------------------------------</p>
<p>apiKey: 12345</p>
<p>username: johndoe@foo.com</p>
<p>Authorization: Basic QWxhZGRpbjpvcGVuIHNlc2FtZQ== ­­­­­­­­­­­­­­­­­­­­­­­­­­</p>
<p>-------------------------------</p>
</div>
-->
