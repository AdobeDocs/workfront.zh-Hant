---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: 取得OAuth2代號
description: 取得OAuth2代號
author: Becky
feature: Workfront API
exl-id: f3a2630d-d34e-4d36-b2bb-707ba0d3258e
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '268'
ht-degree: 4%

---


# 取得OAuth2代號

## 取得OAuth2代號

傳回已驗證使用者的OAuth2重新整理Token和存取Token。 當用戶設定文檔提供程式時，將調用一次。 會進行後續呼叫，以取得更新的存取權杖。

**URL**

POST/any/url

此URL是可設定的，並對應至自訂整合設定頁面上的Token端點URL值。

### 查詢參數

<table style="table-layout:auto">
 <col>
 <col>
 <col>
 <thead>
  <tr>
   <th>名稱</th>
   <th>必要</th>
   <th>說明</th>
  </tr>
 </thead>
 <tbody>
  <tr>
   <td>grant_type</td>
   <td>是</td>
   <td><p>值包括「authorization_code」或「refresh_token」。 指定的值會指出這兩個參數中的哪個將傳遞至此API呼叫：code或refresh_token。</p></td>
  </tr>
  <tr>
   <td>代碼</td>
   <td>dessions</td>
   <td><p>在使用者按一下「授權」按鈕後，授權程式碼即傳送至Adobe Workfront。 只有當授權類型為「authorization_code」時，才需要此選項。 授權代碼應為短期，通常在10分鐘或更短時間內到期。</p></td>
  </tr>
  <tr>
   <td>refresh_token</td>
   <td>dessions</td>
   <td><p>只有在後續呼叫以擷取新access_token時，才需要這個選項，因為先前的access_token已過期。 傳送此值時，請將grant_type參數設為「refresh_token」。</p></td>
  </tr>
  <tr>
   <td>client_id</td>
   <td>是</td>
   <td>在Workfront中針對此自訂整合設定的用戶端ID。</td>
  </tr>
  <tr>
   <td>client_secret</td>
   <td>是</td>
   <td> Workfront中針對此自訂整合設定的用戶端密碼。</td>
  </tr>
 </tbody>
</table>

 

## 個回應

<table style="table-layout:auto">
 <col>
 <col>
 <col>
 <thead>
  <tr>
   <th>名稱</th>
   <th>類型 </th>
   <th>說明</th>
  </tr>
 </thead>
 <tbody>
  <tr>
   <td>access_token </td>
   <td>字串</td>
   <td><p>代表使用者進行授權API呼叫的代號。 此過期時間應該會防止未授權的API呼叫。</p></td>
  </tr>
  <tr>
   <td>refresh_token </td>
   <td>字串</td>
   <td><p>一種長期的Token，可透過呼叫此API方法來擷取新的access_token。</p></td>
  </tr>
  <tr>
   <td>expires_in </td>
   <td>long</td>
   <td><p>（選用）access_token過期的時間（以秒為單位），通常為3,600。</p></td>
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

## 個回應

```
{
access_token:"ad8af5ad5ads759",
refresh_token:"9a0h5d87d808ads",
expires_id:3600
}
```
