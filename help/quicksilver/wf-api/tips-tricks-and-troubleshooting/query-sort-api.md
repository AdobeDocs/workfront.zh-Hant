---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: 排序API中的查詢結果
description: 排序API中的查詢結果
author: Becky
feature: Workfront API
role: Developer
exl-id: f001adb8-6295-4646-b9f1-78244a8c44a6
TQID: https://experienceleague.adobe.com/r7PCHEpU413ajyML7-uzWdmXN11gylNHRU2q60J35Go
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: b58ad82f-df6b-4b01-81a3-3a02ab9567a0
role_v2: id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2: id: c1579802-ddd4-4214-8a91-97b2066abe11
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 60
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
