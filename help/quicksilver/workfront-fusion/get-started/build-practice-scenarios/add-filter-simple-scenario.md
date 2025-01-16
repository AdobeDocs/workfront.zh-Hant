---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: 將篩選器新增至基本情境
description: Adobe Workfront Fusion檔案已移至新位置。 本文已棄用，但包含新文章的連結，內容涵蓋此功能。
author: Becky
feature: Workfront Fusion
exl-id: b43355ed-9329-4080-8e61-7177eb580994
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '558'
ht-degree: 0%

---

# 在[!DNL Adobe Workfront Fusion]中新增篩選器至基本情境

>[!IMPORTANT]
>
>Adobe Workfront Fusion檔案已移至新位置。
>
>本文資訊可在以下文章中找到：
>
>* [將篩選器新增至基本案例](https://experienceleague.adobe.com/docs/workfront-fusion/using/build-practice-scenarios/add-filter-basic-scenario.html)
>
>請更新任何書籤。
>
>本文已不再更新，將於不久將來移除。

篩選可讓您確保您的案例僅在符合某些條件時進展。

在此範例中，您會新增篩選器至情境，以允許只有在請求已提交至特定請求佇列時，才能從請求建立新專案。

此範例修改在[建立基本案例](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md)中建立的案例。

>[!NOTE]
>
>Workfront觸發模組包含篩選器，允許案例只在符合特定條件時啟動。 不過，由於模組間篩選器會用於每個非觸發程式和非Workfront使用案例，因此瞭解如何在模組間使用篩選器非常重要。 此範例針對模組內篩選器可能符合的功能，使用模組間篩選器。

## 先決條件

在執行此程式之前，您必須先建立[建立基本案例](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md)中所述的案例。

## 新增篩選器

### 準備新增篩選器

1. 開啟第一個情境。
1. 在&#x200B;**輸出**&#x200B;區域中，選取`Project`。
您現在應該已選取`ID`、`Name`和`Project`。
1. 按一下「確定」以儲存模組設定。
1. 開啟Workfront。
1. 在Workfront中，找出代表Fusion案例將使用的請求佇列的專案。

   此專案必須位於為Fusion連線設定的Workfront帳戶中。

1. 在URL中記下專案ID。

   範例： https://\&lt;MyDomain\>.my.workfront.com/project/\&lt;ProjectID\>/tasks

### 新增並設定篩選器

1. 在案例編輯器中開啟案例。
1. 按一下第一個模組和第二個模組之間的扳手圖示![扳手圖示](assets/wrench-icon.png)，然後選取&#x200B;**設定篩選器**。
1. 在「標籤」欄位中，輸入此篩選的標籤，例如「篩選請求佇列」。
1. 在&#x200B;**條件**&#x200B;區域中，在頂端欄位中，從第一個模組對應`projectID`。

   ![對應專案識別碼](assets/map-proj-id.png)
1. 將&#x200B;**條件**&#x200B;運運算元保留為Equal to。
1. 在&#x200B;**條件**&#x200B;區域的底部欄位中，貼上您在[準備新增篩選器](#prepare-to-add-the-filter)的專案URL中記下的專案ID。
1. 按一下&#x200B;**確定**&#x200B;以儲存篩選設定。

### 測試並啟動

1. 前往Fusion所連線的Workfront環境，並將問題新增至您在篩選中指定的專案。 將另一個問題新增至其他專案。
1. 按一下案例編輯器左下角的&#x200B;**[!UICONTROL 執行一次]**。
1. 檢查輸出，確保案例如預期般執行。

   這兩個問題都應該出現在第一個案例的輸出中，但只有指定專案中的問題應該作為第二個案例的輸入出現，
1. 當您滿意情境如預期般運作時，請按一下畫面左下角的&#x200B;**排程**&#x200B;切換開關至&#x200B;**開啟**。

   這會啟用情境。
1. 在[!DNL Workfront Fusion]中，按一下左下角附近的&#x200B;**[!UICONTROL 儲存]**，以儲存您的情境進度。

   >[!IMPORTANT]
   >
   >隨時儲存並測試情境。

## 資源

* 如需篩選的詳細資訊，請參閱[將篩選新增至情境](/help/quicksilver/workfront-fusion/scenarios/add-a-filter-to-a-scenario.md)。
