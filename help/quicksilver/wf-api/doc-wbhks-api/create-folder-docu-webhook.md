---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: 使用文檔Webhook建立資料夾
description: 使用文檔Webhook建立資料夾
author: Becky
feature: Workfront API
exl-id: 50905915-58c9-4b50-b8a1-133833884a88
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '66'
ht-degree: 7%

---


# 使用文檔Webhook建立資料夾

在指定目錄中建立資料夾。

## URL

POST/createFolder

## 查詢參數

| **名稱** | **說明** |
|---|---|
| parentId  | 應在其中建立資料夾的資料夾ID |
| 名稱  | 新資料夾的名稱 |




**回應**

新建立資料夾的元資料，由/metadata端點定義。

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
 viewLink:"”,
 downloadLink:"",
 mimeType:"",
 dateModified:"2014­06­05T17:39:45.251Z"
 size: ""
 }
```
