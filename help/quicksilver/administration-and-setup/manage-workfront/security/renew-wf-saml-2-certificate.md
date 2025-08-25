---
user-type: administrator
product-area: system-administration
keywords: SAML 2.0，安全性，憑證，管理員，劐免，設定，中繼資料
navigation-topic: security
title: 續約Adobe Workfront SAML 2.0中繼資料憑證
description: Adobe Workfront伺服器利用SAML 2.0通訊協定進行驗證和授權。 更新後，新憑證的有效期為一年。 當您需要更新身分提供者上的憑證時，您會在Workfront中收到警告，提醒您必須進行此變更。 身為Workfront管理員，您可以在系統層級管理此變更。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 4b481215-36a1-4945-828a-1598502529d8
source-git-commit: 9fa4f85c914121adddcba4189af1398021544776
workflow-type: tm+mt
source-wordcount: '140'
ht-degree: 0%

---

# 續約Adobe Workfront SAML 2.0中繼資料憑證

>[!IMPORTANT]
>
>此頁面上說明的程式已移除，因為它僅適用於尚未上線至Adobe Admin Console的組織。 Adobe Admin Console上的組織不需要執行此程式。
>
>由於所有Workfront組織現已上線至Adobe Admin Console，因此本文將於近期移除。

<!--DELETE ME MARCH 2026-->
<!--
>[!IMPORTANT]
>
>The procedure described on this page applies only to organizations that have not yet been onboarded to the Admin Console. If your organization has been onboarded to the Adobe Admin Console, no action is necessary.
>
>For a list of procedures that differ based on whether your organization has been onboarded to the Adobe Admin Console, see [Platform-based administration differences (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

The Adobe Workfront servers utilize the SAML 2.0 protocol for authentication and authorization. Once updated, the new certificate remains valid for one year. When it is time for you to renew the certificate on your identity provider, you receive a warning in Workfront alerting you that this change must occur. As a Workfront administrator, you can manage this change at the system level.

<!--Use this Important note box in the last few weeks before each update.

You must take action to update the metadata in your identity provider with the information from the renewed certificate before the specified date. Mismatched certificates can keep your users from logging in to Workfront after November 22, 2022.
 


>[!NOTE]
>
>This is not available if your organization's Workfront instance is enabled with Adobe IMS. See your network or IT administrator if you need more information.

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
  <td> <p>New: Standard </p>
 <p>or</p> 
<p>Current: Plan </p> 
</td> 
 </tr>   
 <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>You must be a Workfront administrator.</p> </td> 
  </tr> 
 </tbody> 
</table>

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Configure SAML 2.0 within Workfront

To review the warning message and acknowledge the update of the SAML 2.0 metadata in your identity provider:

{{step-1-to-setup}}

1. Click **System** > **Single Sign-On**.

1. In the **Type** drop-down menu, select **SAML 2.0**.

1. Click **Download SAML 2.0 Metadata**.

   This downloads the renewed Workfront certificate for SAML 2.0, which contains the correct metadata for your server.

1. In your identity provider, copy your current Assertion Consumer Service (ACS) URL (also known as the Reply URL) to a safe place. 

   >[!CAUTION]
   >
   >Before you upload the Workfront metadata to your Single Sign-On (SSO) provider in Step 6, copy your current Assertion Consumer Service (ACS) URL to a safe place. This URL, also known as the Reply URL, is found on your SSO provider's Workfront configuration page. 
   >
   >
   >If the ACS URL changes after you upload the Workfront metadata, this means that the metadata might contain an incorrect ACS URL. You must change it back to the one you copied in order to avoid breaking your Single Sign-On connection. Your updated certificate will still be correct after you do this.

1. In your identity provider server, update the new certificate you downloaded.
1. (Conditional) If the Assertion Consumer Service (ACS) URL or Reply URL has changed in your identity provider, change it back to the URL you copied in Step 5.
1. In Workfront, on the **Single Sign-on (SSO) page**, make sure that this option is selected: **The new Workfront certificate has already been uploaded to the Identity Provider**.

   >[!NOTE]
   >
   >* This option is visible only if all of the following apply:
   >   * Your organization is already set up for SAML 2.0
   >   * The current certificate is ready to expire
   >   * The new certificate is available
   >* When this field is selected, Workfront administrators can log in to Workfront with their SSO credentials or their Workfront credentials.

1. Click **Save**.

   The warning message no longer displays because you acknowledged the renewal of the SAML 2.0 certificate on the server of your identity provider.

1. Click **Test Connection** to test your configuration.

   You should see a message confirming that the connection was successful.

For more information, or for assistance with the manual configuration of metadata, please contact our Support Team, as explained in [Contact Customer Support](../../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).

-->
