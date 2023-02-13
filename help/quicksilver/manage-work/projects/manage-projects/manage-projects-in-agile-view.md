---
product-area: projects;agile-and-teams
navigation-topic: manage-projects
title: 在敏捷檢視中管理專案
description: 所需的計畫、許可類型和訪問Adobe Workfront計畫團隊、專業、企業或企業Workfront許可類型審閱、工作或計畫權限訪問模型中的編輯訪問和建立報告、控制面板和日曆的功能
author: Alina
feature: Work Management
exl-id: fc633fd6-35b4-4949-8045-22c775002436
source-git-commit: a849ecaf6097dcdc924aaab2867f37bf57d5bc09
workflow-type: tm+mt
source-wordcount: '1311'
ht-degree: 0%

---

# 在敏捷檢視中管理專案

所需計畫、許可類型和訪問

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><a href="https://www.workfront.com/plans" target="_blank">Adobe Workfront計畫</a> </p> </td> 
   <td> <p>Team、Pro、Business或Enterprise </p> </td> 
  </tr> 
  <tr> 
   <td> <p><a href="https://one.workfront.com/s/article/Understanding-License-Types-906212506?language=en_US&amp;r=16&amp;ui-comm-runtime-components-aura-components-siteforce-qb.Quarterback.validateRoute=1&amp;ui-communities-components-aura-components-forceCommunity-breadcrumbs.Breadcrumbs.getAncestors=1&amp;ui-communities-components-aura-components-forceCommunity-seoAssistant.SeoAssistant.getSeoData=1&amp;ui-force-components-controllers-recordGlobalValueProvider.RecordGvp.getRecord=1&amp;ui-self-service-components-controller.ArticleTopicList.getTopics=1&amp;ui-self-service-components-controller.ArticleView.getArticleHeaderDetail=1" target="_blank">Workfront授權類型</a> </p> </td> 
   <td> <p>審核、工作或計畫 </p> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td> <p>Permissions in the access model</p> </td> 
    <td> <li>Edit access and ability to create reports, dashboards, and calendars</li> </td> 
   </tr>
  --> 
 </tbody> 
</table>

您可以針對專案運用靈活的功能

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
(such as story boards and burndown charts)
</MadCap:conditionalText>
-->

 避免通常伴隨敏捷做法的管理挑戰（例如管理團隊積壓工作或建立反覆項目）。

如果要在使用團隊積壓工作的靈活環境中工作，並允許您從積壓工作的任務中建立迭代，請按照以下說明操作： [在敏捷的環境中工作](../../../agile/work-in-an-agile-environment/work-in-an-agile-environment.md).

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>審核或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>編輯對以下區域的訪問：</p> 
    <ul> 
     <li> <p>專案</p> </li> 
     <li> <p>報表、控制面板、日曆</p> </li> 
     <li> <p>篩選器、檢視、群組</p> </li> 
    </ul> <p>注意：如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>檢視專案的權限</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 了解敏捷專案

