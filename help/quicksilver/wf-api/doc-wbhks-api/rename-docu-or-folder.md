---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: 重新命名檔案或資料夾（尚未實作）
description: 重新命名檔案或資料夾
author: Becky
feature: Workfront API, Digital Content and Documents
role: Developer
exl-id: 5b1a4a02-a7fd-41f2-9adb-74b40606270b
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '81'
ht-degree: 8%

---


# 重新命名檔案或資料夾（尚未實作）

重新命名外部系統中具有特定ID的檔案或資料夾。

**URL**

PUT/重新命名

## 查詢參數

| 名稱  | 說明 |
|---|---|
| id | 要重新命名的檔案或資料夾ID |
| 名稱  | 檔案或資料夾的新名稱 |


## 個回應

指示成功或失敗的JSON字串，如以下錯誤處理區段中所指定。

**範例：** PUThttps://www.acme.com/api/rename

```
-------------------------------

id=1234

name=Folder B ­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­

-------------------------------
```

傳回

```
{status: "success"
 }returns
 {
 status: "failure", error: "Folder cannot be renamed because a folder with that name already exists."
 }
```
