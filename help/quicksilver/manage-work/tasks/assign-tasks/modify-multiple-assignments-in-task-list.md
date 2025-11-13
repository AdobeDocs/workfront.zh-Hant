---
product-area: projects;user-management
navigation-topic: assign-tasks
title: 修改任務清單中的多個使用者指派
description: 管理任務指派時，您可以使用任務清單中的大量編輯功能，一次為多個任務同時修改它們。
author: Lisa
feature: Work Management, Tasks, Resource Management
role: User
exl-id: 04f7761f-da94-4858-85c5-8dc97bd78bee
source-git-commit: 1f9a0e6064f83c6f0947e3c7ef596e96c934a687
workflow-type: tm+mt
source-wordcount: '1047'
ht-degree: 0%

---

# 修改任務清單中的多個使用者指派

<!--Audited: 11/2025-->

<!--remove the old/new experience references when the toggles are removed-->

<!--
this article is similar and updates on this one might need to be repeated here: help/quicksilver/manage-work/issues/manage-issues/edit-assignments-for-multiple-issues.md</p>
-->

<!--<div class="preview"> 

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers starting with a week from the Preview release.      

For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).  

</div>-->

管理任務指派時，您可以使用任務清單中的大量編輯功能，一次為多個任務同時修改它們。

本文旨在為工作清單中的多個工作修改多個使用者指派。 另請參閱下列文章，瞭解如何修改其他區域中多個任務的指派：

* 如需有關使用工作負載平衡器指派工作的資訊，請參閱在工作負載平衡器[中指派工作的總覽。](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md)

如需將任務指派給清單中一個資源的相關資訊，請參閱[指派任務](../../../manage-work/tasks/assign-tasks/assign-tasks.md)。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront套件</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront授權</td> 
   <td> <p>標準</p>
   <p>工作或更高</p>
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

1. 選取您要修改指派的任務，然後按一下&#x200B;**編輯**&#x200B;圖示![](assets/edit-icon.png)。

   **編輯任務**&#x200B;方塊會在新體驗中開啟。 執行下列其中一項：

   * 若要新增受指派人，請在&#x200B;**搜尋人員、角色或團隊**&#x200B;欄位中開始輸入受指派人名稱，然後在他們顯示在清單中時選取他們。
   * 若要移除受指派人，請按一下其名稱右側的&#x200B;**x**&#x200B;圖示。 只有所有工作通用的受指派者才會顯示在清單中。
   * 按一下「指派給我」 ，將選取的任務指派給您自己。

1. （視條件而定）使用新體驗時，請按一下&#x200B;**儲存**。

1. （選擇性）按一下&#x200B;**編輯工作**&#x200B;方塊底部的&#x200B;**切換到舊體驗**。

   **編輯任務**&#x200B;方塊會在舊體驗中開啟。

   <!--
   >[!TIP]
   >
   >The old experience is available by default in the Production environment.-->

1. （視條件而定）在舊體驗中，執行下列操作以修改受指派人：

   1. 移至&#x200B;**指派**&#x200B;區段。

      >[!IMPORTANT]
      >
      >移除被指定者可能會影響任務時數和分配百分比。 如需詳細資訊，請參閱本文章的[移除受指派人如何影響任務時數及配置百分比](#how-removing-assignees-affects-task-hours-and-allocation-percentages)一節。

   1. 執行下列任一項作業，以新增或移除受指派人：

      * 若要新增受指派人：

         1. 在&#x200B;**工作分派**&#x200B;區段中，選取&#x200B;**受指派人**。

            所有選定任務中通用的資訊隨即顯示。 例如，如果將同一個使用者指派給所有任務，則該使用者會顯示在&#x200B;**受指派人**&#x200B;欄中。 如果選取的任務間資訊不常見，則不會顯示任何資訊。

         1. 開始輸入使用者、角色或團隊的名稱，然後在其顯示在清單中時選取它。 指派會新增，而不會取代所選任務上的目前指派。


        >[!TIP]
        >
        > * 您可以指派多個使用者、工作角色或團隊。 您只能指派作用中的使用者、工作角色和團隊。
        >   
        > * 新增使用者指派時，請注意頭像、使用者的主要角色或其電子郵件地址，以區分具有相同名稱的使用者。 使用者必須至少與一個工作角色相關聯，才能在您新增時檢視該角色。 您必須在存取層級中啟用檢視聯絡資訊設定，使用者才能檢視使用者的電子郵件。 如需詳細資訊，請參閱[授予使用者存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md)。
        > 
        >   如果使用者、工作角色或團隊在停用之前已被指派，則他們仍被指派給工作專案。 在此情況下，我們建議採取下列步驟：
        >   
        >     * 將工作專案重新指派給作用中的資源。
        >     * 將已停用團隊中的使用者與作用中團隊建立關聯，並將工作專案重新指派給作用中團隊。


      * 若要移除個別受指派人，請執行下列動作：

         1. 如果受指派人顯示在「工作總攬」清單中，則按一下您要移除之受指派人名稱旁的&#x200B;**X圖示**。

            或

            （視條件而定）如果您要移除的受指派人未顯示在「工作分派」區段中，因為受指派人僅被指派給您選取的部分工作，請按一下&#x200B;**移除受指派人**，並開始輸入您要移除的受指派人名稱，然後在其出現在下拉式清單中時按一下該名稱。

      * 若要移除所有現有的被指定者：

         1. 按一下&#x200B;**移除所有現有的受指派人**，然後按一下&#x200B;**是，刪除所有受指派人**。

            這不僅會移除常見的被指定者（顯示在「編輯」對話方塊中的被指定者），也會移除所有選定任務中的所有被指定者。

        從任務中移除使用者可能會影響任務時數和分配百分比。

        如需詳細資訊，請參閱[修改任務指派的概觀](../../../manage-work/tasks/assign-tasks/modify-task-assignments-overview.md)。

   1. （選擇性）修改受指派人的下列任一選項：

      * （視條件而定） **配置%或時數**：指定新的配置百分比或時數。

      >[!NOTE]
      >
      >只有在正在編輯的所有任務中，持續時間型別都相同的情況下，才能修改此選項。 當持續時間型別已計算工作或投入比導向時，您可以更新配置%。 當持續時間型別簡單時，您可以更新小時。 如需有關期間型別的資訊，請參閱[任務期間與期間型別的概觀](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md)。
      >
      >
      >如果欄位為空白，表示值在各任務間有所不同；不過，您仍可加以修改。

      * **任務擁有者**：選取此選項，可讓受指派者成為正在編輯之所有任務的所有者。
      * **受指派人的角色**：從下拉式清單中選取一個角色。 如果保持未選取，Adobe Workfront會自動選取使用者的主要角色。

   1. 按一下&#x200B;**儲存變更。**

