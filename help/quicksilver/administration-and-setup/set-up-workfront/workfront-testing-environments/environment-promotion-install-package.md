---
user-type: administrator
content-type: how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: 安裝環境升級套件
description: 環境推進功能旨在提供與組態相關的物件從一個環境移動到另一個環境的功能。 瞭解如何將環境升級套件安裝至目標環境。
author: Becky
feature: System Setup and Administration
role: Admin
hide: true
hidefromtoc: true
recommendations: noDisplay, noCatalog
exl-id: fe213fe7-5bb8-479c-926b-761cbdd7ba4e
source-git-commit: 66b9fc84c18bce2d0cecee9368a125570c822a54
workflow-type: tm+mt
source-wordcount: '717'
ht-degree: 0%

---

# 安裝環境升級套件

建立套件後，您可以在不同的環境中安裝它。

## 先決條件

您必須先建立封裝，才能進行安裝。

如需指示，請參閱 [建立或編輯環境升級套件](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-create-package.md).

## 安裝的封裝狀態

套件必須處於「作用中」狀態才能安裝在生產環境中。

我們建議將套件移至TESTING狀態，並安裝在另一個沙箱中測試套件。  如果此測試成功，且沒有錯誤，請將套件移至「作用中」以將其安裝在生產環境中。

若要編輯套裝程式的狀態：

1. 選取套裝，如所述  [編輯或組合現有套件](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-create-package.md#create-or-edit-an-environment-promotion-package) 在建立並編輯環境升級套件一文中。
1. 按一下 **編輯套裝**.
1. 按一下 **狀態**.
1. 從下拉式選單中選取所需的狀態。

如需狀態的詳細資訊，請參閱 [環境升級狀態](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-in-wf.md#environment-promotion-statuses) 在文章中，概述如何在Workfront環境之間移動物件。

## 安裝套件

>[!NOTE]
>
>* 若要安裝套件，您必須登入要安裝套件的環境。 這是您複製物件的環境 **至**.

1. 前往您要安裝套件的環境。
1. 按一下 **[!UICONTROL 主要功能表]** 圖示 ![主要功能表](/help/_includes/assets/main-menu-icon.png) 在Adobe Workfront的右上角，或（如果有的話）按一下 **[!UICONTROL 主要功能表]** 圖示 ![主要功能表](/help/_includes/assets/main-menu-icon-left-nav.png) 然後按一下「 」 **[!UICONTROL 設定]** ![「設定」圖示](/help/_includes/assets/gear-icon-setup.png).
1. 選取 **系統** 在左側導覽中，然後選取 **環境升級**.
1. 從顯示的清單中選取封裝。
1. 對於每個有衝突的物件，請選取如何解決衝突。

   若要解決衝突，請按一下物件型別旁邊的下拉箭頭，然後選取您要執行的動作。

   如需詳細資訊，請參閱 [衝突](#collisions) 本文章
1. 若要將套件部署至新環境，請按一下 **部署** 在畫面的右上角。

## 衝突

當屬於安裝套裝軟體一部分的物件與目標環境中已存在的物件同名時，就會發生衝突。 發生此情況時，您可以選取如何解決衝突。 衝突會在物件層級上解決。

您可以按一下每個物件型別旁的下拉式清單來檢視衝突。 衝突會顯示在「衝突」欄中。

若要解決衝突，請在「建置動作」欄中選取動作，或使用已顯示的預設動作。

* **以新名稱建立**：在目標環境中建立新物件。 如果物件存在於目標環境中，您可以建立具有新名稱的新物件。 如果目標環境中不存在該物件，您可以用新名稱或物件在封裝中的名稱來建立物件。
* **使用現有**：未安裝套件中的物件，且目標環境中已存在的物件未變更。
* **覆寫**：套件中的物件會取代目標環境中的現有物件。

  即使未偵測到衝突，您也可以選擇要覆寫的物件。

  如需有關覆寫如何影響父物件和子物件的詳細資訊，請參閱 [覆寫父物件和子物件](#overwriting-parent-and-child-objects) 本文章內容。
<!--
* Do not use: The object in the package is not installed in the target environment. If you select Do not use, an error message will appear detailing how this choice will affect other objects or fields.
-->

預設值為 `Create new` 如果物件不存在於目標環境中，且 `Use existing` 如果物件確實存在於目標環境中。 您可以按一下「 」，還原為預設的對應 **重設為預設對應**.

## 覆寫父物件和子物件

推進封裝中的某些物件可能有子物件。 例如，專案（父項）具有任務（子項）。 覆寫父物件時，子物件的處理方式如下：

* 同時存在於封裝和目標中的子物件將會在目標中更新以符合封裝。
* 將會建立存在於封裝中但不存在於目標的子物件。
* 存在於目標中但不存在於封裝中的子物件將維持不變。

此功能會影響下列父物件和子物件：

| 父物件 | 子物件 |
|---|---|
| 專案 | 任務<br>QueueDef （佇列定義）<br>路由規則 |
| 範本 | 範本任務<br>QueueDef （佇列定義）<br>路由規則 |
| 引數（自訂表單欄位） | ParameterOption （自訂表單欄位選項） |
| 行事曆資訊 | 行事曆區段 |
| QueueDef （佇列定義） | QueueTopicGroup<br>佇列主題 |

