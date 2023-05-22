---
user-type: administrator
product-area: system-administration;user-management
keywords: 視圖，組，事件，通知，配置，啟用，禁用
navigation-topic: create-and-manage-groups
title: 查看和配置組的事件通知
description: 作為組管理員，您可以查看為您管理的組激活的事件通知。 此外，如果Adobe Workfront管理員解鎖事件通知，您可以為您管理的頂級組配置該通知。 事件通知的配置包括激活或停用它。
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: a815aeb1-3403-4491-a8ad-7e47c519905c
source-git-commit: 0e8f8973ad4c1310b973bae4e6fe3578c05db204
workflow-type: tm+mt
source-wordcount: '566'
ht-degree: 0%

---

# 查看和配置組的事件通知

作為組管理員，您可以查看為您管理的組激活的事件通知。

此外，如果Adobe Workfront管理員解鎖事件通知，您可以為您管理的頂級組配置該通知。 事件通知的配置包括激活或停用它。

Workfront管理員也可以為任何組執行此操作。

為組配置事件通知會影響該組或其子組之一是其「主組」的用戶。 在用戶配置檔案中，這些用戶將看到為其家庭組激活的事件通知，而不是在系統範圍內激活的事件通知。

有關Workfront管理員如何解鎖事件通知的資訊，請參見 [解鎖或鎖定所有組的事件通知的配置](../../../administration-and-setup/manage-workfront/emails/unlock-configuration-of-event-notifications-for-groups.md)。

有關事件的預設通知設定的資訊，請參閱 [在Adobe Workfront提供事件通知](../../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md)。

## 訪問要求

要執行本文中的步驟，必須具備以下條件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront計畫</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront許可證*</td> 
   <td> <p>計劃 </p> <p>您必須是組的組管理員或Workfront管理員。 有關詳細資訊，請參見 <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">組管理員</a> 和 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予用戶完全管理訪問權限</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;如果您需要瞭解您擁有的計畫或許可證類型，請與Workfront管理員聯繫。

## 查看和配置組的事件通知

1. （有條件和可選）如果您是Workfront的管理員，並且您已經在「電子郵件通知」頁（「設定」>「電子郵件」>「通知」）中，您可以執行以下操作，然後跳至步驟6:刪除 **系統事件通知** 在清單上方的框中，開始在框中鍵入組的名稱，然後在出現時按一下它。
1. 按一下 **主菜單** 表徵圖 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **設定** ![](assets/gear-icon-settings.png)。

1. 在左面板中，按一下 **組** ![](assets/groups-icon.png)。

1. 按一下頂級組的名稱。
1. 在左菜單中，按一下 **事件通知**。

   在顯示的清單中， **活動** 左側的列顯示組中哪些通知處於活動狀態（藍色）和非活動狀態（灰色）。

1. 要激活或停用未鎖定的事件通知，請執行以下操作：按一下 <strong>活動</strong> 列以激活 <img src="assets/email-notification-enabled-unlocked.png"> 停用 <img src="assets/email-notification-disabled-unlocked.png"> 它。

   >[!INFO]
   >
   >**示例：** 您可以配置下面顯示的已解鎖組的前兩個市場營銷組事件通知。</p> <p> <img src="assets/configure-group-event-notifications.png">
   >* 如果 <strong>活動</strong> 列灰色且灰色 <img src="assets/email-notification-disabled-locked.png">，事件通知已停用，因為所有用戶和組管理員都無法激活它或編輯其電子郵件主題行
   >* 如果 <strong>活動</strong> 列為灰色且未灰顯 <img src="assets/email-notification-disabled-unlocked.png">，事件通知為 <strong>已停用，</strong> 組管理員可以為其組激活它。
   >* 如果 <strong>活動</strong> 列藍色且灰色 <img src="assets/email-notification-enabled-locked.png">，已為所有用戶激活事件通知，並且組管理員無法停用事件通知或編輯其組的電子郵件主題行。
   >* 如果 <strong>活動</strong> 列為藍色且不灰顯 <img src="assets/email-notification-enabled-unlocked.png">，事件通知為 <strong>已激活</strong> 組管理員可以為其組停用它。


<!--
This step (with substeps) is for functionality from a Sprint 3 2021 story that got put on hold. Also see the PDF on the story for some text earlier in the article that needs to be added. 

1. To customize the email subject line of an event notification,
  1. Click the name of the event notification.
  1. In the <strong>Event Notification</strong> box that displays, in the <strong>Email Subject Line</strong> box, change the text and fields, including custom fields, then click <strong>Update</strong> to save the new subject lines for your emails.
  IMPORTANT: The names of the fields added must match the camel case syntax of our database structure. For more information about how our objects and their fields are named in the Workfront database, see the <a href="../../../wf-api/workfront-api.md" class="MCXref xref">Adobe Workfront API</a>.
  For more information about customizing the email subject line of an event notification, see <a href="../../../administration-and-setup/manage-workfront/emails/custom-email-subjects-event-notification.md" class="MCXref xref">Customize email subjects for event notifications</a>. 
-->

