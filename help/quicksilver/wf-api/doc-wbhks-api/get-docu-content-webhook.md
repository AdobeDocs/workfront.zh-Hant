---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: 透過Webhook取得檔案內容
description: 傳回檔案的原始位元組
author: Becky
feature: Workfront API, Digital Content and Documents
role: Developer
exl-id: 0f0b5af7-f276-4856-852c-e976fa491f83
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '43'
ht-degree: 9%

---

# 透過Webhook取得檔案內容

傳回檔案的原始位元組

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
   <td> 檔案識別碼。</td> 
  </tr> 
 </tbody> 
</table>

## 回應

檔案的原始位元組。

**範例**：  `https://www.acme.com/api/download?id=123456`
