---
content-type: reference
product-area: resource-management;user-management
navigation-topic: resource-planning
title: 使用「用戶」視圖時，查看資源計畫員中的可用小時數、計畫小時數和實際小時數或FTE
description: 在RP中使用User viewPlanning時查看資源計畫員中的可用小時數、計畫時數和實際小時數或FTE — 可能是「RP中的預算資源」或「RP中的管理資源」。 等…… — 或可能需要從其他POV中重新規劃?!)
author: Alina
feature: Resource Management
exl-id: 6b532aa2-435f-4fda-b7ce-abe0a785638f
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1738'
ht-degree: 1%

---

# 使用「用戶」視圖時，查看資源計畫員中的可用小時數、計畫小時數和實際小時數或FTE

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Consider renaming this article (probably split already) to something other than "Planning" in the RP" - maybe "budgeting resources in the RP" or "Managing Resources in the RP." etc... - or might need to be repurposed from another POV?!)</p>
-->

除了「項目」和「職責」視圖中的預算資源外，您還可以使用「Adobe Workfront資源計畫員」的「用戶視圖」來顯示有關項目和資源的「計畫」、「可用」和「實際小時數」或「FTE」值的資訊。

## 資源計畫員中的用戶視圖概覽

在資源計畫員中查看小時數或FTE資訊時，請考慮以下事項：

* 您可以在資源計畫員的所有視圖中查看用戶、職務職責和項目的可用小時數和計畫小時數或FTE資訊。
* 您只能在「使用者檢視」中檢視下列資訊：

   * 計畫小時數或FTE數與可用小時數或FTE數之差。 然後，您可以在「專案」和「角色」檢視中，根據此差異，為使用者分配預算。
   * 實際小時數或FTE。

