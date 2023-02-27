---
content-type: api
navigation-topic: api-navigation-topic
title: 使用PKCE流處理OAuth 2應用程式
description: 使用PKCE流處理OAuth 2應用程式
author: Becky
feature: Workfront API
exl-id: 61fe77b6-c6d7-4f23-bfb6-617bccaa1989
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '792'
ht-degree: 0%

---

# 使用PKCE流配置和使用貴組織的自定義OAuth 2應用程式

PKCE是一種安全的授權流，它與動態刷新應用程式（如移動應用程式）的效能良好，但在所有OAuth2客戶端中都很有價值。 PKCE不使用靜態客戶端密碼，而是使用動態生成的字串，從而消除了洩露的客戶端密碼的風險。

## PKCE概述

PKCE流具有以下步驟。 本節中的步驟僅供參考。 若要執行這些程式，請參閱本文的其他章節。

1. 用戶端會建立 `code_challenge` 通過改變 `code_verifier` 使用 `S256` 加密。

1. 用戶端會將瀏覽器導向至OAuth2登入頁面，以及產生的 `code_challenge`. 您必須註冊應用程式（用戶端）,OAuth2才能接受授權要求。 註冊後，您的應用程式可將瀏覽器重新導向至OAuth2。

1. OAuth2授權伺服器會將驗證提示重新導向至使用者。

1. 使用者使用其中一個已設定的登入選項進行驗證，且可能會看到同意頁面，列出OAuth2將授予應用程式的權限。

1. OAuth2會透過 `authorization code`.

1. 您的應用程式會傳送此程式碼，以及 `code_verifier`，至OAuth2。

1. OAuth2授權伺服器轉換 `code_verifier` 使用 `code_challenge_method` 從初始授權請求，並根據 `code_challenge`. 如果兩個字串的值相符，則伺服器已驗證請求是否來自相同的用戶端，且會發出 `access token`.

1. OAuth2傳回 `access token`，以及（選） `refresh token`.

1. 您的應用程式現在可以使用這些代號來代表使用者呼叫資源伺服器，例如API。

1. 資源伺服器在回應請求前會先驗證Token。


## 設定您的應用程式

您必須先從Workfront建立應用程式整合，在OAuth2中註冊應用程式，才能實作授權。

