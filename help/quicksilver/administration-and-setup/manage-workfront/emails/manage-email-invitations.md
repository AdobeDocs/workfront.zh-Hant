---
user-type: administrator
product-area: system-administration
navigation-topic: emails-administration
title: 管理新使用者的電子郵件邀請
description: 身為Adobe Workfront管理員，您可以使用電子郵件邀請將使用者新增至Workfront，並通知他們已新增。
author: Courtney
feature: System Setup and Administration
role: Admin
exl-id: e13e3479-391f-4aec-b998-e9b6057f256b
TQID: 'https://experienceleague.adobe.com/ccjCkwwEkjdK-ENjZWEUmqlhhRan7eqRa8VjJbuIaMo'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
  - id: d5896d07-2812-5418-8b18-8957a0d7f0fb
    internal-label: System Setup and Administration
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
topic_v2:
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
    internal-label: Security
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: e7123179a59cd7ed9c76f4718b3b8019854cbfe1
workflow-type: tm+mt
source-wordcount: '98'
ht-degree: 6%
---
# 管理新使用者的電子郵件邀請

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">*** DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

>[!IMPORTANT]
>
>本頁所述的程式僅適用於尚未加入Admin Console的組織。 由於所有組織都已上線至Adobe Admin Console，因此使用者會透過Adobe Admin Console新增。
>
>如需相關資訊與指示，請參閱在Adobe Admin Console中管理使用者一文中的[使用Adobe Admin Console在Workfront中建立使用者](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/admin-console.md)。

<!--

As an Adobe Workfront administrator, you can add users to Workfront and notify them that they have been added, by using email invitations.

The email invitation allows new users to follow a link where they can choose a password for their Workfront account. They can then finish setting up their account.

To ensure the security of the new accounts, we recommend that you use email invitations for your new users, so they can choose their own password. Alternatively, you can also select a password for a new user when creating their account. For more information about adding new users to Workfront, see [Add users](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

You can configure the new user emails for:

* Any new user added to Workfront
* Users added to Workfront with a Requestor license

All new users see the same email when an email invitation is sent.

For information about receiving email invitations, see [Receive email invitations and create a password for Adobe Workfront](../../../workfront-basics/manage-your-account-and-profile/managing-your-workfront-account/receive-email-invitations.md).

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td>
   <p>Standard</p>
   <p>Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>System administrator</p> </td> 
  </tr> 
 </tbody> 
</table>

For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

+++

## Resend email invitations to existing unregistered users

Email invitations are generated in the following scenarios:

* When you create a new user and you select the **Send an invite email to this person** on the **New User** form. For more information about creating new users, see [Add users](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).
* When you import multiple new users and you select the **Send invite emails to these people** option. For more information about importing several new users, see [Import users](../../../administration-and-setup/add-users/create-and-manage-users/import-users.md).
* After the users are created, you can manually generate the invitations to users who have not yet registered their account with Workfront, and they have not established a Workfront password.  
  Users who have an account created but have not yet registered their account are marked as **Unregistered** in Workfront.

  >[!NOTE]
  >
  >If you deselect the **Send an email invite to this person** box when you create the user, the email invitation cannot be generated manually. Resending the email invitations manually is only possible for users who have been sent the original email invitation when their account was created. For more information about creating new users, see [Add users](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

To manually resend email invitations to existing unregistered users:

{{step-1-to-users}} 

1. Select the user who shows the **Unregistered** label after their name.

   ![Unregistered](assets/unreg-user-qs-350x221.png)

1. Click the More icon ![More icon](assets/more-icon.png), then click **Remind user to register**.

   An email invitation is sent to the new user with a new link they can use to create their Workfront password.

   >[!NOTE]
   >
   >If your organization has been onboarded to the Admin Console and you add a user through Workfront, you do not have the option to send an email invitation to new users.
   >
   >New Adobe users are added to the Admin Console, and the Admin Console delivers an email to invite them to complete the registration process. All users must complete the registration process to access any Adobe system.
   >
   >For existing Adobe users, the user may or may not receive an email about Workfront being available. This is a preference controlled by the Adobe administrator for the product.

## Configure email invitations {#configure-email-invitations}

As a Workfront administrator, you can configure the message you include with the email invitations for new users.

{{step-1-to-setup}}

1. In the list on the left, click **Email** > **Invitations**.

1. In the **General Options** section, make any of the following modifications:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Deactivate invitation links after ... days</strong> </td> 
      <td> <p>Choose the amount of time after which the email invitations no longer contain a valid link to Workfront. The default amount of days is 45.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Include a message and/ or term of service</strong> </td> 
      <td> <p>Select this option if you want to modify the email invitation for all new users added to Workfront. This does not include users with a Requestor license.</p> 
       <ul> 
        <li><strong>Message</strong>: If you select to modify the email invitation for all new users, specify the text that you want to include in your email invitations as the email body.</li> 
        <li><strong>Terms and Conditions</strong>: If you select to modify the email invitation for all new users, specify the text that you want to include in your email invitations as the terms and conditions.<br></li> 
        <li><strong>Include a message and/or term of service for helpdesk users</strong>: Select this option if you want to modify the email invitation for all new users added to Workfront that have a Requestor license.</li> 
        <li><strong>Message</strong>: If you select to modify the email invitation for all new users with a Requestor license, specify the text that you want to include in your email invitations as the email body.</li> 
        <li><strong>Terms and Conditions</strong>: If you select to modify the email invitation for all new users with a Requestor license, specify the text that you want to include in your email invitations as the terms and conditions.<br></li> 
        <li> <p>In the <strong>Invitation Preview</strong> section, you can see a preview of your email invitation. If you selected to include a customized message in your email invitation, the customized message shows in this area.</p> <p> <img src="assets/email-invitation-for-all-users-preview-qs-350x190.png" style="width: 350;height: 190;"> </p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. Click **Save**.
-->

