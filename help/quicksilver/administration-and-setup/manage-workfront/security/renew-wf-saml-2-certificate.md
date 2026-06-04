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
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/G7H4JNLLNmQX65RJ-Z-H4zoICtR-cu-baPtRdBfK7Ro
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d8302c96-f652-4d09-896b-19a70bab02a5id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dcid: d095671a-1355-40aa-8b5f-06c33c68080bid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 139
ht-degree: 0%

---

# 續約Adobe Workfront SAML 2.0中繼資料憑證

>[!IMPORTANT]
>
>本頁所述的程式僅適用於尚未加入Admin Console的組織。 如果您的組織已上線Adobe Admin Console，則不需要採取任何動作。
>
>由於所有組織現已上線至Adobe Admin Console，因此此功能已淘汰。

<!--

Remove me October 2026

The Adobe Workfront servers utilize the SAML 2.0 protocol for authentication and authorization. Once updated, the new certificate remains valid for one year. When it is time for you to renew the certificate on your identity provider, you receive a warning in Workfront alerting you that this change must occur. As a Workfront administrator, you can manage this change at the system level.


>[!NOTE]
>
>This is not available if your organization's Workfront instance is enabled with Adobe IMS. See your network or IT administrator if you need more information.

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td><p>Any</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td><p>Standard</p><p>Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>You must be a Workfront administrator.</p> </p> </td> 
  </tr> 
 </tbody> 
</table>

For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

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
