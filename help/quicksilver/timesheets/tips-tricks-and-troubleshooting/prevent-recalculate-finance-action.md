---
content-type: tips-tricks-troubleshooting
product-area: timesheets
navigation-topic: tips-tricks-and-troubleshooting-timesheets
title: 避免重新計算財務動作在費率變更時影響歷史時數
description: 您需要更新使用者或工作角色的每小時成本（由於加薪或其他情況），但您不希望此變更影響先前登入專案的時數，或僅希望其影響一部分歷史時數。
author: Lisa
feature: Timesheets
exl-id: 29d3124b-cf7a-4a47-95c4-cd5379489810
source-git-commit: 69cd5fb1d089b81b7a1673609b92537137b6b68e
workflow-type: tm+mt
source-wordcount: '188'
ht-degree: 0%

---

# 避免重新計算財務動作在費率變更時影響歷史時數

## 問題

您需要更新使用者或工作角色的每小時成本（由於加薪或其他情況），但您不希望此變更影響先前登入專案的時數，或僅希望其影響一部分歷史時數。

## 解決方案

新增您不想變更至專案上記帳記錄的小時，並將記帳記錄的狀態設定為「已記帳」。  這會鎖定舊的比率，且會被重新計算財務動作忽略。  任何不屬於「已記帳」付費記錄的時數，都會以新費率計算。 如需詳細資訊，請參閱[重新計算專案財務](../../manage-work/projects/project-finances/recalculate-project-finances.md)。
