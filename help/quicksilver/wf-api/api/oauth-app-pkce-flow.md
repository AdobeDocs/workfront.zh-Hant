---
content-type: api
navigation-topic: api-navigation-topic
title: 針對OAuth 2應用程式使用PKCE流程
description: 針對OAuth 2應用程式使用PKCE流程
author: Becky
feature: Workfront API
exl-id: 61fe77b6-c6d7-4f23-bfb6-617bccaa1989
source-git-commit: 5480d6b5e97c4c2e21080bb92ffe255f60ed6f60
workflow-type: tm+mt
source-wordcount: '792'
ht-degree: 0%

---

# 使用PKCE流程設定和使用您組織的自訂OAuth 2應用程式

PKCE是安全的授權流程，適用於動態重新整理應用程式，例如行動應用程式，但在所有OAuth2使用者端都很有價值。 PKCE不使用靜態使用者端密碼，而是使用動態產生的字串，消除了使用者端密碼洩露的風險。

## PKCE概述

PKCE流程包含下列步驟。 本節中的步驟僅供參考。 若要執行這些程式，請參閱本文的其他章節。

1. 使用者端建立 `code_challenge` 透過轉換 `code_verifier` 使用 `S256` 加密。

1. 使用者端將瀏覽器導向OAuth2登入頁面，同時顯示產生的 `code_challenge`. 您必須註冊應用程式（使用者端），讓OAuth2可以接受授權請求。 註冊後，您的應用程式可將瀏覽器重新導向至OAuth2。

1. OAuth2授權伺服器會將驗證提示重新導向給使用者。

1. 使用者使用其中一個設定的登入選項進行驗證，並且可能會看到一個同意頁面，其中列出OAuth2將授予應用程式的許可權。

1. OAuth2會重新導向回您的應用程式，並 `authorization code`.

1. 您的應用程式會傳送此程式碼以及 `code_verifier`，重新命名為OAuth2。

1. OAuth2授權伺服器轉換 `code_verifier` 使用 `code_challenge_method` 從初始授權請求，並檢查結果是否符合 `code_challenge`. 如果兩個字串的值相符，則伺服器已驗證請求是否來自相同使用者端，並將發出 `access token`.

1. OAuth2傳回 `access token`，並可選擇使用 `refresh token`.

1. 您的應用程式現在可以使用這些Token來代表使用者呼叫資源伺服器（例如API）。

1. 資源伺服器會在回應要求之前驗證權杖。


## 設定您的應用程式

您必須先從Workfront建立應用程式整合，以便在OAuth2中註冊應用程式，才能實作授權。

