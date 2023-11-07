---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: 取得服務的相關資訊
description: 取得服務的相關資訊
author: Becky
feature: Workfront API
role: Developer
exl-id: a3a423ff-29a6-466e-a568-f64e02dcb484
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '266'
ht-degree: 4%

---


# 取得服務的相關資訊（尚未實作）

>[!NOTE]
>
>此功能的發行日期尚未確定。

傳回服務的相關資訊，例如特性與功能。 Adobe Workfront將使用此資訊在Workfront中自訂使用者介面。 例如，如果webhook實作包含一些自訂動作，JSON應在JSON中列出這些動作。 之後，使用者就可以從Workfront叫用這些動作。

**URL**

GET/serviceInfo

## 查詢參數

無. 此外，對此端點的呼叫不應需要驗證。

## 個回應

包含此服務相關資訊的JSON

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
   <td>webhookVersion </td> 
   <td>字串 </td> 
   <td>此服務實作的webhook版本。 這是列在此規格頂端的版本編號。</td> 
  </tr> 
  <tr> 
   <td>版本 </td> 
   <td>字串 </td> 
   <td>此服務的內部版本號碼。 此數字由webhook服務提供者決定，僅供參考。<br><br></td> 
  </tr> 
  <tr> 
   <td>發佈者 </td> 
   <td>字串 </td> 
   <td>提供webhook實作的公司名稱。</td> 
  </tr> 
  <tr> 
   <td>availableendpoints</td> 
   <td>字串 </td> 
   <td>包含此服務實作之API端點的清單。 這可用來確保Workfront中的使用者介面反映webhook提供者所提供的功能。 清單中的每個專案都必須包含端點的名稱（例如「search」）。</td> 
  </tr> 
  <tr> 
   <td>customActions </td> 
   <td>字串</td> 
   <td>  <p>包含此Webhook實作的自訂作業清單。 每個清單專案都包含名稱和顯示名稱。 顯示名稱會顯示在Workfront的「檔案動作」下拉式清單中。 按一下下拉式清單中的專案時，將會呼叫/customAction端點，以叫用webhook中的動作。</p></td> 
  </tr> 
 </tbody> 
</table>

**範例：** `https://www.acme.com/api/serviceInfo`

傳回

```
{
webhook version: "1.2", version: "1.0", publisher: "Acme, LLC", availableEndpoints: ["files", "metadata", "search", "download"
"thumbnail", "uploadInit", "upload" ], customActions [
{
name: "archive", displayName: "Archive" 
}, 
{name: "doSomethingElse", displayName: "Do Something" }, 
] 
}
```
