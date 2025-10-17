---
title: 群組管理員
user-type: administrator
content-type: reference;overview
product-area: system-administration;user-management
navigation-topic: group-roles
description: 在擁有許多部門的大型組織中，Adobe Workfront管理員可能不想管理這些部門中的所有組織部門和群組。 相反地，他們可以為該群組中的每個部門及子群組建立一個群組，每個群組都由群組管理員管理。
author: Becky
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 589cf9fb-f195-4b69-a240-3f73e6ca623e
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '1047'
ht-degree: 1%

---

# 群組管理員

<!-- Audited: 12/2023 -->

在擁有許多部門的大型組織中，Adobe Workfront管理員可能不想管理這些部門中的所有組織部門和群組。 相反地，他們可以為該群組中的每個部門及子群組建立一個群組，每個群組都由群組管理員管理。

群組管理員可以管理群組的需求，例如使用者成員資格、版面配置範本、自訂資料、狀態和偏好設定。

一個群組下最多可以有14個層級的子群組。

>[!NOTE]
>
>子群組之上階層中的所有群組管理員都擁有管理該子群組的管理許可權。

如需建立和管理群組的相關資訊，請參閱[建立群組](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md)和[管理群組](../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md)。 另請參閱[子群組概述](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md)。

## 指定群組管理員

每個頂層群組都必須至少有一個群組管理員。 Workfront管理員或群組管理員可將群組管理員指派給群組的子群組，但這並非必要。 如需詳細資訊，請參閱[建立群組](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md)。

如果您是Workfront管理員，建議您先執行下列動作，再將使用者指定為群組管理員：

* 記下系統中目前的Workfront管理員人數。
* 記下您在系統中的群組數目。
* 決定是否可變更部分Workfront管理員的存取層級，並將他們指定為群組管理員。

  如需有關群組管理員許可權的詳細資訊，請參閱本文中的[群組管理員完成的工作](#tasks-done-by-group-administrators)。

* 決定您是否希望群組管理員能夠以其他使用者身份登入，或重設您管理之群組中的使用者密碼。 需要額外的存取權才能執行這些工作，如下文[群組管理員所需存取權](#access-needed-for-group-administrators)中所述。
* 為了更好地管理使用者，請考慮將群組或子群組指派給下列物件，而非指派使用者：

   * 版面配置範本
   * 排程
   * 週期性時程表

## 群組管理員所需的存取權 {#access-needed-for-group-administrators}

每個群組管理員都必須擁有

* 目前定價與封裝模式中的計畫授權
* 新定價與封裝模式中的標準授權

我們建議群組管理員擁有使用者的「編輯」存取權，以便他們可執行下列工作：

* 以其他使用者的身份登入他們管理的群組和子群組。
* 重設其他使用者在其管理的群組中的密碼。

>[!IMPORTANT]
>
>群組管理員的存取權必須高於其管理者，否則將無法檢視或修改較低的存取層級。
>&#x200B;>如需授與此存取權的指示，請參閱[建立或修改自訂存取層級](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)。

對於需要為其群組和子群組中的使用者指派時程表設定檔的群組管理員，我們也建議對時程表和時數進行管理存取。 如需授與此存取權的指示，請參閱[授與使用者對特定區域的管理存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md)。

## 群組管理員完成的工作 {#tasks-done-by-group-administrators}

身為群組管理員，您可以執行下列概述的工作，以管理您所監督的群組。 其中的一些功能與Workfront管理員獲得的功能相同。

>[!NOTE]
>
>在新的定價與封裝模式中，您必須有Prime計畫或以上版本，才能執行下列作業：
>
> * 建立群組事件通知
> * 設定群組專案偏好設定
> * 設定群組任務和問題偏好設定
> * 解鎖子群組偏好設定的設定
> * 群組時程表和小時偏好設定
> * 解鎖時程表和小時偏好設定

### 管理群組成員 {#manage-group-members}

* 在您管理的群組和子群組中建立、編輯和刪除子群組。 如需指示，請參閱[建立子群組](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/create-a-subgroup.md)。
* 新增您對其具有編輯許可權的使用者以存取您的群組和子群組。 或者，透過編輯使用者的設定檔來將使用者新增至群組和子群組。

  如果您在存取層級中啟用了使用者管理員（群組使用者）許可權，則也可以更新群組成員設定檔中的欄位。

  如需詳細資訊，請參閱[編輯使用者的設定檔](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)。

  >[!NOTE]
  >
  >Workfront管理員可以覆寫群組管理員對群組成員資格所做的變更。

* 重設您管理之群組成員的使用者密碼。 如需詳細資訊，請參閱[編輯使用者的設定檔](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)。
* 以您管理群組成員的使用者身分登入。 如需詳細資訊，請參閱[以其他使用者身分登入](../../../administration-and-setup/add-users/create-and-manage-users/log-in-as-another-user.md)。
* 檢視您的群組及其下方的子群組可用的授權數量。 如需詳細資訊，請參閱[管理您系統中的可用授權](../../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md)。

### 管理群組物件 {#manage-group-objects}

* 建立群組層級版面配置範本，並將其與您管理的群組和子群組建立關聯。 如需詳細資訊，請參閱[建立及管理配置範本](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md)。
* 建立群組層級的時程表設定檔，將其與您管理的使用者和群組建立關聯，並手動產生時程表。 如需詳細資訊，請參閱[建立、編輯和指派週期性時程表](../../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md)。
* 若沒有核准程式的管理存取權，請為您管理的群組和子群組建立和編輯核准程式。 如需詳細資訊，請參閱[建立工作專案的核准程式](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md)。

  如需有關核准程式之管理存取許可權的資訊，請參閱[授予使用者對特定區域的管理存取許可權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md)。

* 建立排程並將其與您管理的群組建立關聯。 如需詳細資訊，請參閱[建立排程](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)。
* 管理指派給您管理之群組的團隊，但不成為團隊成員。 此外，根據「群組」欄位建立專案團隊報告，以識別將特定專案團隊指派給哪個群組。 如需詳細資訊，請參閱[建立團隊](../../../people-teams-and-groups/create-and-manage-teams/create-a-team.md)。
* 還原與您管理的群組相關聯的專案，以及與專案相關聯的任何任務、問題或檔案。 如需詳細資訊，請參閱[還原已刪除的專案](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md)。

### 管理群組偏好設定和工具 {#manage-group-preferences-and-tools}

* 當系統各群組的專案偏好設定、任務或問題偏好設定、或時程表和時數偏好設定已解鎖時，請編輯您管理之群組的該偏好設定。 這些偏好設定會影響專案、任務和問題行為。 如需詳細資訊，請參閱以下頁面:

   * [設定群組的專案偏好設定](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md)
   * [設定群組的任務和問題偏好設定](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md)

* 為您管理的群組建立和編輯群組狀態。 如需詳細資訊，請參閱[建立或編輯群組狀態](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md)。
* 為您管理的群組設定事件通知。 只有在Workfront管理員解除鎖定透過系統為群組設定事件通知的功能後，您才能執行此動作。 如需詳細資訊，請參閱[檢視並設定群組](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md)的事件通知。
