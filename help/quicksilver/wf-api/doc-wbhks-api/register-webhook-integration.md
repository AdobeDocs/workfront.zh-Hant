---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: 註冊Webhook整合
description: 註冊Webhook整合
author: John
feature: Workfront API
exl-id: 9a4f8dbe-967f-4a41-a42c-8e3acb604972
source-git-commit: 5cb65c3a0c3ffd374c4002867c9c48985378e03c
workflow-type: tm+mt
source-wordcount: '346'
ht-degree: 11%

---


# 註冊Webhook整合

Adobe Workfront管理員可導覽至Workfront中的「設定>檔案>自訂整合」 ，為公司新增自訂網頁連結整合。 從「設定」的「自訂整合」頁面，管理員可以檢視現有檔案Webhook整合的清單。 您可以從本頁面新增、編輯、啟用和停用整合。

若要新增整合，請按一下 **新增自訂整合**.

![](assets/webhooks-integration-350x230.png)

![](assets/webhooks-integration-2-350x220.png)

## 可用欄位

新增整合時，管理員將輸入下列欄位的值。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>欄位名稱</th> 
   <th>說明</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>名稱</td> 
   <td>此整合的名稱。</td> 
  </tr> 
  <tr> 
   <td>基本 API URL</td> 
   <td> <p>回呼API的位置。 呼叫外部系統時，Workfront只會將端點名稱附加至此位址。 例如，如果管理員輸入了基本API URL " https://www.mycompany.com/api/v1 ",Workfront會使用下列URL來取得檔案的中繼資料：https://www.mycompany.com/api/v1/metadata?id=1234。</p> </td> 
  </tr> 
  <tr> 
   <td>要求參數</td> 
   <td> <p>附加至每個 API 呼叫的 querystring 的選用值。例如，access_type </p> </td> 
  </tr> 
  <tr> 
   <td>驗證類型</td> 
   <td>OAuth2或ApiKey</td> 
  </tr> 
  <tr> 
   <td>驗證 URL</td> 
   <td> <p>（僅限OAuth2）用於使用者驗證的完整URL。 Workfront會在OAuth布建程式中，將使用者導覽至此位址。 注意：Workfront會將「state」參數附加至查詢字串。 提供者必須將此檔案附加至Workfront重新導向URI，以將此檔案傳回Workfront。</p> </td> 
  </tr> 
  <tr> 
   <td>權杖端點 URL</td> 
   <td> <p>（僅限OAuth2）用來擷取OAuth2代號的完整API URL。 這是由Webhook提供者或外部檔案提供者托管</p> </td> 
  </tr> 
  <tr> 
   <td>用戶端 ID</td> 
   <td>（僅限OAuth2）此整合的OAuth2用戶端ID</td> 
  </tr> 
  <tr> 
   <td>用戶端密碼</td> 
   <td> <p>（僅限OAuth2）此整合的OAuth2用戶端密碼</p> </td> 
  </tr> 
  <tr> 
   <td>Workfront 重新導向 URI</td> 
   <td>（僅限OAuth2）此為唯讀欄位，由Workfront產生。 此值可用來與外部檔案提供者註冊此整合。 注意：如上所述，驗證URL的提供者在執行重新導向時，必須將「state」參數及其值附加至查詢字串。</td> 
  </tr> 
  <tr> 
   <td>ApiKey</td> 
   <td> <p>（僅限ApiKey）用於向Webhook提供者發出授權API呼叫。 由Webhook提供者發出的API金鑰。</p> </td> 
  </tr> 
 </tbody> 
</table>
