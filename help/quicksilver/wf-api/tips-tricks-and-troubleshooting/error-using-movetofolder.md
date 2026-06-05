---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: 檔案moveToFolder動作無效
description: 使用Document moveToFolder動作時，會傳回422錯誤。
author: Becky
feature: Workfront API
role: Developer
exl-id: 811efabc-e101-4de5-a800-a1447654dc3e
TQID: https://experienceleague.adobe.com/UV4VnQEs-jGJau1UqXTLnp7Ak-cmKRpjuJqxgNTF5z8
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
source-wordcount: 121
ht-degree: 1%

---

# 檔案moveToFolder動作無效

## 問題

使用檔案物件的`moveToFolder`動作時，傳回422錯誤。

或

如果透過Workfront Fusion中的Adobe Authenticator模組使用此動作，檔案不會移動，但不顯示錯誤。 錯誤相同，但Adobe Authenticator模組未顯示錯誤。

## 解決方案

此動作發生422錯誤的一個可能原因是動作嘗試將一個連結資料夾中的檔案移動到另一個連結資料夾。

核取「 」，確認您要移動的檔案不在連結的資料夾中。
