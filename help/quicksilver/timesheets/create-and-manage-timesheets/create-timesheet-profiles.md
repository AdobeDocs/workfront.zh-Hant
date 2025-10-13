---
product-area: timesheets;system-administration
navigation-topic: create-and-manage-timesheets
title: 建立、編輯和指派時程表設定檔
description: 您可以建立、編輯和指派為使用者產生週期性時程表的時程表設定檔，您無需採取任何進一步的干預。 這可為您節省時間，並確保使用者之間的一致性。
author: Lisa
feature: Timesheets
exl-id: 8f4826bd-82b4-4157-a7d4-a7c94b8fc879
source-git-commit: 395a7788ddfda71264b7b964953435affd7761e9
workflow-type: tm+mt
source-wordcount: '1597'
ht-degree: 2%

---

# 建立、編輯和指派時程表設定檔

<!--Audited: 06/2025-->

您可以建立、編輯和指派為使用者產生週期性時程表的時程表設定檔，您無需採取任何進一步的干預。 這可為您節省時間，並確保使用者之間遵循下列原則：

* 時程表時間範圍
* 核准者
* 一般小時型別

如需手動建立時程表的詳細資訊，請參閱[建立單一使用時程表](../../timesheets/create-and-manage-timesheets/create-tmshts.md)。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫</td> 
   <td> <p>任何</p> </td> 
  </tr> 
   <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>新增：標準 </p>
 <p>或</p> 
<p>目前：計畫 </p> 
</td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>您必須擁有時程表的管理存取權。 </p> </td> 
  </tr> 
 </tbody> 
</table>

*如需此表格中資訊的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 建立或編輯週期性時程表

<!--Old info: 
<div style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p style="color: #ff1493;">Alina drafted an Important note under this heading because Tracy/WorkEx said this is not working as designed - the changes WILL take effect the minute to make them for existing timesheets - see this issue - https://hub.workfront.com/issue/5dba59f600c401cca536567c368aa299/overview</p>
<p style="color: #ff1493;">Important: The changes you make to an existing timesheet profile are not automatically applied to timesheets that have already been generated. The changes you make to a timesheet prile are applied only to the timesheets that are&nbsp;generated after the timesheet profiles changes are made. To&nbsp;apply your&nbsp;changes to the timesheet profile for the timesheets that are already generated, you must delete the existing timesheets and manually generate&nbsp;them.For more information about deleting and manually generating timesheets, see&nbsp;Delete and manually generating Timesheets.</p>
</div>
-->

>[!IMPORTANT]
>
>若要在目前時程表中啟用時程表設定檔變更，您必須先刪除現有時程表，才能變更時程表設定檔，然後產生新的時程表。 如需指示，請參閱[刪除Adobe Workfront中的時程表](../../timesheets/create-and-manage-timesheets/delete-timesheets.md)和[手動產生時程表](../../timesheets/create-and-manage-timesheets/manually-generate-timesheets.md)。

{{step-1-to-setup}}

1. 如果您建立或編輯時程表設定檔，以便在整個系統中使用，請按一下&#x200B;**時程表和時數**。

   或

   如果您建立或編輯群組的時程表設定檔，請按一下&#x200B;**群組**，然後按一下群組的名稱。

1. 按一下&#x200B;**週期性時程表**。
1. 若要建立時間表設定檔，請按一下&#x200B;**新增設定檔**。

   或

   若要編輯現有的時程表設定檔，請選取要編輯的時程表設定檔，然後按一下&#x200B;**編輯**。

   新的或現有的時程表設定檔頁面隨即顯示。

