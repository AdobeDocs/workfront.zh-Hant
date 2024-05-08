---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: 將篩選器新增至基本情境
description: 篩選可讓您確保您的案例僅在符合某些條件時進展。
author: Becky
feature: Workfront Fusion
source-git-commit: 5ba5b2e37e2ce58d96d11f24786feef57f8eb638
workflow-type: tm+mt
source-wordcount: '495'
ht-degree: 1%

---

# 將篩選器新增至中的基本案例 [!DNL Adobe Workfront Fusion]

篩選可讓您確保您的案例僅在符合某些條件時進展。

在此範例中，您會新增篩選器至情境，以允許只有在請求已提交至特定請求佇列時，才能從請求建立新專案。

此範例修改中建立的案例 [建立基本情境](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md).

>[!NOTE]
>
>Workfront觸發模組包含篩選器，允許案例只在符合特定條件時啟動。 不過，由於模組間篩選器會用於每個非觸發程式和非Workfront使用案例，因此瞭解如何在模組間使用篩選器非常重要。 此範例針對模組內篩選器可能符合的功能，使用模組間篩選器。

## 先決條件

您必須建立中所述的情境 [建立基本情境](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md) 然後再執行此程式。

## 新增篩選器

### 準備新增篩選器

1. 開啟第一個情境。
1. 在 **輸出** 區域，選取 `Project`.
您現在應該有 `ID`， `Name`、和 `Project` 已選取。
1. 按一下「確定」以儲存模組設定。
1. 開啟Workfront。
1. 在Workfront中，找出代表Fusion案例將使用的請求佇列的專案。

   此專案必須位於為Fusion連線設定的Workfront帳戶中。

1. 在URL中記下專案ID。

   範例： https://\&lt;mydomain>.my.workfront.com/project/\&lt;projectid>/tasks

### 新增並設定篩選器

1. 在案例編輯器中開啟案例。
1. 按一下扳手圖示 ![扳手圖示](assets/wrench-icon.png) 並選取「 」 **設定篩選器**.
1. 在「標籤」欄位中，輸入此篩選的標籤，例如「篩選請求佇列」。
1. 在 **條件** 區域，在頂端欄位中，對應 `projectID` 第一個模組。

   ![對應專案ID](assets/map-proj-id.png)
1. 離開 **條件** 運運算元設為Equal to。
1. 在的底部欄位中 **條件** 區域，貼上您從專案URL中記錄的專案ID [準備新增篩選器](#prepare-to-add-the-filter).
1. 按一下 **確定** 以儲存篩選設定。

### 測試並啟動

1. 前往Fusion所連線的Workfront環境，並將問題新增至您在篩選中指定的專案。 將另一個問題新增至其他專案。
1. 按一下 **[!UICONTROL 執行一次]** 位於情境編輯器的左下角。
1. 檢查輸出，確保案例如預期般執行。

   這兩個問題都應該出現在第一個案例的輸出中，但只有指定專案中的問題應該作為第二個案例的輸入出現，
1. 當您滿意情境如預期般運作時，請按一下 **正在排程** 在熒幕左下角切換為 **開啟**.

   這會啟用情境。
1. 在 [!DNL Workfront Fusion]，按一下 **[!UICONTROL 儲存]** 靠近左下角，儲存情境的進度。

   >[!IMPORTANT]
   >
   >隨時儲存並測試情境。

## 資源

* 如需篩選的詳細資訊，請參閱 [將篩選器新增至案例](/help/quicksilver/workfront-fusion/scenarios/add-a-filter-to-a-scenario.md).