* 您可以在「用戶」視圖中以數字或百分比值的形式顯示「用戶可用」與「計畫小時數」或「FTE」之間的差異。
* 不能按成本在「用戶」視圖中顯示資訊。
* Adobe Workfront會根據排程中與使用者相關聯的工作時間填入可用小時數或FTE。\
   未與排程相關聯的使用者會根據預設排程顯示可用性。\
   有關預設計畫的資訊，請參閱 [建立排程](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

* Workfront會從「計畫小時」資訊填入「計畫小時」或「FTE」，以了解專案上的工作和問題。
* Workfront會以指派給工作和問題的使用者所記錄的實際時間填入實際小時數。 這包括專案上的登入時間。
* 在「使用者」檢視中時，您可以執行下列動作：

   * 展開每個使用者以顯示指派給該使用者的專案清單。

      >[!NOTE]
      >
      >只有與篩選器中包含之專案相關聯的使用者才能展開。

   * 展開每個專案，以顯示使用者可在這些專案履行的工作角色清單。
   * 展開每個角色以顯示指派給該角色中使用者的任務清單。

   如果用戶沒有與他們相關聯的職務角色，則其「可用」、「計畫」和「實際小時數」或「FTE」將列在 **無角色** 區段。\
   有關在將用戶視圖應用於資源計畫員時顯示的欄位和物料的資訊，請參閱 [資源計畫員導航概覽](../../resource-mgmt/resource-planning/resource-planner-navigation.md).

## 資源計畫員的「用戶視圖」中可見的欄位概覽

有關了解在「資源計畫員」的「用戶」視圖中顯示的資訊，請參閱下表。 資訊以小時或FTE值顯示。

* [AVL（可用）欄](#the-avl-available-column)
* [「PLN（計畫）」列](#the-pln-planned-column)
* [ACT（實際）列](#The%C2%A0ACT)
* [DIF（差異）列](#the-dif-difference-column)
* [%（計畫小時數分配百分比）列](#the-planned-hours-allocation-percentage-column)

### AVL（可用）欄 {#the-avl-available-column}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>顯示者</strong> </td> 
   <td> <p><strong>說明</strong> </p> </td> 
  </tr> 
  <tr> 
   <td>使用者</td> 
   <td>根據用戶的計畫，用戶的可用小時數或FTE總數。 </td> 
  </tr> 
  <tr> 
   <td>專案</td> 
   <td>將用戶視圖應用於資源計畫員時，此資訊不適用於項目。 </td> 
  </tr> 
  <tr> 
   <td>角色</td> 
   <td> <p>根據用戶和 <strong>FTE可用性百分比</strong> 角色。</p> </td> 
  </tr> 
  <tr> 
   <td>任務或問題</td> 
   <td>此資訊不適用於任務或問題。 </td> 
  </tr> 
 </tbody> 
</table>

有關如何根據用戶計畫和角色的FTE可用性百分比計算用戶和角色可用性的詳細資訊，請參閱 [在資源計畫員中計算用戶和角色的小時數和FTE的概覽](../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md).

### 「PLN（計畫）」列 {#the-pln-planned-column}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>顯示者</strong> </td> 
   <td> <p><strong>說明</strong> </p> </td> 
  </tr> 
  <tr> 
   <td>使用者</td> 
   <td> 所有項目上分配給用戶的所有任務或問題的計畫小時數或FTE總數。<br><p>這包括指派給使用者但與任何工作角色無關的任務和問題，以及您有權存取「管理」的專案上不相關的任務或問題。</p><p>使用工作負載平衡器修改小時的用戶分配時，如果所選日期僅包含任務或問題的一部分，則資源規劃器中的資料可能會受到影響。 有關修改用戶分配的資訊，請參閱 <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">在工作負載平衡器中管理用戶分配</a> . </p></td> 
  </tr> 
  <tr> 
   <td>專案</td> 
   <td> 分配給項目上特定用戶的所有任務和問題的計畫小時數或FTE總數。<br><p>注意：這不包括未分配給任何用戶的任務或問題的計畫小時數或FTE。 </p></td> 
  </tr> 
  <tr> 
   <td>角色</td> 
   <td> <p>分配給項目上此角色的用戶的所有任務和問題的計畫小時數或FTE總數。</p> <p> <p>注意：這不包括分配給此角色但不分配給此角色的此用戶的任務或問題的計畫小時數或FTE。 </p> </p> </td> 
  </tr> 
  <tr> 
   <td>任務或問題</td> 
   <td>與任務或項目問題關聯的計畫小時數或FTE。</td> 
  </tr> 
 </tbody> 
</table>

檢視「計畫小時數」時，請考量下列事項：

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this is a snippet converted to text because there are difference from project/ role views and the user view (users with no pools DO show in user view)</p>
-->

* 針對分配給任務和問題的每個資源，計畫小時數在任務和問題持續時間內平均分配給每天。 任務或問題持續時間基於其計劃開始和完成日期，並包括該時段內的每個日曆日。\
   Workfront在將「計畫時間」分發給使用者或專案時，會考量使用者或專案的排程。 在這種情況下，計畫小時數在任務的持續時間或問題（不包括週末、超時天數和計畫例外）內平均分配給每天。

   例如，如果按周顯示資源計畫員，並且您的任務跨越項目的多個周，則每週計畫小時數取決於該周內多少天屬於任務持續時間的一部分。 在按月或季度顯示資源計畫器以及任務跨越多個月或季度時，這同樣適用。\
   此分配中不包括週末天數、排程例外和休假天數。

* 計算每個資源的「計畫小時數」時包括以下任務類別：

   * 分配給項目上資源池、作業角色或團隊中用戶的任務。

      >[!TIP]
      >
      >如果將任務指派給團隊，則其分配將顯示在 **無角色** 和 **無用戶** 區段。 您可以看到與團隊相關聯的計畫小時數，但無法預算小時數，因為沒有任何角色或用戶與任務相關聯。

* 資源計畫員中的計畫小時數不包含與以下項目關聯的計畫小時數：

   * 上層任務
   * 未分配的任務
   * 問題，當 **包括來自問題的小時數** 設定已停用。

* 如果任務或發放持續時間為零，計畫小時數不會顯示在資源計畫器中。
* 未顯示與停用的使用者相關聯的計畫小時數。

有關資源計畫員中計畫小時數和FTE的詳細資訊，請參閱 [資源計畫員的「項目」和「職責」視圖中的小時數、FTE和成本資訊概覽](../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md).

### ACT（實際）列

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>顯示者</strong> </td> 
   <td> <p><strong>說明</strong> </p> </td> 
  </tr> 
  <tr> 
   <td>使用者 </td> 
   <td> <p>使用者針對指派給他們的所有工作或問題所記錄的時間。</p> <p>這包括下列項目：</p> 
    <ul> 
     <li>已分配給用戶但未與任何作業角色關聯的任務和問題。</li> 
     <li>您有權存取「管理」的專案上沒有的工作和問題。 </li> 
    </ul> <p>這包括只有在將使用者指派給該專案的任務或問題時，才登入專案的時間。  </p> </td> 
  </tr> 
  <tr> 
   <td>專案 </td> 
   <td> <p>使用者在專案中針對指派給他們的所有工作和問題所記錄的時間。</p> <p>這包括使用者直接登入專案的任何時間。</p> <p>但不包括下列項目：</p> 
    <ul> 
     <li> <p>未指派給任何使用者的登入時間任務和問題。 </p> </li> 
     <li> <p>登入父任務的時間。 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>角色</td> 
   <td> <p>此角色中分配給用戶的所有任務或問題的登錄時間。 </p> <p>但不包括下列項目：</p> 
    <ul> 
     <li>分配給此角色但不分配給此角色的用戶的登錄任務和問題。</li> 
     <li>直接記錄在項目或父任務上的時間。 </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>任務或問題 </td> 
   <td> <p>也分配給任務和問題的用戶登錄的時間。 </p> </td> 
  </tr> 
 </tbody> 
</table>

>[!IMPORTANT]
>
>記錄的時間會顯示在與小時錄入的「參加日期」對應的時間範圍中，而無論記錄小時的任務、問題或專案的時間範圍。

有關「實際小時數」的詳細資訊，請參閱 [查看實際小時數](../../manage-work/tasks/task-information/actual-hours.md).

### DIF（差異）列 {#the-dif-difference-column}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>顯示者</strong> </td> 
   <td> <p><strong>說明</strong> </p> </td> 
  </tr> 
  <tr> 
   <td>使用者</td> 
   <td> <p>用戶的可用小時數和計畫小時數或FTE之間的差值。 </p> <p>小時或FTE差異使用下列公式計算：</p> <p><code style="font-style: normal;">User Hour or FTE Difference = User Available Hours or FTE - User Planned Hours or FTE</code> </p> <p> <p>注意：如果值以負紅色數字顯示，則用戶會被過度分配。 </p> </p> </td> 
  </tr> 
  <tr> 
   <td>專案</td> 
   <td>此資訊不適用於項目。 </td> 
  </tr> 
  <tr> 
   <td>角色</td> 
   <td> <p>職務角色的可用小時數和計畫小時數或FTE之間的差值。 </p> <p>小時或FTE差異使用下列公式計算：</p> <p><code style="font-style: normal;">Role Hour or FTE Difference = Role Available Hours or FTE - Role Planned Hours or FTE</code> </p> <p> <p>注意：如果值以負紅色數字顯示，則角色會被過度分配。 </p> </p> </td> 
  </tr> 
  <tr> 
   <td>任務或問題</td> 
   <td>此資訊不適用於任務、問題或項目。 </td> 
  </tr> 
 </tbody> 
</table>

### %（計畫小時數分配百分比）列 {#the-planned-hours-allocation-percentage-column}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>顯示者</strong> </td> 
   <td> <p><strong>說明</strong> </p> </td> 
  </tr> 
  <tr> 
   <td>使用者</td> 
   <td> <p>計畫小時數或FTE的分配，以可用小時數的百分比表示。 計畫小時數分配的百分比使用以下公式計算：</p> <p><code style="font-style: normal;">User Planned Hours Allocation Percentage = (User Planned Hours/ User Available Hours) * 100</code> </p> <p>FTE值使用的計算相同。 </p> </td> 
  </tr> 
  <tr> 
   <td>專案</td> 
   <td>套用 <strong>按用戶查看</strong> 查看資源計畫員。</td> 
  </tr> 
  <tr> 
   <td>角色</td> 
   <td> 計畫小時數或FTE的分配，以可用小時數的百分比表示。 <p>計畫小時數分配的百分比使用以下公式計算：</p><p><code style="font-style: normal;">Role Planned Hours Allocation Percentage = (Role Planned Hours/ Role Available Hours) * 100</code></p><p>FTE值使用的計算相同。</p></td> 
  </tr> 
  <tr> 
   <td>任務或問題</td> 
   <td>此資訊不適用於任務、問題或項目。 </td> 
  </tr> 
 </tbody> 
</table>

如果計畫小時數或FTE的值為零，則百分比分配為0%。 如果可用小時數或FTE的值為零，則無法計算百分比分配。

有關計畫小時數和FTE以及它們在資源計畫員中的顯示方式的詳細資訊，請參閱 [使用「項目」和「職責」視圖在資源計畫器中使用預算資源](../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;this table is ideal but it does not render in Markdown) </p>
-->

<!--
<table style="table-layout:auto">
<col>
<col>
<col>
<tbody>
<tr>
<td><strong>Column Name (Hours or FTE)</strong> </td>
<td><strong>Displayed By</strong> </td>
<td> <p><strong>Description</strong> </p> </td>
</tr>
<tr>
<td rowspan="5">AVL <br>(Available Hours or FTE)</td>
<td>User</td>
<td>The total of Available Hours or FTE for the user according to their schedule. </td>
</tr>
<tr>
<td>Project</td>
<td>This information is not available for the Project when applying the User view to the Resource Planner. </td>
</tr>
<tr>
<td>Role</td>
<td> <p>The total of Available Hours or FTE for the role according to the schedule of the user and the <strong>Percentage of FTE Availability</strong> of the role.</p> </td>
</tr>
<tr>
<td>Task or Issue</td>
<td>This information is not available for the Task, Issue, or Project.</td>
</tr>
<tr>
<td colspan="2"> <p colspan="2">For more information about how user and role availability is calculated based on the schedule of the user and the Percentage of FTE Availability of the role, see <a href="../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">Overview of calculating hours and FTE for users and roles in the Resource Planner</a>.</p> </td>
</tr>
<tr>
<td rowspan="5">PLN <br>(Planned Hours or FTE)</td>
<td>User</td>
<td> The total of Planned Hours or FTE from all the tasks or issues assigned to the user on all the projects.<br><p>This includes tasks and issues that are assigned to the user but not associated with any job role and tasks or issues that are not on projects that you have access to Manage.</p><p>When the user allocation for hours has been modified using the Workload Balancer, the data in the Resource Planner can be affected if the dates selected contain only a portion of a task or issue. For information about modifying allocations for users, see <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">Manage user allocations in the Workload Balancer</a> . </p></td>
</tr>
<tr>
<td>Project</td>
<td> The total of Planned Hours or FTE from all the tasks and issues assigned to a specific user on the project.<br><note type="note">
This does not include the Planned Hours or FTE from tasks or issues that are not assigned to any users.
</note></td>
</tr>
<tr>
<td>Role</td>
<td> <p>The total of Planned Hours or FTE from all the tasks and issues assigned to the user in this role on the project.</p> <p> <note type="note">
This does not include the Planned Hours or FTE from tasks or issues that are assigned to this role but not to this user in this role.
</note> </p> </td>
</tr>
<tr>
<td>Task or Issue</td>
<td>The Planned Hours or FTE associated with the task or the issue on the project.</td>
</tr>
<tr>
<td colspan="2"> <p>Consider the following when viewing Planned Hours:</p>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this is a snippet converted to text because there are difference from project/ role views and the user view (users with no pools DO show in user view))</p>
<ul>
<li> <p>Planned Hours are equally distributed to each day within the Duration of tasks and issues , for each resource assigned to them. The task or issue Duration is based on their Planned Start and Completion Dates and includes every calendar day within that period of time.<br>Workfront takes into account the schedule of the user or of the project when distributing Planned Hours to users or projects. In this case, Planned Hours are equally distributed to each day within the Duration of tasks or issues excluding weekends, time-off days, and schedule exceptions.</p> <p>If you display the Resource Planner by Week, for example, and you have tasks that span multiple weeks on projects, the number of Planned Hours per week depends on how many days within that week are part of the task Duration. This works similarly when displaying the Resource Planner by Month or Quarter and when tasks span multiple months or quarters.<br>Weekend days, schedule exceptions, and time-off days are excluded from this distribution.</p> </li>
<li> <p>The following categories of tasks are included in calculating the Planned Hours for each resource: </p>
<ul>
<li> <p> tasks assigned to users in Resource Pools, job roles, or teams on the project.</p> <note type="tip">
If tasks are assigned to teams, their allocation will appear under
<strong>No Role</strong> and
<strong>No User</strong> sections. You can see the Planned Hours associated with teams, but you cannot budget the hours, because no roles nor users are associated with the tasks.
</note> </li>
</ul> </li>
</ul>
<ul>
<li> Planned Hours in the Resource Planner do not include Planned Hours associated with the following:
<ul>
<li>parent tasks</li>
<li>unassigned tasks</li>
<li>issues, when the <strong>Include hours from Issues</strong> setting is disabled.</li>
</ul></li>
<li>Planned Hours do not display in the Resource Planner if the task or issue Duration is zero.</li>
<li>Planned Hours associated with deactivated users do not display. </li>
</ul> <p>For more information about Planned Hours and FTE in the Resource Planner, see <a href="../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md" class="MCXref xref">Overview of hours, FTE, and cost information in the Project and&nbsp;Role views of the Resource Planner</a>.</p> </td>
</tr>
<tr>
<td rowspan="5">ACT<br>(Actual Hours or FTE) </td>
<td>User </td>
<td> <p>The time logged by the user on all the tasks or issues assigned to them.</p> <p>This includes the following:</p>
<ul>
<li>Tasks and issues that are assigned to the user but not associated with any job role.</li>
<li>Tasks and issues that are not on projects for which you have access to Manage.. </li>
</ul> <p>This does not include time logged directly on the project or on parent tasks. </p> </td>
</tr>
<tr>
<td>Project </td>
<td> <p>The time logged by the user on all the tasks and issues assigned to them on the project.</p> <p>This includes any time that they logged directly on the project.</p> <p>This does not include the following:</p>
<ul>
<li> <p>Time logged on tasks and issues that are not assigned to any users. </p> </li>
<li> <p>Time logged on parent tasks. </p> </li>
</ul> </td>
</tr>
<tr>
<td>Role</td>
<td> <p>The time logged on all the tasks or issues assigned to the user in this role. </p> <p>This does not include the following:</p>
<ul>
<li>Time logged on tasks and issues assigned to this role but not to this user in this role.<em> </em></li>
<li>Time logged directly on the project or parent tasks. </li>
</ul> </td>
</tr>
<tr>
<td>Task or Issue </td>
<td> <p>The time logged on tasks and issues by the user who is also assigned to them. </p> </td>
</tr>
<tr>
<td colspan="2"> <p> <note type="important">
The time logged is displayed in the timeframe corresponding to the Entry Date of the hour entry, regardless of the timeframe of the task, issue, or project where the hours are logged.
</note> </p> <p>For more information about Actual Hours, see <a href="../../manage-work/tasks/task-information/actual-hours.md" class="MCXref xref">View Actual Hours</a></p> </td>
</tr>
<tr>
<td rowspan="4">DIF <br>(Hour or FTE Difference) <br><br></td>
<td>User</td>
<td> <p>The difference between the Available and Planned Hours or FTE of the user. </p> <p>The Hour or FTE difference is calculated using the following formula:</p> <p><code style="font-style: normal;">User Hour or FTE Difference = User Available Hours or FTE - User Planned Hours or FTE</code> </p> <p> <note type="note">
If the value displays in negative red numbers, the user is overallocated.
</note> </p> </td>
</tr>
<tr>
<td>Project</td>
<td>This information is not available for the Project. </td>
</tr>
<tr>
<td>Role</td>
<td> <p>The difference between the Available and Planned Hours or FTE of the job role. </p> <p>The Hour or FTE difference is calculated using the following formula:</p> <p><code style="font-style: normal;">Role Hour or FTE Difference = Role Available Hours or FTE - Role Planned Hours or FTE</code> </p> <p> <note type="note">
If the value is displayed in negative red numbers, the role is overallocated.
</note> </p> </td>
</tr>
<tr>
<td>Task or Issue</td>
<td>This information is not available for the Task, Issue, or Project. </td>
</tr>
<tr>
<td rowspan="5">Planned Hours or FTE Allocation Percentage (%)</td>
<td>User</td>
<td> <p>The allocation of the Planned Hours or FTE as a percentage of the Available Hours. The percentage of the Planned Hours Allocation is calculated using the following formula:</p> <p><code style="font-style: normal;">User Planned Hours Allocation Percentage = (User Planned Hours/ User Available Hours) * 100</code> </p> <p>The same calculation is used for FTE values. </p> </td>
</tr>
<tr>
<td>Project</td>
<td>This information is not available for the Project when applying the <strong>View by User</strong> view to the Resource Planner.</td>
</tr>
<tr>
<td>Role</td>
<td> The allocation of the Planned Hours or FTE as a percentage of the Available Hours. <p>The percentage of the Planned Hours Allocation is calculated using the following formula:</p><p><code style="font-style: normal;">Role Planned Hours Allocation Percentage = (Role Planned Hours/ Role Available Hours) * 100</code></p><p>The same calculation is used for FTE values.</p></td>
</tr>
<tr>
<td>Task or Issue</td>
<td>This information is not available for the Task, Issue, or Project. </td>
</tr>
<tr>
<td colspan="2"> <p> If the value of the Planned Hours or FTE is zero, the Percentage Allocation is 0%. If the value of the Available Hours or FTE is zero, the Percentage Allocation cannot be calculated. </p> <p>For more information about Planned Hours and FTE and how they are displayed in the Resource Planner, see <a href="../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md" class="MCXref xref">Budget resources in the Resource Planner using the Project and Role views</a>. </p> </td>
</tr>
</tbody>
</table>
-->
