---
product-area: projects;agile-and-teams
navigation-topic: plan-a-project
title: 管理專案團隊
description: 專案團隊由與專案相關聯的使用者組成。 專案團隊的成員會顯示在專案的「人員」區段或範本中，可用來建立專案的「人員」區段。
author: Alina
feature: Work Management, Projects
role: User
exl-id: 6e8036fc-feda-4277-9502-0b973028fccb
source-git-commit: fe51ded26c57e3b7137e42ad2218d79adf032b85
workflow-type: tm+mt
source-wordcount: '1280'
ht-degree: 1%

---

# 管理專案團隊

<!--take preview and production references out at production - August 7-->

<div class="preview">

本頁醒目提示的資訊指出尚未普遍可用的功能。 它僅在預覽環境中可供所有客戶使用。 在預覽版發佈一週後，生產環境中也將提供相同功能給所有客戶。

如需詳細資訊，請參閱[介面現代化](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md)。

</div>

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

+++ 展開以檢視存取需求。

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
   <td> <p>新增：標準 </p>
    <p>目前：計畫 </p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級</td> 
   <td> <p>編輯專案和範本的存取權</p> <p>檢視或更高的使用者存取權</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>檢視專案或範本的或更高許可權</p> </td> 
  </tr> 
 </tbody> 
</table>

*如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

<!--Old access: 

You must have the following access to perform the steps in this article:

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
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects</p> <p>View or higher access to Users</p> <p><b>NOTE</b> 
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions to the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*To find out what plan, license type, or access you have, contact your Workfront administrator.

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

-->

## 管理專案人員

1. 移至您要管理專案團隊的專案。

   >[!TIP]
   >
   >您必須將使用者指派給專案上的任務、問題或利害關係人，他們才會顯示在「人員」區段中。

1. 按一下左側面板中的&#x200B;**人員**。

1. 按一下&#x200B;**新增使用者**。

   顯示&#x200B;**新增使用者至專案團隊**&#x200B;方塊。

   ![add_users_dialog.png](assets/add-users-dialog-350x217.png)

1. 在&#x200B;**新增使用者**&#x200B;方塊中，開始輸入您要新增至專案團隊的作用中Workfront使用者名稱，然後在其出現在清單中時按一下該名稱。

   重複此步驟，將多位使用者新增至專案團隊。 使用者必須屬於與專案相關聯的群組。

   >[!TIP]
   >
   >* 您無法透過新增其團隊、群組、公司或工作角色來新增使用者。
   >* 新增使用者時，請注意頭像、使用者的主要角色及其電子郵件地址，以區分具有相同名稱的使用者。 使用者必須至少與一個工作角色相關聯，才能在您新增時檢視該角色。
   >
   >  您必須在存取層級中啟用檢視聯絡資訊設定，使用者才能檢視使用者的電子郵件。 如需詳細資訊，請參閱[授予使用者存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md)。

1. 按一下&#x200B;**新增**。

   使用者取得專案的檢視許可權，並作為專案團隊的一部分接收有關專案的通知。

1. （選擇性）如果您希望使用者在其工作角色新增至任務、問題或專案核準時收到通知，請按一下使用者的&#x200B;**工作角色**&#x200B;欄，然後選取將與核准關聯的工作角色。

   使用者將收到與指派給所選工作角色的核准相關的通知。

   如需詳細資訊，請參閱文章[專案團隊概觀](/help/quicksilver/manage-work/projects/planning-a-project/project-team-overview.md)中的「角色型核准」一節。

1. 在清單中選取一或多個使用者，然後按一下&#x200B;**移除**&#x200B;圖示![移除圖示](assets/remove-icon.png)，將使用者從團隊中移除。

1. 按一下&#x200B;**是，移除選取的使用者**&#x200B;以確認並移除使用者。

   會從未完成的工作專案移除及取消指派使用者。

   如需詳細資訊，請參閱本文的[從專案團隊](#considerations-for-removing-users-from-a-project-team)移除使用者的考量事項。
1. （選用）若要將此專案的更新傳送給使用者，請按一下「全部更新」將更新傳送給團隊中的每個人

   或

   在清單中選取一或多個使用者，然後按一下&#x200B;**傳送更新給使用者**。

   ![傳送更新給專案的使用者](assets/send-update-to-user-on-project-box.png)

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

1. 在清單中選取一或多個使用者，然後按一下[移除] ****&#x200B;以從團隊中移除這些使用者。

1. 按一下&#x200B;**是，移除選取的使用者**&#x200B;以確認並移除使用者。

   會從範本任務中移除及取消指派使用者。

   如需詳細資訊，請參閱本文的[從專案團隊](#considerations-for-removing-users-from-a-project-team)移除使用者的考量事項。

1. （選用）若要傳送更新給使用者，請按一下全部更新，將更新傳送給清單中的所有使用者

   或

   在清單中選取一或多個使用者，然後按一下[更新]。****

   <!--update screen shot for unshim production, notice the text above the box - it needs to say "Post an update to each person's profile"-->

   ![傳送更新給範本上的使用者方塊](assets/send-update-to-user-on-template-box.png)

   **傳送更新給使用者**&#x200B;方塊開啟。

1. 執行下列動作：

   * 在生產環境中：

      * 為選取的使用者新增更新。
      * 按一下人員圖示可標籤其他使用者，以接收相同的更新。
      * 按一下鎖定圖示，將更新設為貴公司使用者的私密更新。
      * 按一下「**傳送**」。

   * <span class="preview">在預覽環境中： </span>

   <div class="preview">

   * 為選取的使用者新增更新。
   * 按一下「**標籤人員**」以標籤接收相同更新的其他使用者。
   * 選取&#x200B;**我的公司私有**&#x200B;選項，將更新設為貴公司使用者的私有。
   * 按一下「**傳送**」。

   </div>

   更新已新增到每個已標籤使用者設定檔的&#x200B;**更新**&#x200B;區段。

   使用者若已啟用，可能會收到電子郵件通知，並收到新更新的應用程式內通知。

1. （選擇性）按一下[匯出&#x200B;****]將使用者清單匯出至檔案

   或

   選取使用者，然後按一下&#x200B;**匯出**&#x200B;以僅匯出特定使用者。

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

