---
content-type: overview
product-previous: workfront-proof
product-area: documents;system-administration;user-
navigation-topic: manage-security-workfront-proof
title: ' [!DNL Workfront Proof]中的單一登入'
description: 單一登入(SSO)可讓您的使用者使用您組織的現有使用者名稱和密碼登入 [!DNL Workfront Proof] 。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: eb1f6883-6209-4a55-b181-67af4b496ca0
source-git-commit: 405523606094d4f8553b0aee544d71c2b7f97d86
workflow-type: tm+mt
source-wordcount: '165'
ht-degree: 0%

---

# [!DNL Workfront Proof]中的單一登入

>[!IMPORTANT]
>
>本文提及獨立產品[!DNL Workfront Proof]中的功能。 有關[!DNL Adobe Workfront]內部校訂的資訊，請參閱[校訂](../../../review-and-approve-work/proofing/proofing.md)。

需要[!UICONTROL Enterprise] [!DNL Workfront]計畫才能使用此功能。 如需各種可用計畫的詳細資訊，請參閱[Workfront計畫](https://www.workfront.com/plans)。

單一登入(SSO)可讓您的使用者使用您組織現有的使用者名稱和密碼登入[!DNL Workfront Proof]。

為了提供此功能，我們使用[!DNL Security Assertion Markup Language] (SAML) 2.0，這是一種XML型通訊協定，可讓您授權識別提供者與Web服務之間的資料與交換驗證。

這表示您會針對自己的登入系統，而不是[!DNL Workfront Proof]的登入頁面進行驗證。

您必須在[!DNL Workfront]校訂帳戶上設定自訂子網域或網域，才能啟用SAML：

<!--* Custom sub-domains are free to set up. See our [Configure a branded domain in Workfront Proof](../../../workfront-proof/wp-acct-admin/branding/configure-branded-domain-in-wp.md) for more information.-->
* 您可以閱讀[品牌 [!DNL Workfront Proof] 網站 — 進階](../../../workfront-proof/wp-acct-admin/branding/brand-wp-site-advanced.md)中完全自訂網域的詳細資訊。

請參閱[為 [!DNL Workfront Proof] 使用者設定單一登入](../../../workfront-proof/wp-acct-admin/account-settings/configure-sso-for-wp-users.md)，瞭解在您的帳戶上設定SSO的相關資訊。
