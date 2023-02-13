---
product-area: projects;user-management
navigation-topic: assign-tasks
title: 指派任務
description: 您可以將任務指派給使用者、角色或團隊，以指出負責完成任務的人員。 您可以一次將任務指派給多個資源。
author: Alina
feature: Work Management
exl-id: 611b136e-2c3f-4eac-9d75-e8c12e06148d
source-git-commit: e83d4742106bc3cb5adb939040997959315dd1e2
workflow-type: tm+mt
source-wordcount: '1789'
ht-degree: 1%

---

# 指派任務

您可以指派任務給使用者、工作角色或團隊，以指出負責完成工作的人員。 您可以一次將任務指派給多個資源。

>[!TIP]
>
>您可以指派多個使用者、工作角色或團隊。 您只能指派作用中的使用者、工作角色和團隊。
>
>如果在停用前已指派使用者、工作角色或團隊，則他們仍會指派給工作項目。 在此情況下，我們建議：
>
>* 將工作項重新分配給活動資源。
>* 將已停用團隊中的用戶與活動團隊關聯，並將工作項重新分配給活動團隊。
>


分配給任務的用戶數和任務責任人的計畫可以修改任務的計畫日期，從而更改項目的時間表。 有關為任務分配多個用戶的影響的資訊，請參閱 [修改任務分配概覽](../../../manage-work/tasks/assign-tasks/modify-task-assignments-overview.md).

除了本文之外，建議您閱讀下列文章，以取得指派工作的詳細資訊：

* [修改任務分配概覽](../../../manage-work/tasks/assign-tasks/modify-task-assignments-overview.md)
* [智慧分配概述](../../../manage-work/tasks/assign-tasks/smart-assignments.md)
* [進行智慧分配](../../../manage-work/tasks/assign-tasks/make-smart-assignments.md)
* [建立高級分配](../../../manage-work/tasks/assign-tasks/create-advanced-assignments.md)
* [修改任務清單中的多個用戶分配](../../../manage-work/tasks/assign-tasks/modify-multiple-assignments-in-task-list.md)
* [編輯任務](../../../manage-work/tasks/manage-tasks/edit-tasks.md)
* [規劃專案概觀](../../../manage-work/projects/planning-a-project/plan-project.md)
* [任務計畫完成日期概覽](../../../manage-work/tasks/task-information/task-planned-completion-date.md)
* [設定項目計畫完成日期](../../../manage-work/projects/planning-a-project/project-planned-completion-date.md)
* [配置系統範圍的項目首選項](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)
* [工作負載平衡器中分配工作的概述](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md)

## 存取需求

<!--drafted for P&P - replace table below with this:

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
   <td> <p>Current license: Standard</p> 
   Or
   <p>Legacy license: Work or higher</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects and Tasks</p> <p>View or higher access to Users</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Contribute or higher permissions to tasks</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

-->

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
   <td> <p>編輯專案和工作的存取權</p> <p>檢視或更高的使用者存取權</p> <p><b>附註</b>

如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>協助執行工作或擁有更高權限</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 指派給工作角色、團隊和使用者的多項考量事項

為工作項分配多個資源時，請考慮以下事項：

