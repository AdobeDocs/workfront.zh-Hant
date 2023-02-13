---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: 刪除文檔或資料夾
description: 刪除文檔或資料夾
author: John
feature: Workfront API
exl-id: b56ec13a-1ee1-4bef-b39b-e625d00e4952
source-git-commit: 9de8ee7fad2a3cb67c4fc6bfdff4d6ce50f15afd
workflow-type: tm+mt
source-wordcount: '82'
ht-degree: 6%

---


# 刪除文檔或資料夾（尚未實施）

刪除外部系統中具有指定ID的文檔或資料夾。 刪除資料夾也會刪除資料夾內容。

## URL

PUT/刪除

## 查詢參數

| 名稱  | 說明 |
|---|---|
| documentId  | 要刪除的文檔ID |
| folderId  |  要刪除的資料夾ID |



## 個回應

表示成功或失敗的JSON字串，如下方的錯誤處理一節中所指定。

### 範例

PUThttps://www.example.com/api/deleteid=1234
* 傳回 `status: “success”`

* 傳回 `status: “failure”, error: “File not found”`
