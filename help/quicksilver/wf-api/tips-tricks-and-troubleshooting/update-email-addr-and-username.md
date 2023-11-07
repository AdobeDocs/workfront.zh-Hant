---
content-type: api;tips-tricks-troubleshooting
navigation-topic: workfront-api
title: 更新至emailAddr不會更新使用者名稱
description: 更新emailAddr不會更新使用者名稱
author: Becky
feature: Workfront API
role: Developer
exl-id: 2d24d1b8-9504-484f-9cc0-d2f1abd6391a
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '231'
ht-degree: 0%

---


# 更新至emailAddr不會更新使用者名稱

## 問題

一般而言， `emailAddr` 和 `username` 是相同的屬性。 因此，如果您變更使用者的 `emailAddr` 屬性， `username` 屬性會自動更新以相符。

當 `username` 不符合 `emailAddr`，此變數的更新 `emailAddr` 不會更新 `username` 自動。 兩者皆適用 `emailAddr` 透過使用者介面及API進行變更。

## 原因

不相符現象可能以幾種方式產生：

* 在同步化規則存在之前建立的使用者。 非常舊的使用者帳戶可能沒有同步這些屬性。

* 在Workfront中的emailAddr區分大小寫，透過SSO建立的使用者。 SSO自動布建選項會根據身分提供者的使用者屬性，對使用者執行區分大小寫的檢查。 當不存在完全相符專案時，自動布建服務將會建立新使用者。 如果使用者已存在，則使用者名稱和 `emailAddr` 將不會有相同的大小寫。

* 擁有下列專案的使用者： `username` 直接透過API更新的屬性，及其 `emailAddr` 未更新。 此 `username` 和 `emailAddr` 可能不相符。

## 解決方案

使用API變更 `username` 屬性與 `emailAddr`. 同步化屬性後，對 `emailAddr` 也會更新 `username` 以符合（當更新中未包含使用者名稱欄位時）。
