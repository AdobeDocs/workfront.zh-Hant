---
product-area: projects;agile-and-teams
navigation-topic: plan-a-project
title: 管理專案團隊
description: 專案團隊由與專案相關聯的使用者組成。 專案團隊的成員會顯示在專案的「人員」區段或範本中，可用來建立專案的「人員」區段。
author: Alina
feature: Work Management, Projects
role: User
exl-id: 6e8036fc-feda-4277-9502-0b973028fccb
source-git-commit: 00e693fc8b35a59f6ed212bc30da7f85cc78c845
workflow-type: tm+mt
source-wordcount: '838'
ht-degree: 2%

---

# 管理專案團隊

<!--take preview and production references out at production - August 7-->

<!--<div class="preview"> 

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers after a week from the Preview release.      

For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).  

</div>

-->

專案團隊由與專案相關聯的使用者組成。 如需詳細資訊，請參閱[專案團隊概述](/help/quicksilver/manage-work/projects/planning-a-project/project-team-overview.md)。

專案團隊的成員會顯示在專案的「人員」區段中。

從範本建立專案後，顯示在專案範本的「人員」區段中的使用者將成為專案團隊。

下列使用者會針對專案和範本自動新增至專案團隊：

* 所有者
* 贊助者
* 指派給任務的使用者
* 指派給問題的使用者（僅適用於專案）

專案團隊中的使用者會收到有關專案的通知。 如需詳細資訊，請參閱[事件通知型別](/help/quicksilver/administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md)。

您可以新增專案和範本團隊中的使用者（僅限專案）、將其移除或傳送更新給他們，以管理這些使用者。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront套件</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td> <p>標準</p>
    <p>規劃</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>編輯專案和範本的存取權</p> <p>檢視或更高的使用者存取權</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>檢視專案或範本的或更高許可權</p> </td> 
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

<!--Old access: 

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
   <td> <p>Standard </p>
    <p>Plan </p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level</td> 
   <td> <p>Edit access to Projects and Templates</p> <p>View or higher access to Users</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions to a project or to a template</p> </td> 
  </tr> 
 </tbody> 
</table>

*For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).



## Add users to a Project Team

When you add users to the project team, they gain View permissions on the project and the tasks, issues, and documents of the project. For more information, see the article [Project Team overview](../../../manage-work/projects/planning-a-project/project-team-overview.md).

>[!TIP]
>
>Users on the Project Team are not automatically added to the resource management tools for the project.

You can add users to the project team in the following ways:

