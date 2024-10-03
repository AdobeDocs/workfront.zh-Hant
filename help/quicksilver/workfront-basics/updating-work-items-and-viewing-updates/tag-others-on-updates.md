---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: 標籤其他更新的專案
description: 在Adobe Workfront物件上提供更新註解時，專案上的所有使用者都可以看到提交的資訊。 不過，有時候，不在專案中的使用者可以從檢視此資訊中獲益。 您可以在更新中標籤這些使用者，以便與他們共用，而不將他們包含在專案中。 標籤的使用者會收到事件通知。
author: Alina
feature: Get Started with Workfront
exl-id: c4c0d74f-ac50-4fc5-89d6-28f004c25b29
source-git-commit: 1eb1e919bede7e366956d8c0bd969329a641123f
workflow-type: tm+mt
source-wordcount: '1008'
ht-degree: 0%

---

# 標籤其他人的更新

<!--Audited: April, 2024-->

<!--
>[!IMPORTANT]
>
>We are currently redesigning the commenting experience in Adobe Workfront.
>
>Depending on what objects you access the commenting experience for, you might see the following functionality for the Updates section:
>* The new experience
>* The legacy experience
>* The new and the legacy experience
>
>For more information about the new commenting experience and its availability, see [New commenting experience](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md). 
>
><Span class="preview"> The legacy commenting experience has been removed from projects, tasks, issues, and documents in the Preview environment. </span>
>
>The new commenting experience is available only for the Updates section of Workfront objects, and it is not available when you access updates from the following areas:
>
> * Home
> * Summary panel in lists
> * Summary panel in timesheets 
> * Summary panel in the Workload Balancer
>
><span class="preview">The new commenting experience is available in the Summary panel in lists, timesheets, and the Workload Balancer in the Preview environment and in the Production environment for customers who have opted for the fast release process. </span> 
-->

如果您想要吸引使用者注意某個物件，而他們可能不會關注該物件，則可以在更新物件時標籤使用者。

您不可以透過將使用者指派給物件或讓使用者訂閱物件來將他們包含在物件上，而是在更新時標籤他們，以便與他們共用。 標籤的使用者會收到有關您輸入之更新的Workfront通知。 根據他們的通知設定，他們也會收到有關您輸入之更新的電子郵件。

## 在更新中標籤使用者的相關考量事項

* 在更新中被標籤的使用者必須在他們的設定檔中啟用個人通知，以便他們接收電子郵件通知。 如需詳細資訊，請參閱[修改您自己的電子郵件通知](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md)。

  如需新增更新至Workfront物件的詳細資訊，請參閱[更新工作](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md)。

* 當問題轉換為專案或任務時，更新會複製到新專案或任務，但標籤的使用者不會。 若要繼續交談，您必須再次標籤參與者。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront計畫</strong></td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront授權*</strong></td> 
   <td> <p>新增：問題和檔案的貢獻者或更高；所有其他物件的淺色或更高</p>
   <p>目前：問題與檔案的要求或更高；所有其他物件的檢閱或更高</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>存取層級設定</strong></td> 
   <td> <p>檢視您想要張貼回覆之物件的存取權或更高的存取權</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>物件許可權</strong></td> 
   <td> <p>檢視您要張貼回覆之物件的或更高許可權</p> </td> 
  </tr> 
 </tbody> 
</table>

