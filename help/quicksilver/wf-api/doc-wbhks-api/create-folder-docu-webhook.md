---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: 建立包含檔案Webhook的資料夾
description: 建立包含檔案Webhook的資料夾
author: Becky
feature: Workfront API
role: Developer
exl-id: 50905915-58c9-4b50-b8a1-133833884a88
TQID: https://experienceleague.adobe.com/nneISzqXTIVje77d8QU29YPr6mOVplcwgzf48TEi-0A
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2: id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2: id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 66
ht-degree: 12%

---

# 建立包含檔案Webhook的資料夾

在指定目錄中建立資料夾。

## URL

POST /createFolder

## 查詢參數

| **名稱** | **說明** |
|---|---|
| parentId  | 應在其中建立資料夾的資料夾ID |
| 名稱  | 新資料夾的名稱 |




**回應**

新建立資料夾的中繼資料，如/metadata端點所定義。

## 範例

```
POST https://www.acme.com/api/createFolder
­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­-------------------------------
parentId=1234
name=New Folder 
-------------------------------
```

傳回

```
{title:"New Folder",br /> kind:"folder"
 id":"5678",
 viewLink:"",
 downloadLink:"",
 mimeType:"",
 dateModified:"2014­06­05T17:39:45.251Z"
 size: ""
 }
```
