---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: 在更新時標籤其他人
description: 在Adobe Workfront物件上提供更新註解時，專案上的所有使用者都能查看已提交的資訊。 不過，有時候不在專案的使用者可能會受益於檢視此資訊。 您可以在更新中標籤使用者，以便與他們共用，而不是將這些使用者納入專案。 標籤的使用者會收到事件通知。
author: Lisa and Alina
feature: Get Started with Workfront
exl-id: c4c0d74f-ac50-4fc5-89d6-28f004c25b29
source-git-commit: 1eba586f4d3ce6db667839b0620dfeb65f6e28be
workflow-type: tm+mt
source-wordcount: '769'
ht-degree: 0%

---

# 在更新時標籤其他人

在Adobe Workfront物件上提供更新註解時，專案上的所有使用者都能查看已提交的資訊。 不過，有時候不在專案的使用者可能會受益於檢視此資訊。 您可以在更新中標籤使用者，以便與他們共用，而不是將這些使用者納入專案。 標籤的使用者會收到事件通知。

>[!NOTE]
>
>必須啟用事件通知，使用者才能收到。 管理員可以為整個系統或頂層組啟用通知。 使用者也可以在自己的使用者設定檔中啟用和停用個別事件通知。 如需詳細資訊，請參閱下列內容：
>
>* [為系統中的每個人配置事件通知](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).
>* [檢視及設定群組的事件通知](../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md)
>* [啟用或停用您自己的事件通知](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).
>


>[!NOTE]
>
>將問題轉換為項目或任務時，更新將複製到新項目或任務，但標籤的用戶不會。 要繼續對話，必須再次標籤參與者。

如需將更新新增至Workfront物件的相關資訊，請參閱 [更新工作](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

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
