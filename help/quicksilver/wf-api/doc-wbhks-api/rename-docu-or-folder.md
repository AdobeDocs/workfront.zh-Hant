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
TQID: https://experienceleague.adobe.com/-HmJkcMckTK6upblNcqX5LZkdYQxoWPDeuHkFjJarh4
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2: id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 81
ht-degree: 9%

---

# 重新命名檔案或資料夾（尚未實作）

重新命名外部系統中具有特定ID的檔案或資料夾。

**URL**

PUT /rename

## 查詢參數

| 名稱  | 說明 |
|---|---|
| id | 要重新命名的檔案或資料夾ID |
| 名稱  | 檔案或資料夾的新名稱 |


## 回應

指示成功或失敗的JSON字串，如以下錯誤處理區段中所指定。

**範例：** PUT https://www.acme.com/api/rename

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
