---
title: 授予使用者完整管理存取權
description: 您可以授予使用者Workfront的完整管理存取權。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 46bcb65a-1cb7-443b-88ba-6d0e516e3050
source-git-commit: c71c5c4a545f9256ecce123ae3513d01a7251ad7
workflow-type: tm+mt
source-wordcount: '78'
ht-degree: 0%

---

# 授予使用者完整管理存取權

<!--Audited: 12/2024-->

<!--DELETE ME MARCH 2026-->

>[!IMPORTANT]
>
>此頁面上說明的程式已移除，因為它僅適用於尚未上線至Adobe Admin Console的組織。
>
>所有Workfront組織現在都已上線Adobe Admin Console。
>
>如需在Adobe Admin Console中授與完整管理員存取權的指示，請參閱[在Adobe Admin Console中管理使用者](../../../administration-and-setup/add-users/create-and-manage-users/admin-console.md)。

<!--As an Adobe Workfront administrator, you can create another Workfront administrator by assigning them the System Administrator access level. A user with this access level has full administrative access to everything in Workfront, including items they did not create themselves.

>[!NOTE]
>
>This is different from using an access level to grant users administrative access to certain areas of the system. For more information, see the following:
>
>* [Grant users administrative access to certain areas](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md) 
>* [Access of a Workfront administrator vs. access of a Plan user with administrative rights](#access-of-a-workfront-administrator-vs-access-of-a-plan-user-with-administrative-rights) in this article
>

## Access requirements

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
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>New: Standard</p>
   <p>Current: Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>You must be a Workfront administrator. </td> 
  </tr> 
 </tbody> 
</table>

*For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 
+++

## Grant full System Administrator access to a single user

{{step-1-to-users}} 

1. Click the name of the user to whom you want to grant administrator rights.
1. Click the **More** menu ![](assets/more-icon.png) to the right of the user name, then click **Edit**.  

   The **Edit Person** box displays. 
1. Click **Access** in the left panel.
1. In the **Access level** drop-down list, select the **System Administrator** access level.

   Depending on changes made in your system, the name of this access level might have changed.

1. Click **Save Changes.**

   The user now has full System Administrator rights in the system.

## Access of a Workfront administrator vs. access of a Plan user with administrative rights  {#access-of-a-workfront-administrator-vs-access-of-a-plan-user-with-administrative-rights}

The two tables below show the difference between the access rights of a user with a Workfront System Administrator access level versus those of a user with a Plan license with some administrative rights.

Workfront administrators can view all the objects in the system (regardless of who created them), create new ones, and modify or delete existing ones. They have full access to all objects in the system.

Users with a Plan license who can edit functionality in one area have full access to the functionality in that area.

>[!NOTE]
>
>Users with a Plan license who are designated as group administrators can perform some of the actions allowed for Workfront administrators. They are allowed to perform these actions only for the groups they administer, their subgroups, and the users in these groups and subgroups. For more information, see [Group administrators](../../../administration-and-setup/manage-groups/group-roles/group-administrators.md).

* [Access to the Setup area](#access-to-the-setup-area)
* [Access to objects](#access-to-objects)

### Access to the Setup area {#access-to-the-setup-area}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Area/object</th> 
   <th>Workfront administrator </th> 
   <th>User with a Plan license and some administrative rights</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Project Preferences: Projects</td> 
   <td>Full access</td> 
   <td>No access</td> 
  </tr> 
  <tr> 
   <td>Project Preferences: Tasks &amp; Issues</td> 
   <td>Full access</td> 
   <td>No access</td> 
  </tr> 
  <tr> 
   <td>Project Preferences: Statuses</td> 
   <td>Full access</td> 
   <td> <p>No access</p> </td> 
  </tr> 
  <tr> 
   <td>Project Preferences: Priorities</td> 
   <td>Full access</td> 
   <td>No access</td> 
  </tr> 
  <tr> 
   <td>Project Preferences: Severities</td> 
   <td>Full access</td> 
   <td>No access</td> 
  </tr> 
  <tr> 
   <td>Project Preferences: Exchange Rates</td> 
   <td>Full access</td> 
   <td>Full access</td> 
  </tr> 
  <tr> 
   <td>Processes: Approvals</td> 
   <td> <p>Full access</p> </td> 
   <td>Full access</td> 
  </tr> 
  <tr> 
   <td>Processes: Milestone Paths</td> 
   <td>Full access</td> 
   <td>Full access</td> 
  </tr> 
  <tr> 
   <td>Custom Forms</td> 
   <td>Full access</td> 
   <td> <p>Manage custom forms they created or custom forms shared with them.</p> <p>Attach custom forms they created or custom forms shared with them to objects they have manage or contribute permissions to.</p> </td> 
  </tr> 
  <tr> 
   <td>Recycle Bin: Recently Deleted</td> 
   <td>Full access</td> 
   <td> <p>Users who are group administrators can restore projects assigned to Groups they manage, and tasks, issues, or documents associated with those projects.</p> </td> 
  </tr> 
  <tr> 
   <td>Recycle Bin: Recently Restored</td> 
   <td>Full access</td> 
   <td>Users who are group administrators can see the items they have recently restored.</td> 
  </tr> 
  <tr> 
   <td>Job Roles</td> 
   <td>Full access</td> 
   <td> <p>Modify but not delete existing job roles.</p> <p>Add new job roles.</p> </td> 
  </tr> 
  <tr> 
   <td>Teams</td> 
   <td>Full access</td> 
   <td> <p>No access to create Teams.</p> <p>Add existing teams to users when creating or editing users.</p> </td> 
  </tr> 
  <tr> 
   <td>Groups</td> 
   <td>Full access</td> 
   <td> <p>No access to create Groups.</p> <p>Only group administrators can manage group membership, subgroups, and group-level statuses for the groups they manage. </p> </td> 
  </tr> 
  <tr> 
   <td>Companies</td> 
   <td>Full access</td> 
   <td>Full access</td> 
  </tr> 
  <tr> 
   <td>Log in As</td> 
   <td>Full access </td> 
   <td> <p>If their group administrative access is enabled on their access level and they are designated as a group administrator, they can log in as the users in the group they administer and their subgroups. They cannot log in as a System Administrator.<br>For more information about enabling group administrative access for users, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Grant access to users</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Schedules</td> 
   <td>Full access</td> 
   <td> <p>No access to edit Schedules.</p> <p>Access to add existing schedules to other users, at the user level. </p> </td> 
  </tr> 
  <tr> 
   <td>Timesheet &amp; Hours: Timesheet Profiles</td> 
   <td>Full access</td> 
   <td> <p>Access to assign existing Timesheet Profiles to users, at the user level.</p> <p>Users who are group administrators can create Timesheet Profiles for the groups they administer and their subgroups. </p> </td> 
  </tr> 
  <tr> 
   <td>Timesheet &amp; Hours: Hour Types</td> 
   <td>Full access</td> 
   <td> <p>Access to assign Hour Types to users, at the user level.</p> </td> 
  </tr> 
  <tr> 
   <td>Timesheet &amp; Hours: Preferences</td> 
   <td>Full access</td> 
   <td>No access</td> 
  </tr> 
  <tr> 
   <td>Email: Notifications: Event Notifications</td> 
   <td>Activate/ Deactivate all</td> 
   <td>No access</td> 
  </tr> 
  <tr> 
   <td>Email: Notifications: Reminder Notifications</td> 
   <td>Full access</td> 
   <td>Full access</td> 
  </tr> 
  <tr> 
   <td>Email: Notifications: Email Templates</td> 
   <td>Full access</td> 
   <td> <p>No access to edit Email Templates.</p> <p>Access to add existing Email Templates to Reminder Notifications.</p> </td> 
  </tr> 
  <tr> 
   <td>Email: Automatic Reminders</td> 
   <td>Full access</td> 
   <td>No access</td> 
  </tr> 
  <tr> 
   <td>Email: Invitations</td> 
   <td>Full access</td> 
   <td> <p>No access to edit Email Invitations.</p> <p>Access to resend email invitations to unregistered users only from the People tab.</p> </td> 
  </tr> 
  <tr> 
   <td>Email: Setup</td> 
   <td>Full access</td> 
   <td> <p>No access</p> </td> 
  </tr> 
  <tr> 
   <td>Scorecards</td> 
   <td>Full access</td> 
   <td> <p>Full access</p> </td> 
  </tr> 
  <tr> 
   <td>Expense Types</td> 
   <td>Full access</td> 
   <td> <p>No access</p> </td> 
  </tr> 
  <tr> 
   <td>Risk Types</td> 
   <td>Full access</td> 
   <td>No access</td> 
  </tr> 
  <tr> 
   <td>Access Levels</td> 
   <td> <p>Full access to modify all access levels.</p> <p>The System Administrator and External User access levels cannot be modified, by default.</p> </td> 
   <td> <p>No access to edit Access Levels.</p> <p>Assign an access level to other users which is lower or equal to theirs at the user level.</p> </td> 
  </tr> 
  <tr> 
   <td>Interface: Layout Templates</td> 
   <td>Full access</td> 
   <td> <p>Access to assign existing Layout Templates to other users, at the user level. </p> <p>Users designated as group administrators can create Layout Templates for groups and subgroups they manage.</p> </td> 
  </tr> 
  <tr> 
   <td>Interface: Update Feeds</td> 
   <td>Full access</td> 
   <td> <p>No access to modify Update Feeds.</p> <p>Access to add fields to be tracked in the Update Feeds when editing Custom Forms.</p> </td> 
  </tr> 
  <tr> 
   <td>Interface: Filters</td> 
   <td>Full access</td> 
   <td> <p>No access to create Filters in the Setup area.</p> <p>Access to create new filters in a list of objects.</p> </td> 
  </tr> 
  <tr> 
   <td>Interface: Views</td> 
   <td>Full access</td> 
   <td> <p>No access to create Views in the Setup area.</p> <p>Access to create new views in a list of objects.</p> </td> 
  </tr> 
  <tr> 
   <td>Interface: Groupings</td> 
   <td>Full access</td> 
   <td> <p>No access to create Groupings in the Setup area.</p> <p>Access to create new groupings in a list of objects.</p> </td> 
  </tr> 
  <tr> 
   <td>Interface: List Controls</td> 
   <td>Full access</td> 
   <td> <p>No access</p> </td> 
  </tr> 
  <tr> 
   <td>Documents: Cloud Providers</td> 
   <td>Full access</td> 
   <td> <p>No access to configure Cloud Providers.</p> <p>Access to link documents to and from Cloud Providers from the Documents tab, after the Cloud Providers have been integrated with Workfront.</p> </td> 
  </tr> 
  <tr> 
   <td>Documents: Metadata Mapping</td> 
   <td>Full access</td> 
   <td>No access</td> 
  </tr> 
  <tr> 
   <td>Documents: SharePoint Integration</td> 
   <td>Full access</td> 
   <td> <p>No access to configure a SharePoint integration.</p> <p>Access to link documents to and from SharePoint from the Documents tab, after the SharePoint integration with Workfront has been configured.</p> </td> 
  </tr> 
  <tr> 
   <td>Documents: Custom Integration</td> 
   <td>Full access</td> 
   <td> <p>No access to configure a Custom Integration.</p> <p>Access to link documents to and from third-party providers from the Documents tab, after the third-party providers have been integrated with Workfront.</p> </td> 
  </tr> 
  <tr> 
   <td>System: Branding</td> 
   <td>Full access</td> 
   <td>No access</td> 
  </tr> 
  <tr> 
   <td>System: Customer Info</td> 
   <td>Full access</td> 
   <td>No access</td> 
  </tr> 
  <tr> 
   <td>System: Single Sign-On (SSO)</td> 
   <td>Full access</td> 
   <td>No access</td> 
  </tr> 
  <tr> 
   <td>System: Update Users for SSO</td> 
   <td>Full access</td> 
   <td>No access</td> 
  </tr> 
  <tr> 
   <td>System: Kick-Starts</td> 
   <td>Full access</td> 
   <td>No access</td> 
  </tr> 
  <tr> 
   <td>System: Diagnostics</td> 
   <td>Full access</td> 
   <td>No access</td> 
  </tr> 
  <tr> 
   <td>System: Preferences</td> 
   <td>Full access</td> 
   <td>No access</td> 
  </tr> 
 </tbody> 
</table>

### Access to objects {#access-to-objects}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Area/object</th> 
   <th>Workfront administrator </th> 
   <th>User with a Plan license and some administrative rights</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Calendars</td> 
   <td>Full access</td> 
   <td>Manage calendars they create and calendars shared with them.</td> 
  </tr> 
  <tr> 
   <td>Dashboards</td> 
   <td>Full access</td> 
   <td>Manage dashboards they create and dashboards shared with them.</td> 
  </tr> 
  <tr> 
   <td>Documents</td> 
   <td>Full access</td> 
   <td>Manage documents they upload or documents shared with them.</td> 
  </tr> 
  <tr> 
   <td>Issues</td> 
   <td>Full access</td> 
   <td>Manage issues they create or issues shared with them.</td> 
  </tr> 
  <tr> 
   <td>Portfolios</td> 
   <td>Full access</td> 
   <td>Manage portfolios they create or portfolios shared with them. </td> 
  </tr> 
  <tr> 
   <td>Programs</td> 
   <td>Full access</td> 
   <td>Manage programs they create or programs shared with them.</td> 
  </tr> 
  <tr> 
   <td>Project</td> 
   <td>Full access</td> 
   <td>Manage projects they create or projects shared with them.</td> 
  </tr> 
  <tr> 
   <td>Reports</td> 
   <td>Full access</td> 
   <td>Manage reports they create or reports shared with them. View, copy and edit system reports.</td> 
  </tr> 
  <tr> 
   <td>Tasks</td> 
   <td>Full access</td> 
   <td>Manage tasks they create or tasks shared with the</td> 
  </tr> 
  <tr> 
   <td>Templates</td> 
   <td>Full access</td> 
   <td>Manage templates they create or templates shared with them</td> 
  </tr> 
  <tr> 
   <td>Timesheets</td> 
   <td>Full access</td> 
   <td>Full access</td> 
  </tr> 
  <tr> 
   <td>Users</td> 
   <td>Full access</td> 
   <td> <p>Limited access</p> <p>They cannot assign groups to users for which they are not a group administrator or groups that are not public.</p> <p>They cannot assign an access level to users which is higher then their own access level.</p> <p>If their group administrative access is enabled on their access level and they are designated as a group administrator on a group, they can reset the password of and log in as the users in the group they administer and their subgroups. They cannot reset the password of or log in as a System Administrator.<br>For more information about enabling group administrative access for users, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Grant access to users</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->