1. 更新下列資訊：

   * **名稱**：為時程表設定檔新增名稱。 這可以是團隊名稱，或人員與其時程表共用相同時間範圍的群組名稱。 這是必填欄位。
   * **描述**：新增更多關於時程表設定檔的資訊。
   * **具有管理存取權的群組**：如果您正在建立系統層級時程表設定檔，請將此欄位留空。

     任何可以編輯使用者帳戶的使用者都可以將系統層級時程表附加到其他使用者。

     只有Workfront管理員可以編輯系統層級時間表設定檔。

     如果您要為管理的群組建立時間表設定檔，請在此處識別該群組。

     這不會將時程表設定檔指派給群組中的使用者；只允許群組的管理員修改時程表設定檔。 您將在步驟6中將設定檔指派給使用者。

     >[!NOTE]
     >
     >當群組外的使用者將時程表設定檔附加到其他使用者時，他們將無法檢視或附加此時程表設定檔。

   * **建立時程表**：指定時程表設定檔應何時產生時程表。 時程表可設定為每週、每兩週、每半月或每月自動產生。 選取一週中要產生時程表的日期。

     每週時程表從產生日期開始。 例如，如果您每星期四建立每週時程表，則時程表上一週的第一天是星期四。

     >[!NOTE]
     >
     >Workfront一律會同時建立兩個時程表：第一個時程表一律包含目前的日期，第二個時程表從第一時程表的時間範圍結束時開始。

   * **核准者**：核准者是核准與時程表相關聯之使用者之時程表的使用者。 您最多可以在時程表上將7名使用者識別為核准者。 識別多個使用者對於確保在某人不在辦公室時核准者可供使用非常有用。 當使用者提交時程表以供核準時，所有核准者都會收到通知。 時程表只需一名使用者核准即可核准。

     只有具有時程表管理許可權的使用者才能設定為核准者。 如需時程表管理許可權的詳細資訊，請參閱[授予使用者對特定區域的管理存取權](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md)。

     使用下拉式選單來選取時程表的核准者（如果需要核准者）。 您可選取下列選項：

      * **無**：時程表不需要核准。
      * **他們的管理員**：這是系統設定的預設核准者。 在這種情況下，當時程表提交進行核準時，被指定為其管理員的使用者會核准該時程表。
      * **特定人員**：您可以依名稱將特定使用者指定為時程表核准者。 您可以在時程表上擁有多個核准者。 在這種情況下，在核准者核準時程表後，該時程表會被標籤為&#x200B;**已關閉**，並且會從所有剩餘核准者的時程表核准清單中消失。

   * **可以編輯時間**：選取此選項可允許核准者編輯時程表上的時數。

     此選項可與「設定>時程表和時數>偏好設定」區域中的&#x200B;**限制所有者和管理員編輯時程表**&#x200B;設定搭配使用。 如需詳細資訊，請參閱[設定時程表和小時喜好設定](/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md)。

     存在下列情況：

     啟用&#x200B;**限制所有者和管理員編輯時程表**&#x200B;選項時：

      * 核准者只能核准和拒絕時程表，無論是否啟用可編輯時間。
      * 時程表所有者的管理員只能檢視其直接報告的時程表。

     當&#x200B;**限制所有者和管理員編輯時程表**&#x200B;選項停用時：

      * 當&#x200B;**可以編輯時間**&#x200B;啟用時，核准者可以提交、重新開啟或關閉時程表，並且可以編輯時間。
      * 當&#x200B;**可以編輯時間**&#x200B;停用時，核准者無法提交、重新開啟或關閉時程表，也無法編輯時間。 核准者只能核准或拒絕時程表。
      * 時程表所有者的管理員可以提交、撤銷、重新開啟及編輯其直接下屬的時程表。

     >[!NOTE]
     >
     >一旦您提交時程表進行核准，您就無法再編輯小時。 若要將已提交的時程表傳回至可編輯狀態，請撤回該時程表或讓核准者拒絕該時程表。 如需詳細資訊，請參閱[提交時程表以供核准](/help/quicksilver/timesheets/create-and-manage-timesheets/submit-timesheet-for-approval.md)和[核準時程表](/help/quicksilver/timesheets/create-and-manage-timesheets/timesheet-approvals.md)。

   * **加班**：您可以選擇隱藏時程表中的[加班]方塊。 此選項預設為停用。
   * **可用時數型別**：此設定僅參考一般時數型別，不會參考專案特定的時數型別。

     依預設，使用者會在時程表上檢視所有一般時數。 不過，如果您的組織只想為一組特定使用者顯示特定的一般小時，您可以透過在此欄位中選取他們在時程表設定檔中的方式，選取他們需要在時程表中檢視的一般小時。 如果您要停用所有一般時數，請取消選取所有時數型別，以產生不含一般時數區段的時程表。

   * **提醒通知**：新增提醒通知。 Workfront會傳送提醒給使用者，要求他們完成或核准其時程表。 您必須先建立提醒通知，然後才能將其與時程表設定檔建立關聯。

