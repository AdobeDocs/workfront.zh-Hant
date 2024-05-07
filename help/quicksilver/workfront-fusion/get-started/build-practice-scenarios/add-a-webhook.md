---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: 將webhook新增至基本情境
description: Webhook （也稱為即時觸發器）是一種特定的觸發器模組，可以在每次進行變更時啟動案例，而不是按照指定的排程。
author: Becky
feature: Workfront Fusion
source-git-commit: ea3f932e02ad8a9416747d4b9aefe89d087dd414
workflow-type: tm+mt
source-wordcount: '313'
ht-degree: 0%

---

# 將webhook新增至中的基本情境 [!DNL Adobe Workfront Fusion]

Webhook （也稱為即時觸發器）是一種特定的觸發器模組，可以在每次進行變更時啟動案例，而不是按照指定的排程。

在此範例中，只要有任何請求已提交至特定佇列，您就會新增webhook以啟動案例。 然後此情境會將這些請求轉換為專案。

此範例修改中建立的案例 [建立基本情境](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md).

## 先決條件

您必須建立中所述的情境 [建立基本情境](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md) 然後再執行此程式。

## 新增和設定webhook

1. 開啟轉換物件模組。
1. 在「問題ID」欄位中，刪除黑色ID區塊。 區塊為黑色，因為其對應來源模組已無法使用。
1. 在第一個模組（觀看事件）下方選取ID區塊，將其對應至第二個模組。
1. 按一下 **確定**.

### 新增webhook模組

1. 在案例編輯器中開啟案例。
1. 在第一個模組上按一下滑鼠右鍵，然後選取 **刪除模組**.

   模組已刪除，並保留空白預留位置。

1. 按一下空白模組，然後選擇 **Adobe Workfront** 從應用程式清單中。
1. 選取 **觀看活動**.
1. 按一下 **新增** ，位於Webhook欄位旁。
1. 在「記錄型別」欄位中，選取 **問題**，因此模組會觸發問題的變更。
1. 在「狀態」欄位中，選取 **新狀態**. 這是用於篩選的必填欄位，此範例未涵蓋此欄位。
1. 在「記錄來源」欄位中，選取 **僅限新記錄**. 這可讓情境在新增問題時觸發，而不是在更新或刪除問題時觸發。
1. 按一下 **儲存** 以儲存模組組態。


