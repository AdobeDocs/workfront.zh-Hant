---
title: 群組管理員
user-type: administrator
content-type: reference;overview
product-area: system-administration;user-management
navigation-topic: group-roles
description: Adobe Workfront管理員位於擁有許多部門的大型組織中，可能不想管理這些部門內組織的所有部門和群組。 相反，他們可以為該組內的每個部門和子組建立一個組，每個部門和子組由組管理員管理。
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 589cf9fb-f195-4b69-a240-3f73e6ca623e
source-git-commit: 03667fbdd1b0d68b9ad2d2db4a1ed85b8136062b
workflow-type: tm+mt
source-wordcount: '987'
ht-degree: 0%

---

# 群組管理員

Adobe Workfront管理員位於擁有許多部門的大型組織中，可能不想管理這些部門內組織的所有部門和群組。 相反，他們可以為該組內的每個部門和子組建立一個組，每個部門和子組由組管理員管理。

群組管理員可管理群組的需求，例如使用者成員資格、版面範本、自訂資料、狀態和偏好設定。

一個組中最多可以包含14個子組。

>[!NOTE]
>
>子組上方層次結構中的所有組管理員都具有管理該子組的管理權限。

如需建立和管理群組的相關資訊，請參閱 [建立群組](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md) 和 [管理群組](../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md). 另請參閱 [子組概述](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md).

## 指定群組管理員

每個頂級組必須至少有一個組管理員。 組的Workfront管理員或管理員可以將組管理員分配給組的子組，但這不是必需的。 如需詳細資訊，請參閱 [建立群組](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

如果您是Workfront管理員，建議您先執行下列操作，再將使用者指定為群組管理員：

* 請注意您系統中目前的Workfront管理員人數。
* 記下您在系統中的群組數。
* 決定您是否可以變更某些Workfront管理員的存取層級，並指定他們為群組管理員。

   如需群組管理員功能的詳細資訊，請參閱 [由組管理員完成的任務](#tasks-done-by-group-administrators).

* 確定是否希望組管理員能夠以其他用戶身份登錄，或是重置所管理組中用戶的密碼。 執行這些任務需要其他訪問，如 [組管理員所需的訪問權](#access-needed-for-group-administrators).
* 為了更好地管理用戶，請考慮將組或子組（而非用戶）分配給以下對象：

   * 版面配置範本
   * 排程
   * 週期性時程表

## 組管理員所需的訪問權 {#access-needed-for-group-administrators}

每個組管理員都必須擁有計畫許可證。

建議群組管理員擁有使用者的編輯存取權，這樣他們就能執行下列工作：

* 以其管理的群組和子群組中的其他使用者身分登入。
* 在管理的組中重置其他用戶的密碼。

>[!IMPORTANT]
>
>群組管理員的存取權必須高於其管理的存取權；否則，他們將無法查看或修改較低的訪問級別。
>有關授予此訪問權限的說明，請參閱 [建立或修改自訂存取層級](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

對於需要將時間表配置檔案分配給組和子組中的用戶的組管理員，我們還建議對時間表和小時進行管理訪問。 有關授予此訪問權限的說明，請參閱 [授予用戶對特定區域的管理訪問權限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

## 由組管理員完成的任務 {#tasks-done-by-group-administrators}

作為組管理員，您可以執行以下任務來管理您監督的組。 其中一些功能與Workfront管理員所具備的功能相同。

* [管理群組成員](#manage-group-members)
* [管理組對象](#manage-group-objects)
* [管理群組偏好設定和工具](#manage-group-preferences-and-tools)

### 管理群組成員 {#manage-group-members}

* 在您管理的組和子組中建立、編輯和刪除子組。 如需指示，請參閱 [建立子組](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/create-a-subgroup.md).
* 新增您對其擁有群組和子群組編輯存取權的使用者。 或者，編輯使用者的設定檔，將使用者新增至群組和子群組。

   如果您已在存取層級中啟用「使用者管理員（群組使用者）」權限，也可以更新群組成員設定檔中的欄位。

   如需詳細資訊，請參閱 [編輯使用者的設定檔](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

   >[!NOTE]
   >
   >Workfront管理員可以覆寫群組管理員對群組成員資格所做的變更。

* 重設您管理之群組成員之使用者的密碼。 如需詳細資訊，請參閱 [編輯使用者的設定檔](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).
* 以您所管理群組成員的使用者身分登入。 如需詳細資訊，請參閱 [以其他使用者身分登入](../../../administration-and-setup/add-users/create-and-manage-users/log-in-as-another-user.md).
* 查看組及其下面的子組可用許可證的數量。 如需詳細資訊，請參閱 [管理系統中的可用許可證](../../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md).

### 管理組對象 {#manage-group-objects}

* 建立組級別的「佈局模板」，並將它們與您管理的組和子組關聯。 如需詳細資訊，請參閱 [建立和管理版面範本](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
* 建立組級時間表配置檔案，將它們與您管理的用戶和組關聯，並手動生成時間表。 如需詳細資訊，請參閱 [建立、編輯和分配工時單配置檔案](../../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).
* 沒有對批准流程的管理訪問權限，請為您管理的組和子組建立和編輯批准流程。 如需詳細資訊，請參閱 [建立工作項的審批流程](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

   有關對批准流程的管理訪問的資訊，請參閱 [授予用戶對特定區域的管理訪問權限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

* 建立排程，並將其與您管理的群組建立關聯。 如需詳細資訊，請參閱 [建立排程](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).
* 管理指派給您管理之群組的團隊，而不是團隊的成員。 同時，根據「組」(Group)欄位建立組報告，以標識某個組被分配給哪個組。 如需詳細資訊，請參閱 [建立團隊](../../../people-teams-and-groups/create-and-manage-teams/create-a-team.md).
* 還原與您管理的組關聯的項目，以及與項目關聯的任何任務、問題或文檔。 如需詳細資訊，請參閱 [還原已刪除的項](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

### 管理群組偏好設定和工具 {#manage-group-preferences-and-tools}

* 在系統中為組解除鎖定項目首選項、任務或問題首選項，或時間表和小時首選項時，請編輯您管理的組的首選項。 這些首選項會影響項目、任務和問題行為。 如需詳細資訊，請參閱下列內容：

   * [配置組的項目首選項](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md)
   * [配置組的任務和問題首選項](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md)

* 為您管理的群組建立和編輯群組狀態。 如需詳細資訊，請參閱 [建立或編輯群組狀態](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).
* 為您管理的群組設定事件通知。 只有在Workfront管理員解除鎖定透過系統為群組設定事件通知的功能後，才能執行此動作。 如需詳細資訊，請參閱 [檢視及設定群組的事件通知](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).
