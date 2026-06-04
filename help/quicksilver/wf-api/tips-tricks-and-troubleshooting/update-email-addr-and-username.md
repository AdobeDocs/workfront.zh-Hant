---
content-type: api;tips-tricks-troubleshooting
navigation-topic: workfront-api
title: 更新至emailAddr不會更新使用者名稱
description: 更新emailAddr不會更新使用者名稱
author: Becky
feature: Workfront API
role: Developer
exl-id: 2d24d1b8-9504-484f-9cc0-d2f1abd6391a
TQID: https://experienceleague.adobe.com/dkceJuJ6WfaZTnbD6zdP6TsHR5bvkERD-EiBgVmrCck
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: b58ad82f-df6b-4b01-81a3-3a02ab9567a0
role_v2: id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2: id: c1579802-ddd4-4214-8a91-97b2066abe11
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 235
ht-degree: 0%

---

# 更新至emailAddr不會更新使用者名稱

## 問題

通常，`emailAddr`和`username`是相同的屬性。 因此，如果您變更使用者的`emailAddr`屬性，`username`屬性會自動更新以相符。

當`username`不符合`emailAddr`時，`emailAddr`的更新不會自動更新`username`。 對於透過使用者介面及透過API進行的`emailAddr`變更都是如此。

## 原因

不相符現象可能以幾種方式產生：

* 在同步化規則存在之前建立的使用者。 非常舊的使用者帳戶可能沒有同步這些屬性。

* 在Workfront中的emailAddr區分大小寫，透過SSO建立的使用者。 SSO自動布建選項會根據身分提供者的使用者屬性，對使用者執行區分大小寫的檢查。 當不存在完全相符專案時，自動布建服務將會建立新使用者。 如果使用者已存在，則使用者名稱和`emailAddr`可能會有不同的大小寫。

* 已透過API直接更新`username`屬性的使用者，其`emailAddr`未更新。 `username`和`emailAddr`可能不相符。

## 解決方案

使用API將`username`屬性變更為與`emailAddr`相同。 同步化屬性後，`emailAddr`的任何更新也會更新`username`以使其相符（當更新中未包含使用者名稱欄位時）。
