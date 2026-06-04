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
TQID: https://experienceleague.adobe.com/AIN65ofKDJA95iMpvNwoe3oQapmyxzDC16dpf5ehwH0
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2: id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 43
ht-degree: 16%

---

# 透過Webhook取得檔案內容

傳回檔案的原始位元組

## URL

GET /download

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

**範例**： `https://www.acme.com/api/download?id=123456`
