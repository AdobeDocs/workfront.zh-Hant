---
filename: prep-for-admin-console
user-type: administrator
content-type: reference
product-area: system-administration;workfront-integrations
navigation-topic: adobe-admin-console
title: 準備將您的組織加入Adobe Admin Console
description: 由於Adobe Workfront是Adobe產品，因此您可以透過Adobe Admin Console存取。 這可讓您集中管理Workfront，以及使用者的其他Adobe帳戶和產品。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: d9b5e4a1-069e-48be-80d0-84f4bf8aea8b
TQID: 'https://experienceleague.adobe.com/iVdQWwlLpuiS6rjH4U6FRGhPdibD6tyGmmWhLoG6If4'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
    internal-label: Work management
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
    internal-label: Integrations
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
source-git-commit: 3da69fe6ab5bdb843e17bd5ae2ffa985bf2b5cc4
workflow-type: tm+mt
source-wordcount: '73'
ht-degree: 0%
---
# 準備將您的組織加入Adobe Admin Console

<!-- Audited: 12/2023 -->

<!--Remove me January 2027-->

>[!IMPORTANT]
>
>由於所有組織現已移至Adobe Admin Console，因此本文已移除。

<!--

Because Adobe Workfront is an Adobe product, you can access it through the Adobe Admin Console. This enables you to manage Workfront along with other Adobe accounts and products for your users in a central place.

All Workfront customers will soon be moved to the Adobe Admin Console. After your organization moves to the Adobe Admin Console, Workfront authentication is managed by the Console. Preparing and making this move sooner lays the groundwork for efficiency in work management and positions your organization for faster innovation in the future 

For an overview of the Adobe Admin Console, see [Admin Console Overview](https://helpx.adobe.com/tw/enterprise/using/admin-console.html).

## Migration checklist

To ensure that your organization can migrate to the Adobe Admin Console, you must perform the following actions.

1. Identify the desired Adobe Admin Console where you would like to add Workfront.
    
   * If your organization does not have an existing Adobe Admin Console, or if you do not want to use an existing Adobe Admin Console, Workfront Support can assist you in creating a new one.
        
   * If you have multiple Adobe Admin Consoles and you are unsure which one is most appropriate to add Workfront to, contact Workfront Support.

1. Confirm with Workfront Support that you want to use an existing Adobe Admin Console, or have a new one created.
    
1. Set up identity management on the Adobe Admin Console.
    
   >[!IMPORTANT]
   >
   >Be prepared to speak with Workfront Support and your IT team regarding authentication preferences such as Single Sign-on (SSO) or non-SSO.
    
   For instructions, see the Identity Management section of the [Deployment Guide for the Adobe Admin Console](https://helpx.adobe.com/tw/enterprise/using/deployment-planning.html).

1. (Conditional) If using Single Sign-on, connect the new Adobe Admin Console to your existing SSO provider.

   For more information and instructions, see [Set up identity](https://helpx.adobe.com/tw/enterprise/using/set-up-identity.html).

   >[!NOTE]
   >
   >If your organization does not use Single Sign-on, any users migrated to the Adobe Admin Console will receive an email to create their account and password.

1. Ensure that user email addresses are ready for migration:
    
   1. Remove duplicate emails from Workfront.
        
      For instructions, see [Update email addresses of existing users in your Workfront instance](/help/quicksilver/administration-and-setup/manage-workfront/security/prevent-duplicate-users.md#update-email-addresses-of-existing-users-in-your-workfront-instance) in [Prevent duplicate users](/help/quicksilver/administration-and-setup/manage-workfront/security/prevent-duplicate-users.md).
        
      If there are duplicate email address in your organization, the user represented by the email address with the most recent `lastLoginDate` will be moved to the Adobe Admin Console organization. Any other users with that email address will be deactivated.
        
      >[!NOTE]
      >
      >Because only one user with a given email address can be active at a given time, if you need to activate another user with the same email address as a currently active user, you must first deactivate the currently active user before activating the deactivated user.
        
   1. (Conditional) If you are utilizing custom API integrations, confirm those users have a valid email address that they can access.
        
   1. (Optional) We recommend deactivating any users who no longer need access to Workfront, so they are not added to the Adobe Admin Console.
    
   >[!IMPORTANT]
   >
   >These actions regarding user emails must be complete before your organization begins moving to the Adobe Admin Console.
    
1. (Optional) Update all custom integrations to use Adobe Developer Console authentication.

    For information about migrating legacy Workfront OAuth2 integrations, see [Migrate from Workfront OAuth2 to Adobe Developer Console](/help/quicksilver/administration-and-setup/configure-integrations/migrate-oauth2-to-developer-console.md).

    For authentication guidance, see [Adobe Developer Console authentication overview](https://developer.adobe.com/developer-console/docs/guides/authentication/).

    >[!NOTE]
    >
    >This step is optional, but highly recommended. Workfront custom OAuth2 applications can no longer be created after November 1, 2026, and existing custom OAuth2 applications stop working on February 1, 2027. 

After your Adobe Admin Console is configured with Workfront, you can use it to create your Workfront system administrators.

For more information, see [Manage users in the Adobe Admin Console](../../administration-and-setup/add-users/create-and-manage-users/admin-console.md).

For a list of other actions that are different based on whether your organization has been onboarded to the Adobe Admin Console, see [Administration differences between Adobe Workfront and Adobe Business Platform](../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

-->
