---
content-type: api
navigation-topic: api-navigation-topic
title: 為自訂OAuth 2應用程式使用JWT流程
description: 為自訂OAuth 2應用程式使用JWT流程
author: Becky
feature: Workfront API
role: Developer
exl-id: 4bd56fe6-1f36-4c36-82cd-96de748ad680
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '477'
ht-degree: 0%

---

# 使用JWT流程設定並使用您組織的自訂OAuth 2應用程式

為了與Workfront整合併允許您的使用者端應用程式代表使用者與Workfront通訊，您必須：

* 建立Oauth2應用程式
* 建立公開金鑰憑證
* 建立JSON Web權杖(JWT)

## 建立Oauth2應用程式

如需建立OAuth2應用程式的指示，請參閱 [使用伺服器驗證（JWT流程）建立OAuth2應用程式](../../administration-and-setup/configure-integrations/create-oauth-application.md#create2) 在 [為Workfront整合建立OAuth2應用程式](../../administration-and-setup/configure-integrations/create-oauth-application.md)

## 建立公開金鑰憑證

JWT必須經過簽署並以base-64編碼，才能納入存取請求中。 JWT程式庫會提供執行這些工作的功能。

必須使用數位簽署憑證的私密金鑰簽署權杖。 如果這樣做，您可以使用任何關聯憑證的私密金鑰來簽署您的JWT。

使用的演演算法為RS256 （使用SHA-256的RSA簽名）。 這是非對稱演演算法，且使用公開/私密金鑰組。 身分提供者擁有用來產生簽章的私人（秘密）金鑰，而JWT的消費者則取得用來驗證簽章的公開金鑰。

若要產生公開金鑰，請執行 **一** 下列專案中的。

* 開啟您的MacOS/Linux終端機，執行以下命令，然後上傳 `certificate_pub.crt` 使用 **新增公開金鑰** 按鈕(在Workfront中的OAuth2應用程式設定中)。

  <!-- [Copy](javascript:void(0);) -->
  <pre><code>openssl req -x509 -sha256 -nodes -newkey rsa:2048 -keyout private.key -out certificate_pub.crt</code></pre>

* 使用 **產生公用/私用金鑰組** 按鈕(在Workfront中的OAuth2應用程式設定中)來產生RSA。

## 建立JSON Web權杖

服務帳戶驗證的JSON Web權杖需要一組特定的宣告，且必須使用有效的數位簽署憑證簽署。 建議您使用其中一個公開可用的資料庫或工具來建置JWT。

下表包含設定JWT權杖時所需欄位的相關資訊。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">費用</td> 
   <td> <p>必要. 有效期引數是測量01/01/1970 GMT以來絕對時間的必要引數。 您必須確保到期時間晚於問題時間。 在此時間之後，JWT就不再有效。 </p> <p>注意：建議您使用時間非常短的權杖（幾分鐘），以便在交換存取權杖後不久過期。 每次需要新的存取權杖時，都會簽署和交換一個JWT。 這是更安全的方法。 我們不建議視需要重複使用可取得存取權杖的較長存留期權杖。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">iss</td> 
   <td>必要. 簽發者是您來自OAuth2應用程式詳細資料的客戶ID。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">sub</td> 
   <td>必要. 主旨是在設定中建立公開金鑰的使用者ID。</td> 
  </tr> 
 </tbody> 
</table>

## 交換JWT以擷取存取權杖

1. 傳送POST要求至：

   <!-- [Copy](javascript:void(0);) -->
   <pre><code>https://yourdomain.my.workfront.com/integrations/oauth2/api/v1/jwt/exchange</code></pre>

1. 請求內文應包含URL編碼的引數，以及您的使用者端ID、使用者端密碼和JWT：

   <!-- [Copy](javascript:void(0);) -->
   <pre><code>client_id={client_id_value}&client_secret={client_secret_value}&jwt_token={base64_encoded_JWT}</code></pre>

 
