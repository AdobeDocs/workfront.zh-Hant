---
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: security
title: 設定用於驗證的密碼原則
description: 身為Adobe Workfront管理員，您可以設定密碼原則選項，以自訂Workfront系統的驗證體驗。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 7832986b-a5e8-4f14-8802-d3b8e32b14bc
source-git-commit: c71c5c4a545f9256ecce123ae3513d01a7251ad7
workflow-type: tm+mt
source-wordcount: '30'
ht-degree: 33%

---

# 設定用於驗證的密碼原則

{{important-admin-console-onboard}}

<!--REMOVE ME MARCH 2026-->

<!--As an Adobe Workfront administrator, you can configure password policy options to customize the authentication experience to your Workfront system.

We recommend that you configure authentication preferences during the Workfront implementation and only occasionally revisit them afterward.

Improved password management capabilities are coming soon or might already be available for your organization. Use either of the following sections, depending on whether your organization has access to the new authentication experience.

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
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>You must be a Workfront administrator.</p> <p><b>NOTE</b>: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Configure authentication (available for all customers) {#configure-authentication-available-for-all-customers}

Authentication options are displayed for all customers. Improved password management capabilities are coming soon or might already be available for your organization, as described in the section [Configure enhanced authentication)](#configure-enhanced-authentication-coming-soon) in this article.

To configure authentication preferences:

{{step-1-to-setup}}

1. Click **System** > **Authentication**.

1. Select any of the following fields to establish the authentication settings for your organization:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Force users to reset their password every <em>&lt;value&gt;</em> days</td> 
      <td>This establishes the time frame for users to reset their Workfront password. By default, this option is disabled. When you enable it, you can choose between 30, 60, 90, 120, 180 days. The default is 30 days.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Don't allow users to set the same password as any of their previous <em>&lt;value&gt;</em> passwords</td> 
      <td> <p>This field prohibits users from reusing passwords for a set number of resets. By default, this field is disabled. When you enable it, you can set this value to 5, 10, or 15 resets before a password can be reused.</p> <p>When this option is selected, users cannot reset their passwords more than one time in a given day</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">If an incorrect password is entered five consecutive times, lock the account for <em>&lt;value&gt;</em> minutes: </td> 
      <td> <p>Select how long a user will be locked out of Workfront after entering an incorrect password five consecutive times. By default, this option is enabled, and the amount of wait time is 10 minutes. You can lock accounts for 10 minutes, 30 minutes, 1 hour, 8 hours, or 24 hours. </p> <p>Manually resetting the password for the user overrides this default wait value. <br>Users can reset their own passwords when they are locked out via the login screen. For more information about how they can reset their password, if they forgot it, see <a href="../../../workfront-basics/manage-your-account-and-profile/managing-your-workfront-account/reset-your-password.md" class="MCXref xref">Reset your password</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Passwords must contain at least <em>&lt;value&gt;</em> different types of characters:</td> 
      <td> <p>Determines how strong user passwords are required to be by allowing you to select the number of different types of characters required in your passwords.</p> <p>A recognizable dictionary word cannot be used as a password.<br>By default, Workfront requires that at least 2 of the following are present in passwords (you can also require 3 of these characters to be present for a valid password): </p> 
       <ul> 
        <li>Uppercase characters</li> 
        <li>Lowercase characters</li> 
        <li>Numbers</li> 
        <li>Symbols</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. Click **Save**.

## Configure enhanced authentication{#configure-enhanced-authentication-coming-soon}

This section describes the enhanced authentication experience, which might not yet be available for your organization. If your organization has not been migrated to the new authentication experience, you must configure the authentication settings, as described in [Configure authentication (available for all customers)](#configure-authentication-available-for-all-customers).

To configure enhanced authentication preferences:

{{step-1-to-setup}}

1. Click **System** > **Enhanced Authentication**.
1. In the **Password Length** box, enter the minimum number of characters required for a valid password.

   Workfront requires at least 6 characters.

1. (Optional) In the **Password Requirements** section, select the types of characters required in user passwords.

   You can increase the strength of user passwords by requiring any or all the types of characters in the Password Requirement section. The following options are available:

   | Lowercase Letters |Require at least one lowercase letter |
   |---|---|
   | Uppercase Letters |Require at least one uppercase letter |
   | Numbers |Require at least one number |
   | Special Characters |Require at least one special character |

   {style="table-layout:auto"}

1. Click **Save**.
-->