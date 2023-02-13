---
product-area: projects;user-management
navigation-topic: manage-projects
title: 從專案移除使用者
description: 當使用者不再參與完成專案的工作時，您可以將使用者從專案中移除。
author: Alina
feature: Work Management
exl-id: 3a75c78d-faed-41cd-a0a4-59504bb981af
source-git-commit: 301c86152340a184345bd39cec77fdcf28258196
workflow-type: tm+mt
source-wordcount: '573'
ht-degree: 0%

---

# 從專案移除使用者

當使用者不再參與完成專案的工作時，您可以將使用者從專案中移除。 從項目中刪除用戶會影響任務和問題分配以及項目角色。 已移除使用者，停止接收專案團隊專屬的通知。 如需專案團隊通知的詳細資訊，請參閱 [Adobe Workfront中提供的事件通知](../../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

與專案相關聯的使用者會列在專案的「人員」區域中。 他們代表專案團隊。 如需專案團隊的詳細資訊，請參閱 [專案團隊概觀](../../../manage-work/projects/planning-a-project/project-team-overview.md).

## 存取需求

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
   <td> <p>編輯專案的存取權</p> <p><b>附註</b>

如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>管理專案的權限</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 移除使用者會如何影響現有工作、問題和專案

從項目中刪除用戶時，分配給他們的任何任務或問題都可能受到影響，具體取決於刪除用戶時是否已完成任務或問題：

* **如果移除使用者時未完成項目：** 如果已分配了作業角色，則重新將該項目分配給作業角色，或者將其分配給用戶在項目上履行的作業角色。 如果項目或用戶未分配作業角色，則必須手動重新分配項目。
* **如果移除使用者時項目已完成：** 移除的使用者名稱仍保留在項目上。
* **如果移除的使用者也是專案的建立者：** 專案不會從 **正在執行的項目** 清單。 系統會從清單中移除所有其他使用者的專案，這些使用者會依「輸入者」欄位來篩選該專案。
* **如果用戶是項目所有者或贊助商：** 使用者仍擔任專案的贊助者或擁有者。

## 從專案和專案團隊移除使用者

您可以從專案團隊中移除使用者，以從專案中移除使用者。

當使用者履行專案的角色時，就會成為專案團隊的一員。

從使用者在專案中的角色中移除使用者時，使用者仍是專案團隊的一員。

如需使用者在專案上的角色的相關資訊，請參閱 [管理專案團隊](../planning-a-project/manage-project-team.md).

要從項目組中刪除用戶，請執行以下操作：

1. 前往您要移除使用者的專案。

1. 按一下 **人員** 在左側面板中，選取您要移除的使用者。 您可能需要按一下 **顯示更多**，然後 **人員**.

1. 按一下 **移除** 圖示  ![移除項目](assets/remove-icon---x-in-circle.png) ，即可取得Advertising Cloud的說明。

1. 按一下 **是，刪除選定用戶** 確認刪除。

   系統會從專案團隊和任何可能指派給的未完成任務或問題中移除使用者。 他們不再收到專案團隊的通知。
