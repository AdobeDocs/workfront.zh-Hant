---
user-type: administrator
content-type: reference;overview
product-area: system-administration
navigation-topic: single-sign-on-in-workfront
title: Adobe Workfront單一登入概觀
description: Workfront提供集中管理的單一登入(SSO)設定，可輕鬆將Workfront與您現有的企業SSO解決方案整合。 此設定易於設定和管理，適用於OnDemand和OnPremise Enterprise客戶。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 87f1b6c0-6b74-4eac-87cd-899b1c74af25
source-git-commit: 4e3cafafb121371249fb73f2f001477bdbad2d77
workflow-type: tm+mt
source-wordcount: '244'
ht-degree: 0%

---

# Adobe Workfront單一登入概觀

<!--Audited: 12/2023-->

{{important-admin-console-onboard}}


Workfront提供集中管理的單一登入(SSO)設定，將Workfront與您現有的企業SSO解決方案整合。 此設定適用於OnDemand和OnPremise Enterprise客戶。

若要在Workfront中使用SSO功能，您的組織需要設定SSO應用程式。 接著，您可以設定Workfront，使其可與您的SSO解決方案通訊。

同盟解決方案可讓使用者透過在集中式登入入口網站中輸入使用者名稱和密碼，登入其所有應用程式。

![](assets/overview-sso-wf-fed-only.png)


## 設定防火牆

使用SSO解決方案時，Workfront會在指定連線埠上起始與伺服器的連線。

如果您的防火牆或郵件伺服器設定為僅允許特定廠商存取，則必須將特定Workfront IP位址新增至您的防火牆允許清單。 如需詳細資訊，請參閱 [設定防火牆的允許清單](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## 設定單一登入

Workfront已整合下列SSO解決方案：

* 支援SAML 2.0的同盟解決方案

  如需整合Workfront與SAML 2.0的相關資訊，請參閱 [使用SAML 2.0設定Adobe Workfront](../../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md).

* 支援使用ADFS的SAML 2.0同盟解決方案

  如需使用ADFS整合Workfront與SAML 2.0的相關資訊，請參閱 [使用ADFS以SAML 2.0設定Adobe Workfront](../../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2-adfs.md).
