---
title: 刪除使用者
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: 當使用者離開您的組織時，可以將該使用者從Workfront中移除，不過我們建議您停用使用者，而非刪除使用者。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: da57dea3-082b-4a86-ae13-5bf55401122e
source-git-commit: c71c5c4a545f9256ecce123ae3513d01a7251ad7
workflow-type: tm+mt
source-wordcount: '93'
ht-degree: 3%

---

# 刪除使用者

<!--DELETE ME MARCH 2026-->

>[!IMPORTANT]
>
>此頁面上說明的程式已移除，因為它僅適用於尚未上線至Adobe Admin Console的組織。
>
>所有Workfront組織現在都已上線Adobe Admin Console。
>
>  如需在Adobe Admin Console中刪除使用者的指示，請參閱[個別管理使用者](https://helpx.adobe.com/tw/enterprise/using/manage-users-individually.html)一文中的「永久刪除使用者」一節，或連絡您的Adobe Admin Console管理員。

<!--When a user leaves your organization, you can remove that user from Adobe Workfront.

>[!IMPORTANT]
>
>Deleting a user from the system also deletes information associated with the user that you might want to retain. We recommend deactivating users instead of deleting them. For more information, see [Deactivate or reactivate a user](../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md).-->
<!--
>* The procedure described on this page applies only to organizations that have not yet been onboarded to the Admin Console. If your organization has been onboarded to the Adobe Admin Console, you must perform this action through the Adobe Admin Console.
>
>Deleting a user from the [!DNL Adobe Admin Console] deactivates the user in [!DNL Workfront], but does not delete them from [!DNL Workfront].
>
>  For instructions on deleting a user in the Adobe Admin Console, see the section "Permanently delete users" in the article [Manage users individually](https://helpx.adobe.com/enterprise/using/manage-users-individually.html) or contact your Adobe Admin Console Administrator.
>
>  For a list of procedures that differ based on whether your organization has been onboarded to the Adobe Admin Console, see [Platform-based administration differences (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).
>
-->

<!--## Access requirements

+++ Expand to view access requirements for the functionality in this article.

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td><p>New: Standard</p><p>Or</p><p>Current: Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>You must have one of the following:</p> 
    <ul> 
     <li> <p>The System Administrator access level. </li> 
     <li> <p><b>Users</b> setting in your access level configured to <b>Edit</b> access, with <b>Create</b> and at least one of the two <b>User Admin</b> options enabled under <b>Fine-tune your settings</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>Of these two options, if <b>User Admin (Group Users)</b> is enabled, you must be a group administrator of a group where the user is a member.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Deleting vs. deactivating a user

Deactivating a user causes the following things to happen:

* Removes the user's licenses to both Workfront and Workfront Proof if the Workfront Proof component is associated with your Workfront account. For more information about Workfront Proof, see [Workfront Proof: article index](../../../workfront-proof/workfront-proof.md).
* The user can no longer be assigned work.
* The user can no longer be added to updates.
* The user can no longer be added to teams or groups.
* Objects can no longer be shared with the user.
* Their association with the following objects remains intact:

   * Tasks, issues, projects, portfolios
   * Dashboards

     >[!NOTE]
     >
     >If you deactivate a user and can no longer view the reports or dashboards associated with a user, you may need to update the **Run this report with the Access Rights of:** field.  
     >To learn more, see the [Why can't I access a report owned by a deactivated user?](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md#why) section of the [Reports FAQs](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md) article.

   * Documents
   * Updates
   * Hours

* If the user has checked-out documents, the documents remain checked out when you deactivate them. Only a Workfront administrator can check them back in. For more information about checking out documents, see [Check out documents](../../../documents/managing-documents/check-out-documents.md).

Deleting a user causes the following things to happen:

* Removes the user's licenses to both Workfront and Workfront Proof, if the Workfront Proof component is associated with your Workfront account. For more information about Workfront Proof, see [Workfront Proof: article index](../../../workfront-proof/workfront-proof.md).
* The user can no longer be assigned work.
* The user can no longer be added to updates.
* The user can no longer be added to teams or groups.
* Objects can no longer be shared with the user.
* Deletes the association of that user with the following objects:

   * Tasks, issues, projects, portfolio
   * Dashboards

     >[!NOTE]
     >
     >You also lose access to custom sections that contained dashboards associated to the deleted user.  
     >To learn more, see the [How do I access a dashboard that contains a report owned by a deleted user?](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md#how) section of the [Reports FAQs](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md) article.

   * Updates
   * Hours

     >[!NOTE]
     >
     >These objects remain in Workfront but the owner of the object is now blank.

* If the user uploaded any documents under the Documents area in the Global Navigation Bar, the documents are also deleted.
* If the user has checked out documents that they own and the documents are uploaded in the main Documents area (accessed from the Main Menu), the documents are deleted with the user. For more information about checking out documents, see [Check out documents](../../../documents/managing-documents/check-out-documents.md).

For more information about deactivating users, see [Deactivate or reactivate a user](../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md).

You can permanently delete users one at a time, or you can permanently delete multiple users simultaneously. When you delete individual users, you must wait for the deletion process to complete prior to moving on to other activities in Workfront. The process of deleting multiple users simultaneously runs as a background process, so you can continue using Workfront as the users are deleted.

## Delete one or more users

{{step-1-to-users}}

1. Select at least one user that you want to delete, click the More menu ![More icon](assets/more-icon.png), then click **Delete**.
1. In the box that appears, click **Delete** to confirm the deletion.

   The process of deleting users runs as a background process, so you can continue using Workfront as the user or users are deleted.

   Depending on the number of users you are deleting, the process can take several minutes or even a few hours.

   After receiving the confirmation in Workfront that the users were deleted, you might continue to see them in the system until the deletion process is complete in the background.

   At a later time, if you discover that one or more users were not successfully deleted, try to delete them one at a time.-->
