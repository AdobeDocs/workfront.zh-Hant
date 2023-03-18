---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: 在更新時標籤其他人
description: 在Adobe Workfront物件上提供更新註解時，專案上的所有使用者都能查看已提交的資訊。 不過，有時候不在專案的使用者可能會受益於檢視此資訊。 您可以在更新中標籤使用者，以便與他們共用，而不是將這些使用者納入專案。 標籤的使用者會收到事件通知。
author: Lisa and Alina
feature: Get Started with Workfront
exl-id: c4c0d74f-ac50-4fc5-89d6-28f004c25b29
source-git-commit: ba1d8d5a23da7e252e8c182a6bdb1cdd1e304eab
workflow-type: tm+mt
source-wordcount: '773'
ht-degree: 0%

---

# 在更新時標籤其他人

<!--take "Beta" references out when we remove the beta-->

<!-- Drafted for commenting experience: 

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment.</span> 

>[!NOTE]
>
>We are currently redesigning the commenting experience in Adobe Workfront.
>For more information about the new updating experience, see [New commenting experience](../updating-work-items-and-viewing-updates/unified-commenting-experience.md). 
>
>You can access the new design for the following objects:
> * <span class="preview">Issues, when enabling the commenting Beta. </span>
> * Goals
>   The new commenting experience is the default for goals. You must have an additional license to access Workfront Goals. For more information, see [Requirements to uses Workfront Goals](../../workfront-goals/goal-management/access-needed-for-wf-goals.md). 

-->
如果您想要吸引使用者注意他們可能不會關注的物件，則可在對物件進行更新時標籤使用者。
您可以將這些使用者指派給物件或讓他們訂閱物件，以便將其納入物件上，您可以在更新時標籤他們，以便與他們共用物件。 已標籤的使用者會收到您所輸入更新的相關通知。

>[!NOTE]
>
>必須啟用事件通知，使用者才能收到電子郵件通知。 管理員可以為整個系統或頂層組啟用通知。 使用者也可以在自己的使用者設定檔中啟用和停用個別事件通知。 如需詳細資訊，請參閱下列內容：
>
>* [為系統中的每個人配置事件通知](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).
>* [檢視及設定群組的事件通知](../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md)
>* [啟用或停用您自己的事件通知](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).
>


如需將更新新增至Workfront物件的相關資訊，請參閱 [更新工作](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

>[!NOTE]
>
>將問題轉換為項目或任務時，更新將複製到新項目或任務，但標籤的用戶不會。 要繼續對話，必須再次標籤參與者。

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront計畫*</strong></td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront授權*</strong></td> 
   <td> <p>要求或更高的問題和檔案；查看其他所有對象的或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>訪問級別配置*</strong></td> 
   <td> <p>（二）申請事項和檔案的申請人或以上人員；所有其他對象的審閱者或更高版本</p> <p>注意：如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>物件權限</strong></td> 
   <td> <p>檢視物件的存取權</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 在更新時標籤其他人

<!--
Tagging others in an update differs depending on which experience and which object you select.

### Tag others on updates in the current Updates section
-->

1. 開始更新工作項，如 [更新工作](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
1. 在 **通知** 欄位中，開始鍵入要包括的用戶或組的名稱，然後在下拉清單中出現名稱時按一下該名稱。

   或

   在 **開始新更新** 區域中，開始鍵入要包括在更新中的用戶或組的名稱，然後在名稱出現在下拉清單中時按一下該名稱。

   >[!TIP]
   >
   >若要在有名稱類似或相同的使用者時識別正確的使用者，請注意頭像、使用者的主要角色或其電子郵件地址。 用戶必須至少與一個作業角色關聯，才能在您在更新中對其進行標籤時查看該角色。

   ![](assets/tag-users-in-update.png)

1. （選用）若要將更新設為私人，請啟用 **對我的公司私有** （位於更新框的右下角）。 如此一來，更新就只會對您公司中的使用者顯示。

   >[!NOTE]
   >
   >公司外部的已標籤使用者仍可能收到應用程式內通知或電子郵件，即使他們在「更新」索引標籤上看不到私人留言。 如果您不想與外部使用者共用資訊，建議不要在更新時標籤外部使用者。

1. （可選）若要新增多個使用者和團隊，請重複步驟2。

   >[!NOTE]
   >
   >列在「通知」欄位中的所有使用者和團隊成員都會收到更新的應用程式內通知，並且可能會收到電子郵件，具體取決於其電子郵件通知設定的配置。 在留言或回覆中標籤自己的使用者會收到該留言或回覆的通知，且在執行緒的其餘時間內，可在「通知」欄位中看到其名稱，但除非再次標籤自己，否則不會收到其他通知。 如需詳細資訊，請參閱 [啟用或停用您自己的事件通知](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md) 和 [為系統中的每個人配置事件通知](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

1. 按一下 **更新**.\
   更新中包含的用戶會自動被授予對象的「查看」權限，並且可以查看和響應對象所做的更新。

   您可以在更新執行緒頂端查看每個回覆中的標籤者。 這些使用者以及訂閱物件的任何使用者，會在物件進行更新或回覆時收到通知。

   ![](assets/tagging-transparency-350x192.png)

   有關更新工作項時可用的其他功能的資訊，請參閱 [更新工作](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

<!--
<div class="preview">

### Tag others on updates in the commenting Beta experience

1. Begin updating a work item, as described in [Update work](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
1. In the **Tag people or teams** field, begin typing the name of the user or team you want to include, then click the name when it appears in the drop-down list.

   <!- ********************* this doesn't seem to work in Beta - keep drafted for now: 
   Or

   Type the @ symbol in the **Start a new update** area, begin typing the name of the user or team you want to include on the update, then click the name when it appears in the drop-down list. ************close draft

   >[!TIP]
   >
   >To identify the correct user when there are users with similar or identical names, notice the avatar, the user's Primary Role, or their email address. Users must be associated with at least one job role to view it as you tag them in an update.

   ![](assets/tag-others-unified-commenting.png)

      <!-******************* this might not be there for issues yet - keep drafted if not: 
      1. (Optional) To make the update private, enable **Private to my company** in the lower-right corner of the update box. This makes the update visible just to users in your company.

         >[!NOTE]
         >
         >* This option displays only when the user is associated with a Company.
         >* Tagged users outside the company could still receive an in-app notification or email, even though they will not see the private comments on the Updates tab. We recommend not to tag external users on an update if you do not want to share the information with them. - ************close draft 
      
1. (Optional) To add multiple users and teams, repeat step 2.

   >[!NOTE]
   >
   >All users and team members listed in the "Tag people or teams" field receive an in-app notification for the update and might receive an email, depending on the configuration of their email notification settings. Users who tag themselves in a comment or reply receive a notification for that comment or reply and can see their name in listed as a member of the thread for the remainder of the thread, but they do not receive another notification unless they tag themselves again. For more information, see [Activate or deactivate your own event notifications](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md) and [Configure event notifications for everyone in the system](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

1. Click **Submit**.  
   Users included in the update are automatically granted View permission to the object and can view and respond to updates made to the object.

   You can see who has been tagged in each reply under the text of the update, in the Members area. These users, along with any users subscribed to the object, receive a notification whenever an update or reply is made on the object.
1. (Optional) Cick the number of members included in the update to display a list of entities that the update you entered is shared with. 

   ![](assets/members-icons-expanded-unshimmed.png)

   For information about the additional functionality that is available when updating a work item, see [Update work](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

-->