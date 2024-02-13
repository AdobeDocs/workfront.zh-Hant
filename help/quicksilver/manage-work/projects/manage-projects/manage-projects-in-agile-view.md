---
product-area: projects;agile-and-teams
navigation-topic: manage-projects
title: 在敏捷檢視中管理專案
description: 您可以針對專案利用敏捷功能，而不會遇到敏捷實務通常伴隨的管理挑戰（例如管理團隊待辦專案或建立反複專案）。
author: Alina and Lisa
feature: Work Management
exl-id: fc633fd6-35b4-4949-8045-22c775002436
source-git-commit: 4f63bca8634663c4106be0175851af0b982d3408
workflow-type: tm+mt
source-wordcount: '1433'
ht-degree: 0%

---

# 在敏捷檢視中管理專案

您可以針對專案利用敏捷功能，而不會遇到敏捷實務通常伴隨的管理挑戰（例如管理團隊待辦專案或建立反複專案）。

如果您想在使用團隊待辦專案的敏捷環境中工作，並允許您從待辦專案上的任務建立反複專案，請遵循中的指示 [在敏捷環境中工作](../../../agile/work-in-an-agile-environment/work-in-an-agile-environment.md).

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>目前：檢閱或以上</p> 
   <p>新增：投稿人或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>編輯對以下區域的存取權：</p> 
    <ul> 
     <li> <p>專案</p> </li> 
     <li> <p>報告、儀表板、行事曆</p> </li> 
     <li> <p>篩選器、檢視、群組</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>檢視專案的許可權</p>  </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的Workfront管理員。 如需存取需求的詳細資訊，請參閱 [Workfront檔案中的存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## 瞭解敏捷專案

>[!NOTE]
>
>本節僅適用於舊版敏捷檢視，不適用於專案的展示板檢視。

* [專案中的敏捷功能](#agile-functionality-in-a-project)
* [在專案上使用敏捷檢視與疊代使用敏捷檢視時的差異](#differences-when-using-the-agile-view-on-a-project-versus-on-an-iteration)

### 專案中的敏捷功能 {#agile-functionality-in-a-project}

在敏捷檢視中管理專案時，可以使用以下敏捷功能：

* 完成狀態\
  如需有關完成狀態的詳細資訊，請參閱 [反複專案完成狀態概觀](../../../agile/use-scrum-in-an-agile-team/burndown/iteration-completion-status-overview.md).

* 劇本面板\
  如需故事板的詳細資訊，請參閱 [Scrum展示板](../../../agile/use-scrum-in-an-agile-team/scrum-board/scrum-board.md) 區段。

對專案使用敏捷檢視與在純敏捷環境中工作（具有積壓和反複專案）有一些差異。 如需詳細資訊，請參閱 [在專案上使用敏捷檢視與疊代使用敏捷檢視時的差異](#differences-when-using-the-agile-view-on-a-project-versus-on-an-iteration) 本文章內容。

### 在專案上使用敏捷檢視與疊代使用敏捷檢視時的差異 {#differences-when-using-the-agile-view-on-a-project-versus-on-an-iteration}

* [任務和子任務在專案敏捷檢視中和疊代故事板上遵循不同的顯示規則](#tasks-and-subtasks-follow-different-display-rules-on-the-story-board)
* [敏捷檢視中不會使用積壓和反複專案](#backlogs-and-iterations-are-not-used)
* [任務順序是在敏捷檢視中維護，且無法重新排序](#task-order-is-maintained-in-the-agile-view-and-cannot-be-reordered)
* [任務只能在專案清單的計畫時數中測量](#tasks-are-measured-only-in-planned-hours)
* [敏捷團隊未用於敏捷檢視](#the-agile-team-is-not-used)
* [專案中的每個使用者都可以在不同的敏捷檢視中檢視專案](#each-user-on-the-project-can-view-the-project-in-a-different-agile-view)

#### 任務和子任務在專案敏捷檢視中和疊代故事板上遵循不同的顯示規則 {#tasks-and-subtasks-follow-different-display-rules-on-the-story-board}

* 沒有父系任務和子任務的任務一律會顯示為敏捷檢視內文板上的單一內文卡片。\
  例如，這些任務在專案清單檢視中會如下所示：

  ![敏捷專案清單 — 無父系或子系任務的任務](assets/agile-project-single-list-nwe.png)

  這些任務在專案敏捷檢視中顯示如下：

  ![專案敏捷檢視 — 沒有父系或子任務的任務](assets/agile-project-singlecard-nwe.png)

* 具有子任務的父任務一律顯示在 **劇本** 敏捷檢視的故事板欄。 子任務會顯示在父任務的泳道中。\
  例如，這些任務在專案清單檢視中會如下所示：

  ![敏捷專案清單 — 具有父任務和子任務的任務](assets/agile-project-parent-list-nwe.png)\
  這些任務在專案敏捷檢視中顯示如下：

  ![敏捷專案檢視 — 具有父任務和子任務的任務](assets/agile-project-parent-nwe.png)

* 第二層子任務（子任務的子任務）在緊接的父任務中顯示為懸掛的灰色卡片。
* 敏捷檢視中永遠不會顯示第三層子任務（子任務的子任務）。

#### 敏捷檢視中不會使用積壓和反複專案 {#backlogs-and-iterations-are-not-used}

在敏捷檢視中檢視專案時，未使用下列敏捷元件：

* **待處理專案：** 未使用待處理專案，因為專案中的任何任務都會自動顯示為內文。
* **反複專案：** 目前指定於專案時間表上的天數會變成工作天，而非建立反複專案來定義完成工作的日期。

#### 任務順序是在敏捷檢視中維護，且無法重新排序 {#task-order-is-maintained-in-the-agile-view-and-cannot-be-reordered}

當您在敏捷故事板中檢視專案時，會維護專案中任務出現的順序。

在敏捷檢視中檢視專案時，您無法重新排序專案中的任務。 由於修改作業順序可能會影響其他可能具有相依性的作業，因此您必須在標準檢視中檢視專案，才能修改作業順序。

#### 任務只能在專案清單的計畫時數中測量 {#tasks-are-measured-only-in-planned-hours}

專案上的任務一律以計畫時數測量。

在反複專案中，任務（劇本）能以小時或點來測量。

#### 敏捷團隊未用於敏捷檢視 {#the-agile-team-is-not-used}

因為敏捷團隊完成指派給他們的疊代工作，敏捷團隊在敏捷檢視中檢視專案時不使用。

實際上，專案上的任何使用者都會成為該專案的敏捷團隊。

#### 專案中的每個使用者都可以在不同的敏捷檢視中檢視專案 {#each-user-on-the-project-can-view-the-project-in-a-different-agile-view}

不像敏捷疊代，專案上的使用者可以為他們自己自訂敏捷檢視，而其他使用者則使用不同的敏捷檢視。

在敏捷反複專案中，敏捷故事板上可用的資訊（例如可用的狀態列）取決於團隊層級。

有關如何自訂敏捷檢視的資訊，請參閱 [建立或自訂敏捷檢視](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md#create-or-customize-an-agile-view) 在 [在Adobe Workfront中建立或編輯檢視](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md).

## 在敏捷檢視中檢視專案

1. 前往您要在敏捷檢視中檢視的專案（在任務清單或問題清單上）。
1. 按一下 **展示板檢視** 圖示 ![展示板圖示](assets/board-icon-for-agile-view.png).

   預設會顯示專案的展示板檢視。

   ![專案的面板檢視](assets/project-agile-board-view.png)

   <!--(Legacy agile view only) If you previously viewed the project in a custom agile view, the project is displayed in that view rather than in the default agile view.-->

1. （選用）按一下 **設定** 以設定欄和卡片的選項。

   如需詳細資訊，請參閱 [管理展示板欄](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md) 和 [自訂要在卡片上顯示的欄位](/help/quicksilver/agile/get-started-with-boards/customize-fields-on-card.md). 請注意，您無法在專案的展示板檢視上定義欄原則。

1. （選用）按一下 **使用舊版敏捷** 使用舊版敏捷檢視而不使用展示板檢視。

1. （選用 — 僅限舊版敏捷檢視）如果您已建立自訂敏捷檢視，或如果另一個使用者已建立自訂敏捷檢視並與您共用，您可以檢視它，而不是預設敏捷檢視。

   按一下 **檢視** 下拉式功能表，然後按一下您要檢視的自訂敏捷檢視。

   當您下次按一下 **敏捷** 圖示。

   有關如何建立新敏捷檢視的資訊，請參閱 [建立和自訂敏捷檢視](#create-and-customize-agile-views).

   專案會顯示在自訂敏捷檢視中。

1. （條件式 — 僅限舊版敏捷檢視）如果專案中的任務使用「新增」、「進行中」或「完成」以外的狀態（敏捷檢視的預設狀態），您必須將其他狀態新增到敏捷檢視，才能顯示這些狀態的任何任務。

   如果任務處於未顯示在敏捷故事板上的狀態，則任務本身未顯示在敏捷故事板上（但是，這些任務的完成百分比仍然對任何父系任務的完成百分比和整個專案的完成百分比有貢獻）。

   若要將狀態新增到敏捷檢視，請建立新的敏捷檢視或自訂現有的敏捷檢視，如文章的「建立或自訂敏捷檢視」一節中所述 [Adobe Workfront中的檢視概觀](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. （選擇性）若要返回清單檢視，請按一下 **清單** 圖示。

## 建立和自訂敏捷檢視 {#create-and-customize-agile-views}

>[!NOTE]
>
>本節僅適用於舊版敏捷檢視，不適用於專案的展示板檢視。

和Workfront中的標準檢視一樣，您可以自訂現有的敏捷檢視或從頭開始建立新的敏捷檢視。 和標準檢視不同，您無法根據現有的敏捷檢視建立新的敏捷檢視。

如需有關建立和自訂敏捷檢視的詳細資訊，請參閱 [建立或自訂敏捷檢視](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md#create-or-customize-an-agile-view) 文章中的區段 [在Adobe Workfront中建立或編輯檢視](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md).

## 共用現有的敏捷檢視

>[!NOTE]
>
>本節僅適用於舊版敏捷檢視，不適用於專案的展示板檢視。

您可以共用您建立的敏捷檢視，或是以與共用任何其他檢視、篩選或分組相同的方式擁有許可權。

如需詳細資訊，請參閱 [共用篩選、檢視或分組](../../../reports-and-dashboards/reports/reporting-elements/share-filter-view-grouping.md).

## 移除現有的敏捷檢視

>[!NOTE]
>
>本節僅適用於舊版敏捷檢視，不適用於專案的展示板檢視。

您可以用移除任何其他檢視、篩選或分組的相同方式，移除敏捷檢視。

如需詳細資訊，請參閱 [移除篩選器、檢視和群組](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/remove-filters-views-groupings.md).
