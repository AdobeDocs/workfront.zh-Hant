---
content-type: reference
product-area: resource-management;user-management
navigation-topic: resource-planning
title: 使用使用者檢視時檢視資源規劃工具中的可用、計畫和實際時數或FTE
description: 在RP中使用「使用者」檢視計畫時，在「資源規劃工具」中檢視可用、計畫及實際時數或FTE — 可能是「RP中的預算資源」或「RP中的管理資源」。 等等…… — 或可能需要從其他POV重新利用?!)」
author: LIsa
feature: Resource Management
exl-id: 6b532aa2-435f-4fda-b7ce-abe0a785638f
source-git-commit: 3c3175c347431b10aed1a6034df6c756056399b3
workflow-type: tm+mt
source-wordcount: '1739'
ht-degree: 1%

---

# 使用使用者檢視時檢視資源規劃工具中的可用、計畫和實際時數或FTE

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Consider renaming this article (probably split already) to something other than "Planning" in the RP" - maybe "budgeting resources in the RP" or "Managing Resources in the RP." etc... - or might need to be repurposed from another POV?!)</p>
-->

除了在「專案」與「角色」檢視中編列資源預算外，您也可以使用Adobe Workfront資源規劃工具的「使用者檢視」，來顯示有關專案與資源的「計畫」、「可用」與「實際時數」或「約當全職人數」值的資訊。

## 資源規劃工具中的使用者檢視概要

在資源規劃工具中檢視時數或約當全職人數資訊時，請考量下列事項：

* 您可以在資源規劃工具的所有檢視中，檢視使用者、工作角色和專案的可用和計畫時數或FTE資訊。
* 您只能在「使用者檢視」中檢視下列資訊：

   * 計畫時數或約當全職人數與可用時數或約當全職人數之間的差額。 接著，您就可以根據專案和角色檢視中的這項差異，為使用者配置預算。
   * 實際時數或FTE。

* 您可以在「使用者」檢視中，以數字或百分比值顯示「可用使用者」與「計畫時數」或「約當全職人數」之間的差異。
* 您無法在使用者檢視中依成本顯示資訊。
* Adobe Workfront會根據與使用者相關聯的工作時間在其排程中填入可用時數或FTE。\
  未與排程關聯的使用者會根據預設排程顯示可用性。\
  如需有關預設排程的資訊，請參閱[建立排程](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)。

* Workfront會從計畫時數資訊中填入專案上任務和問題的計畫時數或FTE。
* Workfront會將實際時間填入實際小時，實際時間由指派給它們的使用者記錄到任務和問題。 這包括專案的登入時間。
* 在「使用者」檢視中，您可以執行下列動作：

   * 展開每位使用者以顯示指派該使用者的專案清單。

     >[!NOTE]
     >
     >只有與篩選器中所包含專案相關聯的使用者才能展開。

   * 展開每個專案以顯示使用者可在這些專案中完成的工作角色清單。
   * 展開每個角色，以顯示該角色中的使用者指派給該角色的任務清單。

  如果使用者沒有關聯的工作角色，**無角色**&#x200B;區段中會列出他們的可用、計畫和實際時數或FTE。\
  如需有關將使用者檢視套用至資源規劃工具時顯示哪些欄位和專案的資訊，請參閱[資源規劃工具導覽概觀](../../resource-mgmt/resource-planning/resource-planner-navigation.md)中的「專案/角色/使用者檢視選擇」一節。

## 在資源規劃工具的使用者檢視中可見的欄位概觀

請參考下表以瞭解資源規劃工具「使用者」檢視中顯示的資訊。 資訊會以時數或FTE值顯示。

