---
product-area: projects;user-management
navigation-topic: assign-tasks
title: 指派任務
description: 您可以將任務指派給使用者、角色或專案團隊，以指出負責完成任務的人員。 您可以一次將任務指派給多個資源。
author: Alina
feature: Work Management, Tasks
role: User
exl-id: 611b136e-2c3f-4eac-9d75-e8c12e06148d
source-git-commit: 50e52f27f1f3f6f5b601b50303aba409559d8ca8
workflow-type: tm+mt
source-wordcount: '2070'
ht-degree: 1%

---

# 指派任務

<!--remove the span class preview from everywhere but the Rate Card roles referencs must stay in yellow; replace the intro with preview and fast track only but not sure if with the link to third quarter release?!-->

<span class="preview">本頁醒目提示的資訊指出尚未普遍可用的功能。 它僅適用於所有客戶的預覽環境，或適用於啟用快速發行的客戶的生產環境。</span>

<span class="preview">如需快速發行版本的相關資訊，請參閱 [啟用或停用組織的快速發行](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview">如需目前版本的相關資訊，請參閱 [2024年第三季度版本總覽](/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-release-overview.md).</span>

您可以將任務指派給使用者、工作角色或專案團隊，以指出負責完成任務的人員。 您可以一次將任務指派給多個資源。

>[!TIP]
>
>您可以指派多個使用者、工作角色或團隊。 您只能指派作用中的使用者、工作角色和團隊。
>
>如果使用者、工作角色或團隊在停用之前已被指派，則他們仍被指派給工作專案。 在此情況下，我們建議採取下列步驟：
>
>* 將工作專案重新指派給作用中的資源。
>* 將已停用團隊中的使用者與作用中團隊建立關聯，並將工作專案重新指派給作用中團隊。
>

指派給任務的使用者數量和任務擁有者的排程可以修改任務的計畫日期，這會導致變更專案的時間表。 如需將多個使用者指派至一個任務的影響資訊，請參閱 [修改任務指派的概要](../../../manage-work/tasks/assign-tasks/modify-task-assignments-overview.md).

除了本文章之外，我們建議您閱讀下列文章，以取得指派工作的詳細資訊：

* [修改任務指派的概要](../../../manage-work/tasks/assign-tasks/modify-task-assignments-overview.md)
* [智慧指派總覽](../../../manage-work/tasks/assign-tasks/smart-assignments.md)
* [進行智慧型指派](../../../manage-work/tasks/assign-tasks/make-smart-assignments.md)
* [建立進階任務指派](../../../manage-work/tasks/assign-tasks/create-advanced-assignments.md)
* [修改任務清單中的多個使用者指派](../../../manage-work/tasks/assign-tasks/modify-multiple-assignments-in-task-list.md)
* [編輯任務](../../../manage-work/tasks/manage-tasks/edit-tasks.md)
* [計畫專案概述](../../../manage-work/projects/planning-a-project/plan-project.md)
* [任務計畫完成日期總覽](../../../manage-work/tasks/task-information/task-planned-completion-date.md)
* [設定專案計畫完成日期](../../../manage-work/projects/planning-a-project/project-planned-completion-date.md)
* [設定全系統專案偏好設定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)
* [在工作負載平衡器中指派工作的總覽](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md)

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

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
   <td> <p>工作或更高</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>編輯專案和任務的存取權</p> <p>檢視或更高的使用者存取權</p> <p><b>附註</b>

如果您還是沒有存取權，請詢問您的Workfront管理員，他們是否在您的存取層級中設定其他限制。 如需有關Workfront管理員如何修改您的存取層級的資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>貢獻或更高的任務許可權</p> <p>如需請求其他存取許可權的詳細資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">要求物件的存取權 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的Workfront管理員。

+++

## 對工作角色、團隊和使用者的多個指派的考量事項

將多個資源指派給工作專案時，請考量下列事項：

* 使用者可以有多個與其設定檔相關聯的工作角色。 如需將使用者與工作角色建立關聯的資訊，請參閱 [編輯使用者設定檔](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* 如果您將多個使用者指派給一個任務或問題，則您選擇的第一位使用者會自動被指定為任務或問題的擁有者。
如需有關變更此專案的指示，請參閱文章中建立主要選項的資訊 [建立進階任務指派](create-advanced-assignments.md).

* 團隊不能是任務或問題的主要受指派人。 只有使用者或工作角色可以指定為任務或問題上的主要角色。

<!-- If a task is assigned to multiple teams, the primary team sees the Work On It button. waiting on team to verify if this is true. (Courtney)
You cannot make a team be a Primary on a task/ issue. (Alina) -->

* 專案上的任務和問題可能首先指派給一個或多個團隊或工作角色。 當專案準備開始時，他們可能需要也被指派給使用者：

  <table>
  <col> 
  <col> 
  <tbody>
  <tr>
   <td>團隊</td>
   <td>如果您將任務指派給專案團隊且也指派了使用者，則即使使用者不是專案團隊的成員，任務仍會指派給專案團隊和使用者。</td>
  </tr>
  <tr>
   <td>職務角色</td>
   <td><p>如果您將任務或問題指派給一或多個角色，然後又指派使用者，則系統會根據下列規則決定要與其他使用者（如果有）產生關聯的工作角色：</p>
     <ul>
      <li>如果僅指派了一個工作角色，並且該工作角色符合使用者的主要角色（在其設定檔中設定），則任務或問題僅指派給該使用者。</li>
      <li>如果指派了多個角色，並且其中至少一個角色與使用者的其他角色之一匹配，則會將任務或問題指派給使用者（如果有多個匹配，則隨機選擇角色），以及指派的任何其他角色</li>
      <li>如果至少指派了一個工作角色，但沒有匹配使用者的工作角色，則會將任務或問題指派給該角色或使用者。</li>
     </ul>
   <p>如需有關使用者的主要角色和其他角色的資訊，請參閱 <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md">編輯使用者設定檔</a>.</p>
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

1. 移至您要指派的工作。
1. 按一下 **指派給** 在 **指定任務** 任務標題中的欄位

   或

   如果任務或問題已指派，則按一下指派的名稱。

   在生產環境中：
   ![](../assign-tasks/assets/advanced-assignments-link-from-task-header-nwe-350x267.png)

   <span class="preview">在預覽環境中：</span>
   ![指派](assets/assignments-box-in-task-header.png)

1. 執行下列其中一項：

   * 開始輸入您要指派的使用者、角色或團隊名稱，然後當名稱出現在清單中時按一下它。


     >[!TIP]
     >
     >新增使用者指派時，請注意頭像、使用者的主要角色或其電子郵件地址，以區分具有相同名稱的使用者。 使用者必須至少與一個工作角色相關聯，才能在您新增時檢視該角色。
     >
     >您必須在存取層級中啟用檢視聯絡資訊設定，使用者才能檢視使用者的電子郵件。 如需詳細資訊，請參閱 [授予使用者存取許可權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).
     >
     ><span class="preview">新增工作角色指派時，您可以搜尋工作角色或地點。 從「工作角色」清單中選取角色，以使用指定之預設收費率，或從費率卡選取要使用收費率的「費率卡」工作角色。 如需費率卡的詳細資訊，請參閱 [管理費率卡](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/manage-rate-cards.md).</span>


   * （視條件而定）按一下 <span class="preview">**建議的指派**， **使用者和團隊**，或 **職位角色**，或 **評等卡片角色**</span> 清單的顯示時間。 如需詳細資訊，請參閱 [智慧指派總覽](../../../manage-work/tasks/assign-tasks/smart-assignments.md).

     您可以開始鍵入要指派給任務的任何使用者、團隊或工作角色的名稱，然後當它顯示在清單中時選取它。

   * 按一下 **進階**

     有關如何進行進階指派的資訊，請參閱 [建立進階任務指派](../../../manage-work/tasks/assign-tasks/create-advanced-assignments.md).

1. 按一下「**儲存**」。
1. （選擇性和條件性）按一下 **X圖示** 在任務右側面板中的工作分派名稱旁，移除工作分派（如果按一下） **進階**.

## 指派清單中的任務

當清單的檢視中顯示任何指派欄位時，您可以在清單或報告中指派任務。 這是指派任務的更快方式。 本文說明如何修改清單中一個任務的指派。 如需有關修改清單中多個任務的多個指派的資訊，請參閱 [修改任務清單中的多個使用者指派](../../../manage-work/tasks/assign-tasks/modify-multiple-assignments-in-task-list.md).

根據檢視中顯示的欄位，您可以將下列實體指派給任務：

| 欄位 | 已指派的實體 |
|---|---|
| **指派給** | 指派一位使用者 |
| **已指派** | 指派一位使用者 |
| **指派** | 指派使用者、工作角色或團隊 |

若要指派清單中的工作：

1. 移至檢視中具有指派至、指派或工作分派欄位的任務清單。
1. （可選）按一下 **自動儲存** 下拉式功能表，並從下列選項中選取：

   | 選項 | 選項說明 |
   |---|---| 
   | 自動儲存 | 您對任務進行的變更會自動儲存，且您無法還原 |
   | 手動儲存 | 您必須手動儲存變更。 您可以在儲存變更之前先還原變更。 |
   | 時間表計畫 | 您必須手動儲存變更。 您可以在儲存變更之前先還原變更。 儲存您的變更和所有專案相依性比選取「手動儲存」更快。 |

   如需當您在清單中編輯時儲存任務的詳細資訊，請參閱 [編輯清單中的任務](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md).

1. 若要指派工作，請執行下列任一項作業：

   * 按一下 **指派給** 或 **已指派** 欄位並開始輸入您要指派給任務的作用中使用者名稱，然後當它顯示在清單中時按一下它。
   * 按一下 **指定任務** 欄位並開始輸入您要指派給任務的作用中使用者、工作角色或團隊的名稱，然後當它顯示在清單中時按一下它。

     >[!TIP]
     >
     >新增使用者指派時，請注意頭像、使用者的主要角色或其電子郵件地址，以區分具有相同名稱的使用者。 使用者必須至少與一個工作角色相關聯，才能在您新增時檢視該角色。
     >
     >您必須在存取層級中啟用檢視聯絡資訊設定，使用者才能檢視使用者的電子郵件。 如需詳細資訊，請參閱 [授予使用者存取許可權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md)
     >
     ><span class="preview">新增工作角色指派時，您可以搜尋工作角色或地點。 選取「系統/預設工作角色」以使用指定之預設收費率，或選取「費率卡工作角色」以使用費率卡的收費率。 如需費率卡的詳細資訊，請參閱 [管理費率卡](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/manage-rate-cards.md).</span>


1. （視條件而定）當顯示在 **指定任務** 欄位，按一下 **人員** 圖示開啟「工作總攬」方塊的右上角 **進階任務指派** 方塊並建立進階工作分派。

   <!--
   there is a People icon in NWE but it's hard to see - you need to assign the task to at least 2 users, not roles, or teams, before it shows up</p>
   -->

   如需詳細資訊，請參閱 [建立進階任務指派](../../../manage-work/tasks/assign-tasks/create-advanced-assignments.md).

   >[!TIP]
   >
   >您無法從「指派至」或「已指派」欄位進行進階指派。

1. 將您的受指派人新增至工作之後，按下Enter或按一下頁面上的任何位置，以儲存變更（如果您已選取「自動儲存」）。 否則，按一下 **儲存**.

## 指派多個任務給使用者

1. 移至您要大量指派的工作清單。
1. （視條件而定）確定 **自動儲存** 如果您位於專案下的任務清單中，則會選取選項。

   >[!IMPORTANT]
   >
   >在專案上手動儲存任務時，您無法大量編輯任務。

1. 在任務清單中選取數個任務。
1. 按一下 **編輯**.

   此 **編輯任務** 對話方塊開啟。

1. 在 **指定任務** 區域，選取 **被指定者** 方塊，然後開始輸入您要指派給所有任務的使用者、工作角色或團隊名稱。

   >[!IMPORTANT]
   >
   >如果有任何任務已指派，您在此處指定的資源會新增到任務中，而不是取代任務上的現有資源。

1. （選擇性）選取 **任務擁有者** 欄，指明當您指派一個以上的資源給任務時，哪個資源是任務的主要受指派人或擁有者。 這不適用於團隊。
1. （視條件而定）指定 **配置%** 對於指派給任務的每個資源，如果您選取的所有任務的「工期型態」均為「投入比導向」或「計算的工作分派」。 這表示這些資源應該花費多少時間完成任務。 這僅適用於使用者和職位角色。

   或

   指定數量 **小時** 對於指派給任務的每個資源，如果您選取的所有任務的「工期型別」均為「簡單」。 所有資源的所有時數總計應等於任務的計畫時數。

   >[!IMPORTANT]
   >
   >如果您選取的任務具有不同的期間型別或您選取的任務具有不同的期間型別，則無法指定每個資源的配置百分比或時數。

   如需有關工作的期間型別的資訊，請參閱 [任務期間與期間型別概觀](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

1. （選擇性）從中選擇使用者應在任務上履行的角色 **選擇角色** 中的下拉式功能表 **受指派人的角色** 欄。 如果您未選取角色，Workfront會自動選取使用者的主要角色。

1. （選擇性）如果要從所有工作移除現有的受指派人，請執行下列任一項作業：

   1. 開始輸入要從任務中移除的使用者、角色或團隊名稱，然後當它出現在清單中時選取它，然後按一下 **移除被指定者** 以移除更多受指派人。
   1. 按一下 **移除所有現有的被指定者** 以從所有選取的工作中移除所有受指派人。

1. 按一下「**儲存變更**」。
1. （選擇性和條件性）當指派至或工作分派欄位顯示在您的任務清單中時，按一下這些欄位之一的任務，然後按一下 **X圖示** 位於受指派人名稱旁，以將其從任務中移除。

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


