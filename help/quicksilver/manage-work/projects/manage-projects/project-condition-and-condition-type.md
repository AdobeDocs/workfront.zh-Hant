---
title: 專案條件和條件類型概觀
content-type: overview
product-area: projects
navigation-topic: manage-projects
description: 專案條件是專案進展情形的視覺表示。 此為可報告變數，由項目計畫、預計及估計日期之關係釐定。
author: Alina
feature: Work Management
exl-id: 0c847b26-b0cb-49bb-84be-32534c72d5b6
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '706'
ht-degree: 1%

---

# 專案條件和條件類型概觀

專案條件是專案進展情形的視覺表示。 此為可報告變數，由項目計畫、預計及估計日期之關係釐定。

## 專案條件概觀

了解專案的條件時，請考量下列事項：

* 作為項目所有者，您可以決定是手動設定還是自動設定項目的條件。 專案的條件可透過下列方式設定：

   * 手動，由有權管理專案的使用者以及專案的「條件類型」設為「手動」時手動執行。
   * 當專案的「條件類型」設為「進度狀態」時，由Adobe Workfront自動執行。 項目的進度狀態由項目任務的進度確定。 有關項目進度狀態的資訊，請參閱 [項目進度狀態概觀](../../../manage-work/projects/planning-a-project/project-progress-status.md).

   如需如何更新專案的條件類型的相關資訊，請參閱 [設定專案的條件類型](../../../manage-work/projects/manage-projects/set-condition-type-for-project.md).

* 當允許Workfront自動估計項目的條件時，我們建議您在任務上使用前置任務，以便任務進度反映項目的實際進度和進度狀態。
* 作為項目所有者，您可以通過將條件類型從「進度狀態」更改為「手動」，將項目更改為「手動」條件類型，而不是使用「進度狀態」。

   >[!NOTE]
   >
   >處於下列任一狀態的專案一律會標示為「在Target上」，無論工作的日期和進度為何：
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

## Workfront如何根據進度狀態更新專案條件

當項目的「條件類型」設定為「手動」時，您可以確定項目的「條件」與項目的「進度狀態」獨立。

不過，我們建議您將專案的「條件類型」設為「進度狀態」，以便根據工作進度，清楚指出專案的真正進度。 有關Workfront如何計算項目進度狀態的資訊，請參閱 [項目進度狀態概觀](../../../manage-work/projects/planning-a-project/project-progress-status.md).

在這種情況下，「專案條件」的值可以是：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>專案條件</td> 
   <td>項目進度狀態</td> 
   <td>Workfront條件指標</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>達成目標</td> 
   <td> <li>項目進度狀態按時時，項目的條件為 <strong>在Target上</strong>.</li> </td> 
   <td> <img src="assets/on-target-condition-icon.png"> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>有風險</td> 
   <td>項目的進度狀態為 <strong>背後</strong> 或 <strong>風險</strong>，則專案的條件為 <strong>風險</strong>.</td> 
   <td> <img src="assets/at-risk-project-condition-icon.png"> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>陷入困境</td> 
   <td>項目的進度狀態為 <strong>延遲</strong>，則專案的條件為 <strong>麻煩</strong>. </td> 
   <td> <img src="assets/in-trouble-project-condition-icon.png"> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>您可以根據您的環境自訂條件，因此在您的環境中可能會找到三個以上的「條件」選項。 條件的名稱可能與上述名稱不同。 如需在中自訂條件的相關資訊，請參閱文章 [建立或編輯自訂條件](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).

## 報告項目條件、項目條件更新和最後一個條件備注

在專案報表的檢視中，您可以顯示與專案條件相關的下列欄位：

* **專案條件：** 顯示項目的當前條件。
* **專案條件更新**:顯示專案擁有者在專案的更新資料流中提供的最新更新，以及新的條件。\
   在條件更新時所做的註解不會顯示在 **條件更新** 欄；僅顯示主要更新。

* **最後一個條件備注**:顯示對象所有者上次在對象上輸入的更新。 此欄位有助於顯示擁有者在物件上最近的活動或互動。\
   此 **最後一個條件備注** 欄是空的（如果已刪除對象的最後一個備注的備注文本）。 在對象上輸入新注釋時，它將成為最後一個注釋，並在列中再次顯示。

如需如何建立報表的詳細資訊，請參閱文章 [建立自訂報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