* [專案中的靈活功能](#agile-functionality-in-a-project)
* [在專案上使用敏捷檢視與在迭代上使用敏捷檢視的差異](#differences-when-using-the-agile-view-on-a-project-versus-on-an-iteration)

### 專案中的靈活功能 {#agile-functionality-in-a-project}

以敏捷視圖管理專案時，可使用下列敏捷功能：

* 完成狀態\
   如需完成狀態的詳細資訊，請參閱 [迭代完成狀態概覽](../../../agile/use-scrum-in-an-agile-team/burndown/iteration-completion-status-overview.md).

* 展示板\
   如需關於動態圖示板的詳細資訊，請參閱 [洗滌板](../../../agile/use-scrum-in-an-agile-team/scrum-board/scrum-board.md) 區段。

在專案上使用敏捷檢視，與在純敏捷環境（有積壓工作和反覆工作）中運作時，有一些差異。 如需詳細資訊，請參閱 [在專案上使用敏捷檢視與在迭代上使用敏捷檢視的差異](#differences-when-using-the-agile-view-on-a-project-versus-on-an-iteration) 這篇文章。

### 在專案上使用敏捷檢視與在迭代上使用敏捷檢視的差異 {#differences-when-using-the-agile-view-on-a-project-versus-on-an-iteration}

* [任務和子任務遵循「動態板」上的不同顯示規則](#tasks-and-subtasks-follow-different-display-rules-on-the-story-board)
* [不使用回傳和迭代](#backlogs-and-iterations-are-not-used)
* [任務順序在敏捷視圖中保持，無法重新排序](#task-order-is-maintained-in-the-agile-view-and-cannot-be-reordered)
* [任務僅以計畫小時計量](#tasks-are-measured-only-in-planned-hours)
* [未使用Agile Team](#the-agile-team-is-not-used)
* [專案的每位使用者都能以不同的Agile檢視檢視專案](#each-user-on-the-project-can-view-the-project-in-a-different-agile-view)

#### 任務和子任務遵循「動態板」上的不同顯示規則 {#tasks-and-subtasks-follow-different-display-rules-on-the-story-board}

* 沒有父任務或子任務的任務在動態板上始終顯示為單個動態資訊卡。\
   例如，這些項目清單檢視中顯示如下：

   ![敏捷項目清單 — 沒有父項或子任務的任務](assets/agile-project-single-list-nwe.png) 這些任務在項目敏捷視圖中如下所示：

   ![項目敏捷視圖 — 沒有父項或子任務的任務](assets/agile-project-singlecard-nwe.png)

* 具有子任務的父任務始終顯示在 **故事** 文章欄。 子任務顯示在父任務的泳道中。\
   例如，這些項目清單檢視中顯示如下：

   ![敏捷項目清單 — 具有父項和子任務的任務](assets/agile-project-parent-list-nwe.png)\
   這些任務在項目敏捷視圖中如下所示：

   ![敏捷項目視圖 — 具有父項和子任務的任務](assets/agile-project-parent-nwe.png)

* 二級子任務（子任務的子任務）顯示為直接父任務的掛灰卡。
* 動態展示板上不會顯示第三層子任務（子任務的子任務）。

#### 不使用回傳和迭代 {#backlogs-and-iterations-are-not-used}

以敏捷檢視檢視專案時，不會使用下列敏捷元件：

* **積壓：** 不會使用積壓工作，因為項目中的任何任務都會自動顯示為動態。
* **迭代：** 與其建立迭代來定義工作完成日期，不如將項目時間軸上當前指定的天數變為工作天數。

#### 任務順序在敏捷視圖中保持，無法重新排序 {#task-order-is-maintained-in-the-agile-view-and-cannot-be-reordered}

在敏捷的文章展示板中檢視專案時，會維護專案中任務顯示的順序。

以敏捷檢視檢視專案時，您無法重新排序專案中的任務。 由於修改任務順序可能會影響其他可能具有相關性的任務，因此您必須在標準視圖中查看項目，才能修改任務順序。

#### 任務僅以計畫小時計量 {#tasks-are-measured-only-in-planned-hours}

項目上的任務始終以計畫小時計量。

在迭代中，任務（動態）可以以小時或點來測量。

#### 未使用Agile Team {#the-agile-team-is-not-used}

由於敏捷團隊會完成指派給他們的迭代作業，因此在敏捷檢視中檢視專案時不會使用敏捷團隊。

相反，專案上的任何使用者實際上都會成為該專案的敏捷團隊。

#### 專案的每位使用者都能以不同的Agile檢視檢視專案 {#each-user-on-the-project-can-view-the-project-in-a-different-agile-view}

與敏捷迭代不同，項目上的用戶可以為自己定制敏捷視圖，而其他用戶則使用不同的敏捷視圖。

在敏捷迭代中，在敏捷故事板上可用的資訊（例如可用的狀態列）由團隊層確定。

如需如何自訂敏捷檢視的詳細資訊，請參閱  [建立或自訂敏捷檢視](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md#customizing-an-agile-view) in  [Adobe Workfront中的檢視概觀](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md). 

## 以敏捷視圖檢視專案

1. 前往您要以敏捷檢視方式檢視的專案。
1. 按一下 **敏捷** 表徵圖。\
   ![敏捷圖示](assets/agile-icon-nwe.png)\
   專案會以預設的敏捷檢視顯示。\
   如果您先前是以自訂敏捷檢視檢視專案，專案會以該檢視顯示，而非以預設敏捷檢視顯示。

1. （可選）如果您已建立自訂敏捷檢視，或如果其他使用者已建立自訂敏捷檢視並與您共用，則您可以檢視該檢視，而非預設敏捷檢視。\
   按一下 **檢視** 下拉式功能表，然後按一下您要檢視的自訂敏捷檢視。

   下次按一下 **敏捷** 表徵圖。\
   如需如何建立新敏捷檢視的詳細資訊，請參閱 [建立和自訂敏捷檢視](#create-and-customize-agile-views).\
   專案會以自訂敏捷檢視顯示。

1. （條件性）如果項目中的任務使用的狀態不是「新」、「正在進行」或「完成」（「敏捷」視圖的預設狀態），則必須將附加狀態添加到敏捷視圖，才能顯示這些狀態中的任何任務。\
   如果任務的狀態未顯示在敏捷文章板上，則任務本身不會顯示在敏捷文章板上（但是，這些任務的完成百分比仍會導致任何父任務的完成百分比和整個項目的完成百分比）。\
   若要將狀態新增至敏捷檢視，請建立新的敏捷檢視或自訂現有的敏捷檢視，如文章的「建立或自訂敏捷檢視」一節所述 [Adobe Workfront中的檢視概觀](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. （可選）若要返回清單檢視，請按一下 **清單** 表徵圖。\
   ![](assets/list-icon.png)

## 建立和自訂敏捷檢視 {#create-and-customize-agile-views}

如同Workfront中的標準檢視，您可以自訂現有的敏捷檢視，或從頭建立新的敏捷檢視。 與標準檢視不同，您無法根據現有的敏捷檢視建立新的敏捷檢視。

如需建立和自訂敏捷檢視的詳細資訊，請參閱文章的「建立或自訂敏捷檢視」一節 [Adobe Workfront中的檢視概觀](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md). 

## 共用現有的Agile檢視

如需如何共用敏捷檢視的詳細資訊，請參閱 [共用篩選、檢視或分組](../../../reports-and-dashboards/reports/reporting-elements/share-filter-view-grouping.md).

## 移除現有的Agile檢視

如需如何刪除檢視的詳細資訊，請參閱文章中的「移除檢視」一節 [Adobe Workfront中的檢視概觀](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md). 
