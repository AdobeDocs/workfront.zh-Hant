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
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '66'
ht-degree: 10%

---


# 建立包含檔案Webhook的資料夾

在指定目錄中建立資料夾。

## URL

POST/createFolder

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
