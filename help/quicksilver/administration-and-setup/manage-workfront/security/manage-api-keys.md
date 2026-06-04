---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: security
title: 管理API金鑰
description: 為了將API安全性弱點降至最低，Adobe Workfront管理員可以管理API金鑰，讓應用程式能夠代表使用者存取Workfront。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 1176d899-0585-430d-87f2-0823bda2f1be
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/ZZMeRwrZeWgY8HVIHhp9aX-1wi64DCdiZgHsoNkP8ZI
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
  - id: f4e6943a-c91a-4134-a2c7-f4f20cfff2f0
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 740
ht-degree: 3%

---

# 管理 API 金鑰

<!--
DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.</p>
-->



>[!IMPORTANT]
>
>Workfront不再建議使用`/login`端點或API金鑰。 請改用下列其中一種驗證方法：
>
>* 使用JWT進行伺服器驗證
>* 使用OAuth2進行使用者驗證
>
>如需設定這些驗證方法的說明，請參閱[為Workfront整合建立OAuth2應用程式](/help/quicksilver/administration-and-setup/configure-integrations/create-oauth-application.md)
>
>如需在Workfront中使用伺服器驗證的指示，請參閱[使用JWT流程設定和使用您組織的自訂OAuth 2應用程式](/help/quicksilver/wf-api/api/oauth-app-jwt-flow.md)
>
>如需在Workfront中使用使用者驗證的指示，請參閱[使用授權碼流程設定並使用您組織的自訂OAuth 2應用程式](/help/quicksilver/wf-api/api/oauth-app-code-token-flow.md)

為了將API安全性弱點降至最低，Adobe Workfront管理員可以管理API金鑰，讓應用程式能夠代表使用者存取Workfront。

您可以重設或移除目前的管理員API金鑰、設定API金鑰過期時間，以及移除所有使用者的API金鑰。

以下是運用Workfront API的應用程式範例：

* 檔案整合，例如Dropbox、Google Drive和Workfront DAM
* Workfront行動應用計畫

>[!IMPORTANT]
>
>重設或移除API金鑰時，任何運用Workfront API並透過此API金鑰向Workfront驗證的應用程式都必須重新設定，才能重新取得Workfront的存取許可權。

## 存取權要求

+++ 展開以檢視這篇文章中所述功能的存取權要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 封裝</td> 
   <td><p>任何</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td><p>標準</p><p>規劃</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>您必須是Workfront管理員。</p> </p> </td> 
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## Workfront API金鑰

Workfront中的每個使用者都有唯一的API金鑰。 使用者存取運用Workfront API （例如Workfront行動應用程式或檔案整合）的整合時，系統會為每個使用者產生此金鑰。

>[!NOTE]
>
> 您在生產環境中產生的API金鑰會在每週重新整理期間複製到您的預覽環境。 在每週重新整理期間，您在預覽環境中產生的任何API金鑰都會被生產API金鑰覆寫。

Workfront管理員也有唯一的API金鑰。 當應用程式使用管理員API金鑰存取Workfront時，該應用程式將可存取Workfront的管理員存取權。

## 管理管理員API金鑰

您可以為管理員使用者帳戶產生、重設或移除API金鑰。

{{step-1-to-setup}}

1. 按一下&#x200B;**系統>** **客戶資訊。**
1. （視條件而定）執行下列其中一項動作：

   若要產生API金鑰：在&#x200B;**API金鑰設定**&#x200B;區段中，按一下&#x200B;**產生API金鑰**。

   或\
   若要重設API金鑰：在&#x200B;**API金鑰設定**&#x200B;區段中，按一下&#x200B;**重設**，然後按一下&#x200B;**重設。**

   或

   若要移除API金鑰：在&#x200B;**API金鑰設定**&#x200B;區段中，按一下&#x200B;**移除**，然後按&#x200B;**移除**。

<!--

   Remove me October 2026

## Generate an API Key for Non-Admin Users

You can generate and manage API Keys for users in roles other than Workfront administrator.

>[!NOTE]
>
>This is not available if your organization's Workfront instance is enabled with Adobe IMS. See your network or IT administrator if you need more information.

1. (Conditional) If your organization uses Single Sign-On (SSO) access management, temporarily disable the option requiring SSO authentication.

   {{step-1-to-setup}} 
   
   1. Expand **System**, then click **Single Sign-on (SSO)**. 
   1. In the **Type** field, select the type of SSO your organization uses.
   1. With the type selected, scroll down and clear the **Enable** checkbox. 
      ![Enable SSO](assets/sysadmin-security-sso-disable-31620-350x320.png)  
   1. Click **Save**.


1. In the address bar of a browser, enter the following API call:

   `<domain>`.my.workfront.com/attask/api/v7.0/user?action=generateApiKey&username=**username**&password=**password**&method=PUT

   Replace `<domain>` with your Workfront domain name, and username and password with the user's Workfront credentials.

1. (Conditional) Enable the option requiring SSO authentication if you disabled it in Step 1.

   {{step-1-to-setup}}
   
   1. Expand **System**, then click **Single Sign-on (SSO)**.
   
   1. Select your SSO method in the **Type** drop down menu.
   1. Check the checkbox requiring SSO authentication.

   -->

