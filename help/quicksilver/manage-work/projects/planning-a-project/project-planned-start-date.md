---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: 項目計劃開始日期概覽
description: 項目計劃開始日期概覽
author: Alina
feature: Work Management
exl-id: a1223d81-3fb8-42d1-9a7d-c58d1f0fcd36
source-git-commit: bbd64e9deed1b89d720272508b3562c354578704
workflow-type: tm+mt
source-wordcount: '374'
ht-degree: 0%

---

# 項目計劃開始日期概覽

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: ???</p>
<p>This needs to be split in two articles, and add one to the Tasks area.</p>
<p>Linked to&nbsp;Understanding the Projected Start Date for Projects, Tasks, and Issues; Project Condition article. Linked to Managing User Allocations.) </p>
</div>
-->

項目的計劃開始日期和計畫完成日期取決於項目任務的日期。 本文說明項目的計畫起始日期。 有關任務計畫起始日期的資訊，請參閱 [任務計畫起始日期概覽](../../../manage-work/tasks/task-information/task-planned-start-date.md).

根據您是從「開始」還是從「完成」日期計畫項目，可以人工或自動設定項目的「計畫起始日期」。

## 人工設定項目的計畫起始日期

從開始日期開始計畫項目時，您必須人工設定項目的計畫起始日期。

有關設定項目計劃開始日期的資訊，請參閱 [編輯專案](../../../manage-work/projects/manage-projects/edit-projects.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: drafted below, to keep this as an overview article)</p>
-->

<!--
<ol data-mc-conditions="QuicksilverOrClassic.Draft mode">
<li value="1">  Click the <strong>Main Menu</strong> icon <img src="assets/main-menu-icon.png"> in the upper-right corner, then click <strong>Projects</strong>. </li>
<li value="2"> <p>  Click&nbsp; <strong>New Project</strong> then <strong>New Project</strong>. </p> <p>For more information about creating projects, see <a href="../../../manage-work/projects/create-projects/create-project.md" class="MCXref xref">Create a project</a>.</p> </li>
<li value="3">  Click the <strong>Edit Project</strong> icon in the upper-right corner. </li>
<li value="4">In the <strong>Schedule From</strong> field, select <strong>Start Date</strong>.</li>
<li value="5">Specify the <strong>Planned Start Date</strong> of the project.</li>
<li value="6"> <p>Click <strong>Save Changes</strong>.</p> <p>As you start adding tasks to your project, the <strong>Planned Completion Date</strong> of the project calculates based on the total Duration of all of the tasks.&nbsp;</p> </li>
</ol>
-->

## 自動設定項目的計劃開始日期

以下列方式建立專案時，會自動設定專案的計劃開始日期：

* 從頭開始，以及從完成日期開始計畫項目時。

   計畫起始日期由Adobe Workfront根據您為完成日期選擇的日期和項目上所有任務的持續時間自動計算。

   如需從草稿開始建立專案的相關資訊，請參閱 [建立專案](../../../manage-work/projects/create-projects/create-project.md).

* 從Microsoft專案匯入。

   「計畫起始日期」是Microsoft項目中項目的起始日期。

   如需從Microsoft專案匯入專案的相關資訊，請參閱 [從Microsoft專案匯入專案](../../../manage-work/projects/create-projects/import-project-from-ms-project.md).

* 當您是Workfront管理員時，請使用Workfront Kick-Starts匯入。

   除非您在啟動檔案的「項目」工作表的setPlanedStartDate欄位中另外指定，否則「計劃開始日期」始終與電腦的時間和日期匹配。

   有關使用啟動導入資料的資訊，請參閱 [使用Kick-Start範本將資料匯入Adobe Workfront](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).

   如需有關使用啟動匯入專案的資訊，請參閱 [Kick-Starts案例：簡單的項目和任務導入準備](../../../administration-and-setup/manage-workfront/using-kick-starts/kick-starts-scenario-simple-project-task-import-prep.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE:drafted it, to keep this as an overview article)</p>
<p>To schedule a project from Completion Date:</p>
<ol>
<li value="1">  Click the <strong>Main Menu</strong> icon <img src="assets/main-menu-icon.png"> in the upper-right corner, then click <strong>Projects</strong>. </li>
<li value="2"> <p>  Click&nbsp; <strong>New Project</strong> then <strong>New Project</strong>. </p> <p>For more information about creating projects, see <a href="../../../manage-work/projects/create-projects/create-project.md" class="MCXref xref">Create a project</a>.</p> </li>
<li value="3">  Click the <strong>Edit Project</strong> icon in the upper-right corner. </li>
<li value="4">In the <strong>Schedule From</strong> field, select <strong>Completion Date</strong>.</li>
<li value="5">Specify the <strong>Planned Completion Date</strong> of the project.</li>
<li value="6"> <p>Click <strong>Save Changes</strong>.</p> <p>As you start adding tasks to your project, the <strong>Planned Start Date</strong> of the project calculates based on the total Duration of all of the tasks, counting backwards from the Planned Completion Date.&nbsp;</p> <p>For more information about Task Duration, see the article <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Overview of Task Duration and Duration Type</a>.</p> <p>The Planned Start Date of the project coincides, in this case, with the Planned Start Date of the first task on the project.</p> </li>
</ol>
</div>
-->

