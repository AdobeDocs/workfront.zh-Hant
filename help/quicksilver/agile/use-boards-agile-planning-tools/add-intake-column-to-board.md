---
content-type: overview
product-area: agile-and-teams
navigation-topic: agile-navigation-topic
title: 向展示板新增進紙欄
description: 您可以選擇將取用欄新增至展示板，根據您定義的篩選條件，根據在Workfront中新增的任務和問題，自動提取作為已連線卡片的問題。
author: Lisa
feature: Agile
exl-id: 4991f4f7-6f3d-4e15-ae8d-96433ed46557
source-git-commit: 0bcd7cbe43a03216dddabb173aa5888b97cffd23
workflow-type: tm+mt
source-wordcount: '765'
ht-degree: 0%

---

# 向展示板新增進紙欄

您可以選擇在展示板中新增進入欄，以在新增任務和問題時，自動提取連線卡 [!DNL Workfront]，根據您定義的篩選器。 進貨欄可以用作看板小組的積壓欄、支援小組查看問題在添加到請求隊列時的進貨位置，或您需要的任何其他用途。

展示板上只允許使用一個進入欄，且一律顯示為最左側的欄。

入職人數限制為300項任務和300項問題。 它們會依項目上定義的優先順序排序。 如需優先順序的相關資訊，請參閱 [更新任務優先順序](/help/quicksilver/manage-work/tasks/task-information/task-priority.md) 和 [更新問題優先順序](/help/quicksilver/manage-work/issues/issue-information/update-issue-priority.md).

如需欄的詳細資訊，請參閱 [管理展示板欄](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md). 有關已連接卡的資訊，請參閱 [在主板上使用連接的卡](/help/quicksilver/agile/get-started-with-boards/connected-cards.md).

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 計劃*</strong></td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 授權*</strong></td> 
   <td> <p>[!DNL Request] 或更高</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的 [!DNL Workfront] 管理員。

## 建立進氣列

1. 按一下 **[!UICONTROL 主菜單]** 圖示 ![主菜單](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **[!UICONTROL 展示板]**.
1. 存取展示板。 如需詳細資訊，請參閱 [建立或編輯展示板](../../agile/get-started-with-boards/create-edit-board.md).
1. 按一下 **[!UICONTROL 設定]** ，開啟「設定」面板。
1. 展開 **[!UICONTROL 展示板]**.
1. 開啟 **[!UICONTROL 動態吸入要登記的項目]**.

   ![建立進氣列](assets/create-intake-column2.png)

   進料柱在板的左側添加。 在您套用篩選器之前，它會保留為空白。

1. 按一下 **[!UICONTROL 篩選來源]** 選取 **[!UICONTROL 工作]** 或 **[!UICONTROL 問題]**.

   >[!NOTE]
   >
   >您可以篩選進項欄以同時包含任務和問題，但必須針對每個對象類型分別設定篩選器。
   >
   >此外，儲存的篩選器和系統預設篩選器也可供您選取。

1. 在篩選面板上，按一下 **[!UICONTROL 新篩選器]** 開始使用。

   ![按一下「新增篩選器」](assets/intake-filter-dialog5.png)

1. 建置篩選器，然後按一下 **[!UICONTROL 另存為新]**.

   ![篩選產生器](assets/intake-filter-dialog6.png)

   此範例顯示狀態為 [!UICONTROL 新增] 或 [!UICONTROL 進行中]，並指派給我。

   如需建立篩選器的詳細資訊，請參閱文章中的「在測試版產生器中建立或編輯篩選器」一節 [在中建立或編輯篩選器 [!DNL Adobe Workfront]](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-filters.md).

1. 為篩選器命名，然後按一下 **[!UICONTROL 儲存]**.

   ![輸入篩選器的名稱](assets/intake-filter-dialog7.png)

   為篩選器指定唯一名稱，可讓您稍後搜尋。

1. 該篩選器會顯示在已保存的篩選器清單中，並自動應用於進氣列。 按一下篩選面板頂端的X以關閉它。

   ![儲存的篩選](assets/intake-filter-dialog8.png)

1. （選用）若要與他人共用篩選器，請將滑鼠指標暫留在儲存的篩選器上，按一下 **[!UICONTROL 更多]** 功能表 ![「更多」菜單表徵圖](assets/more-icon-spectrum.png)，然後選取 **[!UICONTROL 共用]**. 在「篩選」共用方塊中選擇要共用的使用者或團隊。 如需詳細資訊，請參閱 [共用篩選、檢視或分組](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/share-filter-view-grouping.md).
1. （可選）若要同時納入取用欄的任務和問題，請按一下 **[!UICONTROL 篩選來源]** 並選擇另一個對象以建立另一個篩選器。
1. 新增篩選器後，請檢閱進項欄，確認是否出現正確的工作和問題。

   ![輸入欄](assets/intake-column-added3.png)

   進入欄中的資訊卡必須移至其他展示板欄，才能編輯。 您可以按一下資訊卡，在唯讀檢視中開啟，或按一下 ![開啟任務或問題](assets/boards-launch-icon.png) 在新瀏覽器頁簽中開啟任務或問題。

   >[!NOTE]
   >
   >卡片在進入欄中的唯讀檢視，只能透過的早期功能選擇加入 [!DNL Workfront] [!UICONTROL 展示板].

   您可以手動重新排序進氣列上的項目。

   進入欄右上角的圖示會顯示目前欄中的卡片數，以及套用的篩選器數。

   >[!NOTE]
   >
   >您可以隨時開啟「設定」面板，按一下 **[!UICONTROL 篩選來源]**，然後選取 **[!UICONTROL 工作]** 或 **[!UICONTROL 問題]**.

1. （可選）要搜索進氣列中的項目，請按一下 ![搜尋圖示](assets/search-icon.png) 欄。
1. （可選）若要將卡片從卡入欄移至另一欄，請將卡片拖放至您要顯示的位置。

   或

   按一下 **[!UICONTROL 更多]** 功能表 ![「更多」菜單表徵圖](assets/more-icon-spectrum.png) 在「 」卡片上，然後選取 **[!UICONTROL 移動]**. 然後，在 **[!UICONTROL 移動項目]** 框，選擇另一列並選擇 **[!UICONTROL 移動]**.

1. （可選）若要刪除攝入欄，請按一下 **[!UICONTROL 更多]** 功能表 ![「更多」菜單表徵圖](assets/more-icon-spectrum.png) 選取 **[!UICONTROL 刪除]**.
