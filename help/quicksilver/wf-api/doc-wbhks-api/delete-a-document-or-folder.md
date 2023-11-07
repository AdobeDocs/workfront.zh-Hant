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
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '82'
ht-degree: 8%

---


# 刪除檔案或資料夾（尚未實作）

刪除外部系統中具有特定ID的檔案或資料夾。 刪除資料夾也會刪除資料夾內容。

## URL

PUT/delete

## 查詢參數

| 名稱  | 說明 |
|---|---|
| documentId  | 要刪除的檔案識別碼 |
| folderId  |  要刪除的資料夾識別碼 |



## 個回應

指示成功或失敗的JSON字串，如以下錯誤處理區段中所指定。

### 範例

PUThttps://www.example.com/api/delete­­­­­­­­­­­­­­­­­­­­­­­­­­­­­id=1234
* 傳回 `status: "success"`

* 傳回 `status: "failure", error: "File not found"`
