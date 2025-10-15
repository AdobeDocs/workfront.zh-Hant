---
content-type: reference
product-area: agile-and-teams
navigation-topic: boards
title: 管理工作串流
description: 工作流程是一組可設定的展示板和卡片，用於共同處理工作。
author: Lisa
feature: Agile
exl-id: c46c42e8-e14d-414d-b883-c4d885338e42
source-git-commit: 685177d3a8485aa60d8455e1c329de21cea4abb7
workflow-type: tm+mt
source-wordcount: '934'
ht-degree: 1%

---

# 管理工作流程

>[!IMPORTANT]
>
>工作串流僅適用於特定客戶群組。

工作流程是一組可設定的展示板和卡片，用於共同處理工作。 工作流程可以包含從範本建立的不同版面型別，以及工作專案的卡片清單。 在工作流程中，您可以追蹤反複專案或衝刺中的工作。

如需詳細資訊，請參閱[使用卡片清單](/help/quicksilver/agile/use-boards-agile-planning-tools/use-card-list.md)和[在工作串流中建立反複專案](/help/quicksilver/agile/use-boards-agile-planning-tools/create-an-iteration-in-workstream.md)。

工作串流會與您可以存取的個別面板（不屬於工作串流的一部分）一起顯示在控制面板上。 如需面板儀表板的詳細資訊，請參閱[使用面板儀表板](/help/quicksilver/agile/get-started-with-boards/use-boards-page.md)。 您可以按一下圖示板上的任何電路板名稱來開啟它。

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

## 建立工作流程

{{step1-to-boards}}

1. 按一下儀表板的&#x200B;**[!UICONTROL 工作資料流]**&#x200B;區域中的[!UICONTROL 新增工作資料流]。
1. 輸入名稱以取代&#x200B;**[!UICONTROL 未命名的工作流]**，然後按Enter鍵。

   您可以將面板新增至工作資料流，或按一下「[!UICONTROL **所有面板**]」以返回儀表板。

## 在工作串流中建立新展示板

1. 如果您不在工作流程中，請按一下儀表板上的[檢視工作流程] [!UICONTROL ****]&#x200B;以開啟現有的工作流程。
1. 在工作流的&#x200B;**[!UICONTROL 面板]**&#x200B;索引標籤上按一下[!UICONTROL 新增面板]。
1. 選取展示板的範本。

| 範本 | 說明 |
|---------|----------|
| 基本展示板 | 展示板上提供三個預設欄。 您可以新增欄，以及重新命名或刪除預設欄。 <p>不會套用任何欄原則。 |
| Kanban 展示板 | 展示板上提供下列欄：「待處理專案」、「新增」、「進行中」、「完成」和「保留」。 您可以新增欄，以及重新命名或刪除預設欄。<p>若要使用待處理專案，您必須為輸入欄設定篩選器。 如需詳細資訊，請參閱[將輸入資料行新增到展示板](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md)。 <p>若要檢閱每個欄的預設原則，請按一下欄上的&#x200B;[!UICONTROL **更多**&#x200B;功能表]，然後選取&#x200B;[!UICONTROL **編輯**]。 您可以變更這些預先設定原則中的任何一項。 如需詳細資訊，請參閱[管理展示板資料行](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md)。 |
| 追溯展示板 | 展示板上提供下列欄：哪些方面進展順利？ 有哪些可改善？ 我們應該為誰慶祝？ 我們可以做些什麼來加快進度？ 您可以新增欄，以及重新命名或刪除預設欄。 <p>不會套用任何欄原則。 |
| 疊代程序 | 這是用來定義和執行反複專案的展示板。 <p>展示板上提供下列欄：「待處理專案」、「新增」、「進行中」、「完成」和「保留」。 您無法新增任何欄到展示板。 <p>若要檢閱每個欄的預設原則，請按一下欄上的&#x200B;[!UICONTROL **更多**]&#x200B;功能表，然後選取&#x200B;[!UICONTROL **編輯**]。 您可以變更這些預先設定原則中的任何一項。 如需詳細資訊，請參閱[管理展示板資料行](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md)。 |

