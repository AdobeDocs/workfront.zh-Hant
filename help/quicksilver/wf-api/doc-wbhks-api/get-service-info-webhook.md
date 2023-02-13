---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: 取得服務的相關資訊
description: 取得服務的相關資訊
author: John
feature: Workfront API
exl-id: a3a423ff-29a6-466e-a568-f64e02dcb484
source-git-commit: 5cb65c3a0c3ffd374c4002867c9c48985378e03c
workflow-type: tm+mt
source-wordcount: '266'
ht-degree: 4%

---


# 取得服務的相關資訊（尚未實作）

>[!NOTE]
>
>此功能的發行日期尚未決定。

傳回服務的相關資訊，例如功能。 Adobe Workfront將使用此資訊來自訂Workfront中的使用者介面。 例如，如果網頁連結實作包含某些自訂動作，JSON應在JSON中列出這些操作。 接著，使用者便能從Workfront叫用這些動作。

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
   <td>由此服務實作的WebHook版本。 這是此規格頂部列出的版本號。</td> 
  </tr> 
  <tr> 
   <td>版本 </td> 
   <td>字串 </td> 
   <td>此服務的內部版本號。 此編號由Webhook服務提供商確定，僅用於資訊用途。<br><br></td> 
  </tr> 
  <tr> 
   <td>發佈者 </td> 
   <td>字串 </td> 
   <td>提供Webhook實作的公司名稱。</td> 
  </tr> 
  <tr> 
   <td>availableEndpoints</td> 
   <td>字串 </td> 
   <td>包含此服務實作之API端點的清單。 這可用來確保Workfront中的使用者介面反映Webhook提供者提供的功能。 清單中的每個項目都必須包含端點名稱（例如「search」）。</td> 
  </tr> 
  <tr> 
   <td>customActions </td> 
   <td>字串</td> 
   <td>  <p>包含由此Webhook實作的自訂操作的清單。 每個清單項目都包含名稱和顯示名稱。 顯示名稱會顯示在Workfront的「檔案動作」下拉式清單中。 按一下下拉式清單中的項目，會呼叫/customAction端點來叫用Webhook中的動作。</p></td> 
  </tr> 
 </tbody> 
</table>

**範例：** `https://www.acme.com/api/serviceInfo`

傳回

```
{
webhook version: “1.2”, version: “1.0”, publisher: “Acme, LLC”, availableEndpoints: [“files”, “metadata”, “search”, “download”
“thumbnail”, “uploadInit”, “upload” ], customActions [
{
name: “archive”, displayName: “Archive” 
}, 
{name: “doSomethingElse”, displayName: “Do Something” }, 
] 
}
```
