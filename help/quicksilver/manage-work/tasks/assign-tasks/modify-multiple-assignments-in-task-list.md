---
product-area: projects;user-management
navigation-topic: assign-tasks
title: 修改任務清單中的多個使用者指派
description: 管理任務指派時，您可以使用任務清單中的大量編輯功能，一次為多個任務同時修改它們。
author: Lisa
feature: Work Management, Tasks, Resource Management
role: User
exl-id: 04f7761f-da94-4858-85c5-8dc97bd78bee
source-git-commit: 21c98e443a6d6ca79045e2f4aba5f792340833cd
workflow-type: tm+mt
source-wordcount: '762'
ht-degree: 3%

---

# 修改任務清單中的多個使用者指派

<!--Audited: 11/2025-->

<!--remove the old/new experience references when the toggles are removed-->

<!--
this article is similar and updates on this one might need to be repeated here: help/quicksilver/manage-work/issues/manage-issues/edit-assignments-for-multiple-issues.md</p>
-->

<!--<div class="preview"> 

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers starting with a week from the Preview release.      

For more information, see [Second Quarter 2026 release overview](/help/quicksilver/product-announcements/product-releases/26-q2-release-activity/26-q2-release-overview.md).  

</div>-->

管理任務指派時，您可以使用任務清單中的大量編輯功能，一次為多個任務同時修改它們。

本文旨在為工作清單中的多個工作修改多個使用者指派。 另請參閱下列文章，瞭解如何修改其他區域中多個任務的指派：

* 如需有關使用工作負載平衡器指派工作的資訊，請參閱在工作負載平衡器[中指派工作的總覽。](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md)

如需將任務指派給清單中一個資源的相關資訊，請參閱[指派任務](../../../manage-work/tasks/assign-tasks/assign-tasks.md)。

## 存取權要求

+++ 展開以檢視這篇文章中所述功能的存取權要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront 封裝</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront授權</td> 
   <td> <p>標準</p>
   <p>工作或更高層級</p>
   </td> 
  </tr> 
  <tr> 
   <td>存取層級設定</td> 
   <td> <p>編輯專案和任務的存取權</p> <p>檢視或更高的使用者存取權</p> </td> 
  </tr> 
  <tr> 
   <td>物件許可權</td>
   <td>貢獻或更高的任務許可權</td>
  </tr>
 </tbody>
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

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
<p>Removing users can affect task hours and allocation percentages. The effect that removing a user has on the task depends on the Duration Type that was selected for the task. For information about Duration Type, see <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Overview of Task Duration and Duration Type</a>.</p>
<p>When you delete a user from a task with the following Duration Types:</p>
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

1. 移至包含您要修改指派之任務的清單。
1. （選擇性）建立篩選器，只顯示指派給您要修改之受指派人的任務。

   例如，如果您的專案包含特定角色作為多個任務的預設受指派人，您可以建立一個篩選器，以僅顯示以該角色作為受指派人的任務。 然後，您可以使用特定使用者來取代角色。

   如需建立篩選的詳細資訊，請參閱[建立或編輯篩選](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md)。


1. 若要篩選角色，請選取&#x200B;**指派角色**，然後按一下&#x200B;**識別碼**。

   >[!TIP]
   >
   >請勿使用&#x200B;**指派至**&#x200B;欄位。 這只會尋找任務的主要所有者，而非可指派給他們的任何角色。

   或

   若要篩選使用者，請選取&#x200B;**指派使用者，**，然後按一下&#x200B;**識別碼。**

   >[!TIP]
   >
   >請勿使用&#x200B;**指派至**&#x200B;欄位。 這只會尋找任務的主要所有者，而非可指派給他們的任何使用者。

1. 選取您要修改指派的任務，然後按一下&#x200B;**編輯**&#x200B;圖示![編輯圖示](assets/edit-icon.png)。

   1. 若要新增或移除受指派人，請執行下列任一項作業：

      * 若要新增受指派人，請在&#x200B;**搜尋人員、角色或團隊**&#x200B;欄位中開始輸入受指派人名稱，然後在他們顯示在清單中時選取他們。

        新的被指定者會新增至所選任務上的現有受指定者。
      * 若要移除被指定者，請在&#x200B;**移除被指定者**&#x200B;方塊中按一下被指定者的名稱

        或

        按一下&#x200B;**移除所有現有的受指派人**。

        受指派人會從所有選取的任務中移除。

        從任務中移除使用者可能會影響任務時數和分配百分比。

        如需詳細資訊，請參閱[修改任務指派的概觀](../../../manage-work/tasks/assign-tasks/modify-task-assignments-overview.md)。


        >[!TIP]
        >
        >* 您可以指派多個使用者、工作角色或團隊。 您只能指派作用中的使用者、工作角色和團隊。
        >   
        >* 新增使用者指派時，請注意頭像、使用者的主要角色或其電子郵件地址，以區分具有相同名稱的使用者。 使用者必須至少與一個工作角色相關聯，才能在您新增時檢視該角色。 您必須在存取層級中啟用檢視聯絡資訊設定，使用者才能檢視使用者的電子郵件。 如需詳細資訊，請參閱[授予使用者存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md)。
        > 
        >   如果使用者、工作角色或團隊在停用之前已被指派，則他們仍被指派給工作專案。 在此情況下，我們建議採取下列步驟：
        >   
        >* 將工作專案重新指派給作用中的資源。
        >* 將已停用團隊中的使用者與作用中團隊建立關聯，並將工作專案重新指派給作用中團隊。


   1. （選擇性）修改受指派人的下列任一選項：

      * （視條件而定） **配置%或時數**：指定新的配置百分比或時數。

      >[!NOTE]
      >
      >只有在正在編輯的所有任務中，持續時間型別都相同的情況下，才能修改此選項。 當持續時間型別已計算工作或投入比導向時，您可以更新配置%。 當持續時間型別簡單時，您可以更新小時。 如需有關期間型別的資訊，請參閱[任務期間與期間型別的概觀](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md)。
      >
      >
      >如果欄位為空白，表示值在各任務間有所不同；不過，您仍可加以修改。

      * **設為主要任務**：將滑鼠指標暫留在選取的任務上，並選取此選項，讓受指派人成為正在編輯之所有任務的所有者。
      * **受指派人的角色**：從下拉式清單中選取一個角色。 如果保持未選取，Adobe Workfront會自動選取使用者的主要角色。
      * **期間類型**
      * **期間**
      * **規劃時數**

   1. 按一下「**儲存**」。

