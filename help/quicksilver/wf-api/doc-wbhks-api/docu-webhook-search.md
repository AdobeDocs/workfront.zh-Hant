---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: 通過文檔Webhook進行搜索
description: 通過文檔Webhook進行搜索
author: Becky
feature: Workfront API, Digital Content and Documents
exl-id: 8a3bf0c4-4a20-4311-8c05-15f4ef3a1d42
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '154'
ht-degree: 4%

---

# 通過文檔Webhook進行搜索

返回從搜索返回的檔案和資料夾的元資料。 這可以作為全文搜索或作為常規資料庫查詢來實現。 當使用者從外部檔案瀏覽器執行搜尋時，Adobe Workfront會呼叫/search端點。

## URL

GET/搜尋

## 查詢參數

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>名稱 </th> 
   <th>說明</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>查詢</td> 
   <td>搜尋詞或片語。</td> 
  </tr> 
  <tr> 
   <td>parentId</td> 
   <td> <p>（可選）執行搜尋的資料夾ID。 注意：這是Workfront未來功能的預留位置。 目前，Workfront未傳遞此參數。 </p> </td> 
  </tr> 
  <tr> 
   <td>最大</td> 
   <td>要傳回的項目數上限。 用於分頁。</td> 
  </tr> 
  <tr> 
   <td>偏移</td> 
   <td> 頁面位移，與「max」搭配使用。</td> 
  </tr> 
 </tbody> 
</table>

 

## 個回應

JSON包含符合查詢之檔案和資料夾的中繼資料清單。 「符合」的構成由Webhook提供者決定。 理想情況下，它應該進行全文搜索。 執行檔案名稱型搜尋也是可行的。

**範例:**

範例:  `https://www.acme.com/api/search?query=test-query`

```
[ 
{ File/Folder Metadata },
{ File/Folder Metadata } 
]
```