* 使用者可以有多個與其設定檔相關聯的工作角色。 有關將用戶與作業角色關聯的資訊，請參閱 [編輯使用者的設定檔](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* 如果為任務或問題分配了多個用戶，則您選擇的第一個用戶將自動指定為任務或問題的所有者。
如需變更此項目的說明，請參閱文章中「設為主要」選項的相關資訊 [建立高級分配](create-advanced-assignments.md).

* 團隊不能是任務或問題上的主要受託人。 在任務或問題上，只能將用戶或作業角色指定為主角色。

<!-- If a task is assigned to multiple teams, the primary team sees the Work On It button. waiting on team to verify if this is true. (Courtney)
You cannot make a team be a Primary on a task/ issue. (Alina) -->

* 項目上的任務和問題可能首先分配給一個或多個團隊或作業角色。 當專案準備好開始時，可能也需要將其指派給使用者：

   <table>
  <col> 
  <col> 
  <tbody>
  <tr>
   <td>團隊</td>
   <td>如果將任務分配給某個團隊，並且也分配了某個用戶，則任務仍會分配給該團隊和該用戶，即使該用戶不是該團隊的成員亦然。</td>
  </tr>
  <tr>
   <td>工作角色</td>
   <td><p>如果將任務或問題分配給一個或多個角色，然後也分配了用戶，則根據以下規則決定要與其他用戶關聯的作業角色（如果有）:</p>
     <ul>
      <li>如果只分配了一個作業角色，並且該角色與用戶的主要角色（在其配置檔案中配置）匹配，則任務或問題只分配給該用戶。</li>
      <li>如果已分配多個角色，且其中至少一個角色與用戶的其他角色之一匹配，則會將任務或問題分配給用戶（如果有多個匹配，則隨機選擇該角色），以及分配的任何附加角色</li>
      <li>如果至少分配了一個作業角色，並且沒有與用戶的作業角色匹配的角色，則將該任務或問題分配給該角色或角色以及該用戶。</li>
     </ul>
   <p>如需使用者主要角色和其他角色的相關資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">編輯使用者的設定檔</a>.</p>
   </td>
  </tr>
  </tbody>
  </table>

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Considerations for multiple user assignments and using schedules</h2>
<p>(NOTE: moved to the Modify task assignments overview standalone article)</p>
<p>You can assign multiple resources to a task. When you assign a user to a task, Workfront uses the user's schedule to calculate the planned dates for the task which ultimately determine the timeline of the project. Using the schedule of the user takes into account their time off, holidays, and weekend days which are considered non-working days when task activity cannot occur. </p>
<p>When you assign multiple users to a task, your Workfront administrator <span>or a group administrator</span> determines which one of the following schedules Workfront uses to determine the planned dates of the tasks, based on schedules: </p>
<ul>
<li> <p><strong>The Primary Assignee's schedule</strong>: this is the schedule associated with the user designated as the task Owner.</p> <p>For information about associating users with schedules, see <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Edit a user's profile</a>.</p> </li>
<li><strong>The Project's schedule</strong>: this is the schedule associated with the project. For adding a schedule to a project, see <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">Edit projects</a>.</li>
</ul>
<p>For information about setting up which schedule a project uses in the case of multiple assignments, see <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configure system-wide project preferences</a>. </p>
</div>
-->

## 指派單一任務

1. 轉到要分配的任務。
1. 按一下 **指派給** 在 **分配** 欄位。

   或

   如果已分配任務或問題，請按一下分配的名稱。

![](../assign-tasks/assets/advanced-assignments-link-from-task-header-nwe-350x267.png)

1. 執行下列任一項作業：

   * 開始鍵入要指派的用戶、角色或團隊的名稱，然後在清單上出現時按一下。


      >[!TIP]
      >
      >新增使用者指派時，請注意頭像、使用者的主要角色或其電子郵件地址，以區分名稱相同的使用者。 用戶必須至少與一個作業角色關聯，才能在添加時查看該角色。


   * （條件性）按一下 **建議的分配** 清單（如果顯示此清單）。 如需詳細資訊，請參閱 [智慧分配概述](../../../manage-work/tasks/assign-tasks/smart-assignments.md).

   * 按一下 **進階**

      有關如何進行高級分配的資訊，請參閱 [建立高級分配](../../../manage-work/tasks/assign-tasks/create-advanced-assignments.md).

1. 按一下&#x200B;**儲存**。
1. （選用和條件式）按一下 **X圖示** 按一下「 」後，在任務的右側面板中刪除分配的分配名稱旁邊 **進階**.

## 在清單中分配任務

在清單視圖中顯示任何分配欄位時，您可以在清單或報告中分配任務。 這是指派任務的更快方法。 本文介紹如何修改清單中某個任務的分配。 有關修改清單中多個任務的多個分配的資訊，請參閱 [修改任務清單中的多個用戶分配](../../../manage-work/tasks/assign-tasks/modify-multiple-assignments-in-task-list.md).

根據視圖中顯示的欄位，您可以為任務分配以下實體：

| 欄位 | 已分配的實體 |
|---|---|
| **指派給** | 指派一個使用者 |
| **已指派** | 指派一個使用者 |
| **指派** | 指派使用者、工作角色或團隊 |

要分配清單中的任務：

1. 轉至視圖中具有「已分配至」(Assigned To)、「已分配」(Assigned)或「分配」(Assignments)欄位的任務清單。
1. （選用）按一下 **自動儲存** 下拉式選單中選取下列選項：

   | 選項 | 選項說明 |
   |---|---| 
   | 自動儲存 | 您對任務所做的更改將自動保存，並且無法還原 |
   | 手動儲存 | 您必須手動儲存變更。 您可以在儲存變更之前先還原變更。 |
   | 時間表計畫 | 您必須手動儲存變更。 您可以在儲存變更之前先還原變更。 儲存變更和所有專案相依性的速度，都比選取「手動儲存」時快。 |

   有關在清單中編輯任務時保存任務的詳細資訊，請參閱 [編輯清單中的任務](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md).

1. 要分配任務，請執行以下操作之一：

   * 按一下內部 **指派給** 或 **已指派** 欄位，然後開始鍵入要分配給任務的活動用戶的名稱，然後在清單中顯示時按一下它。
   * 按一下內部 **分配** 欄位，然後開始鍵入要分配給任務的活動用戶、作業角色或團隊的名稱，然後在清單中顯示時按一下它。

      >[!TIP]
      >新增使用者指派時，請注意頭像、使用者的主要角色或其電子郵件地址，以區分名稱相同的使用者。 用戶必須至少與一個作業角色關聯，才能在添加時查看該角色。
      >
      >
   >

1. （條件性）當顯示於 **分配** 欄位，按一下 **人員** 表徵圖，以開啟 **高級分配** 框和建立高級分配。

   <!--
   there is a People icon in NWE but it's hard to see - you need to assign the task to at least 2 users, not roles, or teams, before it shows up</p>
   -->

   如需詳細資訊，請參閱 [建立高級分配](../../../manage-work/tasks/assign-tasks/create-advanced-assignments.md).

   >[!TIP]
   不能從「已分配至」或「已分配」欄位進行高級分配。

1. 將任務添加到任務後，按Enter鍵或按一下頁面上的任意位置以保存更改（如果您選擇了自動保存）。 否則，按一下 **儲存**.

## 為用戶分配多個任務

1. 轉至要批量分配的任務清單。
1. （條件性）確保 **自動儲存** 選項。

   >[!IMPORTANT]
   在專案上手動儲存任務時，無法大量編輯任務。

1. 在任務清單中選擇多個任務。
1. 按一下 **編輯**.

   此 **編輯任務** 對話框。

1. 在 **分配** ，選擇 **受託人** 框中，然後開始鍵入要分配給所有任務的用戶、作業角色或團隊的名稱。

   >[!IMPORTANT]
   如果已分配任何任務，則在此處指定的資源將添加到任務中，而不是替換任務上的現有資源。

1. （選用）選取 **任務所有者** 欄，指明在為任務分配多個資源時，哪個資源是主要受託人或任務的所有者。 這不適用於團隊。
1. （條件性）指定 **分配%** 如果您選擇的所有任務的「持續時間類型」為「工作驅動」或「計算分配」，則對於分配給任務的每個資源。 這表示這些資源應花費多少時間來完成任務。 這僅適用於使用者和工作角色。

   或

   指定 **小時** 如果您選擇的所有任務的「持續時間類型」為「簡單」，則對於分配給任務的每個資源。 所有資源的所有小時總數應等於任務的計畫小時數。

   >[!IMPORTANT]
   如果您選擇的任務具有不同的持續時間類型，或您選擇的任務具有不同的持續時間類型，則無法指定每個資源的分配百分比或小時數。

   有關任務的「持續時間類型」的資訊，請參閱 [任務持續時間和持續時間類型概覽](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

1. （可選）從 **選擇角色** 中的下拉式功能表 **受託人的角色** 欄。 如果您未選取角色，Workfront會自動選取使用者的主要角色。

1. （可選）如果要從所有任務中刪除現有的受分配者，請執行以下操作之一：

   1. 開始鍵入要從任務中刪除的用戶、角色或團隊的名稱，然後在清單上顯示時選擇它，然後按一下 **刪除受託人** 刪除更多受分配者。
   1. 按一下 **刪除所有現有受分配者** 從所有選定任務中刪除所有受分配者。

1. 按一下 **儲存變更**.
1. （可選和條件性）當任務清單中顯示「已分配給」或「工作總攬」欄位時，按一下其中一列內的任務，然後按一下 **X圖示** 在受託人名稱旁邊，將其從任務中刪除。

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Considerations about unassigning tasks</h2>
<p>(NOTE: moved this to the new article: /Content/Manage work/Tasks/Assign tasks/modify-task-assignments-overview.htm)</p>
<p>You can remove assignments from one task at a time, or you can remove assignments from multiple tasks in bulk.</p>
<p>For more information about removing assignments from tasks in bulk, see <a href="../../../manage-work/tasks/assign-tasks/modify-multiple-assignments-in-task-list.md" class="MCXref xref">Modify multiple user assignments in a task list</a>. </p>
<p>Consider the following when removing assignments from tasks: </p>
<ul>
<li>When you unassign a user from a task, the task remains assigned to the job role that the user fulfilled on the task.</li>
<li>When you unassign a job role or a team from a task, the task remains unassigned if it is not assigned to any other resources. </li>
</ul>
</div>
-->