<!-- temporary content - for Assignments redesign:

Editing assignments on tasks differs depending on which environment you choose. 

1. (Conditional) If you are using the Production environment to assign tasks, the **Edit Tasks** box opens in the new experience. Do the following in the Production environment: 

   1. To add or remove assignees, do one of the following:

      * To add assignees, start typing the name of an assignee in the **Search people, roles, or teams** field, then select them when they display in the list. 
      * To remove assignees, click the **x** icon to the right of their name. Only assignees that are common to all tasks display in the list. 
      * Click Assign to me to assign the selected tasks to yourself.

   1. (Conditional) When using the new experience, click **Save**.

   1. (Optional) Click **Switch to old experience** at the bottom of the **Edit Tasks** box.
      
      The **Edit Tasks** box opens in the old experience.

   1. (Conditional) In the old experience, do the following to modify the assignees:

      1. Go to the **Assignments** section.

         >[!IMPORTANT]
         >
         >Removing assignees can affect the task hours and allocation percentages. For more information, see the section [How removing assignees affects task hours and allocation percentages](#how-removing-assignees-affects-task-hours-and-allocation-percentages) in this article.

      1. Do one of the following to add or remove assignees:

         * To add a new assignee:

            1. In the **Assignments** section, select **Assignee**.

               Information that is common across all tasks selected displays. For example, if the same user is assigned to all tasks, that user displays in the **Assignee** column. If information is not common across the tasks selected, no information displays.
            
            1. Start typing the name of a user, role, or team, then select it when it displays in the list. The assignment is added and does not replace the current assignments on the selected tasks.

            >[!TIP]
            >
            > * You can assign multiple users, job roles, or teams. You can assign only active users, job roles, and teams.
            >   
            > * When adding a user assignment, notice the avatar, the user's Primary Role, or their email address to distinguish between users with identical names. Users must be associated with at least one job role to view it as you add them. You must have the View Contact Info setting enabled in your access level for Users to view users' emails. For information, see [Grant access to users](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).
            > 
            >   If a user, job role, or a team was assigned before they were deactivated, they remain assigned to the work item. In this case, we recommend the following:
            >   
            >     * Reassign the work item to active resources.
            >     * Associate the users in a deactivated team with an active team and reassign the work item to the active team.


         * To remove individual assignees:

            1. Click the **X icon** next to the name of the assignee that you want to remove if the assignee displays in the Assignments list.

               Or

               (Conditional) If the assignee that you want to remove does not display in the Assignments section because the assignee is assigned to only some of the tasks that you have selected, click **Remove Assignee** and start typing the name of the assignee that you want to remove, then click the name when it appears in the drop-down list.

         * To remove all existing assignees:

            1. Click **Remove All Existing Assignees**, then click **Yes, Delete All Assignees**.

               This removes not only common assignees (assignees that are displayed in the edit dialog box), but also all assignees on all the selected tasks.

            Removing users from tasks can affect task hours and allocation percentages.
            
            For more information, see [Overview of modifying task assignments](../../../manage-work/tasks/assign-tasks/modify-task-assignments-overview.md).

      1. (Optional) Modify any of the following options for assignees:

         * (Conditional) **Allocation % or Hours**: Specify a new allocation percentage or hours.

         >[!NOTE]
         >
         >This option can be modified only if the Duration Type is the same across all tasks that are being edited. When the Duration Type is Calculated Work or Effort Driven you can update the Allocation %. When the Duration Type is Simple you can update the Hours. For information about Duration Type, see [Overview of Task Duration and Duration Type](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).
         >
         >
         >If the field is blank, this means that the value is different across tasks; however, you are still able to modify it.

         * **Task Owner**: Select this option to make the assignee the owner of the task for all tasks being edited.
         * **Assignee's Role**: Select a role from the drop-down list. If left unselected, Adobe Workfront automatically selects the Primary Role of the user. 

      1. Click **Save Changes.**
        

1. <span class="preview">(Conditional) If you are using the Preview environment to assign tasks, the **Edit Tasks** box opens. Do the following in the Preview environment: </span>

   <div class="preview">-->





