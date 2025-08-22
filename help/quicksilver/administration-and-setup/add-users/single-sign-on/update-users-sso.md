---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: single-sign-on-in-workfront
title: 更新單一登入的使用者
description: 您可以在Workfront中更新單一登入的使用者。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 0f9c543a-2ae2-4c2c-9c4d-647079263a7e
source-git-commit: c71c5c4a545f9256ecce123ae3513d01a7251ad7
workflow-type: tm+mt
source-wordcount: '19'
ht-degree: 26%

---

# 更新單一登入的使用者

<!-- Audited: 1/2024 -->

{{important-admin-console-onboard}}

<!--REMOVE ME MARCH 2026-->

<!--When single sign-on (SSO) is enabled in your Adobe Workfront instance, your users can log into Workfront with their SSO credentials.

If you have an existing system that is already populated with users associated with SSO credentials, you can import the users' IDs into Workfront by importing a comma-separated values (CSV) file into Workfront.

For more information about integrating Workfront with an SSO system, see [Overview of single sign-on in Adobe Workfront](../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md).


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
   <td role="rowheader">Adobe Workfront license</td> 
   <td><p>New: Standard</p><p>Or</p><p>Current: Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>You must be a Workfront administrator.</p>  </td> 
  </tr> 
 </tbody> 
</table>

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## SSO usernames

Depending on what SSO solution you use, the username in your SSO environment can be called any of the following:

* SSO Username
* Federation ID 
* Federation Username

Regardless of what the username is called in your SSO environment, the value of the field is stored in the SSO Username field, on the User object.

In order for your users to be able to use their SSO credentials to log in to Workfront, you must update their profile to include their SSO Username, in addition to their Workfront username.

As a Workfront administrator, you can bulk update the SSO Username field for your Workfront users by importing a list of usernames into Workfront. This list must:

* Contain the Workfront User ID (GUID) as well as the corresponding SSO Username for each user
* Be saved as a CSV or a TSV file. 

This process either updates existing SSO Usernames in Workfront, or adds a new SSO Username, if one is missing for users.

## Prepare the import file {#prepare-the-import-file}

You can start preparing your import file by building a report of all users in Workfront that must have their SSO Username fields updated.

1. Build a user report in Workfront.

   For instructions on building user reports in Workfront, see [Create a custom report](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md). 

1. Select the following fields in your report:

   |Field|Explanation|
   |---|---|
   | Name |The full name of the Workfront user. |
   | ID |The ID is the Workfront alphanumeric GUID. |
   | SSO Username |Adding the SSO Username field to ensures that are no usernames you are overwriting with your import. This field should be blank for all users, if your users have not yet been updated for SSO. |

   ![Users with SSO username but no access](assets/users-with-sso-username-and-no-sso-access-only-field.png)

1. Save the report. 
1. Click **Export** at the top of the report and export the report to Excel. 
1. Open the exported Excel file, and add your SSO Usernames for each user in the report in the SSO Username column.

   >[!IMPORTANT]
   >
   >SSO usernames are case-sensitive.

1. Delete all columns in the Excel file, except  the **ID** and the **SSO Username** columns. 

1. Delete the column headers and ensure there are no blank rows at the top of the report.

   The file you are using for updating your Workfront users with the SSO usernames **must** contain just 2 columns, in this order:

   * The first column must display the Workfront user ID (the user GUID as found in Workfront).
   * The second column must contain the SSO Username, as it displays in your SSO system.
   * The columns must have no headers, and there must not be any empty rows at the top of the list of names.

     ![Update users CSV](assets/update-users-for-sso-csv-file-for-import.png)

1. Save the report as a CSV or TSV file on your computer.

## Update your users for SSO {#update-your-users-for-sso}

The process of updating users for SSO either adds the SSO Username field to your Workfront users if one is not present, or updates the value in that field if there is a value already associated with the users.

{{step-1-to-setup}}

1. Click **System**, then select **Update Users For SSO**.

1. Click **Choose File** to browse for the file you prepared.

   For more information about how to prepare this file, see [Prepare the import file](#prepare-the-import-file).

1. Select the file from where it is saved on your computer, then click **Open**.

   This inserts the SSO credentials to Workfront, enabling all users to log in to Workfront using their SSO credentials.

   The **Only Allow `<SSO Configuration>` Authentication** setting is enabled for all users included in the CSV. This ensures that users must log in through SSO.

## Verify SSO against your users' Workfront usernames

For instructions on building a user report containing SSO Username information, see [Prepare the import file](#prepare-the-import-file).

1. Run a user report containing SSO Username information.

   Notice that the SSO Username column is populated for each user.

1. Ensure that the values for the SSO Username column match the SSO Username on your SSO server.
1. If the SSO Username column is blank, update your users' SSO Usernames.

   ![Users with SSO field](assets/users-with-sso-field-updated.png)

   For instructions on updating your users for SSO, see [Update your users for SSO](#update-your-users-for-sso).-->
