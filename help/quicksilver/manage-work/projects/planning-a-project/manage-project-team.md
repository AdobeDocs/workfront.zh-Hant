---
product-area: projects;agile-and-teams
navigation-topic: plan-a-project
title: 管理專案團隊
description: 專案團隊由與專案相關聯的使用者組成。 專案團隊的成員會顯示在專案的「人員」區段中。
author: Alina
feature: Work Management, Projects
role: User
exl-id: 6e8036fc-feda-4277-9502-0b973028fccb
source-git-commit: afbf2e2fbfcc2c527223da008518bc7632872c23
workflow-type: tm+mt
source-wordcount: '679'
ht-degree: 0%

---

# 管理專案團隊

專案團隊由與專案相關聯的使用者組成。 專案團隊的成員會顯示在專案的「人員」區段中。

## 存取需求

<!--drafted for P&P:
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
   <td> <p>Current license: Standard </p>
   Or
   <p>Legacy license: Plan </p>
    </td> 
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
   <td> <p>計劃 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>編輯專案的存取權</p> <p>檢視或更高的使用者存取權</p> <p><b>附註</b>

如果您還是沒有存取權，請詢問您的Workfront管理員，他們是否在您的存取層級中設定其他限制。 如需Workfront管理員如何修改存取層級的詳細資訊，請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>。</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>檢視專案或更高的許可權</p> <p>如需請求其他存取權的資訊，請參閱<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求物件</a>的存取權。</p> </td> 
  </tr> 
 </tbody> 
</table>

*若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的Workfront管理員。

## 將使用者新增至專案團隊

當您將使用者新增到專案團隊時，他們將獲得有關專案以及專案的任務、問題和檔案的檢視許可權。 如需詳細資訊，請參閱文章[專案團隊概述](../../../manage-work/projects/planning-a-project/project-team-overview.md)。

>[!TIP]
>
>專案團隊中的使用者不會自動新增至專案的資源管理工具。

您可以透過下列方式將使用者新增至專案團隊：

* [自動新增使用者至專案團隊](#automatically-add-users-to-a-project-team)
* [手動新增使用者至專案團隊](#manually-add-users-to-a-project-team)

### 自動將使用者新增至專案團隊 {#automatically-add-users-to-a-project-team}

在專案中履行下列角色的使用者會自動新增至專案團隊，並在建立專案時顯示在「人員」區段中：

* 專案的建立者
* 專案所有者
* 專案贊助者

當使用者被指派到以下專案時，他們也會被自動新增到專案團隊：

* 任務
* 問題

### 手動新增使用者至專案團隊 {#manually-add-users-to-a-project-team}

如果專案上未履行任何角色的使用者希望在專案存留期間收到有關某些更新或變更的通知，您可以手動將其新增到專案團隊。

如需專案團隊使用者可啟用哪些通知的詳細資訊，請參閱[事件通知型別](../../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md)。

<!--drafted - this used to be the case, in the note below but this limitation was removed on Jan 5, 2023 - as a patch, not a release feature:

>[!IMPORTANT]
>
>You can add to the Project Team only users that belong to the Group associated with the project. You cannot add users that belong to the Subgroups of the project's group. 

-->

1. 前往您要新增使用者的專案。

1. 按一下左側面板中的&#x200B;**人員**。 您可能需要先按一下&#x200B;**顯示更多**。

1. 按一下&#x200B;**新增使用者**。

   新增使用者至專案團隊對話方塊隨即顯示。

   ![add_users_dialog.png](assets/add-users-dialog-350x217.png)

1. 在&#x200B;**新增使用者**&#x200B;方塊中，開始輸入您要新增至專案團隊的作用中Workfront使用者名稱，然後在其出現在下拉式清單中時按一下該名稱。

   重複此步驟，將多位使用者新增至專案團隊。 使用者必須屬於與專案相關聯的群組。

   >[!TIP]
   >
   >* 您無法透過新增其團隊、群組、公司或工作角色來新增使用者。
   >* 新增使用者時，請注意頭像、使用者的主要角色及其電子郵件地址，以區分具有相同名稱的使用者。 使用者必須至少與一個工作角色相關聯，才能在您新增時檢視該角色。
   >
   >  您必須在存取層級中啟用檢視聯絡資訊設定，使用者才能檢視使用者的電子郵件。 如需詳細資訊，請參閱[授予使用者存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md)。


1. 按一下&#x200B;**新增**。

   使用者取得專案的檢視許可權，並作為專案團隊的一部分接收有關專案的通知。

## 從專案團隊中移除使用者

當您從使用者在專案中的角色中移除使用者時，他們仍然是專案團隊的一部分。

如果您從專案團隊中移除使用者，並且使用者被指派到專案中的任務或問題，則會從未完成的任務和問題中取消指派使用者。 在這種情況下，任務和問題返回到工作負載平衡器中的未指派工作區域。

即使您將使用者從專案團隊中移除，仍會指派給指派給已完成任務和問題的使用者。

如需有關從專案團隊移除使用者的詳細資訊，請參閱[從專案移除使用者](../../../manage-work/projects/manage-projects/remove-users-from-projects.md)。
