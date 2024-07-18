---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: 列出檔案或資料夾的中繼資料
description: 列出檔案或資料夾的中繼資料
author: Becky
feature: Workfront API
role: Developer
exl-id: 9c9f9222-59ac-4643-8297-d4939bec7e64
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '96'
ht-degree: 3%

---


# 取得資料夾內容的專案清單

列出指定資料夾的檔案和資料夾的中繼資料。

**URL**

GET/files

## 查詢參數

| 名稱  | 說明 |
|---|---|
| parentId  | 資料夾識別碼。 若要取得根目錄的中繼資料，請使用值&#39;/&#39;。 |
| max  | 要傳回的專案數上限。 用於分頁。 |
| offset  |  頁面位移，與「最大值」搭配使用。 |


## 回應

包含檔案和資料夾清單的JSON。 每個專案的中繼資料與/metadata端點傳回的中繼資料相同。

**範例：** https://www.acme.com/api/files?parentId=123456

```
[ 
{
title:"Folder A",
kind:"folder"
id":"2lj23lkj",
viewLink:" https://www.acme.com/viewDocument?id=2lj23lkj ",
downloadLink:"https://www.acme.com/downloadDocument?id=2lj23lkj",
mimeType:"",
dateModified:"2014­06­05T17:39:45.251Z"
size: ""
},
{
title:"My Document",
kind:"file"
id":"da8cj234",
viewLink:" https://www.acme.com/viewDocument?id=da8cj234 ",
downloadLink:"https://www.acme.com/downloadDocument?id=da8cj234",
mimeType:"image/png",
dateModified:"2014­06­05T17:39:45.251Z"
size: "32554694"
}
]
```
