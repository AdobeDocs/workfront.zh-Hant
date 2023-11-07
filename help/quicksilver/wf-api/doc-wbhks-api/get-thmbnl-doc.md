---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: 取得檔案的縮圖
description: 取得檔案的縮圖
author: Becky
feature: Workfront API
role: Developer
exl-id: 31960689-1811-4ba7-a63d-0842caedf3ea
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '54'
ht-degree: 11%

---


# 取得檔案的縮圖

傳回檔案的原始縮圖位元組。

**URL**

GET/thumbnail

## 查詢參數

| 名稱  | 說明 |
|---|---|
| id  | 檔案識別碼。 |
| 大小  |  縮圖的寬度。 |


## 個回應

原始縮圖位元組。

**範例：**： https://www.acme.com/api/thumbnail?id=123456
