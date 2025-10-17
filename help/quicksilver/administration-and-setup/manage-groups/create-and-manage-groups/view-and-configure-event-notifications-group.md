---
user-type: administrator
product-area: system-administration;user-management
keywords: 檢視，群組，事件，通知，設定，啟用，停用
navigation-topic: create-and-manage-groups
title: 檢視和設定群組的事件通知
description: 作為群組管理員，您可以檢視針對您管理的群組啟用的事件通知。 此外，如果Adobe Workfront管理員解除鎖定事件通知，您可以為您管理的最上層群組設定該通知。 事件通知的設定包含啟用或停用。
author: Becky
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: a815aeb1-3403-4491-a8ad-7e47c519905c
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '523'
ht-degree: 0%

---

# 檢視和設定群組的事件通知

作為群組管理員，您可以檢視針對您管理的群組啟用的事件通知。

此外，如果Adobe Workfront管理員解除鎖定事件通知，您可以為您管理的最上層群組設定該通知。 事件通知的設定包含啟用或停用。

Workfront管理員也可以為任何群組執行此動作。

為群組設定事件通知會影響該群組或其子群組之一為其主群組的使用者。 在其使用者設定檔中，這些使用者會看到為其主群組啟用的事件通知，而不是在整個系統內啟用的事件通知。

如需Workfront管理員如何解除鎖定事件通知的詳細資訊，請參閱[解除鎖定或鎖定所有群組的事件通知設定](../../../administration-and-setup/manage-workfront/emails/unlock-configuration-of-event-notifications-for-groups.md)。

如需事件預設通知設定的相關資訊，請參閱[事件通知型別](../../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md)。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront套件</td> 
   <td><p>任何</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront授權</td> 
   <td><p>標準</p>
       <p>規劃</p></td>
  </tr>
  <tr> 
   <td>存取層級設定</td> 
   <td>您必須是群組的群組管理員或系統管理員。</td>
  </tr>
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 檢視及設定群組的事件通知

>[!TIP]
>
>如果您是Workfront管理員，而且您已在「電子郵件通知」頁面（「設定>電子郵件>通知」），您可以執行下列動作，然後跳至步驟6：刪除清單上方方塊中的&#x200B;**系統事件通知**，開始在方塊中輸入群組名稱，然後在其出現時按一下。

{{step-1-to-setup}}

1. 在左側面板中，按一下&#x200B;**群組** ![群組](assets/groups-icon.png)。

1. 按一下最上層群組的名稱。
1. 在左側功能表中，按一下&#x200B;**事件通知**。

   在顯示的清單中，左側的&#x200B;**作用中**&#x200B;欄顯示群組的作用中（藍色）和非作用中（灰色）通知。

1. 若要啟用或停用已解除鎖定的事件通知：按一下<strong>啟用</strong>欄中的按鈕以啟用 <img src="assets/email-notification-enabled-unlocked.png">或停用 <img src="assets/email-notification-disabled-unlocked.png">它。

   >[!INFO]
   >
   >**範例：**&#x200B;您可以設定下面顯示的前兩個行銷群組事件通知，它們已為群組解除鎖定。</p> <p> <img src="assets/configure-group-event-notifications.png">
   >* 如果<strong>Active</strong>欄中的按鈕是灰色且變暗的 <img src="assets/email-notification-disabled-locked.png">，已為所有的使用者停用事件通知，群組管理員無法啟用或編輯其電子郵件主旨列
   >* 如果<strong>Active</strong>資料行中的按鈕是灰色且未變暗 <img src="assets/email-notification-disabled-unlocked.png">，事件通知已針對所有使用者<strong>停用，且</strong>群組管理員可為其群組啟用該通知。
   >* 如果<strong>Active</strong>資料行中的按鈕為藍色且變暗 <img src="assets/email-notification-enabled-locked.png">，已為所有的使用者啟用事件通知，群組管理員無法停用或編輯其群組的電子郵件主旨列。
   >* 如果<strong>Active</strong>資料行中的按鈕為藍色且未變暗 <img src="assets/email-notification-enabled-unlocked.png">，已為所有使用者<strong>啟用事件通知，且</strong>群組管理員可為其群組停用該通知。

<!--
This step (with substeps) is for functionality from a Sprint 3 2021 story that got put on hold. Also see the PDF on the story for some text earlier in the article that needs to be added. 

1. To customize the email subject line of an event notification,
  1. Click the name of the event notification.
  1. In the <strong>Event Notification</strong> box that displays, in the <strong>Email Subject Line</strong> box, change the text and fields, including custom fields, then click <strong>Update</strong> to save the new subject lines for your emails.
  IMPORTANT: The names of the fields added must match the camel case syntax of our database structure. For more information about how our objects and their fields are named in the Workfront database, see the <a href="../../../wf-api/workfront-api.md" class="MCXref xref">Adobe Workfront API</a>.
  For more information about customizing the email subject line of an event notification, see <a href="../../../administration-and-setup/manage-workfront/emails/custom-email-subjects-event-notification.md" class="MCXref xref">Customize email subjects for event notifications</a>. 
-->

