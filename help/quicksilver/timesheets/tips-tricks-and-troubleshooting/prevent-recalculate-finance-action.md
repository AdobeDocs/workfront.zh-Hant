---
content-type: tips-tricks-troubleshooting
product-area: timesheets
navigation-topic: tips-tricks-and-troubleshooting-timesheets
title: 防止在費率變化時重新計算財務活動影響歷史小時數
description: 您需要更新用戶或職務角色的小時成本（由於加薪或其他情況），但您不希望此更改影響以前已登錄項目的小時數，或您希望它僅影響部分歷史小時。
author: Alina
feature: Timesheets
exl-id: 29d3124b-cf7a-4a47-95c4-cd5379489810
source-git-commit: 7786d899841cb82cc4d3832fb083c6e2bda2e197
workflow-type: tm+mt
source-wordcount: '188'
ht-degree: 0%

---

# 防止在費率變化時重新計算財務活動影響歷史小時數

## 問題

您需要更新用戶或職務角色的小時成本（由於加薪或其他情況），但您不希望此更改影響以前已登錄項目的小時數，或您希望它僅影響部分歷史小時。

## 解決方案

添加您不希望更改為項目上的計費記錄的小時數，並將計費記錄的狀態設定為「計費」。  這將鎖定在舊比率中，並將被「重新計算財務」操作忽略。  任何不屬於已開單開單記錄的小時，都按新費率計算。 如需詳細資訊，請參閱 [重新計算項目財務](../../manage-work/projects/project-finances/recalculate-project-finances.md).
