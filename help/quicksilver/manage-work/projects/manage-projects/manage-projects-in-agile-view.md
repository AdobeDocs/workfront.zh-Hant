---
product-area: projects;agile-and-teams
navigation-topic: manage-projects
title: 在敏捷視圖中管理項目
description: 必需的計畫、許可證類型和訪問Adobe Workfront計畫團隊、專業、業務或企業Workfront許可證類型查看、工作或計畫訪問模型中的權限編輯訪問權限和建立報告、儀表板和日曆的能力
author: Alina
feature: Work Management
exl-id: fc633fd6-35b4-4949-8045-22c775002436
source-git-commit: 888c938e5d649557df69374a55d4e4ecc2da6f55
workflow-type: tm+mt
source-wordcount: '1296'
ht-degree: 0%

---

# 在敏捷視圖中管理項目

所需計畫、許可證類型和訪問

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><a href="https://www.workfront.com/plans" target="_blank">Adobe Workfront計畫</a> </p> </td> 
   <td> <p>團隊、專業、業務或企業 </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Workfront許可證類型</p> </td> 
   <td> <p>審閱、工作或計畫 </p> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td> <p>Permissions in the access model</p> </td> 
    <td> <li>Edit access and ability to create reports, dashboards, and calendars</li> </td> 
   </tr>
  --> 
 </tbody> 
</table>

您可以利用項目的靈活功能

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
(such as story boards and burndown charts)
</MadCap:conditionalText>
-->

 而不會遇到通常伴隨敏捷做法的管理難題（例如管理團隊積壓工作或建立迭代）。

如果要在使用團隊積壓工作的靈活環境中工作，並允許您從積壓工作的任務中建立迭代，請按照中的說明進行操作 [在敏捷環境中工作](../../../agile/work-in-an-agile-environment/work-in-an-agile-environment.md)。

## 訪問要求

您必須具有以下訪問權限才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront許可證*</td> 
   <td> <p>審閱或更高</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>編輯對以下區域的訪問：</p> 
    <ul> 
     <li> <p>專案</p> </li> 
     <li> <p>報表、儀表板、日曆</p> </li> 
     <li> <p>篩選器、視圖、分組</p> </li> 
    </ul> <p>注：如果您仍然沒有訪問權限，請詢問您的Workfront管理員是否在您的訪問級別設定了其他限制。 有關Workfront管理員如何修改您的訪問級別的資訊，請參見 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自定義訪問級別</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">對象權限</td> 
   <td> <p>查看對項目的權限</p> <p>有關請求附加訪問的資訊，請參見 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求訪問對象 </a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要瞭解您擁有的計畫、許可證類型或訪問權限，請與您的Workfront管理員聯繫。

## 瞭解敏捷項目

