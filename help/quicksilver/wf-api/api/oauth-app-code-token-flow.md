---
content-type: api
navigation-topic: api-navigation-topic
title: 自訂OAuth 2應用程式的授權代碼流程
description: 自訂OAuth 2應用程式的授權代碼流程
author: Becky
feature: Workfront API
role: Developer
exl-id: a1ab60c4-4255-4d80-87f1-f36d325254c2
source-git-commit: 6f041459caf040846ffdec5bc75e9d74c99e318b
workflow-type: tm+mt
source-wordcount: '709'
ht-degree: 0%

---


# 使用授權程式碼流程設定及使用您組織的自訂OAuth 2應用程式

為了與Workfront整合併允許您的使用者端應用程式代表使用者與Workfront通訊，您必須：

* 建立Oauth2應用程式
* 設定協力廠商應用程式
* 連結至授權使用者頁面
* 設定授權代碼流程：使用者登入Workfront執行個體，並同意允許使用者端應用程式代表他們連線至Workfront。 因此，您會取得授權代碼，以便與存取權杖交換並重新整理Token。
* 設定重新整理Token流程：在此流程中，您可使用重新整理Token，在舊的Token過期時取得新的Access Token。

## 建立Oauth2應用程式

如需建立OAuth2應用程式的指示，請參閱 [使用使用者認證建立OAuth2應用程式（授權代碼流程）](../../administration-and-setup/configure-integrations/create-oauth-application.md#create3) 在 [為Workfront整合建立OAuth2應用程式](../../administration-and-setup/configure-integrations/create-oauth-application.md)

>[!NOTE]
>
>您一次最多可以有十個OAuth2應用程式。

## 連結至授權使用者頁面

您的使用者需要登入，才能在其帳戶中授權此整合。 使用者可授權的頁面具有特定格式，如下所述。 使用此資訊來判斷應用程式的授權頁面位址，並提供您的使用者此位址或連結。

* 您組織網域的完整URL。 範例：

  ```
  https://myorganization.my.workfront.com
  ```


* `client_id`：這是您在Workfront中建立OAuth2應用程式時產生的使用者端ID。

* `redirect_uri`：這是您在建立應用程式時輸入的重新導向URL。 您的使用者在為其帳戶授權應用程式後，即會被導向此頁面。

* `response_type`：此值必須是 `code`.

因此，授權頁面的URL為：

```
https://<URL of your organization's domain>/integrations/oauth2/authorize?client_id=<Your ClientID>&redirect_uri=<Your redirect URL>&response_type=code
```

>[!NOTE]
>
>建議您建立按鈕或其他連結，讓使用者按一下即可導向此頁面。

## 設定協力廠商應用程式

協力廠商應用程式可能需要設定。 下表包含設定協力廠商應用程式時可能需要的欄位相關資訊。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">授權URI</td> 
   <td> <p><code>https://&lt;the full URL of your organization's domain&gt;/integrations/oauth2/authorize</code> </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>範例： </b></span></span><code> https://myorganization.my.workfront.com/integrations/oauth2/authorize</code> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">權杖URL</td> 
   <td> <p><code>https://&lt;the full URL of your organization's domain&gt;/integrations/oauth2/api/v1/token</code> </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>範例： </b></span></span><code>https://myorganization.my.workfront.com/integrations/oauth2/api/v1/token</code> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">範圍</td> 
   <td>您不需要指定範圍。 </td> 
  </tr> 
 </tbody> 
</table>

## 設定授權代碼流程

![](assets/oauth-2-authorization-code-flow.png)

若要使用OAuth2登入使用者，請使用下列程式：

1. 使用者開啟授權頁面時，會重新導向至Workfront登入頁面，讓使用者可登入Workfront。 如果使用者有SSO組態，將會開啟識別提供者登入頁面。

   如果使用者已在相同瀏覽器上登入Workfront，或使用者已成功登入Workfront，則會將使用者重新導向至同意畫面：

   ![](assets/consent-screen-350x227.png)

1. 如果使用者允許存取，頁面會重新導向至 `redirect_url`. 重新導向必須包括下列查詢引數：

* `code`：取得存取/重新整理Token所需的授權代碼。
* `domain`：您組織的網域。 範例：在 `myorganization.my.workfront.com`，網域為 `myorganization`.
* `lane`：請求的通道。 範例：在 `myorganization.preview.workfront.com`，車道為 `preview`.

  >[!IMPORTANT]
  >
  >此 `code` 僅有效2分鐘。 因此，您必須在該時間內取得重新整理和存取權杖。

1. 有了程式碼後，您可以將程式碼連同使用者端應用程式認證傳送至 `/integrations/oauth2/api/v1/token` 端點。

   完整的權杖請求URL為

   ```
   https://<URL of your organization's domain></span>/integrations/oauth2/api/v1/token
   ```

   **範例：**  對權杖端點進行CURL呼叫的範例：

   範例1

   ```
      curl --location --request POST '**<workfront host>**/integrations/oauth2/api/v1/token' \
      --header 'Authorization: Basic **<base64(client_id:client_secret)>**' \
      --header 'Content-Type: application/json' \
      --data-raw '{
      "code": "**<code>**",
      "grant_type": "**authorization_code**",
      "redirect_uri": "**<redirect_url>**"
      }'
   ```

   範例2

   ```
      curl --location --request POST '**<workfront host>**/integrations/oauth2/api/v1/token' \
      --header 'Content-Type: application/x-www-form-urlencoded' \
      --data-urlencode 'grant_type=**authorization_code**' \
      --data-urlencode 'redirect_uri=**<redirect_url>**' \
      --data-urlencode 'code=**<code>**' \
      --data-urlencode 'client_id=**<client_id>**' \
      --data-urlencode 'client_secret=**<client_secret>**'  
   ```


   >[!IMPORTANT]
   >
   > 在Workfront中註冊應用程式時產生使用者端密碼。 您應將其儲存在安全的地方，因為如果遺失則無法復原。

   當所有傳遞的引數都正確時，權杖端點會傳回以下裝載：

   ```
   {
      "token_type": "sessionID",
      "access_token": "string", // the value of sessionID
      "refresh_token": "string",
      "expires_in": 0,
      "wid": "string"
   }
   ```

   存取權杖與相同 ```sessionID```，而且過期時間與一般使用者相同 ```sessionID```

   >[!IMPORTANT]
   >
   > 將重新整理權杖儲存在安全的地方。 舊的Token過期時，您需要它才能取得新的Refresh Token。 Workfront不會儲存您的重新整理Token。

1. 現在當您有存取權杖時，可以對Workfront進行API呼叫

   ```
   curl --request GET 'https://<workfront host>/attask/api/v14.0/proj/search \
   --header 'sessionID: <access_token>'
   ```

## 設定重新整理存取權杖

![](assets/refresh-access-token-flow-350x142.png)

若要重新整理access_token，我們再次需要對token端點執行「POST」呼叫。 這次我們會傳送不同的表單資料，如下所示：

```
curl --location --request POST '<workfront host>/integrations/oauth2/api/v1/token' \
--header 'Authorization: Basic <base64(client_id:client_secret)>' \
--header 'Content-Type: application/json' \
--data-raw '{
   "grant_type": "refresh_token",
   "refresh_token": "<refresh_token>"
}'

###### OR

curl --location --request POST '<workfront host>/integrations/oauth2/api/v1/token' \
--header 'Content-Type: application/x-www-form-urlencoded' \
--data-urlencode 'grant_type=refresh_token' \
--data-urlencode 'redirect_uri=<redirect_url>' \
--data-urlencode 'refresh_token=<refresh_token>' \
--data-urlencode 'client_id=<client_id>' \
--data-urlencode 'client_secret=<client_secret>'
```

它會傳回以下結果：

```
{
  "token_type": "sessionID",
  "access_token": "string", // the value of sessionID
  "refresh_token": "string",
  "expires_in": 0,
  "wid": "string"
}
```

存取權杖也是 `sessionID` ，可用來向Workfront提出API請求。
