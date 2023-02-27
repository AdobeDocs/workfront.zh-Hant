---
content-type: api;tips-tricks-troubleshooting
navigation-topic: workfront-api
title: emailAddr的更新不會更新使用者名稱
description: emailAddr的更新不會更新使用者名稱
author: Becky
feature: Workfront API
exl-id: 2d24d1b8-9504-484f-9cc0-d2f1abd6391a
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '231'
ht-degree: 0%

---


# emailAddr的更新不會更新使用者名稱

## 問題

通常， `emailAddr` 和 `username` 是相同的屬性。 因此，若您變更了使用者的 `emailAddr` 屬性， `username` 屬性會自動更新以符合。

當 `username` 不符合 `emailAddr`，更新 `emailAddr` 不會更新 `username` 自動。 兩者皆適用 `emailAddr` 透過使用者介面和API進行變更。

## 原因

不匹配可通過以下幾種方式產生：

* 在同步規則存在之前建立的用戶。 非常舊的用戶帳戶可能沒有這些屬性同步。

* 在Workfront中的emailAddr區分大小寫時，透過SSO建立的使用者。 SSO自動布建選項會根據來自身分提供者之使用者的屬性，對使用者執行區分大小寫的檢查。 當不存在完全匹配時，自動布建服務將建立新用戶。 如果使用者已存在，則使用者名稱和 `emailAddr` 不會有同樣的外殼。

* 擁有 `username` 屬性（透過API直接更新）及其 `emailAddr` 未更新。 此 `username` 和 `emailAddr` 可能不匹配。

## 解決方案

使用API來變更 `username` 屬性與 `emailAddr`. 同步屬性後，更新至 `emailAddr` 也會更新 `username` 相符（更新中未包含使用者名稱欄位時）。
