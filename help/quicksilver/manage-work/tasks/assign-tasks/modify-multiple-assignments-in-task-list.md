---
product-area: projects;user-management
navigation-topic: assign-tasks
title: 修改任務清單中的多個用戶分配
description: 在管理任務分配時，您可以使用任務清單中的批量編輯功能一次同時修改多個任務的任務。
author: Alina
feature: Work Management
exl-id: 04f7761f-da94-4858-85c5-8dc97bd78bee
source-git-commit: fb538c6511514eedf81f4b9be452d5f87e3f7577
workflow-type: tm+mt
source-wordcount: '976'
ht-degree: 0%

---

# 修改任務清單中的多個用戶分配

<!--
<p>There is a similar article in Resource Scheduling and a similar one for Issues; when things change, you might need to update all 3</p>
-->

在管理任務分配時，您可以使用任務清單中的批量編輯功能一次同時修改多個任務的任務。

本文涉及修改任務清單中多個任務的多個用戶分配。 另請參閱以下文章，以修改其他領域中多個任務的分配：

* 有關使用工作負載平衡器分配任務的資訊，請參見 [工作負載平衡器中分配工作的概述](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md).

有關將任務分配給清單中的一個資源的資訊，請參閱 [指派任務](../../../manage-work/tasks/assign-tasks/assign-tasks.md).

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
   <td> <p>工作或更高</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>編輯專案和工作的存取權</p> <p>檢視或更高的使用者存取權</p> <p>注意：如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>協助執行工作或擁有更高權限</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>When to modify user assignments on tasks</h2>
<p>(NOTE: moved to the new article: /Content/Manage work/Tasks/Assign tasks/modify-task-assignments-overview.htm) </p>
<p>You might want to modify the user assignments for multiple tasks for a variety of reasons, including the following:</p>
<ul>
<li>Users join or leave your team</li>
<li> <p>A user takes a vacation that extends beyond task due dates</p> <note type="note">
When assigning users to work, their availability according to their schedules affects the Planned and Projected Dates of tasks. For information about schedules, see
<a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Create a schedule</a>.
</note> </li>
<li>A specific role or user is set as the assignee for multiple tasks and you want to quickly modify all items to be assigned to a different user or role</li>
</ul>
<p><strong>How removing assignees affects task hours and allocation percentages</strong></p>
<p>(NOTE: move to the new article: /Content/Manage work/Tasks/Assign tasks/modify-task-assignments-overview.htm) </p>
<p>Removing users can affect task hours and allocation percentages. The effect that removing a user has on the task depends on the Duration Type that was selected for the task. For information about Duration&nbsp;Type, see <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Overview of Task Duration and Duration Type</a>.</p>
<p>When you delete a user from a task with the following Duration&nbsp;Types:</p>
<ul>
<li> <p><strong>Simple:</strong> The planned hours assigned to that user are subtracted from the task's total planned hours.</p> <note type="important">
<span class="s1">This could negatively affect your project plan because it changes the total planned hours for the task and the project.</span>
</note> </li>
<li><span class="s1"><strong>Effort Driven:</strong> The allocation percentage does not change for other users.</span> </li>
<li><span class="s1"><strong>Calculated Assignment:</strong> The allocation percentages of other users are adjusted so that the total equals 100%.</span> </li>
<li><span class="s1"><strong>Calculated Work:</strong> The allocation percentage does not change for other users.</span> </li>
</ul>
</div>
-->

## 修改多個任務的分配

1. 轉到包含要修改分配的任務的清單。
1. （可選）建立篩選器，僅顯示分配給要修改的受託人的任務。

   例如，如果您的項目包含作為多個任務的預設受託人的特定角色，則可以建立篩選器以僅顯示作為受託人具有該角色的任務。 然後，您可以將角色取代為特定使用者。

   如需建立篩選器的相關資訊，請參閱 [建立或編輯篩選器](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md).


