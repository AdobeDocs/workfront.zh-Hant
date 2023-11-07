---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: 大型分頁搜尋期間傳回的重複專案
description: 大型分頁搜尋期間傳回的重複專案
author: Becky
feature: Workfront API
role: Developer
exl-id: 0359d6ba-b219-4d11-9f6f-cec2ff9ee058
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '111'
ht-degree: 0%

---


# 大型分頁搜尋期間傳回的重複專案

## 問題

在API中針對物件執行大型分頁搜尋時，客戶會收到重複的專案和遺失的記錄。

## 解決方案

當未正式定義順序時，我們依賴Oracle資料庫傳回的列順序，這無法保證任何確定性排序。 例如，具有相同查詢的兩個連續呼叫可能會以不同順序傳回列。 同樣地，在執行分頁時，列可能會隨機指派給不同的「頁面」，導致重複。 最簡單的解決方案是新增依ID排序：

```
&ID_Sort=asc
```

