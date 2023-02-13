---
user-type: administrator
product-area: system-administration;user-management
keywords: 檢視，群組，事件，通知，設定，啟用，停用
navigation-topic: create-and-manage-groups
title: 檢視及設定群組的事件通知
description: 身為群組管理員，您可以檢視針對您管理之群組啟動的事件通知。 此外，如果Adobe Workfront管理員解除鎖定事件通知，您可以為您管理的頂層群組進行設定。 事件通知的設定包括啟用或停用。
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: a815aeb1-3403-4491-a8ad-7e47c519905c
source-git-commit: 306d6493ff0413d5814f4aed8ab44fb897f3568d
workflow-type: tm+mt
source-wordcount: '592'
ht-degree: 0%

---

# 檢視及設定群組的事件通知

身為群組管理員，您可以檢視針對您管理之群組啟動的事件通知。

此外，如果Adobe Workfront管理員解除鎖定事件通知，您可以為您管理的頂層群組進行設定。 事件通知的設定包括啟用或停用。

Workfront管理員也可以對任何群組執行此動作。

為組配置事件通知會影響該組或其子組中的一個作為其「主組」的用戶。 這些使用者在其使用者設定檔中會看到為其首頁群組啟動的事件通知，而非為全系統啟動的事件通知。

如需Workfront管理員如何解除鎖定事件通知的詳細資訊，請參閱 [解鎖或鎖定所有組的事件通知配置](../../../administration-and-setup/manage-workfront/emails/unlock-configuration-of-event-notifications-for-groups.md).

如需事件預設通知設定的相關資訊，請參閱 [Adobe Workfront中提供的事件通知](../../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

## 存取需求

您必須具備下列條件才能執行本文所述步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">Workfront計畫</a>*</td> 
   <td> <p>Pro或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="https://one.workfront.com/s/document-item?bundleId=the-new-workfront-experience&amp;topicId=Content%2FAdministration_and_Setup%2FAdd_users%2FAccess_levels_and_object_permissions%2Fwf-licenses.html&amp;_LANG=en" target="_blank">Adobe Workfront授權</a>*</td> 
   <td> <p>計劃 </p> <p>您必須是群組的群組管理員或Workfront管理員。 如需詳細資訊，請參閱 <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">群組管理員</a> 和 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予使用者完整的管理存取權</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;如果您需要了解您擁有的計畫或授權類型，請聯絡Workfront管理員。

## 檢視及設定群組的事件通知

1. （有條件和選用）如果您是Workfront管理員，且已進入「電子郵件通知」頁面（「設定>電子郵件>通知」），您可以執行下列操作，然後跳至步驟6:刪除 **系統事件通知** 在清單上方的方塊中，開始在方塊中輸入群組名稱，然後在出現群組時按一下。
1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **設定** ![](assets/gear-icon-settings.png).

1. 在左側面板中，按一下 **群組** ![](assets/groups-icon.png).

1. 按一下頂層群組的名稱。
1. 在左側功能表中，按一下 **事件通知**.

   在顯示的清單中， **作用中** 左側欄顯示群組的哪些通知處於作用中（藍色）和非作用中（灰色）。

1. 要激活或停用解鎖事件通知，請執行以下操作：按一下 <strong>作用中</strong> 欄以啟用 <img src="assets/email-notification-enabled-unlocked.png"> 或停用 <img src="assets/email-notification-disabled-unlocked.png"> 它。

   >[!INFO]
   >
   >**範例：** 您可以設定下方顯示的針對群組解除鎖定的前兩個行銷群組事件通知。</p> <p> <img src="assets/configure-group-event-notifications.png">
   >* 若 <strong>作用中</strong> 欄為灰色和灰色 <img src="assets/email-notification-disabled-locked.png">，則會停用事件通知，因為所有使用者和群組管理員都無法啟用或編輯其電子郵件主旨行
   >* 若 <strong>作用中</strong> 欄為灰色且不灰顯 <img src="assets/email-notification-disabled-unlocked.png">，事件通知為 <strong>已停用，</strong> 群組管理員可為其群組啟用。
   >* 若 <strong>作用中</strong> 欄為藍色和灰色 <img src="assets/email-notification-enabled-locked.png">，則會為所有使用者啟用事件通知，而群組管理員無法將其停用，或為其群組編輯其電子郵件主旨行。
   >* 若 <strong>作用中</strong> 欄為藍色且不暗顯 <img src="assets/email-notification-enabled-unlocked.png">，事件通知為 <strong>已激活，</strong> 群組管理員可為其群組停用該功能。


<!--
This step (with substeps) is for functionality from a Sprint 3 2021 story that got put on hold. Also see the PDF on the story for some text earlier in the article that needs to be added. 

1. To customize the email subject line of an event notification,
  1. Click the name of the event notification.
  1. In the <strong>Event Notification</strong> box that displays, in the <strong>Email Subject Line</strong> box, change the text and fields, including custom fields, then click <strong>Update</strong> to save the new subject lines for your emails.
  IMPORTANT: The names of the fields added must match the camel case syntax of our database structure. For more information about how our objects and their fields are named in the Workfront database, see the <a href="../../../wf-api/workfront-api.md" class="MCXref xref">Adobe Workfront API</a>.
  For more information about customizing the email subject line of an event notification, see <a href="../../../administration-and-setup/manage-workfront/emails/custom-email-subjects-event-notification.md" class="MCXref xref">Customize email subjects for event notifications</a>. 
-->

