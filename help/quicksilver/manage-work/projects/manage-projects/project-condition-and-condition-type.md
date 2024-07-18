---
title: 專案狀態與狀態型別概觀
content-type: overview
product-area: projects
navigation-topic: manage-projects
description: 專案狀態是專案進度方式的視覺化表示。 這是可報告變數，由專案的計畫、預計和估計日期之間的關係決定。
author: Alina
feature: Work Management
exl-id: 0c847b26-b0cb-49bb-84be-32534c72d5b6
source-git-commit: e4de185f172b173dcc3ad966afa69ffb3bc479eb
workflow-type: tm+mt
source-wordcount: '706'
ht-degree: 1%

---

# 專案狀態與狀態型別概觀

<!-- Audited: 12/2023 -->

專案狀態是專案進度方式的視覺化表示。 這是可報告變數，由專案的計畫、預計和估計日期之間的關係決定。

## 專案狀態概觀

瞭解專案條件時，請考量下列事項：

* 作為專案所有者，您可以決定專案條件是以手動還是自動方式設定。 專案狀態可透過下列方式設定：

   * 由有權管理專案的使用者手動設定，且專案的條件型別設定為手動時。
   * 當專案的「條件型別」設定為「進度狀態」時，由Adobe Workfront自動進行。 專案的進度狀態是由專案上任務的進度所決定。 如需有關專案進度狀態的資訊，請參閱[專案進度狀態概觀](../../../manage-work/projects/planning-a-project/project-progress-status.md)。

  如需有關如何更新專案狀態型別的資訊，請參閱[設定專案的狀態型別](../../../manage-work/projects/manage-projects/set-condition-type-for-project.md)。

* 允許Workfront自動估計專案狀態時，我們建議您在任務上使用前置任務，以便任務進度反映在實際進度和專案進度狀態中。
* 身為專案擁有者，您可以透過將條件型別從進度狀態變更為手動來將專案變更為使用手動條件型別，而不使用進度狀態。

  >[!NOTE]
  >
  >無論任務的日期及其進度為何，處於下列任一狀態的專案一律會標示為「達成目標」：
  >
  >* 構想
  >* 已請求
  >* 已核准
  >* 已拒絕

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Set the Condition Type for a project</h2>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: drafted here and moved it to a separate article: /Content/Manage work/Projects/Manage projects/set-condition-type-for-project.htm)</p>
<ol>
<li value="1">Go to the project for which you want to update the Condition Type. </li>
<li value="2"> <p>  Click the <strong>More</strong> menu <img src="assets/qs-more-menu.png"> to the right of the project name, then click <strong>Edit</strong>.  <br> </p> </li>
<li value="3">In the <strong>Condition Type</strong> field, choose one of the following:
<ul>
<li><p><strong>Manual:</strong> The project owner sets the Condition on the project manually.</p><p data-mc-conditions="QuicksilverOrClassic.Quicksilver">In this case, the project owner can update the Condition of the project in the project header, or the Project Details section. </p></li>
<li><p><strong>Progress Status:</strong> Workfront sets the Condition based on the Progress Status of the project. <br></p></li>
</ul></li>
<li value="4">Click <strong>Save Changes</strong>. </li>
</ol>
</div>
-->

## Workfront如何根據進度狀態更新專案狀態

當專案的「狀態型別」設定為「手動」時，您可以決定專案的狀態與專案的進度狀態無關。

不過，我們建議您將專案的「條件型別」設定為「進度狀態」，以便根據任務的進度，清楚指出專案的真正進度。 如需Workfront如何計算專案進度狀態的資訊，請參閱[專案進度狀態概觀](../../../manage-work/projects/planning-a-project/project-progress-status.md)。

在此案例中，專案條件的值可以是：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>專案狀況</strong></td> 
   <td><strong>專案進度狀態</strong></td> 
   <td><strong>Workfront條件指示器</strong></td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>達成目標</td> 
   <td>當專案的進度狀態為準時時，專案的狀態為目標</strong>上的<strong>。 </td> 
   <td> <img src="assets/on-target-condition-icon.png"> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>有風險</td> 
   <td>當專案的進度狀態為<strong>落後</strong>或<strong>有風險</strong>時，則專案的狀況為<strong>有風險</strong>。</td> 
   <td> <img src="assets/at-risk-project-condition-icon.png"> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>陷入困境</td> 
   <td>當專案的進度狀態為<strong>延遲</strong>時，則專案的狀況為<strong>發生問題</strong>。 </td> 
   <td> <img src="assets/in-trouble-project-condition-icon.png"> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>條件可以根據您的環境自訂，因此您可以在環境中找到三個以上的條件選項。 條件的名稱可能與上方列出的名稱不同。 如需有關自訂中條件的資訊，請參閱文章[建立或編輯自訂條件](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md)。

## 專案狀態、專案狀態更新和上次狀態附註的報告

在專案報告的檢視中，您可以顯示與專案狀態相關的下列欄位：

* **專案狀況：**&#x200B;顯示專案目前的狀況。
* **專案狀態更新**：顯示專案擁有者在專案更新流中提供的最新更新，以及新的狀態。\
  條件更新的註解不會顯示在&#x200B;**條件更新**&#x200B;欄中；只會顯示主要更新。

* **上次條件備註**：顯示物件擁有者上次在物件上輸入的更新。 此欄位有助於顯示物件上擁有者最近的活動或互動。\
  如果物件最後一個附註的附註文字已刪除，**最後一個條件附註**&#x200B;欄會空白。 當在物件上輸入新註記時，它會變成最後一個註記，並再次顯示在欄中。

如需有關如何建立報告的資訊，請參閱文章[建立自訂報告](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)。
