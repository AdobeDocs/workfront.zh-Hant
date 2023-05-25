---
content-type: reference
product-area: agile-and-teams
navigation-topic: boards
title: 管理工作流程
description: 工作流程是一組可設定的展示板和卡片，用於合作處理工作。
author: Lisa
feature: Agile
exl-id: c46c42e8-e14d-414d-b883-c4d885338e42
source-git-commit: 0ccec525069557fdc2a17e37e00968f8fb6d3a41
workflow-type: tm+mt
source-wordcount: '905'
ht-degree: 2%

---

# 管理工作流程

工作流程是一組可設定的展示板和卡片，用於合作處理工作。 工作串流可包含從範本建立的不同型別的展示板，以及工作專案的卡片清單。 在工作流程中，您可以追蹤反複專案或衝刺中的工作。

如需詳細資訊，請參閱 [使用卡片清單](/help/quicksilver/agile/use-boards-agile-planning-tools/use-card-list.md) 和 [在工作串流中建立反複專案](/help/quicksilver/agile/use-boards-agile-planning-tools/create-an-iteration-in-workstream.md).

工作串流會連同您有權存取的個別面板（不屬於工作串流）一起顯示在控制面板上。 有關面板儀表板的資訊，請參閱 [使用面板儀表板](/help/quicksilver/agile/get-started-with-boards/use-boards-page.md). 您可以按一下圖示板上的任何電路板名稱來開啟它。

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

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
   <td> <p>[！UICONTROL Request]或更高版本</p> </td> 
  </tr> 
 </tbody> 
</table>

## 建立工作流程

{{step1-to-boards}}

1. 按一下 **[!UICONTROL 新增工作流程]** 在 [!UICONTROL 工作串流] 圖示板區域。
1. 輸入名稱以取代 **[!UICONTROL 未命名工作流程]** 並按Enter。

   您可以將面板新增至工作流程或按一下 [!UICONTROL **所有展示板**] 以返回控制面板。

## 在工作串流中建立新展示板

1. 如果您尚未在工作流程中，請按一下 [!UICONTROL **檢視工作流程**] ，以開啟現有的工作流程。
1. 按一下 **[!UICONTROL 新增展示板]** 於 [!UICONTROL 展示板] 工作流程的索引標籤。
1. 選取展示板的範本。

| 範本 | 說明 |
|---------|----------|
| 基本展示板 | 展示板上提供了三個預設欄。 您可以新增欄並重新命名或刪除預設欄。 <p>未套用任何欄原則。 |
| Kanban 展示板 | 展示板上提供下列欄位：「待處理專案」、「新增」、「進行中」、「完成」和「保留」。 您可以新增欄並重新命名或刪除預設欄。<p>若要使用待處理專案，您必須為輸入欄設定篩選器。 如需詳細資訊，請參閱 [將輸入欄新增到展示板](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md). <p>若要複查每欄的預設原則，請按一下 [!UICONTROL **更多** 功能表] 在欄上並選取 [!UICONTROL **編輯**]. 您可以變更這些預先設定原則中的任何一項。 如需詳細資訊，請參閱 [管理展示板欄](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md). |
| 追溯展示板 | 展示板上提供下列欄：哪些專案進展順利？ 有哪些可以改進的地方? 我們應該為誰慶祝? 我們可以做些什麼來加快進度? 您可以新增欄並重新命名或刪除預設欄。 <p>未套用任何欄原則。 |
| 疊代程序 | 這是用來定義和執行疊代的展示板。 <p>展示板上提供下列欄位：「待處理專案」、「新增」、「進行中」、「完成」和「保留」。 您無法將任何欄新增到展示板中。 <p>若要複查每欄的預設原則，請按一下 [!UICONTROL **更多**] 功能表並選取 [!UICONTROL **編輯**]. 您可以變更這些預先設定原則中的任何一項。 如需詳細資訊，請參閱 [管理展示板欄](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md). |

