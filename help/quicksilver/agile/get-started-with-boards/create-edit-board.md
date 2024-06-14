---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: 建立或編輯展示板
description: 從 [!UICONTROL 展示板] 圖示板，您可以建立新電路板或編輯現有電路板。
author: Lisa
feature: Agile
exl-id: 5f755177-c8ea-4509-a34f-57ffcfd8ba7f
source-git-commit: e896d156854c6729e5ea0a82dcbc641fbfa9415e
workflow-type: tm+mt
source-wordcount: '813'
ht-degree: 1%

---

# 建立或編輯展示板

<!-- Audited: 12/2023 -->

從 [!UICONTROL 展示板] 圖示板，您可以建立新電路板或編輯現有電路板。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計劃</td> 
   <td> <p>任何</p> </td> 
  </tr> 
    <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權</td> 
   <td> <p>新增：投稿人或更高版本 </p>
 <p>或</p> 
<p>目前： [！UICONTROL Request]或以上 </p> 
</td> 
  </tr>
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱 [Workfront檔案中的存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## 建立新展示板

{{step1-to-boards}}

1. 按一下 **[!UICONTROL 新增展示板]**.

1. 選取展示板的範本。

   | 範本 | 說明 |
   |---------|----------|
   | 基本展示板 | 展示板上提供三個預設欄。 您可以新增欄，以及重新命名或刪除預設欄。 <p>展示板上提供三個預設欄。 您可以新增欄，以及重新命名或刪除預設欄。 |
   | Kanban 展示板 | 展示板上提供下列欄：「待處理專案」、「新增」、「進行中」、「完成」和「保留」。 您可以新增欄，以及重新命名或刪除預設欄。<p>若要使用待處理專案，您必須為輸入欄設定篩選器。 如需詳細資訊，請參閱 [將輸入欄新增到展示板](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md). <p>若要複查每一欄的預設原則，請按一下 [!UICONTROL **更多** 功能表] 在欄上並選取 [!UICONTROL **編輯**]. 您可以變更這些預先設定原則中的任何一項。 如需詳細資訊，請參閱 [管理展示板欄](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md). |
   | 追溯展示板 | 展示板上提供下列欄：哪些方面進展順利？ 有哪些可改善？ 我們應該為誰慶祝？ 我們可以做些什麼來加快進度？ 您可以新增欄，以及重新命名或刪除預設欄。 <p>不會套用任何欄原則。 |
   | 動態展示板 | 展示板上提供下列欄：「未選取」、「新增」、「進行中」、「保留」和「完成」。 您可以新增欄，以及重新命名或刪除預設欄。 (未選取欄可以重新命名，但不能刪除。 此欄會保留狀態不符合任何其他欄狀態的所有卡片。) <p>預設欄原則會根據欄的狀態為欄指派卡片。 如需詳細資訊，請參閱 [管理展示板欄](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md). |

1. 僅適用於動態主機板，請遵循設定精靈步驟：

   1. 輸入展示板的名稱，然後按一下 [!UICONTROL **下一個**].
   1. 搜尋並選取 [!DNL Workfront] [!UICONTROL **專案**] 將任務和問題帶入討論區。
   1. 搜尋並選取 [!UICONTROL **指定任務**] 將任務和問題帶入討論區。

      所有物件都會以連線的卡片形式顯示在展示板上。

      此 [!UICONTROL **正在新增的卡片**] 計數器會顯示展示板上有多少張卡片。 例如，如果您選取包含100個任務和問題的專案，計數器會顯示100。 如果您新增使用者指派，且該人員指派至專案上的5個任務，則計數器會顯示5。

      >[!NOTE]
      >
      >動態主機板的卡片限製為700個任務和700個問題，總共1,400張卡片。 主機板上的卡片數量過多可能會影響主機板效能。

   1. （選用）選取 [!UICONTROL **不要封存完成的卡片**] 將已完成的任務和問題帶入展示板，在「已完成」欄中顯示卡片。 未選取此選項時，建立展示板時完成的卡片會作為封存卡片帶入展示板上。

      >[!NOTE]
      >
      >預設情況下，已封存的卡片不會顯示在展示板上。 若要顯示封存的卡片，您必須開啟組態設定，然後篩選展示板以顯示封存的卡片。 如需詳細資訊，請參閱 [自訂要在卡片上顯示的欄位](/help/quicksilver/agile/get-started-with-boards/customize-fields-on-card.md) 和 [在展示板中篩選和搜尋](/help/quicksilver/agile/get-started-with-boards/filter-search-in-board.md).

   1. （選用）按一下 [!UICONTROL **使用進階篩選**] 以顯示其他篩選選項。

      此程式與在輸入欄上建立篩選器的程式相同。 如需詳細資訊，請參閱 [將輸入欄新增到展示板](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md).

      如果您在建立動態展示板後更新其上的篩選器，則未納入Workfront任務或問題的卡片設定（例如標籤）會重設。

   1. 新增篩選器後，按一下 [!UICONTROL **建立展示板**].

1. 在「 」中輸入展示板的名稱 **[!UICONTROL 展示板]** 欄位並按Enter。
1. 視需要設定主機板。

   如需詳細資訊，請參閱 [從展示板新增或移除成員](../../agile/get-started-with-boards/add-members-to-board.md)， [管理展示板欄](../../agile/get-started-with-boards/manage-board-columns.md)， [新增臨機卡到展示板](../../agile/get-started-with-boards/add-card-to-board.md)、和 [在展示板上使用連線的卡片](/help/quicksilver/agile/get-started-with-boards/connected-cards.md).

1. 按一下 **[!UICONTROL 所有展示板]** 以返回面板儀表板。

   您也可以找到標示為目前主機板名稱的下拉式功能表，然後按一下該功能表以切換至另一個主機板。

   ![展示板清單](assets/boards-button-list-of-boards-350x188.png)

## 編輯現有展示板

{{step1-to-boards}}

1. 在控制面板上，選取要開啟的面板。
1. 視需要編輯展示板。 您可以按一下電路板名稱來重新命名。

   如需詳細資訊，請參閱 [從展示板新增或移除成員](../../agile/get-started-with-boards/add-members-to-board.md)， [管理展示板欄](../../agile/get-started-with-boards/manage-board-columns.md)、和 [將卡片新增到展示板](../../agile/get-started-with-boards/add-card-to-board.md).

1. 按一下 **[!UICONTROL 所有展示板]** 以返回面板儀表板。

   您也可以找到標示為目前主機板名稱的下拉式功能表，然後按一下該功能表以切換至另一個主機板。

