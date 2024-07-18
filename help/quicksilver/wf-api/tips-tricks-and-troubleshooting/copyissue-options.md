---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: OPTASK copyIssue的選項設定
description: copyIssue端點所需整數值的說明。
author: Becky
feature: Workfront API
role: Developer
exl-id: a2b8ef01-1c14-47a5-8b0a-550b17b526ff
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '122'
ht-degree: 4%

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
