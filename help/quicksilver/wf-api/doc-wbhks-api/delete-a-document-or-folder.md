---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: 刪除檔案或資料夾
description: 刪除檔案或資料夾
author: Becky
feature: Workfront API
role: Developer
exl-id: b56ec13a-1ee1-4bef-b39b-e625d00e4952
TQID: https://experienceleague.adobe.com/7-f8Z3qQQ2z7ZHHfSrGgJqIQCKdeqEoL96XlfCGzYSo
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2:
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 75
ht-degree: 9%

---

# 刪除檔案或資料夾（尚未實作）

刪除外部系統中具有特定ID的檔案或資料夾。 刪除資料夾也會刪除資料夾內容。

## URL

PUT /delete

## 查詢參數

| 名稱  | 說明 |
|---|---|
| documentId  | 要刪除的檔案識別碼 |
| folderId  |  要刪除的資料夾識別碼 |



## 回應

指示成功或失敗的JSON字串，如以下錯誤處理區段中所指定。

### 範例

```
PUT https://www.example.com/api/deleteid=1234

* returns `status: "success"`

* returns `status: "failure", error: "File not found"`
```
