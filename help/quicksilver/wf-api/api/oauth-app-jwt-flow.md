---
content-type: api
navigation-topic: api-navigation-topic
title: 將JWT流程用於自訂OAuth 2應用程式
description: 將JWT流程用於自訂OAuth 2應用程式
author: Becky
feature: Workfront API
exl-id: 4bd56fe6-1f36-4c36-82cd-96de748ad680
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '477'
ht-degree: 0%

---

# 使用JWT流程設定及使用貴組織的自訂OAuth 2應用程式

若要與Workfront整合，並允許您的用戶端應用程式代表使用者與Workfront通訊，您必須：

* 建立OAuth2應用程式
* 建立公開金鑰憑證
* 建立JSON網頁代號(JWT)

## 建立OAuth2應用程式

如需建立OAuth2應用程式的指示，請參閱 [使用伺服器驗證（JWT流程）建立OAuth2應用程式](../../administration-and-setup/configure-integrations/create-oauth-application.md#create2) in [建立OAuth2應用程式以進行Workfront整合](../../administration-and-setup/configure-integrations/create-oauth-application.md)

## 建立公開金鑰憑證

JWT必須經過簽署，並以64為底編碼，才能納入存取要求中。 JWT程式庫提供執行這些工作的功能。

代號必須使用數位簽署憑證的私密金鑰簽署。 若您這麼做，您可以使用任何相關憑證的私密金鑰來簽署JWT。

採用的算法是RS256（RSA簽名與SHA-256）。 這是非對稱演算法，使用公開/私密金鑰組。 身分提供者有一個用來產生簽名的私密（秘密）金鑰，而JWT的使用者取得一個公開金鑰來驗證簽名。

若要產生公開金鑰，請執行 **one** 下列項目。

* 開啟您的MacOS/Linux終端機並執行下列命令，然後上傳 `certificate_pub.crt` 使用 **新增公開金鑰** 按鈕(在Workfront中設定OAuth2應用程式)。

   <!-- [Copy](javascript:void(0);) -->
   <pre><code>openssl req -x509 -sha256 -nodes -newkey rsa:2048 -keyout private.key -out certificate_pub.crt</code></pre>

* 使用 **產生公開/私用金鑰組** 按鈕(在Workfront中設定OAuth2應用程式以產生RSA)。

## 建立JSON網頁代號

服務帳戶驗證的JSON Web Token需要一組特定聲明，且必須使用有效的數位簽署憑證簽署。 建議您使用其中一個公開可用的程式庫或工具來建置JWT。

下表包含設定JWT代號時可能需要之欄位的相關資訊。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">exp</td> 
   <td> <p>必要. 有效期參數是測量自GMT時間以來絕對時間的必要參數01/01/1970。 您必須確保過期時間晚於問題時間。 此後，JWT便不再有效。 </p> <p>注意：建議您使用非常短的Token（幾分鐘），這樣它就會在以存取Token交換後很快過期。 每次需要新的存取權杖時，都會簽署和交換一個JWT。 這是更安全的方法。 我們建議不要視需要重複使用來取得存取權杖的使用時間延長。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">is</td> 
   <td>必要. 核發者是您來自OAuth2應用程式詳細資訊的客戶ID。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">sub</td> 
   <td>必要. 主旨是您在設定中建立公開金鑰的使用者ID。</td> 
  </tr> 
 </tbody> 
</table>

## 交換JWT以擷取存取權杖

1. 傳送POST要求至：

   <!-- [Copy](javascript:void(0);) -->
   <pre><code>https://yourdomain.my.workfront.com/integrations/oauth2/api/v1/jwt/exchange</code></pre>

1. 要求內文應包含URL編碼參數，以及您的用戶端ID、用戶端密碼和JWT:

   <!-- [Copy](javascript:void(0);) -->
   <pre><code>client_id={client_id_value}&client_secret={client_secret_value}&jwt_token={base64_encoded_JWT}</code></pre>

 
