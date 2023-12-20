---
content-type: overview;how-to-procedural
product-area: projects;user-management
navigation-topic: assign-tasks
title: 智慧指派總覽
description: 在管理任務和問題指派時，您可以使用智慧指派來識別誰是完成工作的最佳使用者。 智慧型指派是Adobe Workfront在您根據演演算法將工作專案指派給資源時所顯示的建議，該演演算法會決定最適合工作的資源。
author: Alina
feature: Work Management
exl-id: 8d17eff6-5ff0-4985-b575-4934a3bb7c0b
source-git-commit: daba001c28df268721c87df7d2516ffb76e535d9
workflow-type: tm+mt
source-wordcount: '520'
ht-degree: 0%

---

# 智慧指派總覽

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers.</span>   
  
<span class="preview">For information about the current release schedule, see [First Quarter 2024 release overview](/help/quicksilver/product-announcements/product-releases/24-q1-release-activity/24-q1-release-overview.md).</span> 
-->

在管理任務和問題指派時，您可以使用智慧指派來識別誰是完成工作的最佳使用者。 智慧型指派是Adobe Workfront在您根據演演算法將工作專案指派給資源時所顯示的建議，該演演算法會決定最適合工作的資源。

>[!NOTE]
>
>智慧型指派未考慮使用者的可用性。 但是，根據它們的排程可用性，會影響任務和問題在指派時的計畫和預計日期。 如需有關排程的資訊，請參閱文章 [建立排程](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

本文包含智慧指派的一般資訊。 有關使用智慧指派指派指派任務和問題給使用者的資訊，請參閱 [進行智慧型指派](../../../manage-work/tasks/assign-tasks/make-smart-assignments.md).

## 智慧指派總覽

使用智慧型指派時，請考量下列事項：

* 演演算法可獨立處理任務和問題。 這表示問題的建議使用者清單可能與任務的建議使用者清單不同，因為Workfront會根據與問題和任務分別相關的准則來建立清單。
* 智慧指派不建議職務角色或團隊。 相反地，他們是最適合完成任務或問題的使用者的建議。
* 建議的指派一律為作用中的使用者。
* 首先列出的使用者應該是此任務的最佳相符者。

## 尋找智慧指派建議

您可以在下列區域中檢視智慧型指派，您可指派任務或問題：

* 任務、問題清單或報告 <!--edit this to say just issue list or report and update screen shot - add new one-->

  ![](assets/smart-assignments-task-list-nwe-350x280.png)

<!--
* <span class="preview">A task list or report (******insert shot here*****)</span>
-->

* 任務或問題標題

  ![](assets/smart-assignments-task-header-nwe-350x302.png)

* 任務或問題摘要面板

  ![](assets/smart-assignments-summary-panel-nwe-350x332.png)

* 「首頁」區域中列出之專案的「工作總攬」欄位

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


## 智慧指派條件

<!--
<div class="preview">

Smart assignments work differently for tasks than for issues.  

### Smart assignments criteria for tasks

Task smart assignments work in two phases:  

#### First phase of smart assignment calculation criteria for tasks 

Workfront calculates a similarity score for every assignment. The calculation for the similarity score and the order in which the assignments are listed take into account the following:  

* A score of 100% is given to an existing assignment where the task, project, and portfolio names are identical to the task you're trying to assign. The project and portfolio names of the task of an existing assignment must also match the project and portfolio of the task you are trying to assign.   

* If only some of this information from other assignments matches on the existing tasks, the score might be lower.  

  For example, if you are assigning a task called "My second task" on a project called "My project" in a portfolio called "My portfolio" and you have an existing task called "My task" in another project called "My project" in a portfolio called "My portfolio", the user assigned to "My task" might get a score of 95% because the name of the existing task and the task you're trying to assign now are similar, but not identical.  
 
    >[!TIP]
    >
    >  Workfront looks for matches only in the Name fields of tasks, projects, and portfolios and not in any other fields. 

* An assignment could get a higher score when they are assigned to a lot of tasks in the system that are similar in names. For example, if a team called "Development" is assigned to 50% of the tasks in the system containing "AI" in the name and you are now assigning another task with "AI" in the name, the score of the "Development" team is higher. In this case, the names of  projects and portfolios are not as important.  

* Taking into account this scoring system, the first 7 suggestions are listed as smart assignments, in the descending order of their scores. Assignments with scores lower than 40% do not display.  

* If several assignments have identical scores, they display in descending order of the date on which the assignments were made.  
For example, if Rick was assigned to a similar task earlier today and Jennifer was assigned to a similar task two days ago, Rick displays first.  

* If there are no matches using this calculation, the second step of smart assignments applies which is calculated using a different algorithm.  

#### Second phase of smart assignment calculation criteria for tasks

If the first step of task smart assignments has found no matches, Workfront calculates smart assignments for tasks in the same way that it calculates them for issues.  

### Smart assignments criteria for tasks and issues 

</div> 

>[!NOTE]
>
><span class="preview">The following criteria applies for tasks only when the first phase of the task smart assignment calculation did not find any matches. The following criteria always applies for issues, by default. </span>

-->

根據以下條件的組合，建議在智慧指派下拉式清單中使用者（按照從最重要到最不重要的順序列出）：

1. 由進行指派的使用者在過去30天內指派給其他工作專案的使用者。 符合此條件的前50名使用者隨即顯示。 最常被指派的使用者會先顯示。

2. 如果將工作專案指派給團隊或角色，則會進一步篩選建議的使用者清單，並考量以下現有的指派。 在此情況下，建議清單只會顯示下列使用者：

   * 主團隊是指派給工作專案的團隊的使用者。
   * 主要角色是指派給工作專案的角色的使用者。

>[!TIP]
>
>* 如果任務或問題未指派任何角色或團隊，Workfront會顯示過去30天指派的所有使用者，最多50名使用者。
>
>* 如果您在過去30天內未進行任何指派，則只有屬於指派的團隊或擁有指派給工作專案的角色的使用者才會顯示在智慧指派清單中。

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
