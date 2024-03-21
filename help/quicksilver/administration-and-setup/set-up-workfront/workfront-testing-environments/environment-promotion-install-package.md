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
source-git-commit: 610469811a937fde70a938af829b156e69cca391
workflow-type: tm+mt
source-wordcount: '357'
ht-degree: 0%

---

# 安裝環境升級套件


1. 前往您要安裝套件的環境。 這是您複製物件的環境 **至**.
1. 按一下 **[!UICONTROL 主要功能表]** 圖示 ![主要功能表](/help/_includes/assets/main-menu-icon.png) 在Adobe Workfront的右上角，或（如果有的話）按一下 **[!UICONTROL 主要功能表]** 圖示 ![主要功能表](/help/_includes/assets/main-menu-icon-left-nav.png) 然後按一下「 」 **[!UICONTROL 設定]** ![「設定」圖示](/help/_includes/assets/gear-icon-setup.png).
1. 選取 **系統** 在左側導覽中，然後選取 **環境升級**.
1. 從顯示的清單中選取封裝。
1. 若要安裝套件，請按一下 **安裝** 在畫面的右上角。
1. 將套件中的每個物件對應至目標環境中對應的物件。

   如需詳細資訊，請參閱 [對應](#mapping) 本文章


## 對應

每個物件型別都會列在左側導覽和卡片上。 卡片會顯示該型別的物件，以及這些物件是否存在於目標環境中。 您可以決定如何將這些物件移動到目標環境。

* 新建：在目標環境中建立新物件。 如果物件存在於目標環境中，您可以建立具有新名稱的新物件。 如果目標環境中不存在該物件，您可以用新名稱或物件在封裝中的名稱來建立物件。
* 使用現有：未安裝套件中的物件，且目標環境中已存在的物件未變更。
* 覆寫現有： （目前無法使用）封裝中的物件會取代目標環境中的現有物件。
* 請勿使用：套件中的物件未安裝在目標環境中。 如果您選取「不使用」，則會出現一則錯誤訊息，詳細說明此選擇將如何影響其他物件或欄位。

預設值為 `Create new` 如果物件不存在於目標環境中，且 `Use existing` 如果物件確實存在於目標環境中。 您可以按一下「 」，還原為預設的對應 **重設為預設對應**.



<!--
## Collisions

A collision occurs when <!--???--.

In Workfront, a potential collision is marked with a blue dot. You can select 

You can select whether to show all package contents, or collisions only.

## Comparison tool

-->
