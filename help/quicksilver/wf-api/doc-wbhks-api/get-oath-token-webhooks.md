---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: 取得OAuth2 Token
description: 取得OAuth2 Token
author: Becky
feature: Workfront API
role: Developer
exl-id: f3a2630d-d34e-4d36-b2bb-707ba0d3258e
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '253'
ht-degree: 3%

---


# 取得OAuth2 Token

## 取得OAuth2 Token

傳回已驗證使用者的OAuth2重新整理權杖和存取權杖。 當使用者布建檔案提供者時，就會叫用一次。 進行後續呼叫以取得更新的存取Token。

**URL**

POST/any/url

URL可設定，並與自訂整合設定頁面上的權杖端點URL值相對應。

### 查詢參數

<table style="table-layout:auto">
 <col>
 <col>
 <col>
 <thead>
  <tr>
   <th>姓名</th>
   <th>必要</th>
   <th>說明</th>
  </tr>
 </thead>
 <tbody>
  <tr>
   <td>grant_type</td>
   <td>是</td>
   <td><p>值包括「authorization_code」或「refresh_token」。 指定的值表示將傳遞至此API呼叫的兩個引數之一： code或refresh_token。</p></td>
  </tr>
  <tr>
   <td>程式碼</td>
   <td>根據</td>
   <td><p>使用者按一下「授予」按鈕後就會傳送至Adobe Workfront的授權代碼。 僅當授權型別為「authorization_code」時才需要此項。 授權碼應為短期，通常在10分鐘或更短時間內到期。</p></td>
  </tr>
  <tr>
   <td>refresh_token</td>
   <td>根據</td>
   <td><p>只有在進行後續呼叫以擷取新的access_token時才需要此專案，因為先前的access_token已過期。 傳送此值時，請將grant_type引數設為"refresh_token"。</p></td>
  </tr>
  <tr>
   <td>client_id</td>
   <td>是</td>
   <td>在Workfront中針對此自訂整合設定的使用者端ID。</td>
  </tr>
  <tr>
   <td>client_secret</td>
   <td>是</td>
   <td> Workfront中針對此自訂整合設定的使用者端密碼。</td>
  </tr>
 </tbody>
</table>

 

## 回應

<table style="table-layout:auto">
 <col>
 <col>
 <col>
 <thead>
  <tr>
   <th>姓名</th>
   <th>型別 </th>
   <th>說明</th>
  </tr>
 </thead>
 <tbody>
  <tr>
   <td>access_token </td>
   <td>字串</td>
   <td><p>代號，用來代表使用者進行授權的API呼叫。 此專案應該會過期，以防止未經授權的API呼叫。</p></td>
  </tr>
  <tr>
   <td>refresh_token </td>
   <td>字串</td>
   <td><p>長效權杖，用於透過呼叫此API方法擷取新的access_token。</p></td>
  </tr>
  <tr>
   <td>expires_in </td>
   <td>長</td>
   <td><p>（選用） access_token過期前的時間（以秒為單位），通常為3,600。</p></td>
  </tr>
 </tbody>
</table>

**範例**

```
POST /oauth2/token
grant_type=authorization_code
code=d9ac7asdf6asdf579d7a8
client_id=123456
client_secret=6asdf7a7a9a4af
```

## 回應

```
{
access_token:"ad8af5ad5ads759",
refresh_token:"9a0h5d87d808ads",
expires_id:3600
}
```
