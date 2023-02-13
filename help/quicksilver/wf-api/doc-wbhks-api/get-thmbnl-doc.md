---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: 獲取文檔的縮略圖
description: 獲取文檔的縮略圖
author: John
feature: Workfront API
exl-id: 31960689-1811-4ba7-a63d-0842caedf3ea
source-git-commit: 5cb65c3a0c3ffd374c4002867c9c48985378e03c
workflow-type: tm+mt
source-wordcount: '54'
ht-degree: 7%

---


# 獲取文檔的縮略圖

傳回檔案的原始縮圖位元組。

**URL**

GET/縮圖

## 查詢參數

| 名稱  | 說明 |
|---|---|
| id  | 文檔ID。 |
| 大小  |  縮圖的寬度。 |


## 個回應

原始縮圖位元組。

**範例：**: https://www.acme.com/api/thumbnail?id=123456
