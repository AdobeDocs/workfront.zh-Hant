---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: 註冊Webhook整合
description: 註冊Webhook整合
author: Becky
feature: Workfront API
role: Developer
exl-id: 9a4f8dbe-967f-4a41-a42c-8e3acb604972
source-git-commit: 494c7bf8aaf3570d4a01b5e88b85410ee3f52f18
workflow-type: tm+mt
source-wordcount: '339'
ht-degree: 11%

---


# 註冊Webhook整合

Adobe Workfront管理員可透過導覽至Workfront中的「設定>檔案>自訂整合」，為其公司新增自訂webhook整合。 在「設定」的「自訂整合」頁面中，管理員可以檢視現有檔案Webhook整合的清單。 您可以在此頁面新增、編輯、啟用和停用整合。

若要新增整合，請按一下[新增自訂整合]。****

![新增自訂整合](assets/webhooks-integration-2-350x220.png)

## 可用欄位

新增整合時，管理員將在下列欄位中輸入值。

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
   <td>姓名</td> 
   <td>此整合的名稱。</td> 
  </tr> 
  <tr> 
   <td>基底 API URL</td> 
   <td> <p>回撥API的位置。 呼叫外部系統時，Workfront僅會將端點名稱附加至此位址。 例如，如果管理員輸入基本API URL " https://www.mycompany.com/api/v1 "，Workfront將使用以下URL來取得檔案的中繼資料：https://www.mycompany.com/api/v1/metadata?id=1234。</p> </td> 
  </tr> 
  <tr> 
   <td>要求引數</td> 
   <td> <p>附加至每個 API 呼叫的 querystring 的選用值。例如，access_type </p> </td> 
  </tr> 
  <tr> 
   <td>驗證類型</td> 
   <td>OAuth2或ApiKey</td> 
  </tr> 
  <tr> 
   <td>驗證 URL</td> 
   <td> <p>（僅限OAuth2）用於使用者驗證的完整URL。 Workfront會在OAuth布建程式過程中，將使用者導覽至此位址。 注意： Workfront會將「state」引數附加至查詢字串。 提供者必須透過將此附加至Workfront重新導向URI，將其傳回Workfront。</p> </td> 
  </tr> 
  <tr> 
   <td>權杖端點 URL</td> 
   <td> <p>（僅限OAuth2）用於擷取OAuth2 Token的完整API URL。 這是由webhook提供者或外部檔案提供者所託管</p> </td> 
  </tr> 
  <tr> 
   <td>用戶端 ID</td> 
   <td>（僅限OAuth2）此整合的OAuth2使用者端ID</td> 
  </tr> 
  <tr> 
   <td>用戶端密碼</td> 
   <td> <p>（僅限OAuth2）此整合的OAuth2使用者端密碼</p> </td> 
  </tr> 
  <tr> 
   <td>Workfront 重新導向 URI</td> 
   <td>（僅限OAuth2）這是唯讀欄位，由Workfront產生。 此值可用來向外部檔案提供者註冊此整合。 注意：如上述驗證URL所述，提供者在執行重新導向時，必須將"state"引數及其值附加至查詢字串。</td> 
  </tr> 
  <tr> 
   <td>ApiKey</td> 
   <td> <p>（僅限ApiKey）用來對webhook提供者進行授權的API呼叫。 webhook提供者所發行的API金鑰。</p> </td> 
  </tr> 
 </tbody> 
</table>
