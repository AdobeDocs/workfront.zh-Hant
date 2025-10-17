---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: 從展示板中刪除或封存卡片
description: 當您從展示板中刪除卡片時，該卡片將會永久刪除且無法還原。 封存卡片會將卡片傳送至封存，您稍後可以將其還原至展示板。
author: Jenny
feature: Agile
exl-id: 68b7d2e5-92f0-462d-8122-eaecb1e6b87c
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '516'
ht-degree: 1%

---

# 從展示板中刪除或封存卡片

當您從展示板中刪除臨機卡時，該卡片將會永久刪除且無法還原。 連線的卡片在刪除後，可以手動新增回展示板。

如果您從動態展示板中刪除已連線的卡片，當您重新整理展示板時，它會重新出現，因為此展示板型別會從特定專案中拉入所有任務和問題。 若要刪除卡片，您必須從Workfront專案中刪除已連線的任務或問題。

當您從任何其他具有輸入欄的展示板型別中刪除已連線的卡片時，如果連線的工作或問題尚未標籤為完成，則當您重新整理展示板時，該卡片將重新出現在輸入欄中。 如需輸入資料行的詳細資訊，請參閱[將輸入資料行新增到展示板](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md)。

封存卡片會將卡片傳送至封存，您稍後可以將其還原至展示板。

封存的卡片不會同步至Workfront任務和問題。 如果您還原卡片，它將再次同步。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront套件</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td> 
   <p>投稿人或以上</p> 
   <p>要求或更高版本</p>
   </td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 從展示板中刪除卡片

{{step1-to-boards}}

1. 存取展示板。 如需詳細資訊，請參閱[建立或編輯展示板](../../agile/get-started-with-boards/create-edit-board.md)。
1. 按一下卡片上的&#x200B;**[!UICONTROL 更多]**&#x200B;功能表![更多](assets/more-icon-spectrum.png)，然後選取&#x200B;**[!UICONTROL 刪除]**。
1. 按一下確認訊息上的&#x200B;**[!UICONTROL 刪除]**。

## 從展示板封存卡片

1. 存取展示板。
1. 按一下卡片上的&#x200B;**[!UICONTROL 更多]**&#x200B;功能表![更多](assets/more-icon-spectrum.png)，然後選取&#x200B;**[!UICONTROL 封存]**。

   已封存的卡片會隱藏在展示板上，除非您套用篩選器來顯示它們。 如需詳細資訊，請參閱本文中的[篩選展示板以顯示封存的卡片](#filter-a-board-to-show-archived-cards)。

   已封存的卡片上會出現[!UICONTROL 封存]圖示![封存](assets/archive-icon-spectrum-25x20.png)。 您無法編輯已封存的卡片，但可以將其刪除或移至其他欄。

1. 若要還原已封存的卡片，請按一下卡片上的&#x200B;**[!UICONTROL 更多]**&#x200B;功能表![更多](assets/more-icon-spectrum.png)，然後選取&#x200B;**[!UICONTROL 還原]**。

## 篩選展示板以顯示已封存的卡片

依預設，電路板上只會顯示作用中的卡片。 您可以篩選展示板以顯示任何已封存的卡片。

1. 存取展示板。
1. 按一下主機板右側的&#x200B;[!UICONTROL **[設定]**]&#x200B;以開啟[設定]面板。
1. 展開&#x200B;[!UICONTROL **卡片**]。
1. 開啟&#x200B;[!UICONTROL **在展示板上顯示封存的卡片**]。
1. 按一下&#x200B;[!UICONTROL **篩選器**]，展開[!UICONTROL 已封存的卡片]區段，然後選取&#x200B;**[!UICONTROL 已封存的卡片]**&#x200B;以顯示任何已封存的卡片。

   篩選器會顯示已封存的卡片數量。

   ![篩選已封存的卡片](assets/filter-by-archived-cards.png)

   >[!NOTE]
   >
   >如果您尚未開啟顯示已封存卡片的組態設定，則篩選器中無法使用[!UICONTROL 已封存卡片]區段。 如需詳細資訊，請參閱[自訂卡片上顯示的欄位](/help/quicksilver/agile/get-started-with-boards/customize-fields-on-card.md)。

1. 再次選取&#x200B;**[!UICONTROL 已封存的卡片]**&#x200B;以清除選項並僅顯示作用中的卡片。