如需設定展示板的詳細資訊，請參閱[建立或編輯展示板](/help/quicksilver/agile/get-started-with-boards/create-edit-board.md)。

## 篩選工作流程上的展示板清單

將預設值以外的篩選器套用至展示板清單時，篩選器圖示![已套用篩選器](assets/boards-filterapplied-30x30.png)上會顯示指示器。 按一下[全部清除][!UICONTROL **以移除所有篩選器，然後按一下[隱藏篩選器]**]&#x200B;以關閉篩選器面板。[!UICONTROL ****]

{{step1-to-boards}}

1. 在儀表板上，按一下&#x200B;[!UICONTROL **檢視工作流程**]&#x200B;以開啟工作流程。
1. 如果尚未顯示&#x200B;[!UICONTROL **面板**]&#x200B;標籤，請按一下該標籤。
1. 按一下&#x200B;[!UICONTROL **篩選器**]。
1. 選取您要依狀態檢視的面板（已封存的面板、作用中的面板或所有面板）。
1. 選取您要依範本檢視的面板。

## 將成員新增至工作流程

必須先將人員和團隊作為成員新增到工作流程中，他們才能檢視工作流程及其內容。 工作流程成員可以在工作流程中加入和移除成員，並檢視哪些面板位於工作流程中。

>[!NOTE]
>
>工作流程成員必須先新增到該特定展示板作為成員，才能在工作流程上開啟展示板。

{{step1-to-boards}}

1. 在儀表板上，按一下&#x200B;[!UICONTROL **檢視工作流程**]&#x200B;以開啟工作流程。
1. 按一下&#x200B;**[!UICONTROL 新增成員]**&#x200B;圖示![新增成員](assets/boards-addmember-spectrum-25x25.png)，將成員和團隊新增至工作流程。

   此程式與將成員加入展示板的程式相同。 如需詳細資訊，請參閱[從展示板新增或移除成員](/help/quicksilver/agile/get-started-with-boards/add-members-to-board.md)。

## 將來源新增至工作流程

來源會決定工作流程中卡片的來源。

{{step1-to-boards}}

1. 按一下&#x200B;[!UICONTROL **來源**]&#x200B;圖示![來源圖示](assets/sources-icon.png)以定義將卡片匯入工作資料流的來源。 目前唯一可用的來源是[!DNL Adobe Workfront]。
1. 新增篩選器以卡片形式從Workfront匯入任務和問題。

   為工作流程來源新增篩選器，與為基本展示板或Kanban展示板上的輸入欄新增進階篩選器相同。 如需詳細資訊，請參閱[將輸入資料行新增到展示板](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md)。

## 設定工作流程

{{step1-to-boards}}

1. 在儀表板上，按一下&#x200B;[!UICONTROL **檢視工作流程**]&#x200B;以開啟工作流程。
1. 按一下「[!UICONTROL **設定**]」以開啟「[!UICONTROL 設定工作流程]」面板。
1. （選擇性）展開&#x200B;[!UICONTROL **工作流程**]&#x200B;並輸入工作流程的描述。 此說明會顯示在控制面板上。
1. （選用）展開&#x200B;[!UICONTROL **反複專案**]&#x200B;以定義此工作資料流的反複專案程式。

   卡片總數、所指向的卡片數以及反複專案數都會顯示在「卡片清單」區段中。 按一下&#x200B;[!UICONTROL **檢視清單**]&#x200B;以開啟清單並新增卡片。 如需詳細資訊，請參閱[使用卡片清單](/help/quicksilver/agile/use-boards-agile-planning-tools/use-card-list.md)。

   如果已定義反複專案，則會顯示其開始日期、卡片數和點數。 按一下&#x200B;[!UICONTROL **檢視面板**]&#x200B;以開啟反複專案面板。 如需詳細資訊，請參閱[在工作串流中建立反複專案](/help/quicksilver/agile/use-boards-agile-planning-tools/create-an-iteration-in-workstream.md)。

1. （選用）展開&#x200B;[!UICONTROL **標籤**]&#x200B;以將標籤新增至工作流程。 搜尋標籤，或在搜尋方塊中輸入新標簽名稱，然後按Enter建立標籤。
