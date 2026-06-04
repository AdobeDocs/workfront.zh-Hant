---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: API錯誤訊息400錯誤請求
description: API錯誤訊息400錯誤請求
author: Becky
feature: Workfront API
role: Developer
exl-id: ab7c76a9-16ce-41f9-b7af-5943eb2dfdff
TQID: https://experienceleague.adobe.com/19PIdv4u8de0BlasXD0Yy6GssO3vv6Jt8BzcljB-m1w
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: b58ad82f-df6b-4b01-81a3-3a02ab9567a0
role_v2:
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 93
ht-degree: 2%

---

# API錯誤：「遠端伺服器傳回錯誤(400)錯誤請求」

## 問題

嘗試使用API將自訂欄位匯入問題時，出現以下錯誤：

`The remote server returned an error: (400) Bad Request`

## 原因

當您嘗試透過API匯入專案的自訂欄位時，此錯誤會發生，該專案沒有與佇列主題相關聯的自訂表單。

## 解決方案

將正確的自訂表單新增至佇列主題。

若要深入瞭解佇列主題，請參閱[建立佇列主題](../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md)。