如需建立OAuth2應用程式的指示，請參閱 [使用PKCE建立OAuth2單頁Web應用程式 ](../../administration-and-setup/configure-integrations/create-oauth-application.md#create-an-oauth2-single-page-web-application-using-pkce) in [建立OAuth2應用程式以進行Workfront整合](../../administration-and-setup/configure-integrations/create-oauth-application.md)


## 建立代碼交換的校樣金鑰

與標準授權程式碼流程類似，您的應用程式的啟動方式是將使用者的瀏覽器重新導向至授權伺服器的 `/authorize` 端點。 不過，在此例中，您也必須傳遞程式碼挑戰。

第一步是生成代碼驗證程式和質詢。

<table>
  <col/>
  <col/>
    <tbody>
      <tr>
        <td role="rowheader">代碼驗證器</td>
        <td>
          <p>最少長度為43個字元的隨機URL安全字串</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">程式碼挑戰</td>
        <td>
          <p>程式碼驗證器的SHA-256雜湊（Base64 URL編碼）</p>
        </td>
      </tr>
    </tbody>
</table>


您必須在用戶端應用程式中新增程式碼，才能建立程式碼驗證器和程式碼疑難排解。

PKCE生成器代碼建立的輸出類似於以下內容：

>[!INFO]
>
>**範例:**
>
>
```
>{
>
>
  "code\_verifier":"N28zVMsKU6ptUjHaYWg3T1NFTDQqcW1R4BU5NXywapNac4hhfkxjwfhZQat",
>
>
  "code\_challenge":"wzgjYF9qEiWep-CwqgrTE78-2ghjwCtRO3vj23o4W\_fw"
>
>
}
>```

您的應用程式會儲存 `code_verifier` ，並傳送 `code_challenge` 以及向授權伺服器的 `/authorize` URL。

## 請求授權代碼

如果您使用預設的自訂授權伺服器，則您的請求URL將類似下列：

>[!INFO]
>
>**範例:**
>
>
>
```
>/authorize?client\_id=<clientID>&response\_type=code&redirect\_uri=<redirectURL>
>
>
&code\_challenge\_method=S256&code\_challenge=wzgjYF9qEiWep-CwqgrTE78-2ghjwCtRO3vj23o4W\_fw"
>```

請注意要傳遞的參數：

* `client_id` 比對您在設定應用程式時於中建立之OAuth2應用程式的用戶端ID。

   如需指示，請參閱「建立OAuth2應用程式以進行Workfront整合」中的使用PKCE建立OAuth2單頁Web應用程式。

* `response_type` is `code`，因為應用程式使用授權代碼授權類型。

* `redirect_uri` 是使用者代理與 `code`. 這必須符合您建立OAuth2應用程式時指定的其中一個重新導向URl。

* `code_challenge_method` 是用來產生挑戰的雜湊方法，這一律 `S256` 適用於使用PKCE的Workfront Oauth2應用程式。

* `code_challenge` 是用於PKCE的代碼挑戰。


## 交換代號的程式碼

若要交換存取權杖的授權碼，請將其傳遞至您的授權伺服器 `/token` 端點以及 `code_verifier`.

>[!INFO]
>
>**範例:**
>
>
```
>/token \\
>
>
  --header 'accept: application/json' \\
>
>
  --header 'cache-control: no-cache' \\
>
>
  --header 'content-type: application/x-www-form-urlencoded' \\
>
>
  --data 'grant\_type=authorization\_code&client\_id=<clientID>&redirect\_uri=<redirectURL>&code=<code>&code\_verifier=N28zVMsKU6ptUjHaYWg3T1NFTDQqcW1R4BU5NXywapNac4hhfkxjwfhZQat
>```

>[!IMPORTANT]
>
> 與一般的授權程式碼流程不同，此呼叫不需要具有用戶端ID和密碼的授權標題。 因此，此版本的授權程式碼流程適用於沒有後端的原生應用程式，例如行動應用程式或單頁應用程式。

請注意要傳遞的參數：

* `grant_type` is `authorization_code`，因為應用程式使用授權代碼授權類型。

* `redirect_uri` 必須與用於獲取授權代碼的URI匹配。

* `code` 是您從/authorize端點收到的授權代碼。

* `code_verifier` 是您的應用程式在中生成的PKCE代碼驗證器 [建立代碼交換的校樣金鑰](#Create).

* `client_id` 識別您的用戶端，且必須符合OAuth2中預先註冊的值。


如果程式碼仍有效，且程式碼驗證器相符，您的應用程式會收到存取權杖。

>[!INFO]
>
>**範例:**
>
>
```
>{
>
>
    "access\_token": "eyJhd\[...\]Yozv",
>
>
    "expires\_in": 3600,
>
>
    "token\_type": "Bearer"
>
>
}
>```

## 驗證存取權杖

當您的應用程式以存取權杖傳遞請求時，資源伺服器需要驗證請求。

您可以使用類似下列的API呼叫來驗證您的存取權杖：

>[!INFO]
>
>**範例:**
>
>
```
>/attask/api/<api version>/proj/search \\
>
>
  --header 'sessionID: <access\_token>' \\
>```

## 請求重新整理Token

若要要求重新整理Token，您可以對API進行POST呼叫，如下所示：

>[!INFO]
>
>**範例:**
>
>
```
>/token \\
>
>
  --header 'accept: application/json' \\
>
>
  --header 'cache-control: no-cache' \\
>
>
  --header 'content-type: application/x-www-form-urlencoded' \\
>
>
  --data 'grant\_type=refresh\_token&client\_id=<clientID>&redirect\_uri=<redirectURL>&refresh\_token=<refresh\_token>
>```
