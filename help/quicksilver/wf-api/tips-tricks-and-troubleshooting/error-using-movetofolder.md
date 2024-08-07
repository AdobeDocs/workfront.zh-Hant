---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: 檔案moveToFolder動作無效
description: 使用Document moveToFolder動作時，會傳回422錯誤。
author: Becky
feature: Workfront API
role: Developer
exl-id: 811efabc-e101-4de5-a800-a1447654dc3e
source-git-commit: 53edc378e000e5b36fe0ce5750b8917fb13cfde1
workflow-type: tm+mt
source-wordcount: '121'
ht-degree: 0%

---

# 檔案moveToFolder動作無效

## 問題

使用檔案物件的`moveToFolder`動作時，傳回422錯誤。

或

如果透過Workfront Fusion中的Adobe Authenticator模組使用此動作，檔案不會移動，但不顯示錯誤。 錯誤相同，但Adobe Authenticator模組未顯示錯誤。

## 解決方案

此動作發生422錯誤的一個可能原因是動作嘗試將一個連結資料夾中的檔案移動到另一個連結資料夾。

核取「 」，確認您要移動的檔案不在連結的資料夾中。
