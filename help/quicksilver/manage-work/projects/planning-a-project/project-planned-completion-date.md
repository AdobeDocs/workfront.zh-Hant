---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: 設定專案計畫完成日期
description: 專案的計畫完成日期是專案設定為完成的日期。
author: Alina
feature: Work Management, Projects
role: User
exl-id: 996398c5-de92-445e-8e86-36b2efdcf6b5
source-git-commit: fedb0328450896d212081715df4cde7644b169bc
workflow-type: tm+mt
source-wordcount: '591'
ht-degree: 1%

---

# 設定專案計畫完成日期

<!-- Audited: 4/2025 -->

專案的計畫完成日期是專案設定完成的日期。

專案的計劃開始日期和計畫完成日期取決於專案上任務的日期。 本文說明如何手動或自動設定專案的規劃完成日期。 如需有關任務計畫完成日期的詳細資訊，請參閱[任務計畫完成日期的總覽](../../../manage-work/tasks/task-information/task-planned-completion-date.md)。

您可以手動或自動設定專案的「計畫完成日期」，視您是從「開始」還是從「完成日期」排程專案而定。

## 存取需求

<!--drafted for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Standard </p>
   Or
   <p>Legacy license: Plan </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

+++ 展開以檢視本文中功能的存取需求。

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
   <td role="rowheader">Adobe Workfront授權</td> 
   <td><p>
   新增：標準

或

目前：計畫 </p>

</td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>編輯專案的存取權</p> <p><b>附註</b>

如果您還是沒有存取權，請詢問您的Workfront管理員，他們是否在您的存取層級中設定其他限制。 如需Workfront管理員如何修改存取層級的詳細資訊，請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>。</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>管理專案的許可權</p> <p>如需請求其他存取權的資訊，請參閱<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求物件</a>的存取權。</p> </td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 手動設定專案的計畫完成日期

當您從完成日期開始排程專案時，必須手動設定專案的「計畫完成日期」。

>[!NOTE]
>
>當您手動設定專案的規劃完成日期時，Workfront會根據所有任務的期間自動計算專案的規劃開始日期。


若要從「完成日期」排程專案，請執行下列步驟：

{{step1-to-projects}}

1. 按一下&#x200B;**新增專案**，然後從出現的下拉式清單中選取&#x200B;**新增專案**。

   如需有關建立專案的詳細資訊，請參閱文章[建立專案](../../../manage-work/projects/create-projects/create-project.md)。

1. 在左側面板中選取&#x200B;**專案詳細資料**。

1. 按一下右上角的&#x200B;**編輯專案**&#x200B;圖示![編輯圖示](/help/quicksilver/manage-work/projects/planning-a-project/assets/qs-edit-icon.png)，然後在出現的下拉式清單中選取&#x200B;**概觀**。

1. 在&#x200B;**專案日期**&#x200B;區段中，按一下&#x200B;**排程模式**&#x200B;欄位，然後選取&#x200B;**完成日期**。

1. 指定專案的&#x200B;**計畫完成日期**。
1. 按一下「**儲存變更**」。

   當您開始新增任務至專案時，專案的&#x200B;**計劃開始日期**&#x200B;會根據所有任務的總持續時間計算。 

## 自動設定專案的計畫完成日期

當您從開始日期排程專案時，Workfront會自動計算專案的計畫完成日期。 

若要從「開始日期」排程專案，請執行下列步驟：

{{step1-to-projects}}

1. 按一下&#x200B;**新增專案**，然後從出現的下拉式清單中選取&#x200B;**新增專案**。

   如需有關建立專案的詳細資訊，請參閱文章[建立專案](../../../manage-work/projects/create-projects/create-project.md)。

1. 在左側面板中選取&#x200B;**專案詳細資料**。

1. 按一下右上角的&#x200B;**編輯專案**&#x200B;圖示![編輯圖示](/help/quicksilver/manage-work/projects/planning-a-project/assets/qs-edit-icon.png)，然後在出現的下拉式清單中選取&#x200B;**概觀**。

1. 在&#x200B;**專案日期**&#x200B;區段中，按一下&#x200B;**排程模式**&#x200B;欄位，然後選取&#x200B;**開始日期**。

