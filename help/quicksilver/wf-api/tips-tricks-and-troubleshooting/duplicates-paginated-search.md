---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: 在大型編頁搜索期間返回的重複項
description: 在大型編頁搜索期間返回的重複項
author: Becky
feature: Workfront API
exl-id: 0359d6ba-b219-4d11-9f6f-cec2ff9ee058
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '111'
ht-degree: 0%

---


# 在大型編頁搜索期間返回的重複項

## 問題

在API中針對物件執行大型編頁搜尋時，客戶會收到重複項目和遺失記錄。

## 解決方案

當順序未正式定義時，我們依賴Oracle資料庫返回的行順序，這不能保證任何確定性的排序。 例如，具有相同查詢的兩個連續呼叫可能會以不同順序傳回列。 同樣地，執行分頁時，行可能會隨機分配給不同的「頁面」，導致重複。 最簡單的解決方案是依ID新增排序：

```
&ID_Sort=asc
```

