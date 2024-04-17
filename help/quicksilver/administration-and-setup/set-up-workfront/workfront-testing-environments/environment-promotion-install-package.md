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
source-git-commit: f65fbe7ceab19cee75aa0346c389907707c47c8b
workflow-type: tm+mt
source-wordcount: '401'
ht-degree: 0%

---

# 安裝環境升級套件

>[!NOTE]
>
>若要安裝套件，您必須登入要安裝套件的環境。 這是您要複製物件的環境 **至**.

1. 前往您要安裝套件的環境。
1. 按一下 **[!UICONTROL 主要功能表]** 圖示 ![主要功能表](/help/_includes/assets/main-menu-icon.png) 在Adobe Workfront的右上角，或（如果有的話）按一下 **[!UICONTROL 主要功能表]** 圖示 ![主要功能表](/help/_includes/assets/main-menu-icon-left-nav.png) 然後按一下「 」 **[!UICONTROL 設定]** ![「設定」圖示](/help/_includes/assets/gear-icon-setup.png).
1. 選取 **系統** 在左側導覽中，然後選取 **環境升級**.
1. 從顯示的清單中選取封裝。
1. 對於每個有衝突的物件，請選取如何解決衝突。

   若要解決衝突，請按一下物件型別旁邊的下拉箭頭，然後選取您要採取的動作。

   如需詳細資訊，請參閱 [衝突](#collisions) 本文章
1. 若要將套件部署至新環境，請按一下 **部署** 在畫面的右上角。

## 衝突

當屬於安裝套裝軟體的物件已經存在於目標環境中時，就會發生衝突。 發生此情況時，您可以選取如何解決衝突。 衝突會在物件層級上解決。

您可以按一下每個物件型別旁的下拉式清單來檢視衝突。 衝突會顯示在「衝突」欄中。

若要解決衝突，請在「建置動作」欄中選取動作，或使用已顯示的預設動作。

* **以新名稱建立**：在目標環境中建立新物件。 如果物件存在於目標環境中，您可以建立具有新名稱的新物件。 如果目標環境中不存在該物件，您可以用新名稱或物件在封裝中的名稱來建立物件。
* **使用現有**：未安裝套件中的物件，且目標環境中已存在的物件未變更。
* **覆寫**：套件中的物件會取代目標環境中的現有物件。
<!--
* Do not use: The object in the package is not installed in the target environment. If you select Do not use, an error message will appear detailing how this choice will affect other objects or fields.
-->

預設值為 `Create new` 如果物件不存在於目標環境中，且 `Use existing` 如果物件確實存在於目標環境中。 您可以按一下「 」，還原為預設的對應 **重設為預設對應**.



<!--
## Collisions

A collision occurs when <!--???--.

In Workfront, a potential collision is marked with a blue dot. You can select 

You can select whether to show all package contents, or collisions only.

## Comparison tool

-->
