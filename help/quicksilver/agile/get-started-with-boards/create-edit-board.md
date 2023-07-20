---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: 建立或編輯展示板
description: 從 [!UICONTROL 展示板] 圖示板，您可以建立新電路板或編輯現有電路板。
author: Lisa
feature: Agile
exl-id: 5f755177-c8ea-4509-a34f-57ffcfd8ba7f
source-git-commit: a4ccd48956fedbafc04ce19198592efdad49e5a3
workflow-type: tm+mt
source-wordcount: '721'
ht-degree: 3%

---

# 建立或編輯展示板

從 [!UICONTROL 展示板] 圖示板，您可以建立新電路板或編輯現有電路板。

若要將展示板新增至工作流程，請參閱 [管理工作流程](/help/quicksilver/agile/use-boards-agile-planning-tools/manage-collections.md).

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 計劃*</strong></td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 授權*</strong></td> 
   <td> <p>[！UICONTROL Request]或更高版本</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有哪些計畫、授權型別或存取權，請聯絡您的 [!DNL Workfront] 管理員。

## 建立新展示板

1. 按一下 **[!UICONTROL 主要功能表]** 圖示 ![](assets/main-menu-icon.png) 右上角的 [!DNL Adobe Workfront]，然後按一下 **[!UICONTROL 展示板]**.
1. 若要建立獨立主機板，請按一下 **[!UICONTROL 新增展示板]** 在 [!UICONTROL 展示板] 區域。 若要將展示板新增至工作流程，請參閱 [管理工作流程](/help/quicksilver/agile/use-boards-agile-planning-tools/manage-collections.md).

1. 選取展示板的範本。

   | 範本 | 說明 |
   |---------|----------|
   | 基本展示板 | 展示板上提供了三個預設欄。 您可以新增欄並重新命名或刪除預設欄。 <p>展示板上提供了三個預設欄。 您可以新增欄並重新命名或刪除預設欄。 |
   | Kanban 展示板 | 展示板上提供下列欄位：「待處理專案」、「新增」、「進行中」、「完成」和「保留」。 您可以新增欄並重新命名或刪除預設欄。<p>若要使用待處理專案，您必須為輸入欄設定篩選器。 如需詳細資訊，請參閱 [將輸入欄新增到展示板](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md). <p>若要複查每欄的預設原則，請按一下 [!UICONTROL **更多** 功能表] 在欄上並選取 [!UICONTROL **編輯**]. 您可以變更這些預先設定原則中的任何一項。 如需詳細資訊，請參閱 [管理展示板欄](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md). |
   | 追溯展示板 | 展示板上提供下列欄：哪些專案進展順利？ 有哪些可以改進的地方? 我們應該為誰慶祝? 我們可以做些什麼來加快進度? 您可以新增欄並重新命名或刪除預設欄。 <p>未套用任何欄原則。 |
   | 動態展示板 | 展示板上提供下列欄：「未選取」、「新增」、「進行中」、「保留」和「完成」。 您可以新增欄並重新命名或刪除預設欄。 (未選取欄可以重新命名，但不能刪除。 此欄包含狀態不符合任何其他欄狀態的所有卡片。) <p>預設欄原則會根據其狀態為欄指派卡片。 如需詳細資訊，請參閱 [管理展示板欄](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md). |

1. 僅適用於動態主機板，請遵循設定精靈步驟：

   1. 搜尋並選取 [!DNL Workfront] [!UICONTROL **專案**] 將任務和問題帶入展示板。
   1. 搜尋並選取 [!UICONTROL **指定任務**] 將任務和問題帶入展示板。

      所有物件都會以連線的卡片形式顯示在展示板上。

      此 [!UICONTROL **正在新增的卡片**] 計數器會顯示展示板上有多少張卡片。 例如，如果您選取一個具有100個任務和問題的專案，計數器會顯示100。 如果您新增使用者指派，並且該人員被指派到專案上的5個任務，則計數器顯示5。

   1. （選用）選取 [!UICONTROL **包含已完成的工作**] 將完成的卡片加入展示板中。

      >[!NOTE]
      >
      >如果未選取此選項，則當處於其他狀態的卡片標籤為完成時，它們將「從」展示板上「掉落」，並且不再顯示。

   1. （可選）按一下 [!UICONTROL **使用進階篩選**] 以顯示其他篩選選項。

      此程式與在輸入欄上建立篩選器相同。 如需詳細資訊，請參閱 [將輸入欄新增到展示板](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md).

   1. 新增篩選器後，按一下 [!UICONTROL **建立展示板**].

1. 在「 」中輸入展示板的名稱 **[!UICONTROL 展示板]** 欄位並按Enter。
1. 視需要設定主機板。

   如需詳細資訊，請參閱 [從展示板新增或移除成員](../../agile/get-started-with-boards/add-members-to-board.md)， [管理展示板欄](../../agile/get-started-with-boards/manage-board-columns.md)， [新增臨機卡到展示板](../../agile/get-started-with-boards/add-card-to-board.md)、和 [在展示板上使用連線的卡片](/help/quicksilver/agile/get-started-with-boards/connected-cards.md).

1. 按一下 **[!UICONTROL 所有展示板]** 以返回面板儀表板。

   您也可以找到標示為目前主機板名稱的下拉式選單，然後按一下該選單以切換至另一個主機板。

   ![展示板清單](assets/boards-button-list-of-boards-350x188.png)

## 編輯現有展示板

1. 按一下 **[!UICONTROL 主要功能表]** 圖示 ![](assets/main-menu-icon.png) 右上角的 [!DNL Adobe Workfront]，然後按一下 **[!UICONTROL 展示板]**.
1. 在圖示板上，選取要開啟的面板。
1. 視需要編輯展示板。 您可以按一下電路板名稱來重新命名。

   如需詳細資訊，請參閱 [從展示板新增或移除成員](../../agile/get-started-with-boards/add-members-to-board.md)， [管理展示板欄](../../agile/get-started-with-boards/manage-board-columns.md)、和 [新增卡片至展示板](../../agile/get-started-with-boards/add-card-to-board.md).

1. 按一下 **[!UICONTROL 所有展示板]** 以返回面板儀表板。

   您也可以找到標示為目前主機板名稱的下拉式選單，然後按一下該選單以切換至另一個主機板。