* [項目中的靈活功能](#agile-functionality-in-a-project)
* [在項目上使用敏捷視圖與在迭代上使用敏捷視圖時的差異](#differences-when-using-the-agile-view-on-a-project-versus-on-an-iteration)

### 項目中的靈活功能 {#agile-functionality-in-a-project}

在敏捷視圖中管理項目時，可使用以下靈活功能：

* 完成狀態\
   有關完成狀態的詳細資訊，請參見 [迭代完成狀態概述](../../../agile/use-scrum-in-an-agile-team/burndown/iteration-completion-status-overview.md)。

* 故事板\
   有關文章板的詳細資訊，請參見 [洗滌板](../../../agile/use-scrum-in-an-agile-team/scrum-board/scrum-board.md) 的子菜單。

在項目上使用敏捷視圖與在純靈活環境（使用積壓工作和迭代）中工作時存在一些差異。 有關詳細資訊，請參見 [在項目上使用敏捷視圖與在迭代上使用敏捷視圖時的差異](#differences-when-using-the-agile-view-on-a-project-versus-on-an-iteration) 在本文中。

### 在項目上使用敏捷視圖與在迭代上使用敏捷視圖時的差異 {#differences-when-using-the-agile-view-on-a-project-versus-on-an-iteration}

* [任務和子任務在文章板上遵循不同的顯示規則](#tasks-and-subtasks-follow-different-display-rules-on-the-story-board)
* [不使用積壓記錄和小版本](#backlogs-and-iterations-are-not-used)
* [任務順序在「敏捷」視圖中維護，無法重新排序](#task-order-is-maintained-in-the-agile-view-and-cannot-be-reordered)
* [任務僅以計畫小時數計量](#tasks-are-measured-only-in-planned-hours)
* [未使用敏捷團隊](#the-agile-team-is-not-used)
* [項目上的每個用戶都可以以不同的敏捷視圖查看項目](#each-user-on-the-project-can-view-the-project-in-a-different-agile-view)

#### 任務和子任務在文章板上遵循不同的顯示規則 {#tasks-and-subtasks-follow-different-display-rules-on-the-story-board}

* 既沒有父任務也沒有子任務的任務始終顯示為文章板上的單個文章卡。\
   例如，這些任務在項目清單視圖中如下所示：

   ![敏捷項目清單 — 沒有父任務或子任務的任務](assets/agile-project-single-list-nwe.png) 這些任務在項目敏捷視圖中如下所示：

   ![項目敏捷視圖 — 沒有父任務或子任務的任務](assets/agile-project-singlecard-nwe.png)

* 具有子任務的父任務始終顯示在 **故事** 欄。 子任務顯示在父任務的任務分配中。\
   例如，這些任務在項目清單視圖中如下所示：

   ![敏捷項目清單 — 具有父任務和子任務的任務](assets/agile-project-parent-list-nwe.png)\
   這些任務在項目敏捷視圖中如下所示：

   ![敏捷項目視圖 — 具有父任務和子任務的任務](assets/agile-project-parent-nwe.png)

* 二級子任務（子任務的子任務）顯示為直接父任務的掛灰卡。
* 文章板上從不顯示第三級子任務（子任務子任務的子任務）。

#### 不使用積壓記錄和小版本 {#backlogs-and-iterations-are-not-used}

在敏捷視圖中查看項目時，不使用以下敏捷元件：

* **積壓：** 不使用積壓工作，因為項目中的任何任務都自動顯示為文章。
* **迭代：** 不是建立迭代來定義完成工作的日期，而是當前在項目時間線上指定的天數成為工作日。

#### 任務順序在「敏捷」視圖中維護，無法重新排序 {#task-order-is-maintained-in-the-agile-view-and-cannot-be-reordered}

在敏捷的故事板中查看項目時，項目中任務的顯示順序會得到維護。

在敏捷視圖中查看項目時，無法重新排序項目中的任務。 由於修改任務順序可能會影響其他可能具有相關性的任務，因此您必須在標準視圖中查看項目才能修改任務順序。

#### 任務僅以計畫小時數計量 {#tasks-are-measured-only-in-planned-hours}

項目上的任務始終以計畫小時數計量。

在迭代中，任務（故事）可以以小時或點來度量。

#### 未使用敏捷團隊 {#the-agile-team-is-not-used}

由於敏捷團隊完成了分配給它們的迭代的工作，因此在敏捷視圖中查看項目時不使用敏捷團隊。

相反，項目上的任何用戶實際上都成了該項目的靈活團隊。

#### 項目上的每個用戶都可以以不同的敏捷視圖查看項目 {#each-user-on-the-project-can-view-the-project-in-a-different-agile-view}

與敏捷迭代不同，項目上的用戶可以自定義敏捷視圖，而其他用戶則使用不同的敏捷視圖。

在敏捷迭代中，在敏捷故事板上可用的資訊（例如可用的狀態列）在團隊級別上確定。

有關如何自定義敏捷視圖的資訊，請參見  [建立或自定義敏捷視圖](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md#customizing-an-agile-view) 在  [Adobe Workfront視圖概述](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)。 

## 在「敏捷」視圖中查看項目

1. 轉到要在敏捷視圖中查看的項目。
1. 按一下 **敏捷** 表徵圖\
   ![敏捷表徵圖](assets/agile-icon-nwe.png)\
   項目顯示在預設敏捷視圖中。\
   如果您以前在自定義敏捷視圖中查看項目，則項目將顯示在該視圖中，而不是在預設敏捷視圖中。

1. （可選）如果您已建立自定義敏捷視圖，或者如果其他用戶已建立自定義敏捷視圖並將其與您共用，則可以查看它，而不是預設敏捷視圖。\
   按一下 **視圖** 下拉菜單，然後按一下要查看的自定義敏捷視圖。

   下次按一下 **敏捷** 表徵圖\
   有關如何建立新敏捷視圖的資訊，請參見 [建立和自定義敏捷視圖](#create-and-customize-agile-views)。\
   項目顯示在自定義敏捷視圖中。

1. （條件）如果項目中的任務使用的狀態不是「新建」、「正在進行」或「完成」（敏捷視圖的預設狀態），則必須將附加狀態添加到敏捷視圖中，才能顯示處於這些狀態的任何任務。\
   如果任務處於未顯示在敏捷故事板上的狀態，則任務本身不會顯示在敏捷故事板上（但是，這些任務的完成百分比仍然會導致任何父任務的完成百分比和整個項目的完成百分比）。\
   要向敏捷視圖添加狀態，請建立新的敏捷視圖或自定義現有的敏捷視圖，如文章「建立或自定義敏捷視圖」部分所述 [Adobe Workfront視圖概述](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)。

1. （可選）要返回清單視圖，請按一下 **清單** 表徵圖\
   ![](assets/list-icon.png)

## 建立和自定義敏捷視圖 {#create-and-customize-agile-views}

與Workfront的標準視圖一樣，您可以自定義現有的敏捷視圖或從頭建立新的敏捷視圖。 與標準視圖不同，不能基於現有的敏捷視圖建立新的敏捷視圖。

有關建立和定制敏捷視圖的詳細資訊，請參閱文章中的「建立或定制敏捷視圖」部分 [Adobe Workfront視圖概述](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)。 

## 共用現有的敏捷視圖

有關如何共用敏捷視圖的資訊，請參見 [共用篩選器、視圖或分組](../../../reports-and-dashboards/reports/reporting-elements/share-filter-view-grouping.md)。

## 刪除現有的敏捷視圖

有關如何刪除視圖的資訊，請參閱文章中的「刪除視圖」部分 [Adobe Workfront視圖概述](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)。 
