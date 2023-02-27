---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: 更名文檔或資料夾（尚未實施）
description: 更名文檔或資料夾
author: Becky
feature: Workfront API, Digital Content and Documents
exl-id: 5b1a4a02-a7fd-41f2-9adb-74b40606270b
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '81'
ht-degree: 6%

---


# 更名文檔或資料夾（尚未實施）

在外部系統中使用指定ID更名文檔或資料夾。

**URL**

PUT/重新命名

## 查詢參數

| 名稱  | 說明 |
|---|---|
| id | 要更名的文檔或資料夾ID |
| 名稱  | 文檔或資料夾的新名稱 |


## 個回應

表示成功或失敗的JSON字串，如下方的錯誤處理一節中所指定。

**範例：** PUThttps://www.acme.com/api/rename

```
-------------------------------

id=1234

name=Folder B ­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­

-------------------------------
```

傳回

```
{status: “success”
 }returns
 {
 status: “failure”, error: “Folder cannot be renamed because a folder with that name already exists.”
 }
```