## 設定API金鑰何時到期

您可以設定API金鑰，讓系統中所有使用者到期。 當使用者的API金鑰過期時，使用者必須向使用Workfront API存取Workfront的任何應用程式重新驗證。 您可以變更API金鑰的過期頻率。 您也可以設定API金鑰是否在使用者密碼過期時過期。

{{step-1-to-setup}}

1. 按一下&#x200B;**系統** > **客戶資訊**。
1. 在&#x200B;**API金鑰設定**&#x200B;區域的&#x200B;**建立**&#x200B;後，**API金鑰將在**&#x200B;下拉式清單中到期，請選取您希望API金鑰過期的時間範圍。

   當您變更此選項時，新的時間範圍將從您進行變更的時間開始。 例如，如果您將此選項從&#x200B;*1個月*&#x200B;變更為&#x200B;*6個月*，則API金鑰將在您進行變更後6個月到期。

   根據預設，API金鑰每個月都會過期。

1. 若要設定API金鑰在使用者的密碼過期時到期，請啟用&#x200B;**在使用者的密碼過期時移除API金鑰**。

   依預設，此選項不會啟用。

   如需有關如何設定使用者密碼到期的資訊，請參閱[設定系統安全性偏好設定](../../../administration-and-setup/manage-workfront/security/configure-security-preferences.md)。

1. 按一下「**儲存**」。

## 移除所有使用者的API金鑰

如果您對Workfront系統特定的安全性違反有所顧慮，您可以同時為所有使用者移除API金鑰。

>[!IMPORTANT]
>
>移除所有使用者的API金鑰會使系統中所有使用者的所有API金鑰失效。 在您於Workfront中產生新的API金鑰並更新所有整合之前，此動作會導致Workfront中的所有整合失敗。

{{step-1-to-setup}}

1. 展開&#x200B;**系統**，然後按一下&#x200B;**客戶資訊**。

1. 在&#x200B;**API金鑰設定**&#x200B;區域中，按一下&#x200B;**移除所有API金鑰**，然後按一下&#x200B;**移除** **全部**。

<!--

Remove me October 2026

## Restricting API logins with an X.509 certificate

>[!IMPORTANT]
>
>The procedure described in this section applies only to organizations that have not yet been onboarded to the Adobe Business Platform. Logging in to Workfront through the Workfront API is not available if your organization has been onboarded to the Adobe Business Platform.
>
>For a list of procedures that differ based on whether your organization has been onboarded to the Adobe Business Platform, see [Administration differences between Adobe Workfront and Adobe Business Platform](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

>[!NOTE]
>
>This is not available if your organization's Workfront instance is enabled with Adobe IMS. See your network or IT administrator if you need more information.

Third-party applications can communicate with Workfront through the API. To increase the security of your Workfront site, you can configure Workfront to restrict API login requests by uploading an X.509 certificate to Workfront. Once enabled, all login requests through the API must include a client certificate in addition to username and password.

* [Obtain the X.509 certificate](#obtain-the-x-509-certificate) 
* [Upload the certificate to Workfront](#upload-the-certificate-to-workfront) 
* [Verify API login calls are restricted](#verify-api-login-calls-are-restricted)

### Obtain the X.509 certificate {#obtain-the-x-509-certificate}

Obtain a valid X.509 certificate from a trusted Certificate Authority (such as Verisign), and save it to a temporary location on your workstation. 

### Upload the certificate to Workfront {#upload-the-certificate-to-workfront}

After you have obtained the X.509 certificate from your Certificate Authority, you need to upload it to Workfront.

1. Click the **Main Menu** icon ![Main menu icon](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Setup** ![Gear settings icon](assets/gear-icon-settings.png).  

1. Expand **System**, then click **Customer Info**.

1. In the **API Key Settings** area, select **Require X.509 Certificate for API logins**.
1. Click **Change Certificate**.
1. On your workstation, browse to and select the X.509 certificate that you previously downloaded.
1. (Optional) Click **View Details** next to the certificate name to view the following details about the certificate:

   * Subject Common Name
   * Subject Organization
   * Subject Organization Unit
   * Issuer Common Name
   * Issuer Organization
   * Issuer Organization Unit
   * Serial Number
   * Issue Date
   * Expiration Date

1. Click **Save**. 

### Verify API login calls are restricted {#verify-api-login-calls-are-restricted}

Prior to configuring your instance of Workfront to require an X.509 certificate, perform an API request to the `/login` endpoint using valid username and password parameters. You will receive a 200 response that contains a sessionID.

After making the X.509 certificate a requirement via the customer info page in your instance of Workfront, make another login attempt. This time you will receive a 500 error response with the following message: "Untrusted request. Please contact your system administrator and attach certificate."

After confirming that the X.509 certificate is required, perform the same login request with an additional parameter for apiCertificate set to the value of your certificate. If this operation was performed correctly you will receive a 200 response that contains a valid sessionID.

-->
