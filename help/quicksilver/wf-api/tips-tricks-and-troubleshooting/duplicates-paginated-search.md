---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: 大型分頁搜尋期間傳回的重複專案
description: 大型分頁搜尋期間傳回的重複專案
author: Becky
feature: Workfront API
role: Developer
exl-id: 0359d6ba-b219-4d11-9f6f-cec2ff9ee058
TQID: https://experienceleague.adobe.com/1FXTHSro-rlUVHaajM1monR2Y-sxVHN6KIviogoXqRc
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
source-wordcount: 111
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

