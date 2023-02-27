---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: 在API中排序查詢結果
description: 在API中排序查詢結果
author: Becky
feature: Workfront API
exl-id: f001adb8-6295-4646-b9f1-78244a8c44a6
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '60'
ht-degree: 0%

---


# 在API中排序查詢結果

如果您將下列項目附加至API呼叫，則可依任何欄位來排序結果：

```
&entryDate_Sort=asc
```

例如，如果要按任務計畫起始日期排序，請刪除 `entryDate` 用 `plannedCompletionDate`.

這適用於Adobe Workfront的大部分欄位。