如需建立OAuth2應用程式的指示，請參閱 [使用PKCE建立OAuth2單頁網頁應用程式](../../administration-and-setup/configure-integrations/create-oauth-application.md#create-an-oauth2-single-page-web-application-using-pkce) 在 [為Workfront整合建立OAuth2應用程式](../../administration-and-setup/configure-integrations/create-oauth-application.md)


## 建立用於程式碼交換的校訂金鑰

與標準的授權代碼流程類似，您的應用程式一開始會將使用者的瀏覽器重新導向至您的授權伺服器的 `/authorize` 端點。 不過，在此情況下，您也必須傳送程式碼挑戰。

您的第一步是產生程式碼驗證器和質詢。

<table>
  <col/>
  <col/>
    <tbody>
      <tr>
        <td role="rowheader">程式碼驗證器</td>
        <td>
          <p>最小長度為43個字元的隨機URL安全字串</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">程式碼挑戰</td>
        <td>
          <p>程式碼驗證器的Base64 URL編碼SHA-256雜湊</p>
        </td>
      </tr>
    </tbody>
</table>


您必須在使用者端應用程式中新增程式碼，以建立程式碼驗證器和程式碼挑戰。

PKCE產生器程式碼會建立類似下列的輸出：

>[!INFO]
>
>**範例:**
>
>```
>{
>  "code\_verifier":"N28zVMsKU6ptUjHaYWg3T1NFTDQqcW1R4BU5NXywapNac4hhfkxjwfhZQat",
>  "code\_challenge":"wzgjYF9qEiWep-CwqgrTE78-2ghjwCtRO3vj23o4W\_fw"
>}
>```

您的應用程式會儲存 `code_verifier` 稍後，並傳送 `code_challenge` 連同對授權伺服器的授權要求 `/authorize` URL。

## 要求授權碼

如果您使用預設的自訂授權伺服器，則您的請求URL會類似於以下內容：

>[!INFO]
>
>**範例:**
>
>
>```
>/authorize?client\_id=<clientID>&response\_type=code&redirect\_uri=<redirectURL>
>&code\_challenge\_method=S256&code\_challenge=wzgjYF9qEiWep-CwqgrTE78-2ghjwCtRO3vj23o4W\_fw"
>```

請注意正在傳遞的引數：

* `client_id` 符合您在設定應用程式時在中建立的OAuth2應用程式的使用者端ID。

  如需指示，請參閱為Workfront整合建立OAuth2應用程式中的「使用PKCE建立OAuth2單頁網頁應用程式」。

* `response_type` 是 `code`，因為應用程式使用授權代碼授予型別。

* `redirect_uri` 是使用者代理程式所導向的回呼位置，以及 `code`. 這必須符合您在建立OAuth2應用程式時指定的其中一個重新導向URL。

* `code_challenge_method` 是用來產生問詢的雜湊方法，一律為 `S256` 適用於使用PKCE的Workfront Oauth2應用程式。

* `code_challenge` 是用於PKCE的程式碼挑戰。


## 交換代號的程式碼

若要交換存取權杖的授權碼，請將其傳遞至授權伺服器的 `/token` 端點以及 `code_verifier`.

>[!INFO]
>
>**範例:**
>
>```
>/token \\
>  --header 'accept: application/json' \\
>  --header 'cache-control: no-cache' \\
>  --header 'content-type: application/x-www-form-urlencoded' \\
>  --data 'grant\_type=authorization\_code&client\_id=<clientID>&redirect\_uri=<redirectURL>&code=<code>&code\_verifier=N28zVMsKU6ptUjHaYWg3T1NFTDQqcW1R4BU5NXywapNac4hhfkxjwfhZQat
>```

>[!IMPORTANT]
>
> 與一般的授權碼流程不同，此呼叫不需要具有使用者端ID和密碼的授權標頭。 這就是為什麼這個版本的授權碼流程適用於沒有後端的原生應用程式，例如行動應用程式或單頁應用程式。

請注意正在傳遞的引數：

* `grant_type` 是 `authorization_code`，因為應用程式使用授權代碼授予型別。

* `redirect_uri` 必須符合用來取得授權碼的URI。

* `code` 是您從/authorize端點收到的授權代碼。

* `code_verifier` 是您的應用程式在中產生的PKCE程式碼驗證器 [建立用於程式碼交換的校訂金鑰](#Create).

* `client_id` 會識別您的使用者端，且必須符合OAuth2中預先註冊的值。


如果程式碼仍然有效，且程式碼驗證器相符，則您的應用程式會收到存取權杖。

>[!INFO]
>
>**範例:**
>
>```
>{
>    "access\_token": "eyJhd\[...\]Yozv",
>    "expires\_in": 3600,
>    "token\_type": "Bearer"
>}
>```

## 驗證存取權杖

當您的應用程式傳遞具有存取權杖的請求時，資源伺服器需要驗證它。

您可以使用類似下列的API呼叫來驗證您的存取Token：

>[!INFO]
>
>**範例:**
>
>```
>/attask/api/<api version>/proj/search \\
>  --header 'sessionID: <access\_token>' \\
>```

## 請求重新整理權杖

若要請求重新整理Token，您可以對API進行POST呼叫，如下所示：

>[!INFO]
>
>**範例:**
>
>```
>/token \\
>  --header 'accept: application/json' \\
>  --header 'cache-control: no-cache' \\
>  --header 'content-type: application/x-www-form-urlencoded' \\
>  --data 'grant\_type=refresh\_token&client\_id=<clientID>&redirect\_uri=<redirectURL>&refresh\_token=<refresh\_token>
>```
