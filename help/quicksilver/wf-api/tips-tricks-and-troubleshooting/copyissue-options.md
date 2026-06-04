---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: OPTASK copyIssue的選項設定
description: copyIssue端點所需整數值的說明。
author: Becky
feature: Workfront API
role: Developer
exl-id: a2b8ef01-1c14-47a5-8b0a-550b17b526ff
TQID: https://experienceleague.adobe.com/9cDJFoKl6zqpaAvqzpGqzflcbGZNrAWvEnUAFuqD-Rc
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: b58ad82f-df6b-4b01-81a3-3a02ab9567a0
role_v2: id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2: id: c1579802-ddd4-4214-8a91-97b2066abe11
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 122
ht-degree: 8%

---

# OPTASK copyIssue的選項設定


copyIssue API呼叫的其中一個屬性是名為`options`的欄位。 此欄位必須是整數。

若要包含下列其中一個選項，請輸入相符的整數。 若要包含多個選項，請輸入相符整數的加總。

| 選項 | value* |
|---|---|
| 清除指派 | 2 |
| 清除進度 | 4 |
| 清除檔案 | 128 |
| 清除更新 | 65536 |
| 清除許可權 | 524288 |
| 清除自訂資料 | 1048576 |

*所有值皆為2的冪。

範例：

* 若要在複製問題時清除進度，請輸入`options`值`4`。

* 若要清除進度與檔案，請輸入`132`的`options`值。

  清除進度= 4

  清除檔案= 128

  4 + 128 = 132
