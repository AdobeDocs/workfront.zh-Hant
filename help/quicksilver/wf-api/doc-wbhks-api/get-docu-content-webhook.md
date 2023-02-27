---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: 透過Webhook取得檔案內容
description: 返回文檔的原始位元組
author: Becky
feature: Workfront API, Digital Content and Documents
exl-id: 0f0b5af7-f276-4856-852c-e976fa491f83
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '53'
ht-degree: 7%

---

# 透過Webhook取得檔案內容

返回文檔的原始位元組

## URL

GET/下載

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
   <td> <p>id</p> </td> 
   <td> 文檔ID。</td> 
  </tr> 
 </tbody> 
</table>

## 個回應

文檔的原始位元組。

**範例：**:  [https://www.acme.com/api/download?id=123456](https://www.acme.com/api/download?id=123456)
