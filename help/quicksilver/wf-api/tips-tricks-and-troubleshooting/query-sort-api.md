---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: 排序API中的查詢結果
description: 排序API中的查詢結果
author: Becky
feature: Workfront API
role: Developer
exl-id: f001adb8-6295-4646-b9f1-78244a8c44a6
source-git-commit: 5936982217adc6cfcaf9e400bfff67a1496d3a78
workflow-type: tm+mt
source-wordcount: '60'
ht-degree: 0%

---


# 排序API中的查詢結果

如果您將以下內容附加至API呼叫，則可以根據任何欄位來排序結果：

```
&entryDate_Sort=asc
```

例如，如果您想要依任務計畫完成日期排序，請移除`entryDate`並將其取代為`plannedCompletionDate`。

```
&plannedCompletionDate_Sort=asc
```

這適用於Adobe Workfront中的大部分欄位。
