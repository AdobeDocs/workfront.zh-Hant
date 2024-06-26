---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: 從展示板中刪除或封存卡片
description: 當您從展示板中刪除卡片時，該卡片將會永久刪除且無法還原。 封存卡片會將卡片傳送至封存，您稍後可以將其還原至展示板。
author: Lisa
feature: Agile
exl-id: 68b7d2e5-92f0-462d-8122-eaecb1e6b87c
source-git-commit: 46099e6ceba4310453743c023823e8952f5ce553
workflow-type: tm+mt
source-wordcount: '505'
ht-degree: 0%

---

# 從展示板中刪除或封存卡片

當您從展示板中刪除臨機卡時，該卡片將會永久刪除且無法還原。 連線的卡片在刪除後，可以手動新增回展示板。

如果您從動態展示板中刪除已連線的卡片，當您重新整理展示板時，它會重新出現，因為此展示板型別會從特定專案中拉入所有任務和問題。 若要刪除卡片，您必須從Workfront專案中刪除已連線的任務或問題。

當您從任何其他具有輸入欄的展示板型別中刪除已連線的卡片時，如果連線的工作或問題尚未標籤為完成，則當您重新整理展示板時，該卡片將重新出現在輸入欄中。 如需輸入欄的詳細資訊，請參閱 [將輸入欄新增到展示板](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md).

封存卡片會將卡片傳送至封存，您稍後可以將其還原至展示板。

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 計畫*</strong></td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 授權*</strong></td> 
   <td> <p>[！UICONTROL Request]或更高版本</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的 [!DNL Workfront] 管理員。

## 從展示板中刪除卡片

1. 按一下 **[!UICONTROL 主要功能表]** 圖示 ![](assets/main-menu-icon.png) 位於的右上角 [!DNL Adobe Workfront]，然後按一下 **[!UICONTROL 展示板]**.
1. 存取展示板。 如需詳細資訊，請參閱 [建立或編輯展示板](../../agile/get-started-with-boards/create-edit-board.md).
1. 按一下 **[!UICONTROL 更多]** 功能表 ![更多選單](assets/more-icon-spectrum.png) ，然後選取「 」 **[!UICONTROL 刪除]**.
1. 按一下 **[!UICONTROL 刪除]** 於確認訊息上。

## 從展示板封存卡片

1. 存取展示板。
1. 按一下 **[!UICONTROL 更多]** 功能表 ![更多選單](assets/more-icon-spectrum.png) ，然後選取「 」 **[!UICONTROL 封存]**.

   已封存的卡片會隱藏在展示板上，除非您套用篩選器來顯示它們。 如需詳細資訊，請參閱 [篩選展示板以顯示已封存的卡片](#filter-a-board-to-show-archived-cards) 本文章內容。

   一個 [!UICONTROL 封存] 圖示 ![封存](assets/archive-icon-spectrum-25x20.png) 會顯示在已封存的卡片上。 您無法編輯已封存的卡片，但可以將其刪除或移至其他欄。

1. 若要還原已封存的卡片，請按一下 **[!UICONTROL 更多]** 功能表 ![更多選單](assets/more-icon-spectrum.png) 在卡片上，然後選取 **[!UICONTROL 還原]**.

## 篩選展示板以顯示已封存的卡片 {#filter-a-board-to-show-archived-cards}

依預設，電路板上只會顯示作用中的卡片。 您可以篩選展示板以顯示任何已封存的卡片。

1. 存取展示板。
1. 按一下 [!UICONTROL **設定**] ，以開啟「設定」面板。
1. 展開 [!UICONTROL **卡片**].
1. 開啟 [!UICONTROL **在展示板上顯示已封存的卡片**].
1. 按一下 [!UICONTROL **篩選**]，展開 [!UICONTROL 已封存的卡片] 部分，然後選取 **[!UICONTROL 已封存的卡片]** 以顯示任何已封存的卡片。

   篩選器會顯示已封存的卡片數量。

   ![篩選已封存的卡片](assets/filter-by-archived-cards.png)

   >[!NOTE]
   >
   >此 [!UICONTROL 已封存的卡片] 如果您未開啟顯示封存卡片的組態設定，則區段在篩選中無法使用。 如需詳細資訊，請參閱 [自訂要在卡片上顯示的欄位](/help/quicksilver/agile/get-started-with-boards/customize-fields-on-card.md).

1. 選取 **[!UICONTROL 已封存的卡片]** 再次清除選項並僅顯示作用中的卡片。
