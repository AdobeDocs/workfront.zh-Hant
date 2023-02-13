---
product-area: projects;agile-and-teams
navigation-topic: plan-a-project
title: 管理專案團隊
description: 專案團隊包含與專案相關聯的使用者。 專案團隊的成員會顯示在專案的「人員」區段中。
author: Alina
feature: Work Management
exl-id: 6e8036fc-feda-4277-9502-0b973028fccb
source-git-commit: bbd64e9deed1b89d720272508b3562c354578704
workflow-type: tm+mt
source-wordcount: '658'
ht-degree: 0%

---

# 管理專案團隊

專案團隊包含與專案相關聯的使用者。 專案團隊的成員會顯示在專案的「人員」區段中。

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
   <td> <p>計劃 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>編輯專案的存取權</p> <p>檢視或更高的使用者存取權</p> <p><b>附註</b>

如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>檢視專案的或更高權限</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 新增使用者至專案團隊

將用戶添加到項目組時，他們將獲得項目的「查看」權限以及項目的任務、問題和文檔。 如需詳細資訊，請參閱文章 [專案團隊概觀](../../../manage-work/projects/planning-a-project/project-team-overview.md).

>[!TIP]
>
>項目團隊中的用戶不會自動添加到項目的資源管理工具中。

您可以透過下列方式新增使用者至專案團隊：

* [自動將使用者新增至專案團隊](#automatically-add-users-to-a-project-team)
* [手動將使用者新增至專案團隊](#manually-add-users-to-a-project-team)

### 自動將使用者新增至專案團隊 {#automatically-add-users-to-a-project-team}

在專案上履行下列角色的使用者會自動新增至專案團隊，並在建立專案時顯示在「人員」區段中：

* 項目的建立者
* 專案擁有者
* 項目贊助商

當使用者被指派給下列項目團隊時，也會自動將他們新增至專案團隊：

* 任務
* 問題

### 手動將使用者新增至專案團隊 {#manually-add-users-to-a-project-team}

如果未履行項目任何角色的用戶希望在項目期間收到某些更新或更改的通知，則可以手動將它們添加到項目組。

如需可為專案團隊的使用者啟用哪些通知的詳細資訊，請參閱 [Adobe Workfront中提供的事件通知](../../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

<!--drafted - this used to be the case, in the note below but this limitation was removed on Jan 5, 2023 - as a patch, not a release feature:

>[!IMPORTANT]
>
>You can add to the Project Team only users that belong to the Group associated with the project. You cannot add users that belong to the Subgroups of the project's group. 

-->

1. 前往您要新增使用者的專案。

1. 按一下 **人員** 中。 您可能需要按一下 **顯示更多** 第一個。

1. 按一下 **新增使用者**.

   將顯示「向項目團隊添加用戶」對話框。

   ![add_users_dialog.png](assets/add-users-dialog-350x217.png)

1. 在 **新增使用者** 框中，開始鍵入要添加到項目團隊的活動Workfront用戶的名稱，然後在下拉清單中顯示該名稱時按一下。

   重複此步驟，將多個使用者新增至專案團隊。 使用者必須屬於與專案相關聯的群組。

   >[!TIP]
   >
   >* 您無法新增其團隊、群組、公司或工作角色，以新增使用者。
   >* 新增使用者時，請注意頭像、使用者的主要角色及其電子郵件地址，以區分名稱相同的使用者。 用戶必須至少與一個作業角色關聯，才能在添加時查看該角色。



1. 按一下 **新增**.

   使用者取得專案的「檢視」權限，並在專案團隊中接收專案的相關通知。

## 從專案團隊中移除使用者

從使用者在專案中的角色中移除使用者時，使用者仍是專案團隊的一員。

如果從項目組中刪除了用戶，並且該用戶被分配給項目中的任務或問題，則從未完成的任務和問題中取消分配該用戶。 在這種情況下，任務和問題將返回到工作負載平衡器中的「未分配的工作」區域。

即使您將任務和問題從項目組中刪除，這些任務和問題仍被分配。

如需從專案團隊移除使用者的詳細資訊，請參閱 [從專案移除使用者](../../../manage-work/projects/manage-projects/remove-users-from-projects.md).
