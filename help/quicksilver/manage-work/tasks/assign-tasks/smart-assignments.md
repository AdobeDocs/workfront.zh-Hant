---
content-type: overview;how-to-procedural
product-area: projects;user-management
navigation-topic: assign-tasks
title: 智慧分配概述
description: 在管理任務和問題分配時，您可以使用智慧分配來確定最適合的用戶來完成工作。 智慧分配是當您根據演算法將工作項目指派給資源時，Adobe Workfront會向您顯示的建議，演算法可決定該工作的最合適資源。
author: Alina
feature: Work Management
exl-id: 8d17eff6-5ff0-4985-b575-4934a3bb7c0b
source-git-commit: 7e220e496aff2675910416bd86e3ddf7b9231afa
workflow-type: tm+mt
source-wordcount: '526'
ht-degree: 0%

---

# 智慧分配概述

在管理任務和問題分配時，您可以使用智慧分配來確定最適合的用戶來完成工作。 智慧分配是當您根據演算法將工作項目指派給資源時，Adobe Workfront會向您顯示的建議，演算法可決定該工作的最合適資源。

>[!NOTE]
>
>智慧分配不考慮用戶的可用性。 但是，根據其計畫提供它們會影響任務和問題的計畫日期和預計日期（在分配任務和問題時）。 如需排程的相關資訊，請參閱文章 [建立排程](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

本文包含有關智慧分配的一般資訊。 有關使用智慧分配將任務和問題分配給用戶的資訊，請參閱 [進行智慧分配](../../../manage-work/tasks/assign-tasks/make-smart-assignments.md).

## 智慧分配概述

使用智慧指派時，請考量下列事項：

* 演算法可獨立運作於任務和問題。 這表示問題的建議使用者清單可能與任務的建議使用者清單不同，因為Workfront會根據與問題和任務相關的標準分別建立清單。
* 智慧分配不建議作業角色或團隊。 而是最適合完成工作或問題的使用者建議。
* 建議的分配始終為活動用戶。
* 第一個列出的使用者應是該工作的最佳相符者。

## 查找智慧分配建議

您可以在以下區域查看智慧分配，在這些區域中可以分配任務或問題：

* 任務或問題清單或報告

   ![](assets/smart-assignments-task-list-nwe-350x280.png)

* 任務或問題標題

   ![](assets/smart-assignments-task-header-nwe-350x302.png)

* 任務或問題摘要面板

   ![](assets/smart-assignments-summary-panel-nwe-350x332.png)

* 「主」區域中所列項的「分配」欄位

   ![](assets/smart-assignments-in-home-nwe-350x216.png)


<!--removed for scheduling deprecation: 

* Resource Scheduling

  ![](assets/smart-assignments-scheduling-350x219.png)

  >[!CAUTION]
  >
  >Resource Scheduling is a deprecated feature. For more information, see [Deprecation of Resource Scheduling tools in Adobe Workfront](../../../resource-mgmt/resource-mgmt-overview/deprecate-resource-scheduling.md).

-->
* 工作負載平衡器

   ![](assets/smart-assignments-workload-balancer-bulk-assignments.png)


## 智慧分配條件

智慧型指派會根據專屬演算法顯示前50個建議。

根據以下條件的組合（按從最重要到最不重要的順序列出），在智慧分配下拉清單中建議用戶：

* 過去30天內由進行分配的用戶分配給其他工作項的用戶。 接下來會顯示符合此條件的前50位使用者。 最常被指派的使用者會先顯示。

   如果工作項被分配給團隊或角色，則建議用戶的清單會進一步篩選，同時考慮到下面的現有分配。 在此情況下，建議清單中只會顯示下列使用者：

   * 其「主團隊」是指派給工作項的團隊的用戶。
   * 其「主要角色」是指派給工作項的角色的用戶。

      >[!TIP]
      >
      >* 若 <!--you're not part of any team and --> 沒有為任務或問題指派任何角色或團隊，Workfront會顯示過去30天（最多50個使用者）指派的所有使用者。
      >* 如果過去30天內未進行任何分配，則智慧分配清單中只會顯示屬於已分配團隊或已分配給工作項的角色的用戶。


<!--the commented out piece in the tip above was live before but I am not totally sure that smart assignments look at your team. I think they look JUST at the team/ role assigned to the work item; see this help site request for more info: https://experience.adobe.com/#/@adobeinternalworkfront/so:hub-Hub/workfront/issue/62fd222200037eb87572c5b6ad6bf53e/overview -->
<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<div>
<h3>Smart assignments criteria for the Production environment</h3>
<p>(NOTE: drafted,this was the case BEFORE we updated the logic in the WB - with the 21.4 release)</p>
</div>
<p>Smart assignments display on tasks and issues when the following conditions are met:</p>
<ul>
<li>The task or issue is subordinate to a parent task or issue that has a user, team, or job role currently assigned. </li>
</ul>
<p>Smart assignments display the top twenty recommendations based on a proprietary algorithm that uses your own team information.</p>
<p>Users are recommended in the smart assignments drop-down list based on a combination of the following criteria (listed in order from most important to least important):</p>
<ul>
<li>The user has the team assigned to the task or issue designated as their Home Team</li>
<li>The user is also assigned to the parent task</li>
<li>The user has the same primary job role as is currently assigned to the task or issue</li>
<li>The user has the team assigned to the parent task or issue designated as their Home Team</li>
<li>The user is associated with the same primary job role currently assigned to the parent task</li>
<li>The user is a member of the same team as the user who assigned the task or issue and the team is designated as their Home Team</li>
<li>The user is a member of the same Home Group as the user who is assigning the task or issue</li>
<li>The user has the same primary job role as the user who is assigning the task or issue.</li>
</ul>
</div>
-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Make smart assignments</h2>
<p>(NOTE:&nbsp;this was moved to its own article: make-smart-assignments.) </p>
<p>Smart assignments are available in most locations where you can make assignments in Workfront.</p>
<p>You can use smart assignments on tasks and issues that have previously been assigned to a job role or a team.</p> <note type="note">
You must have a Plan or a Work license and have at least Contribute permissions to a task or an issue to be able to make assignments to the task or the issue. You must have the Make Assignments option enabled in your permission level to make assignments.
</note>
<p>To use smart assignments:</p>
<ol>
<li value="1">Navigate to an issue or a task and click one of the following fields to edit them: <br>
<ul>
<li><p data-mc-conditions="QuicksilverOrClassic.Quicksilver">The <strong>Assignments</strong> field in the task or issue header</p></li>
<li>The <strong>Assignments</strong> field of a task or issue list using in-line editing in a task or issue list. </li>
<li>The <strong>Assignee</strong> field after you have clicked <strong>Advanced</strong> from a task or an issue. </li>
</ul></li>
<li value="2"> <p>Place your cursor in the assignment field, and wait for two seconds, then the <strong>Suggestions</strong> list is displayed.</p> <p>Users displayed in this list are the smart assignment suggestions for the task or the issue.<br></p> <p> <img src="assets/nwe-smart-assignment-suggestions-350x160.png" style="width: 350;height: 160;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> </p> </li>
<li value="3"> <p>Select the user in the recommendations list by clicking their name. </p> <p>If there are no suggestions, the suggestion list does not open.</p> </li>
<li value="4">(Optional) If you do not want to use one of the recommended users from the smart assignments list, start typing the name of the desired user and select the name when it appears in the list.</li>
<li value="5">Click <strong>Enter</strong> to make the assignment. </li>
</ol>
</div>
-->