1. 要篩選角色，請選擇 **分配角色**，然後按一下 **ID**.

   >[!TIP]
   >
   >請勿使用 **指派給** 欄位。 這只會查找任務的主要所有者，而不能查找可以分配給它們的任何角色。

   或

   若要篩選使用者，請選取 **分配用戶，** 然後按一下 **ID.**

   >[!TIP]
   >
   >請勿使用 **指派給** 欄位。 這只會找到任務的主要所有者，而不是任何可分配給它們的用戶。

1. 選擇要修改其分配的任務，然後按一下 **編輯** 圖示 ![](assets/edit-icon.png).

   將顯示「編輯任務」頁。 您編輯的項目會顯示在頁面的左上角。

1. 前往 **分配** 區段。
1. 執行以下操作之一以添加或刪除受分配者：

   >[!IMPORTANT]
   >
   >刪除受分配者會影響任務小時數和分配百分比。 如需詳細資訊，請參閱 [刪除受分配者如何影響任務小時數和分配百分比](#how-removing-assignees-affects-task-hours-and-allocation-percentages) 這篇文章。

   * 要添加新的受託人，請執行以下操作：

      1. 在 **分配** 部分，選擇 **受託人**.

         會顯示所有所選任務中的常見資訊。 例如，如果將相同的使用者指派給所有工作，該使用者會顯示在 **受託人** 欄。 如果資訊在所選任務中不常見，則不會顯示任何資訊。

      1. 開始鍵入用戶、角色或團隊的名稱，然後在清單中顯示時選擇它。 會添加分配，不會替換所選任務上的當前分配。
      >[!TIP]
      >
      > * 您可以指派多個使用者、工作角色或團隊。 您只能指派作用中的使用者、工作角色和團隊。
      >   
      > * 新增使用者指派時，請注意頭像、使用者的主要角色或其電子郵件地址，以區分名稱相同的使用者。 用戶必須至少與一個作業角色關聯，才能在添加時查看該角色。

         > 
         >   如果在停用前已指派使用者、工作角色或團隊，則他們仍會指派給工作項目。 在此情況下，我們建議：
         >   
         >     * 將工作項重新分配給活動資源。
         >     * 將已停用團隊中的用戶與活動團隊關聯，並將工作項重新分配給活動團隊。



   * 要刪除單個受分配者，請執行以下操作：

      1. 按一下 **X圖示** 如果「分配」清單中顯示了受分配人，則您要刪除的受分配人的名稱旁邊。

         或

         （條件性）如果要刪除的受託人不會顯示在「分配」部分，因為受託人僅被分配給您選擇的某些任務，請按一下 **刪除受託人** 然後開始鍵入要刪除的受託人的名稱，然後在下拉清單中出現名稱時按一下該名稱。
   * 要刪除所有現有受分配者：

      1. 按一下 **刪除所有現有受分配者**，然後按一下 **是，刪除所有受分配者**.

         這不僅會刪除常見的受分配者（在編輯對話框中顯示的受分配者），而且還會刪除所有選定任務上的所有受分配者。
      從任務中刪除用戶會影響任務小時數和分配百分比。

      如需詳細資訊，請參閱 [修改任務分配概覽](../../../manage-work/tasks/assign-tasks/modify-task-assignments-overview.md).





1. （可選）為受分配者修改以下任一選項：

   * （有條件） **分配%或小時**:指定新的分配百分比或小時數。

      >[!NOTE]
      >
      >只有在正在編輯的所有任務中持續時間類型相同時，才能修改此選項。 當「工作」或「工作」驅動的持續時間類型時，您可以更新「分配」百分比。 當「持續時間類型」為「簡單」時，您可以更新「小時」。 如需持續時間類型的相關資訊，請參閱 [任務持續時間和持續時間類型概覽](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).
      如果欄位空白，這表示值在不同工作間不同；不過，您仍可以修改它。

   * **任務所有者**:選擇此選項可使受託人成為所有正在編輯的任務的所有者。
   * **受託人的角色**:從下拉式清單中選取角色。 如果未選取，Adobe Workfront會自動選取使用者的主要角色。

1. 按一下 **儲存變更。**