*若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的Workfront管理員。 如需詳細資訊，請參閱[Workfront檔案的存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 標籤其他人的更新

您可以透過下列方式，在更新中標籤其他人：

* **自動**：當使用者啟動對話串、新增註解或新增回覆時，系統會自動標籤他們，並將其新增至註解方塊的「標籤人員」或「團隊」區域。
* **手動**：當您手動將使用者新增到評論方塊的[標籤人員]區域時。

您也可以在編輯或回複評論時，移除被錯誤標籤的使用者。

1. 開始更新工作專案，如[更新工作](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md)中所述。 您身為註解擁有者，會自動被標籤並新增至註解方塊的「標籤人員」或「團隊」區域。

   >[!TIP]
   >
   >評論擁有者在評論方塊的「標籤人員」或「團隊」區域中看不到自己的名稱。

1. 在&#x200B;**標籤人員或團隊**&#x200B;欄位中，開始輸入您要包含的使用者或團隊名稱，然後在其出現在下拉式清單中時按一下該名稱。

   或

   在&#x200B;**撰寫註解**&#x200B;區域輸入@符號，開始輸入您要在更新中包含的使用者或團隊名稱，然後當名稱出現在下拉式清單中時按一下該名稱。

   >[!TIP]
   > 
   >當存在具有類似或相同名稱的使用者時，若要識別正確的使用者，請注意顯示圖片、使用者的主要角色或其電子郵件地址。
   > 
   >使用者必須至少與一個工作角色相關聯，才能在更新中標籤他們時檢視該工作角色。
   > 
   >您必須在存取層級中啟用檢視聯絡資訊設定，使用者才能檢視使用者的電子郵件。 如需詳細資訊，請參閱[授予使用者存取權](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md)。

   ![標籤使用者](assets/tag-others-unified-commenting-with-all-tab.png)

1. （選擇性）若要將更新設為私人，請在更新方塊的右下角啟用&#x200B;**我的公司私有**。 這可讓貴公司的使用者看到更新。 **我的公司私有**&#x200B;選項只有在您的Workfront設定檔中指定了公司時才可用。

   >[!NOTE]
   >
   >* 只有在使用者與公司相關聯時，才會顯示此選項。
   >* 公司外部的已標籤使用者仍可收到應用程式內通知或電子郵件，即使他們不會在更新索引標籤上看到私人評論。 如果您不想與外部使用者共用資訊，建議不要在更新時標籤這些使用者。

1. （選用）若要新增多個使用者和團隊，請重複步驟2。<!--insure this stays accurate-->

   >[!NOTE]
   >
   >「標籤人員或團隊」欄位中列出的所有使用者和團隊成員都會收到更新的應用程式內通知，且可能會收到電子郵件，具體取決於其電子郵件通知設定的設定。 在評論或回覆中標籤自己的使用者會收到該評論或回覆的通知，並可以在中看到他們的名稱被列為對話串剩餘部分的成員，但他們不會收到另一個通知，除非他們再次標籤自己。 如需詳細資訊，請參閱[修改您自己的電子郵件通知](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md)和[設定系統中每個人的事件通知](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md)。

1. 按一下&#x200B;**提交**。\
   更新中包含的使用者會自動被授予物件的檢視許可權，而且可以檢視和回應對物件所做的更新。

   標籤實體的名稱會顯示在其頭像旁，最多兩個實體。 如果標籤了兩個以上的實體，除了會標籤多少個其他實體外，還會顯示第一個實體的名稱。

   ![](assets/members-icons-expanded-unshimmed.png)

   當您在註解文字中被標籤時，您的名稱會在這些註解中反白顯示。

   如需有關更新工作專案時可用的其他功能的資訊，請參閱[更新工作](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md)。

1. （選擇性）按一下評論右上角的&#x200B;**更多**&#x200B;功能表![](assets/more-menu.png)，然後按一下&#x200B;**編輯**。 移除所有已標籤的使用者，然後按一下&#x200B;**提交**。

   >[!IMPORTANT]
   >
   >您只能在輸入註解後15分鐘內進行編輯。 您只能編輯您新增的註解。


<!--
   >[!TIP]
   >
   >When using the legacy commenting experience to add comments and replies, comment owners that were not specifically tagged cannot be manually removed by people who use the new commenting experience.
-->

<!--
### Tag others on updates in the legacy Updates section

You can manually tag users in the legacy Updates section. 

1. Begin updating a work item, as described in [Update work](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
1. In the **Notify** field, begin typing the name of the user or team you want to include, then click the name when it appears in the drop-down list.

   Or

   Type the @ symbol in the **Start a new update** area, begin typing the name of the user or team you want to include on the update, then click the name when it appears in the drop-down list.

   >[!TIP]
   >
   >To identify the correct user when there are users with similar or identical names, notice the avatar, the user's Primary Role, or their email address. 
   >
   >Users must be associated with at least one job role to view it as you tag them in an update. 
   >
   >You must have the View Contact Info setting enabled in your access level for Users to view users' emails. For information, see [Grant access to users](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

   ![](assets/tag-users-in-update.png)

1. (Optional) To make the update private, enable **Private to my company** in the lower-right corner of the update box. This makes the update visible just to users in your company. The **Private to my company** option is available only when a Company is specified in your Workfront profile. 

   >[!NOTE]
   >
   >Tagged users outside the company could still receive an in-app notification or email, even though they will not see the private comments on the Updates tab. We recommend not to tag external users on an update if you do not want to share the information with them.  

1. (Optional) To add multiple users and teams, repeat step 2.

   >[!NOTE]
   >
   >All users and team members listed in the Notify field receive an in-app notification for the update and might receive an email, depending on the configuration of their email notification settings. Users who tag themselves in a comment or reply receive a notification for that comment or reply and can see their name in the Notify field for the remainder of the thread, but they do not receive another notification unless they tag themselves again. For more information, see [Modify your own email notifications](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md) and [Configure event notifications for everyone in the system](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

1. Click **Update**.  
   Users included in the update are automatically granted View permission to the object and can view and respond to updates made to the object.

   You can see who has been tagged in each reply at the top of the update thread. These users, along with any users subscribed to the object, receive a notification whenever an update or reply is made on the object.

   ![](assets/tagging-transparency-350x192.png)
-->

如需有關更新工作專案時可用的其他功能的資訊，請參閱[更新工作](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md)。