1. 指定專案的&#x200B;**計劃開始日期**。
1. 按一下「**儲存變更**」。

   當您開始新增任務至專案時，專案的&#x200B;**計畫完成日期**&#x200B;會根據所有任務的總持續時間計算。 

   如需有關工作持續時間的詳細資訊，請參閱文章[工作持續時間和持續期間型別概觀](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md)。

   專案的計畫完成日期與專案上最後一個任務的計畫完成日期一致（在此案例中為）。

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>The Planned Completion Date of a task</h2>
<p>(NOTE: drafted because I created a new article, here: /Content/Manage work/Tasks/Task information/task-planned-completion-date.htm)</p>
<p>You can either specify the Planned Completion Date of a task, or you can leave it up to Workfront to calculate it depending on certain criteria.&nbsp;</p>
<ul>
<li><a href="#manually-set-the-planned-completion-date-of-a-task" class="MCXref xref">Manually set the Planned Completion Date of a task</a> </li>
<li><a href="#how-the-planned-completion-date-is-calculated-for-a-task" class="MCXref xref">How the Planned Completion Date is calculated for a task</a> </li>
</ul>
<p><strong>Manually set the Planned Completion Date of a task</strong></p>
<p>Setting the Planned Completion Date of a task depends on the type of Task Constraint you assign to the task.&nbsp;</p>
<p>You can manually set the Planned Completion Date&nbsp;when creating a task, as described in&nbsp;the article <a href="../../../manage-work/tasks/create-tasks/create-tasks-in-project.md" class="MCXref xref">Create tasks in a project</a>.</p>
<p>You can manually specify the Planned Completion Date when you select any of the following Task Constraints:&nbsp;</p>
<table border="1" cellspacing="15" cellpadding="1">
<col>
<col>
<thead>
<tr>
<th> <p><strong>Task Constraint Type</strong> </p> </th>
<th> <p><strong>Effect of Manually Changing the Planned Completion Date</strong> </p> </th>
</tr>
</thead>
<tbody>
<tr>
<td> <p>Must Finish On</p> <p>Finish No Later Than</p> <p>Finish No Earlier Than</p> </td>
<td> <p><span class="s1">The Planned Start Date is adjusted in order to keep the Duration the same.</span> </p> </td>
</tr>
<tr>
<td> <p>Fixed Dates</p> </td>
<td> <p>The Duration is adjusted in order to keep the Planned Start Date the same.</p> </td>
</tr>
</tbody>
</table>
<p><strong>How the Planned Completion Date is calculated for a task</strong></p>
<p>When it is calculated automatically by the system, the following can influence the Planned Completion Date of a Task:</p>
<ul>
<li> <p>Task Constraint</p> <p>For more information about Task Constraints, see the article <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">Task Constraint overview</a>.</p> </li>
<li> <p>Task predecessor relationship</p> <p>For more information about task predecessors, see the article <a href="../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md" class="MCXref xref">Overview of task predecessors</a>.</p> </li>
<li>Project Completion Date, when the project is scheduled from Completion Date.</li>
<li> <p>The time off schedule of the Primary&nbsp;Assignee of the task. </p> <p>When the Primary Assignee has time off scheduled during the duration of the task, the planned dates of the task adjust accordingly when the <strong>Consider user time off in task durations</strong> setting is selected for the <strong>User Time Off</strong> field. New projects inherit this setting from the Project&nbsp;Preferences area, but you can edit the setting at the project level. </p> <p>For example, if a task with a Constraint of As Soon As Possible is scheduled to start on June 1 and complete on June 3, and the Primary Assignee has June 2 marked for Time-off, the task Planned Completion Date becomes June 4. </p> <p>For information about the <strong>User Time Off</strong> preference, see the articles <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configure system-wide project preferences</a> or <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">Edit projects</a>.</p> </li>
</ul>
<p>When set automatically, the Planned Completion Date&nbsp;is determined based on the following calculation:&nbsp;</p>
<p><code>Planned Completion Date = Planned Start Date + Duration</code> </p>
<p>For example, if your task has a start date of September 16 and a duration of 10 days, the Planned Completion Date is September 26.</p> <note type="note">
&nbsp;The Update Type for the project must also be&nbsp;set to Automatic and On Change or Automatically in order for the Planned Hours and Duration to be automatically&nbsp;adjusted.
<br>For more information about the Update Type, see the article
<a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Select the project Update Type </a>.
</note>
</div>
-->
