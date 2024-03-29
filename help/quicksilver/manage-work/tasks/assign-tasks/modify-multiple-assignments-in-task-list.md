---
product-area: projects;user-management
navigation-topic: assign-tasks
title: 修改任務清單中的多個使用者指派
description: 管理任務指派時，您可以使用任務清單中的大量編輯功能，一次為多個任務同時修改它們。
author: Alina
feature: Work Management, Tasks, Resource Management
role: User
exl-id: 04f7761f-da94-4858-85c5-8dc97bd78bee
source-git-commit: 4041d61ada0be7195b3af3260d419a686e1ada4a
workflow-type: tm+mt
source-wordcount: '1002'
ht-degree: 0%

---

# 修改任務清單中的多個使用者指派

<!--
<p>There is a similar article in Resource Scheduling and a similar one for Issues; when things change, you might need to update all 3</p>
-->

管理任務指派時，您可以使用任務清單中的大量編輯功能，一次為多個任務同時修改它們。

本文旨在為工作清單中的多個工作修改多個使用者指派。 另請參閱下列文章，瞭解如何修改其他區域中多個任務的分配：

* 如需有關使用工作負載平衡器指派任務的資訊，請參閱 [在工作負載平衡器中指派工作的總覽](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md).

如需將任務指派給清單中一個資源的詳細資訊，請參閱 [指派任務](../../../manage-work/tasks/assign-tasks/assign-tasks.md).

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

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
   <td> <p>工作或以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>編輯對專案和任務的存取權</p> <p>檢視或更高的使用者存取權</p> <p>注意：如果您仍然沒有存取權，請詢問您的Workfront管理員是否對您的存取層級設定了其他限制。 如需有關Workfront管理員如何修改您的存取層級的資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>貢獻或更高的任務許可權</p> <p>如需請求其他存取許可權的詳細資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">要求物件的存取權 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的Workfront管理員。

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

## 修改多個任務的指派

1. 前往包含您要修改指派之任務的清單。
1. （可選）建立篩選器，以便只顯示指派給您要修改之受指派人的任務。

   例如，如果您的專案包含特定角色作為多個任務的預設受指派人，您可以建立一個篩選條件，以僅顯示以該角色作為受指派人的任務。 然後，您可以使用特定使用者來取代該角色。

   如需建立篩選的詳細資訊，請參閱 [建立或編輯篩選器](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md).


1. 若要篩選角色，請選取 **指派角色**，然後按一下 **ID**.

   >[!TIP]
   >
   >請勿使用 **指派給** 欄位。 這只會尋找任務的主要擁有者，而不是可指派給他們的任何角色。

   或

   若要篩選使用者，請選取 **指派使用者，** 然後按一下 **ID。**

   >[!TIP]
   >
   >請勿使用 **指派給** 欄位。 這只會尋找任務的主要擁有者，而非可指派給他們的任何使用者。

1. 選取您要修改其指派的任務，然後按一下 **編輯** 圖示 ![](assets/edit-icon.png).

   便會顯示「編輯工作」頁面。 您編輯的專案會顯示在頁面的左上角。

1. 前往 **指定任務** 區段。
1. 執行下列任一項作業，以新增或移除被指定者：

   >[!IMPORTANT]
   >
   >移除被指定者可能會影響任務時數和分配百分比。 如需詳細資訊，請參閱區段 [移除被指定者如何影響任務時數和分配百分比](#how-removing-assignees-affects-task-hours-and-allocation-percentages) 本文章內容。

   * 若要新增受指派人，請執行下列動作：

      1. 在 **指定任務** 區段，選取 **被指定者**.

         所有選定任務中通用的資訊隨即顯示。 例如，如果將同一個使用者指派給所有任務，則該使用者會顯示在 **被指定者** 欄。 如果所選工作間資訊不常見，則不會顯示任何資訊。

      1. 開始輸入使用者、角色或團隊的名稱，然後在其顯示在清單中時選取它。 指派已新增，不會取代所選任務上的目前指派。


     >[!TIP]
     >
     > * 您可以指派多個使用者、工作角色或團隊。 您只能指派作用中的使用者、工作角色和團隊。
     >   
     > * 新增使用者指派時，請注意頭像、使用者的主要角色或其電子郵件地址，以區分具有相同名稱的使用者。 使用者必須至少與一個工作角色相關聯，才能在您新增時檢視該角色。 您必須在存取層級中啟用「檢視連絡人資訊」設定，使用者才能檢視使用者的電子郵件。 如需詳細資訊，請參閱 [授予使用者存取許可權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).
     > 
     >   如果在停用使用者、工作角色或團隊之前已將其指派，則他們仍會被指派給工作專案。 在此情況下，我們建議採取下列步驟：
     >   
     >     * 將工作專案重新指派給使用中資源。
     >     * 將已停用團隊中的使用者與作用中團隊建立關聯，並將工作專案重新指派給作用中團隊。


   * 若要移除個別受指派人，請執行下列動作：

      1. 按一下 **X圖示** 如果受指派人顯示在「工作總攬」清單中，則位於您要移除的受指派人名稱旁。

         或

         （視條件而定）如果您要移除的受指派人並未顯示在「工作總攬」區段中，因為受指派人僅被指派給您選取的某些工作，請按一下 **移除被指定者** 開始輸入您要移除的被指定者名稱，然後在其出現在下拉式清單中時按一下該名稱。

   * 若要移除所有現有的被指定者：

      1. 按一下 **移除所有現有的被指定者**，然後按一下 **是，刪除所有被指定者**.

         這不僅會移除常見的受指派人（顯示在「編輯」對話方塊中的受指派人），也會移除所有選定任務上的所有受指派人。

     從任務中移除使用者可能會影響任務時數和分配百分比。

     如需詳細資訊，請參閱 [修改任務指派的概要](../../../manage-work/tasks/assign-tasks/modify-task-assignments-overview.md).

1. （選擇性）修改受指派人的下列任一選項：

   * （條件式） **分配%或小時**：指定新的配置百分比或時數。

     >[!NOTE]
     >
     >只有在正在編輯的所有任務中，持續時間型別都相同時，才能修改此選項。 當持續時間型別為已計算的工作或投入比導向時，您可以更新配置%。 當期間型別為簡單時，您可以更新小時。 如需持續時間型別的詳細資訊，請參閱 [任務工期與工期型別概要](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).
     >
     >
     如果欄位為空白，表示值在任務間有所不同；不過，您仍可修改它。

   * **任務擁有者**：選取此選項，可讓受分派者成為所有正在編輯之任務的所有者。
   * **受指派人的角色**：從下拉式清單中選取角色。 如果未選取，Adobe Workfront會自動選取使用者的主要角色。

1. 按一下 **儲存變更。**
