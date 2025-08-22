---
user-type: administrator
product-area: system-administration
navigation-topic: single-sign-on-in-workfront
title: 更新身分提供者中的SAML 2.0中繼資料
description: 您可以在身分提供者中更新SAML 2.0中繼資料。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 75cd0ab5-8d76-40a4-96a8-00e9f0f4fec6
source-git-commit: c71c5c4a545f9256ecce123ae3513d01a7251ad7
workflow-type: tm+mt
source-wordcount: '26'
ht-degree: 0%

---

# 更新身分提供者中的SAML 2.0中繼資料

{{important-admin-console-onboard}}

<!--REMOVE ME MARCH 2026-->

<!--The following sections describe how to update your Security Assertion Markup Language (SAML) 2.0 metadata when using Active Directory Federation Services (ADFS) as your identity provider.

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

## Use ADFS as your identity provider

You can update your ADFS metadata prior to Adobe Workfront updating the SAML 2.0 certificate or after. If you choose to update the ADFS metadata prior to Workfront updating the SAML 2.0 certificate, additional steps are required.

* [Update your ADFS metadata](#update-your-adfs-metadata) 
* [Force your ADFS metadata to update](#force-your-adfs-metadata-to-update)

### Update your ADFS metadata {#update-your-adfs-metadata}

To set your ADFS metadata to update automatically, complete the steps in this section.

By default, ADFS is configured to automatically check for updates to all of its relying party trust metadata; however, the default is set to poll only every 24 hours. You can change this value with powershell commands.

1. Log in to the ADFS server and open the ADFS Management Console. 
1. In the left-hand panel, expand **ADFS 2.0,** then expand **Trust Relationships.**

1. Click the **Relying Party Trusts** folder.
1. Select the relying party trust that you previously configured to be used with Workfront, then in the right-hand panel, click**Update from Federation Metadata**.
1. (Conditional) If this option is dimmed (which means that the relying party trust was previously configured using a metadata file), complete the following.

   1. Click the **Main Menu** icon ![Main menu icon](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Setup** ![Gear settings icon](assets/gear-icon-settings.png).
   
   1. Click **System** > **Single Sign On (SSO)**.
   
   1. Click **Edit Settings.** 
   1. Click **Edit Configuration**, then select **SAML 2.0** in the **Type** drop-down list. 
   
   1. Copy the **Metadata URL**, which should be similar to the following:

      `https://<yourdomain>.my.workfront.com/sso/downloadSAML2MetaData`
   
   1. On the ADFS server, right-click on the relying party trust that you previously configured, then click **Properties.**
   1. Click the **Monitoring** tab, then paste the URL that you copied from Workfront into the **Relying party's federation metadata URL** field.
   
   1. Check the options to **Monitor relying party** and **Automatically update relying party**.
   
   1. Click **OK.**
   1. Select the relying party trust that you previously configured to be used with Workfront; then, in the right-hand panel, click **Update from Federation Metadata.**

1. Click **OK** to ignore the message about some of the content in the federation metadata not being supported by ADFS 2.0.
1. Open **Windows Powershell Modules.**
1. After all the modules load, run the following command in powershell:

   `Get-ADFSProperties`

1. Look for the value next to **Monitoring Interval.**

   It will be a number that represents the number of minutes between polls. The default should be 1440 (1440 minutes = 24 hours).

1. Set a new value by running the following command in powershell:

   `Set-ADFSProperties -MonitoringInterval 1`
   
   This changes the monitoring interval from every 24 hours to every minute. You can change the 1 to another larger value if you want it to poll less frequently.

1. To verify that this is working correctly, use the **Event Viewer** to look for the following information in the ADFS2.0 logs:

   **Event ID 156 and 157**

### Force your ADFS metadata to update {#force-your-adfs-metadata-to-update}

To update your ADFS metadata complete the steps in the following section.

To force metadata to be exchanged between Workfront and your SAML 2.0 provider when using Active Directory Federation Services (ADFS):

>[!NOTE]
>
>Some of these changes might need to be done by your IT department.

1. Log in to the ADFS server and open the **ADFS Management Console**.
1. In the left-hand panel, expand **ADFS 2.0**, then expand **Trust Relationships**.

1. Click the **Relying Party Trusts** folder.
1. Select the relying party trust that you previously configured to be used with Workfront, then in the right-hand panel, click **Update from Federation Metadata**.

   If this option is dimmed and cannot be selected, complete the following:

   (The option is dimmed only when the relying party trust was previously configured using a metadata file.)

   1. In Workfront, in the Setup area, copy the **Metadata URL** from your Workfront Single Sign-On setup screen.

      To access the information for the **Metadata URL**:

      1. Click **Setup** near the upper-right corner of Adobe Workfront on the Global Navigation Bar.
      1. Click > **System** > **Single Sign On (SSO)**.
      1. Click **Edit Settings.**
      1. Click **Edit Configuration**, then select **SAML 2.0** in the **Type** drop-down list.
      1. Copy the **Metadata URL**, which should be similar to the following:

         `https://<yourdomain>.my.workfront.com/sso/downloadSAML2MetaData`

   1. On the ADFS server, right-click on the relying party trust that you previously configured, then click **Properties.**
   1. Click the **Monitoring** tab, then paste the URL that you copied from Workfront into the **Relying party's federation metadata URL** field.
   1. Check the options to **Monitor relying party** and **Automatically update relying party**.
   1. Click **OK**.
   1. Select the relying party trust that you previously configured to be used with Workfront, then in the right-hand panel, click **Update from Federation Metadata.**

1. Click **OK** to ignore the message about some of the content in the federation metadata not being supported by ADFS 2.0.
1. Click **Update** to complete updating your federation metadata.

Users who are allowed to access Workfront via the native login screen using Workfront login credentials (this can be configured from each user's profile page in the **Access** section) can log in using their Workfront user name and password by navigating to the following URL: `https://<yourdomain>.my.workfront.com/Workfront/login.cmd`.

## Using other identity providers

When using identity providers other than ADFS (such as Ping, Okta, or Centrify), you must re-upload the Workfront metadata to your identity provider.

For more information about how to obtain a new Workfront Metadata URL, see [Update your ADFS metadata](#update-your-adfs-metadata).

For additional information about using Active Directory Federation Services (ADFS) with SAML 2.0 in Workfront, see [Configure Adobe Workfront with SAML 2.0 using ADFS](../../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2-adfs.md).-->
