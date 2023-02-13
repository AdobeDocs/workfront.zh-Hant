---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: 列出檔案或資料夾的元資料
description: 列出檔案或資料夾的元資料
author: John
feature: Workfront API
exl-id: 9c9f9222-59ac-4643-8297-d4939bec7e64
source-git-commit: d89d8cec90678aa3a047d1bfc0f1a8dd1682c58a
workflow-type: tm+mt
source-wordcount: '100'
ht-degree: 5%

---


# 獲取資料夾內容的項清單

列出給定資料夾的檔案和資料夾的元資料。

**URL**

GET/檔案

## 查詢參數

| 名稱  | 說明 |
|---|---|
| parentId  | 資料夾ID。 要獲取根目錄的元資料，請使用值「/」。 |
| 最大  | 要傳回的項目數上限。 用於分頁。 |
| 偏移  |  頁面位移，與「max」搭配使用。 |


## 個回應

JSON包含檔案和資料夾清單。 每個項的元資料與/metadata端點返回的元資料相同。

**範例：** https://www.acme.com/api/files?parentId=123456

```
[ 
{
title:"Folder A",
kind:"folder"
id":"2lj23lkj",
viewLink:" https://www.acme.com/viewDocument?id=2lj23lkj ”,
downloadLink:"https://www.acme.com/downloadDocument?id=2lj23lkj",
mimeType:"",
dateModified:"2014­06­05T17:39:45.251Z"
size: ""
},
{
title:"My Document",
kind:"file"
id":"da8cj234",
viewLink:" https://www.acme.com/viewDocument?id=da8cj234 ”,
downloadLink:"https://www.acme.com/downloadDocument?id=da8cj234",
mimeType:"image/png",
dateModified:"2014­06­05T17:39:45.251Z"
size: "32554694"
}
]
```