* [AVL （可用）資料行](#the-avl-available-column)
* [計畫（計畫）資料行](#the-pln-planned-column)
* [ACT （實際）資料行](#The%C2%A0ACT)
* [DIF （差異）資料行](#the-dif-difference-column)
* [% （計畫時數配置百分比）欄](#the-planned-hours-allocation-percentage-column)

### AVL （可用）欄 {#the-avl-available-column}

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
   <td>使用者根據其排程的可用時數或FTE總數。 </td> 
  </tr> 
  <tr> 
   <td>專案</td> 
   <td>將使用者檢視套用至資源規劃工具時，此資訊不適用於專案。 </td> 
  </tr> 
  <tr> 
   <td>角色</td> 
   <td> <p>根據使用者的排程和角色的<strong>FTE可用性百分比</strong>，角色的可用時數或FTE總數。</p> </td> 
  </tr> 
  <tr> 
   <td>任務或問題</td> 
   <td>此資訊不適用於任務或問題。 </td> 
  </tr> 
 </tbody> 
</table>

如需有關如何根據使用者的排程和角色的FTE可用性百分比計算使用者和角色可用性的詳細資訊，請參閱[計算資源規劃工具中使用者和角色的時數和FTE的概觀](../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md)。

### 計畫（計畫）欄 {#the-pln-planned-column}

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
   <td> 從所有專案中指派給使用者的所有任務或問題的總計畫時數或FTE。<br><p>這包括指派給使用者但與任何工作角色沒有關聯的任務和問題，以及您無權管理之專案上的任務或問題。</p><p>當使用工作負載平衡器修改使用者時數分配時，如果所選的日期僅包含任務或問題的一部分，則資源規劃工具中的資料可能會受到影響。 如需有關修改使用者的配置資訊，請參閱在工作負載平衡器</a>中管理使用者配置。<a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref"> </p></td> 
  </tr> 
  <tr> 
   <td>專案</td> 
   <td> 從所有任務和問題中指派給專案中特定使用者的總計畫時數或FTE。<br><p>注意：這不包括未指派給任何使用者的任務或問題的計畫時數或FTE。 </p></td> 
  </tr> 
  <tr> 
   <td>角色</td> 
   <td> <p>從所有任務和問題中指派給專案中此角色之使用者的總計畫時數或FTE。</p> <p> <p>注意：這不包括計畫時數或來自指派給此角色但不指派給此角色中此使用者的任務或問題的FTE。 </p> </p> </td> 
  </tr> 
  <tr> 
   <td>任務或問題</td> 
   <td>與專案上的任務或問題關聯的計畫時數或FTE。</td> 
  </tr> 
 </tbody> 
</table>

檢視計畫時數時，請考慮下列事項：

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this is a snippet converted to text because there are difference from project/ role views and the user view (users with no pools DO show in user view)</p>
-->

* 對於指派給它們的每個資源，計畫時數會平均分配給任務和問題期間內的每一天。 任務或問題期間以其計劃開始和完成日期為基礎，並包含該時段內的每個行事曆日。\
  當向使用者或專案分配計畫時數時，Workfront會考慮使用者或專案的排程。 在這種情況下，計畫時數平均分配給任務或問題期間內的每一天，不包括週末、休假天和排程例外。

  例如，如果您按周顯示「資源規劃工具」，而您有專案上跨越多個周的任務，則每週的計畫時數取決於該周內的多少天屬於任務「工期」。 當按月或季度顯示資源規劃工具，以及任務跨越多個月或季度時，其作用類似。\
  週末天數、排程例外和休假天數會從此分佈中排除。

* 計算每個資源的計畫時數時，會包含下列任務類別：

   * 指派給資源集區、工作角色或專案團隊中使用者的任務。

     >[!TIP]
     >
     >如果任務已指派給團隊，則其配置將顯示在&#x200B;**無角色**&#x200B;和&#x200B;**無使用者**&#x200B;區段下。 您可以檢視與團隊關聯的計畫時數，但無法預算時數，因為沒有任何角色或使用者與任務相關聯。

* 資源規劃工具中的計畫時數不包含與下列專案關聯的計畫時數：

   * 父系任務
   * 未指派任務
   * 問題，當&#x200B;**包含來自問題的時數**&#x200B;設定停用時。

* 如果任務或問題期間為零，則計畫時數未顯示在資源規劃工具。
* 未顯示與已停用使用者相關的計畫時數。

如需資源規劃工具中計畫時數和FTE的詳細資訊，請參閱資源規劃工具專案和角色檢視中的[時數概觀、FTE和成本資訊](../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md)。

### ACT （實際）欄

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
   <td> <p>使用者在指派給他們的所有任務或問題上記錄的時間。</p> <p>這包含下列專案：</p> 
    <ul> 
     <li>指派給使用者但不與任何工作角色相關聯的任務和問題。</li> 
     <li>不在您有權管理的專案上的任務和問題。 </li> 
    </ul> <p>這包括僅當使用者被指派至該專案上的任務或問題時登入專案的時間。  </p> </td> 
  </tr> 
  <tr> 
   <td>專案 </td> 
   <td> <p>使用者在專案上記錄所有指派給他們的任務和問題的時間。</p> <p>這包括使用者直接登入專案的任何時間。</p> <p>這不包括下列專案：</p> 
    <ul> 
     <li> <p>登入未指派給任何使用者的任務和問題的時間。 </p> </li> 
     <li> <p>父系任務的登入時間。 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>角色</td> 
   <td> <p>登入指派給此角色中使用者的所有任務或問題的時間。 </p> <p>這不包括下列專案：</p> 
    <ul> 
     <li>登入指派給此角色但未指派給此角色之使用者的任務和問題的時間。</li> 
     <li>直接在專案或父系任務上記錄的時間。 </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>任務或問題 </td> 
   <td> <p>受指派的使用者登入任務和問題的時間。 </p> </td> 
  </tr> 
 </tbody> 
</table>

>[!IMPORTANT]
>
>記錄的時間會以與時數專案的「輸入日期」對應的時間範圍顯示，無論記錄時數的任務、問題或專案的時間範圍為何。

如需實際時數的詳細資訊，請參閱[檢視實際時數](../../manage-work/tasks/task-information/actual-hours.md)。

### DIF （差異）欄 {#the-dif-difference-column}

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
   <td> <p>可用和計畫時數之間的差異，或使用者的FTE。 </p> <p>小時或FTE差異的計算公式如下：</p> <p><code style="font-style: normal;">User Hour or FTE Difference = User Available Hours or FTE - User Planned Hours or FTE</code> </p> <p> <p>備註：如果值以負數紅色顯示，則表示使用者過度配置。 </p> </p> </td> 
  </tr> 
  <tr> 
   <td>專案</td> 
   <td>此資訊不適用於專案。 </td> 
  </tr> 
  <tr> 
   <td>角色</td> 
   <td> <p>工作角色的可用和計畫時數或FTE之間的差異。 </p> <p>小時或FTE差異的計算公式如下：</p> <p><code style="font-style: normal;">Role Hour or FTE Difference = Role Available Hours or FTE - Role Planned Hours or FTE</code> </p> <p> <p>備註：如果值以負數顯示，則會過度配置角色。 </p> </p> </td> 
  </tr> 
  <tr> 
   <td>任務或問題</td> 
   <td>任務、問題或專案無法提供此資訊。 </td> 
  </tr> 
 </tbody> 
</table>

### % （計畫時數配置百分比）欄 {#the-planned-hours-allocation-percentage-column}

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
   <td> <p>計畫時數或FTE的配置，以可用時數的百分比表示。 計畫時數配置的百分比使用下列公式計算：</p> <p><code style="font-style: normal;">User Planned Hours Allocation Percentage = (User Planned Hours/ User Available Hours) * 100</code> </p> <p>FTE值會使用相同的計算。 </p> </td> 
  </tr> 
  <tr> 
   <td>專案</td> 
   <td>將<strong>依使用者的檢視</strong>套用至資源規劃工具時，此資訊無法供專案使用。</td> 
  </tr> 
  <tr> 
   <td>角色</td> 
   <td> 計畫時數或FTE的配置，以可用時數的百分比表示。 <p>計畫時數配置的百分比使用下列公式計算：</p><p><code style="font-style: normal;">Role Planned Hours Allocation Percentage = (Role Planned Hours/ Role Available Hours) * 100</code></p><p>FTE值會使用相同的計算。</p></td> 
  </tr> 
  <tr> 
   <td>任務或問題</td> 
   <td>任務、問題或專案無法提供此資訊。 </td> 
  </tr> 
 </tbody> 
</table>

如果計畫時數或FTE的值為零，則百分比配置為0%。 如果「可用時數」或「約當全職人數」的值為零，則無法計算「百分比配置」。

如需計畫時數和FTE的詳細資訊，以及它們在「資源規劃工具」中的顯示方式，請參閱資源規劃工具中使用「專案」和「角色」檢視的[預算資源](../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md)。

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