* [Automatically add users to a Project Team](#automatically-add-users-to-a-project-team) 
* [Manually add users to a Project Team](#manually-add-users-to-a-project-team)

### Automatically add users to a Project Team {#automatically-add-users-to-a-project-team}

The users that fulfill the following roles on the project are automatically added to the project team and appear  in the People section when the project is created:

* The creator of the project
* The project owner
* The project sponsor

Users are also automatically added to the project team when they are assigned to the following:

* Tasks
* Issues

### Manually add users to a Project Team {#manually-add-users-to-a-project-team}

If users that don't fulfill any role on the project want to be notified about certain updates or changes during the life of the project, you can manually add them to the project team. 

 For more information about what notifications can be enabled for users on the project team, see [Event notification types](../../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md). 

 <!--drafted - this used to be the case, in the note below but this limitation was removed on Jan 5, 2023 - as a patch, not a release feature:

>[!IMPORTANT]
>
>You can add to the Project Team only users that belong to the Group associated with the project. You cannot add users that belong to the Subgroups of the project's group. 



## Manage people on a project

1. Go to the project you want to manage the project team for.

   >[!TIP]
   >
   >You must have users assigned to tasks, issues or as stakeholders on the project to have them display in the People section.

1. Click **People** in the left panel. 

1. Click **Add users**. 

   The **Add users to Project Team** box displays.

   ![add_users_dialog.png](assets/add-users-dialog-350x217.png)

1. In the **Add users** box, begin typing the name of an active Workfront user that you want to add to the project team, then click the name when it appears in the list.

   Repeat this step to add multiple users to the project team. The users must belong to the group associated with the project. 

   >[!TIP]
   >
   >* You cannot add users by adding their teams, groups, companies, or job roles.
   >* As you add the users, notice the avatar, the user's Primary Role, and their email address to distinguish between users with identical names. Users must be associated with at least one job role to view it as you add them.
   >
   >  You must have the View Contact Info setting enabled in your access level for Users to view users' emails. For information, see [Grant access to users](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

1. Click **Add**.

   The users gain View permissions to the project and receive notifications about the project as part of the project team.

1. (Optional) If you want a user to receive a  notification when their job role is added to a task, issue, or project approval, click inside the **Job Role** column for the user, and select a job role that will be associated with the approval. 

   The users will receive notifications related to the approvals assigned to the selected job role. 

   For more information see the "Role-based approvals" section in the article [Project Team overview](/help/quicksilver/manage-work/projects/planning-a-project/project-team-overview.md).

1. Select one or several users in the list, then click the **Remove** icon ![Remove icon](assets/remove-icon.png) to remove them from the team. 
 
1. Click **Yes, Remove Selected Users** to confirm and remove the users.

   Users are removed and unassigned from incomplete work items.

   For more information, see the [Considerations for removing users from a project team](#considerations-for-removing-users-from-a-project-team) section in this article.
1. (Optional) To send an update for this project to users, click **Update All** to send the update to everyone on the team

   Or 

   Select one or multiple users in the list, then click **Send Update to User**.

   <!--update screen shot when they fix the bug - the text above the box needs to match the OLD box, below-->

![傳送更新給專案上的使用者方塊](assets/send-update-to-user-on-project-box-2025.png)

<!--Old UI for projects but the text above the comment box is right and matches the functionality):
   ![OLD Send update to user on a project](assets/send-update-to-user-on-project-box.png)-->

**傳送更新給使用者**&#x200B;方塊開啟。

1. 執行下列其中一項：

   * 為選取的使用者新增更新。
   * 按一下鎖定圖示，將更新設為貴公司使用者的私密更新。
   * 標籤接收相同更新的其他使用者。
   * 按一下「**傳送**」。

   更新已新增至專案的&#x200B;**更新**&#x200B;區段，且所有選取的使用者都會顯示為已標籤的使用者。

   使用者若已啟用，可能會收到電子郵件通知，並收到新更新的應用程式內通知。

1. （選擇性）按一下&#x200B;**匯出**&#x200B;圖示![匯出圖示](assets/export-icon.png)，將使用者清單匯出至檔案

   或

   選取使用者，然後按一下&#x200B;**匯出**&#x200B;圖示以僅匯出特定使用者。

## 管理範本上的人員

1. 移至您要為其管理專案團隊的範本。

   >[!TIP]
   >
   >您必須將使用者指派給任務或範本上的利害關係人，他們才會顯示在「人員」區段中。

1. 按一下左側面板中的&#x200B;**人員**。

1. 在清單中選取一或多個使用者，然後按一下&#x200B;**移除**&#x200B;圖示，將他們從團隊中移除。

1. 按一下&#x200B;**是，移除選取的使用者**&#x200B;以確認並移除使用者。

   會從範本任務中移除及取消指派使用者。

   如需詳細資訊，請參閱本文的[從專案團隊](#considerations-for-removing-users-from-a-project-team)移除使用者的考量事項。

1. （選擇性）若要傳送更新給使用者，請按一下[全部更新]，將更新傳送給清單中的所有使用者&#x200B;**&#x200B;**

   或

   在清單中選取一或多個使用者，然後按一下&#x200B;**傳送更新給使用者**。

   <!--update screen shot for unshim production, notice the text above the box - it needs to say "Post an update to each person's profile"-->

   ![傳送更新給範本上的使用者方塊](assets/send-update-to-user-on-template-box.png)

   **傳送更新給使用者**&#x200B;方塊開啟。

1. 請執行下列動作：

   * 為選取的使用者新增更新。
   * 按一下「**標籤人員**」以標籤接收相同更新的其他使用者。
   * 選取&#x200B;**我的公司私有**&#x200B;選項，將更新設為貴公司使用者的私有。
   * 按一下「**傳送**」。

     >[!TIP]
     >
     >**我的公司專用**&#x200B;設定只有在您的Workfront設定檔與公司相關聯時才可用。

   更新已新增到每個已標籤使用者設定檔的&#x200B;**更新**&#x200B;區段。

   使用者若已啟用，可能會收到電子郵件通知，並收到新更新的應用程式內通知。

1. 按一下&#x200B;**匯出**&#x200B;圖示![匯出圖示](assets/export-icon.png)，將使用者清單匯出至檔案

   或

   選取使用者，然後按一下&#x200B;**匯出**&#x200B;圖示以僅匯出特定使用者。

## 從專案團隊中移除使用者的考量事項

當您從使用者在專案中的角色中移除使用者時，他們仍然是專案團隊的一部分。

您必須從專案團隊從專案的「人員」區段中移除這些人員，他們才能停止接收傳送給專案團隊的通知。

如果您從專案團隊中移除使用者，並且使用者被指派到專案中的任務或問題，則會從未完成的任務和問題中取消指派使用者。 在這種情況下，任務和問題返回到工作負載平衡器中的未指派工作區域。

指派給已完成任務和問題的使用者仍會指派給任務和問題，即使您將其從專案團隊中移除後亦然。

從專案或範本的「人員」區段移除下列使用者時，系統就會從他們在專案中的角色中移除這些使用者：

* 指派給未完成任務的使用者
* 指派給未完成問題的使用者

從專案或範本的「人員」區段中移除下列使用者時，系統不會將他們從其在專案中的角色中移除：

* 所有者
* 贊助者

如需有關從專案團隊移除使用者的詳細資訊，請參閱[從專案移除使用者](../../../manage-work/projects/manage-projects/remove-users-from-projects.md)。