如需設定主機板的詳細資訊，請參閱 [建立或編輯展示板](/help/quicksilver/agile/get-started-with-boards/create-edit-board.md).

## 篩選工作流程上的展示板清單

當預設值以外的篩選器套用到電路板清單上時，篩選器圖示上會顯示一個指示器 ![已套用篩選器](assets/boards-filterapplied-30x30.png). 按一下 [!UICONTROL **全部清除**] 以移除所有篩選器，然後按一下 [!UICONTROL **隱藏篩選器**] 以關閉篩選面板。

{{step1-to-boards}}

1. 在控制面板上，按一下 [!UICONTROL **檢視工作流程**] 以開啟工作流程。
1. 按一下 [!UICONTROL **展示板**] 標籤（如果尚未顯示）。
1. 按一下 [!UICONTROL **篩選**].
1. 選取您要依狀態檢視的面板（已封存的面板、作用中的面板或所有面板）。
1. 選取您要依範本檢視的面板。

## 將成員新增至工作流程

必須先將人員和團隊作為成員新增到工作流程中，他們才能檢視工作流程及其內容。 工作流程成員可以新增和移除工作流程上的成員，並檢視哪些面板在工作流程中。

>[!NOTE]
>
>工作流程成員必須先新增為該特定展示板的成員，才能開啟工作流程上的展示板。

{{step1-to-boards}}

1. 在控制面板上，按一下 [!UICONTROL **檢視工作流程**] 以開啟工作流程。
1. 按一下 **[!UICONTROL 新增成員]** 圖示 ![新增成員](assets/boards-addmember-spectrum-25x25.png) 將成員和團隊新增至工作流程。

   此程式與將成員新增至展示板的程式相同。 如需詳細資訊，請參閱 [從展示板新增或移除成員](/help/quicksilver/agile/get-started-with-boards/add-members-to-board.md).

## 將來源新增至工作流程

來源會決定工作流程中卡片的來源。

{{step1-to-boards}}

1. 按一下 [!UICONTROL **來源**] 圖示 ![「來源」圖示](assets/sources-icon.png) 以定義將卡片匯入工作資料流的來源。 目前，唯一可用的來源為 [!DNL Adobe Workfront].
1. 新增篩選器以卡片形式從Workfront匯入任務和問題。

   為工作流程來源新增篩選器，與在基本展示板或Kanban展示板上為輸入欄新增進階篩選器相同。 如需詳細資訊，請參閱 [將輸入欄新增到展示板](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md).

## 設定工作流程

{{step1-to-boards}}

1. 在控制面板上，按一下 [!UICONTROL **檢視工作流程**] 以開啟工作流程。
1. 按一下 [!UICONTROL **設定**] 以開啟 [!UICONTROL 設定工作流程] 面板。
1. （可選）展開 [!UICONTROL **工作流程**] 和輸入工作資料流的說明。 此說明會顯示在控制面板上。
1. （可選）展開 [!UICONTROL **反複專案**] 以定義此工作資料流的反複專案處理。

   卡片總數、所指向的卡片數以及反複專案數都會顯示在「卡片清單」區段中。 按一下 [!UICONTROL **檢視清單**] 以開啟清單並新增卡片。 如需詳細資訊，請參閱 [使用卡片清單](/help/quicksilver/agile/use-boards-agile-planning-tools/use-card-list.md).

   如果已定義反複專案，則會顯示其開始日期、卡片數和點數。 按一下 [!UICONTROL **檢視展示板**] 以開啟反複專案展示板。 如需詳細資訊，請參閱 [在工作串流中建立反複專案](/help/quicksilver/agile/use-boards-agile-planning-tools/create-an-iteration-in-workstream.md).

1. （可選）展開 [!UICONTROL **標籤**] 以將標籤新增至工作流程。 搜尋標籤，或在搜尋方塊中輸入新標簽名稱，然後按Enter建立標籤。
