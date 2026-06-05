---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: 透過Document Webhook搜尋
description: 透過Document Webhook搜尋
author: Becky
feature: Workfront API, Digital Content and Documents
role: Developer
exl-id: 8a3bf0c4-4a20-4311-8c05-15f4ef3a1d42
TQID: https://experienceleague.adobe.com/flRrmTOPVSGP83tVYfKG9AZOT7CNZN4IeWZNsVwcOO4
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2:
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 139
ht-degree: 5%

---

# 透過Document Webhook搜尋

傳回搜尋傳回之檔案和資料夾的中繼資料。 這可作為全文檢索搜尋或一般資料庫查詢來實施。 當使用者從外部檔案瀏覽器執行搜尋時，Adobe Workfront會呼叫/search端點。

## URL

GET /search

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
   <td>搜尋字詞或片語。</td> 
  </tr> 
  <tr> 
   <td>parentId</td> 
   <td> <p>（選用）執行搜尋的來源資料夾ID。注意：這是Workfront中未來功能的預留位置。目前，Workfront不傳遞此引數。 </p> </td> 
  </tr> 
  <tr> 
   <td>max</td> 
   <td>要傳回的專案數上限。 用於分頁。</td> 
  </tr> 
  <tr> 
   <td>offset</td> 
   <td> 頁面位移，與「最大值」搭配使用。</td> 
  </tr> 
 </tbody> 
</table>

 

## 回應

JSON，其中包含符合查詢的檔案和資料夾的中繼資料清單。 構成「符合」的專案由webhook提供者決定。 理想情況下，應該執行全文檢索搜尋。 執行檔案名稱式搜尋也可運作。

**範例：**

範例： `https://www.acme.com/api/search?query=test-query`

```
[ 
{ File/Folder Metadata },
{ File/Folder Metadata } 
]
```