1. 若要將時間表設定檔與特定使用者、群組或(如果您是Workfront管理員)團隊建立關聯，請捲動至頁面底部，並找到&#x200B;**指派人員**&#x200B;區段。

   開始輸入使用者、群組或團隊的名稱，然後當它出現在下拉式清單中時按一下它。

   <!--To associate the timesheet profile with specific users, groups, or (if you are a Workfront administrator) teams, scroll towards the bottom of the page and find the **Assign People** section.-->

   如果您是群組管理員，您可以將時程表設定檔指派給您管理的群組，但不能指派給團隊。 如需詳細資訊，請參閱本文中的[群組管理員指派時程表設定檔的限制](#limitations-for-a-group-administrator-assigning-a-timesheet-profile)。

   >[!NOTE]
   >
   >* 您也可以編輯使用者設定檔，將使用者與時程表設定檔建立關聯。 如需詳細資訊，請參閱[編輯使用者的設定檔](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)。
   >* 新增群組時，「指派人員」標籤上只會顯示群組名稱，而不會顯示群組成員清單。 如果您想要檢視這裡列出的群組成員，請按一下儲存變更，然後按一下您剛建立之時程表設定檔的名稱。
   >* 當您完成這些步驟時，時間表設定檔只會為指派的使用者或群組成員產生時間表，這些使用者或群組成員沒有當期的時間表。

1. 按一下「**儲存**」。

1. 在時程表設定檔清單頂端，按一下&#x200B;**更多**&#x200B;圖示![更多](assets/more-icon.png)，然後按一下&#x200B;**產生時程表**。

   畫面底部會顯示已成功產生時程表的確認訊息。 系統會根據您建立的新設定檔產生新的時間表。

   如需詳細資訊，請參閱[手動產生時間表](/help/quicksilver/timesheets/create-and-manage-timesheets/manually-generate-timesheets.md)。

   週期性時程表首次產生時程表時，系統會為每個使用者建立兩個時程表，針對包含目前時間的時間範圍以及下列時間範圍。

   之後，每次產生新時程表時，就會為每個使用者建立一個時程表。

   <!--the content in the table above will need to match the content in the Create timesheets article-->

## 群組管理員指派時程表設定檔的限制 {#limitations-for-a-group-administrator-assigning-a-timesheet-profile}

如果您是群組管理員，而且存取層級中已停用管理存取選項時程表和時數，您可以建立時程表設定檔，但您只能將其指派給：

* 您管理的群組
* 您有權編輯的個別使用者，其所屬群組由您管理

對於這些群組和使用者，您將無權存取週期性時程表產生的時程表。

此外，如果您的存取層級也停用了「使用者管理員（群組使用者）」選項，您可以將時程表設定檔指派給您管理的群組，但這只會影響您有權編輯之群組中的使用者。 如果群組包含您無權編輯的使用者，則不會將時間表設定檔與群組的其餘部分指派給他們。

如需有關存取層級中時程表和時數的選項資訊，請參閱[授與使用者對特定區域的管理存取權](../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md)。

如需存取層級中選項「使用者管理員（群組使用者）」的相關資訊，請參閱[授予使用者存取權](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md)。

## 多個週期性時程表設定檔

您的組織可以有多個時間表設定檔，如果存在：

* 不同使用者集的不重複付薪期間
* 不同使用者集的不重複核准者
* 不同使用者組的不重複一般時數需求

一個使用者無法一次與多個時程表設定檔建立關聯。

<!--
<table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Name</strong> </td> 
      <td> <p> Add a name for the timesheet profile. It could be the name of a team or a group whose people share the same timeframe for their timesheets. </p> <p>This ia a required field.</p> </td> 
     </tr> 

   <tr> 
      <td role="rowheader"><strong>Description</strong> </td> 
      <td> <p> Add more information about the timesheet profile.     
      </p> </td> 
     </tr>

   <tr> 
   <td role="rowheader"><strong>Group with Administration Access</strong> </td> 
      <td> <p> 
      <ul> 
      <li> <p>If you are creating a system-level timesheet profile, leave this field blank.</p> <p>Any user who can edit user accounts can attach a system-level timesheet to other users.</p> <p>Only a Workfront administrator can edit a system-level timesheet profile.</p> </li> 
      </ul> 
     <ul> 
      <li> <p>If you are creating a timesheet profile for a group you administer, identify the group here.</p> <p>This does not assign the timesheet profile to the users in the group; it only allows the group's administrators to modify the timesheet profile. You will assign the profile to users in Step 6.</p>

   <p><b>NOTE</b>: When users outside the group are attaching timesheet profiles to other users, they won't be able to see or attach this timesheet profile.</p> </li> 
      </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Create timesheets</strong> </td> 
      <td> <p> <p>Specify when the timesheet profile should generate the timesheets. A timesheet can be set to automatically generate on a weekly, bi-weekly, semi-monthly, or monthly basis. Select the day of the week when you want the timesheet to be produced.</p>
      <p>A weekly timesheet begins on the date it is generated. For example, if you create weekly timesheets every Thursday, the first day of the week on the timesheet is Thursday.</p>
    
      
   <p><b>NOTE</b>: Workfront always creates two timesheets at a time: the first timesheet always includes the current date, and the second timesheet starts when the time frame of the first one ends.</p> </p> </td> 
   </tr> 
     <tr> 
      <td role="rowheader"><p><strong>Approvers</strong></p> </td> 
      <td> <p> <p>Approvers are users who approve the timesheet for the users associated with the timesheet. You can identify up to 7 users as approvers on a timesheet. Identifying multiple users is useful to ensure an approver is available when someone is out of the office. All approvers are notified when a user submits the timesheet for approval. Only one user is required to approve the timesheet in order for it to be approved.</p> <p>Only users with timesheet administrative rights can be set as approvers. For more information about timesheet administrative rights, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Grant users administrative access to certain areas</a>.</p> <p>Use the drop-down menu&nbsp;to select&nbsp;the approver&nbsp;for the timesheet (if an approver is required). You can select from the following options:</p> 
      <ul> 
      <li><strong>None</strong>: The timesheet does not need to&nbsp;be approved.</li> 
      <li><strong>Their Manager</strong>: This is the default approver, set by the system. In this case, the user designated as their manager approves the timesheet when it is submitted for approval.</li> 
      <li><strong>Specific People:</strong>&nbsp;You can designate specific users, by name, as timesheet approvers. You can have multiple approvers on a timesheet. In this case, after&nbsp;one of the approvers approves the timesheet, the timesheet is marked as <strong>Closed</strong> and it disappears from the timesheet approvals list of all the remaining approvers.</li> 
       </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Can edit time </strong> </td> 
      <td> <p> <p>Select this option to allow the approvers to edit hours on the timesheet. 

   <p>This option works together with the **Restrict timesheet editing to owners and admins** setting in the Setup > Timesheet & Hours > Preferences area. For more information, see <a href="../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md">Configure timesheet and hour preferences</a>.</p>

   <p>The following scenarios exist: </p>

   <ul>
      <li>When the <b>Restrict timesheet editing to owners and admins</b> option is enabled:</li>
      <ul><li>Approvers can only approve and reject timesheet, regardless of whether the <b>Can edit time</b> is enabled or not. </li>
      <li>Timesheet owners' managers can only view their direct reports' timesheets.</li></ul>
      <li>When the <b>Restrict timesheet editing to owners and admins</b> option is disabled:</li>
    <ul><li>When the <b>Can edit time</b> is enabled, approvers can submit, reopen, or close the timesheet and can edit the time.</li>
      <li>When the <b>Can edit time</b> is disabled, approvers cannot submit, reopen, or close the timesheet and cannot edit the time. Approvers can only approve or reject the timesheet. </li>
      <li>Timesheet owners' managers can submit, recall, reopen, and edit their direct reports' timesheets.</li></ul>
      </ul>

   <p>

   <b>NOTE</b>: Once you submit a timesheet for approval, you can no longer edit the hours. To return a submitted timesheet to an editable state, recall the timesheet or have the approver reject the timesheet. For more information, see <a href="../../timesheets/create-and-manage-timesheets/submit-timesheet-for-approval.md">Submit a timesheet for approval</a> and <a href="../../timesheets/create-and-manage-timesheets/timesheet-approvals.md">Approve a timesheet</a>.</p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Overtime</strong> </td> 
      <td>You can choose to hide the Overtime box in timesheets. This option is disabled by default.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Available Hour Types</strong> </td> 
      <td><p>This setting refers only to General Hour Types, and not to project-specific hour types. </p>
      <p>By default, users see all general hours on a timesheet. However, if your organization wants only specific general hours to be shown for a particular set of users, you can select the general hours that they need to see in their timesheets by selecting them in their timesheet profile in this field. If you want to disable all general hours, deselect all hour types to generate the timesheet without a section for general hours.</p></td> 
     </tr> 

   <tr> 
      <td role="rowheader"><strong>Reminder notifications</strong> </td> 
      <td> <p> Add a reminder notification. Workfront will send reminders to users to ask them to complete or approve their timesheets. You must create reminder notifications before you can associate them with a timesheet profile.  </p> </td> 
     </tr>
    </tbody> 
   </table>
-->