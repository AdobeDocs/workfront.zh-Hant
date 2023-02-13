---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: OPTASK copyIssue的選項配置
description: copyIssue端點預期的整數值說明。
author: Becky
feature: Workfront API
exl-id: a2b8ef01-1c14-47a5-8b0a-550b17b526ff
source-git-commit: 93a67b3dbd59f188dad6b060ec93c3f137c981b2
workflow-type: tm+mt
source-wordcount: '117'
ht-degree: 6%

---

# OPTASK copyIssue的選項配置


copyIssue API呼叫的其中一個屬性是名為的欄位 `options`. 此欄位需要整數。

要包括以下選項之一，請輸入匹配的整數。 若要包含多個選項，請輸入相符整數的總和。

| 選項 | value* |
|---|---|
| 清除分配 | 2 |
| 明確進展 | 4 |
| 清除文檔 | 128 |
| 清除更新 | 65536 |
| 清除權限 | 524288 |
| 清除自訂資料 | 1048576 |

*所有值都是2的冪。

範例:

* 若要在複製問題時清除進度，請輸入 `options` 值 `4`.

* 要清除進度和文檔，請輸入 `options` 值 `132`.

   清除進度= 4

   清除文檔= 128

   4 + 128 = 132