## 任務的計畫起始日期

您可以指定任務的「計劃開始日期」，或根據特定標準讓Workfront自行計算。

有關任務的計畫起始日期的資訊，請參閱 [任務計畫起始日期概覽](../../../manage-work/tasks/task-information/task-planned-start-date.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2> </h2>
<p>(NOTE: drafted and this content was moved to the article linked in the above paragraph)</p>
<p>The Planned Start Date of a task</p>
<p>You can either specify the Planned Start Date of a task, or you can leave it up to Workfront to calculate it depending on certain criteria.&nbsp;</p>
<ul>
<li><a href="#manually-set-the-planned-start-date-of-a-task" class="MCXref xref">Manually set the Planned Start Date of a task</a> </li>
<li><a href="#how-the-planned-start-date-is-calculated-for-a-task" class="MCXref xref">How the Planned Start Date is calculated for a task</a> </li>
</ul>
<p><strong>Manually set the Planned Start Date of a task</strong></p>
<p>Setting the Planned Start Date of a task depends on the type of Task Constraint you assign to the task.&nbsp;</p>
<p>You can manually set the Planned Start Date&nbsp;when creating a task, as described in&nbsp;the article <a href="../../../manage-work/tasks/create-tasks/create-tasks-in-project.md" class="MCXref xref">Create tasks in a project</a>.</p>
<p>You can manually specify the Planned Start Date when you select any of the following Task Constraints:&nbsp;</p>
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
<td> <p>Must Start On</p> <p>Start No Earlier Than</p> <p>Start No Later Than</p> </td>
<td> <p><span class="s1">The Planned Completion Date is adjusted in order to keep the Duration the same.</span> </p> </td>
</tr>
<tr>
<td> <p>Fixed Dates</p> </td>
<td> <p>The Duration is adjusted in order to keep the Planned Completion Date the same.</p> </td>
</tr>
</tbody>
</table>
<p><strong>How the Planned Start Date is calculated for a task</strong></p>
<p>When it is calculated automatically by the system, the following can influence the Planned Start Date of a task:</p>
<ul>
<li> <p>The Start&nbsp;Date preference setting in the Tasks & Issues area in Setup</p> <p>Your Workfront or group administrator can determine whether a new task starts on the same date as the project's Planned Start&nbsp;Date or on the day you create the task.</p> <p>For information about Tasks &&nbsp;Issues preferences, see <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md" class="MCXref xref">Configure system-wide task and issue preferences</a>.</p> </li>
<li> <p>Task Constraint</p> <p>For more information about Task Constraints, see the article <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">Task Constraint overview</a></p> </li>
<li> <p>Task predecessor relationship</p> <p>For more information about task predecessors, see the article <a href="../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md" class="MCXref xref">Overview of task predecessors</a>.</p> </li>
<li>Project Start Date, when the project is scheduled from Start Date.</li>
<li> <p>The time off schedule of the Primary&nbsp;Assignee of the task. </p> <p>When the Primary Assignee has time off scheduled during the duration of the task, the planned dates of the task adjust accordingly when the <strong>Consider user time off in task durations</strong> setting is selected for the <strong>User Time Off</strong> field. New projects inherit this setting from the Project&nbsp;Preferences area, but you can edit the setting at the project level. </p> <p>For example, if a task with a Constraint of As Soon As Possible is scheduled to start on June 1 and complete on June 3, and the Primary Assignee has June 1 marked for Time-off, the task Planned Start Date becomes June 2. </p> <p>For information about the <strong>User Time Off</strong> preference, see the articles <span href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md"><a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configure system-wide project preferences</a></span> and <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">Edit projects</a>.</p> </li>
</ul>
<p>When set automatically, the Planned Start Date&nbsp;is determined based on the following calculation:&nbsp;</p>
<p><code>Planned Start Date = Planned Completion Date - Task Duration</code> </p>
<p>For example, if your task has a Completion Date of September 16 and a duration of 10 days, the Planned Start Date is September 6.</p> <note type="note"> &nbsp;The Update Type for the project must also be&nbsp;set to 'Automatic and On Change' or 'Automatically' in order for the Planned Hours and Duration to be automatically&nbsp;adjusted.
<br>For more information about the Update Type, see the article
<a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Select the project Update Type </a>.
</note>
</div>
-->
