---
product-previous: workfront-proof
product-area: documents;system-administration;user-
navigation-topic: account-settings-workfront-proof
title: 設定 [!DNL Workfront Proof] 使用者的單一登入
description: 如果您有Select或Premium計畫，您可以提供單一登入(SSO)功能，讓您使用現有組織的使用者名稱和密碼來存取您的 [!DNL Workfront Proof] 帳戶。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 52ac1919-1821-424f-89f8-72865b236e4e
source-git-commit: 74a877145b55ccc14b4d5aefd1889919a39e1f20
workflow-type: tm+mt
source-wordcount: '1225'
ht-degree: 0%

---

# 設定[!DNL Workfront Proof]使用者的單一登入

>[!IMPORTANT]
>
>本文提及獨立產品[!DNL Workfront Proof]中的功能。 有關[!DNL Adobe Workfront]內部校訂的資訊，請參閱[校訂](../../../review-and-approve-work/proofing/proofing.md)。

如果您有Select或Premium計畫，您可以提供單一登入(SSO)功能，讓您使用現有組織的使用者名稱和密碼來存取您的[!DNL Workfront Proof]帳戶。

這表示您會針對自己的登入系統，而不是[!DNL Workfront Proof]登入頁面進行驗證。

>[!NOTE]
>
>您必須在[!DNL Workfront Proof]帳戶上設定自訂子網域或網域，才能啟用SAML。 自訂子網域可自由設定。 如需詳細資訊，請參閱[品牌](https://support.workfront.com/hc/en-us/sections/115000921208-Branding)。您可以閱讀有關我們的[品牌 [!DNL Workfront Proof] 網站 — 進階](../../../workfront-proof/wp-acct-admin/branding/brand-wp-site-advanced.md)上完全自訂網域的詳細資訊。

## 在[!DNL Workfront Proof]中啟用SSO

您可在[!UICONTROL 帳戶設定]的[!UICONTROL 單一登入]索引標籤上啟用單一登入功能，此功能將套用至您[!DNL Workfront Proof]帳戶上的所有使用者。 如需詳細資訊，請參閱[帳戶設定](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings)。

## 實體ID

身為服務提供者，我們已於下列位置發佈實體ID：

[https://yoursubdomain.proofhq.com/saml/module.php/saml/sp/metadata.php/phq](https://yoursubdomain.proofhq.com/saml/module.php/saml/sp/metadata.php/phq) （其中「您的子網域」為您的帳戶的子網域）

[!DNL Workfront Proof]需要使用者的電子郵件地址作為其唯一識別碼，此識別碼可作為下列屬性之一傳遞：

* urn:mace:dir:attribute-def:電子郵件地址
* http://schemas.xmlsoap.org/ws/2005/05/identity/claims/emailaddress
* http://schemas.xmlsoap.org/claims/EmailAddress
* urn:oid:0.9.2342.19200300.100.1.3
* http://axschema.org/contact/email
* openid.sreg.email
* 郵件
* 電子郵件
* 電子郵件地址

若要設定SSO：

1. 開啟&#x200B;**[!UICONTROL 單一登入]**&#x200B;標籤(1)。
1. 輸入&#x200B;**SSO URL** (2)。
這是您SSO伺服器的連結(例如，**https://sso.mycompany.com/opensso**)。

1. 輸入&#x200B;**登入URL** (3)。
系統會叫用此URL，將使用者重新導向至您的身分提供者。

   這不是您在瀏覽器中輸入的實際URL，而是端點，將處理我們傳送的資訊，以顯示登入畫面。

1. 輸入&#x200B;**登出URL** (4)。
例如，這是您登出後將會傳回的URL

   **https://www.yourcompany.com/services/logout.asp**

1. 輸入&#x200B;**憑證指紋** (5)。
1. 您的SAML身分提供者提供的SAML憑證的SHA1指紋。
1. 透過在您的身分提供者上設定此專案，確保包括金鑰資訊。
1. 將&#x200B;**SSO**&#x200B;切換為&#x200B;**[!UICONTROL 已啟用]** (6)。
啟用SSO後，您和您帳戶上的其他使用者將使用您自己的驗證機制登入。 這表示當使用者存取您的[!DNL Workfront Proof]帳戶登入畫面(例如，**yourcompany.proofhq.com/login**)時，將會透過傳輸視窗提示他們前往您自己的驗證登入頁面。

1. （選擇性）啟用&#x200B;**自動布建使用者** (7)。
啟用此選項後，將自動為沒有自己的[!DNL Workfront Proof]設定檔，但將使用其Single Sign-On認證存取您的[!DNL Workfront Proof]帳戶的使用者建立使用者帳戶。 只有在您的帳戶尚未達到使用者限制時，才會執行此動作。

1. 根據預設，新布建的使用者將會獲得指派的Manager設定檔許可權。 如果您需要更多資訊，請參閱 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md)中的[校訂許可權設定檔。

![啟用_SSO_SAML_2.0.png](assets/enable-sso-saml-2.0-350x236.png)

## 為附屬帳戶啟用SSO

當您將附屬帳戶連線到您的中心帳戶時，您可以從中心帳戶層級管理這些帳戶。

「單一登入」是「選取」與「進階」功能，因此您只能在屬於「選取」與「進階」計畫的衛星上啟用「單一登入」。

1. 按一下「**[!UICONTROL 設定]**」>「**[!UICONTROL 帳戶設定]**」(1)。

1. 在下拉式功能表(2)中按一下附屬帳戶。
1. 開啟&#x200B;**[!UICONTROL 單一登入]**&#x200B;標籤(3)。
1. 開始編輯SSO設定(4)。
1. ![正在啟用_SSO_-_Satellite_Account.png](assets/enabling-sso---satellite-account-350x266.png)
以下是兩種設定方法(5)：

1. **已繼承：**個SSO，組態取自您的中心帳戶。
如果使用者透過**預設登入頁面** ([https://www.proofhq.com/login](https://www.proofhq.com/login))存取[!DNL Workfront Proof]，將會有&#x200B;**兩個授權等級**：首先，系統會要求使用者使用[!DNL Workfront Proof]存取資料（電子郵件和密碼）登入；然後會透過SSO視窗將使用者傳送到SSO登入頁面。
因此，啟用SSO服務後，建議您透過自己的[!DNL Workfront Proof]子網域/網域登入。

   >[!NOTE]
   >
   >此時，當您的[!DNL Workfront Proof]帳戶已啟用單一登入時，您將無法使用這些認證登入iPhone應用程式。

   1. **手動** （預設）：具有不同設定的SSO （例如，指向另一個識別提供者）。

      >[!NOTE]
      >
      >如果附屬帳戶從中心帳戶繼承SSO設定，則登入畫面將會是中心帳戶的登入畫面。 當衛星帳戶使用者在此頁面上輸入其SSO登入詳細資訊時，他們將被重新導向回衛星帳戶。

      ![正在啟用_SSO_-_Satellite_Account_2.png](assets/enabling-sso---satellite-account-2-350x224.png)

   1. 按一下&#x200B;**[!UICONTROL 儲存]** (6)。

## 從中心帳戶繼承的SSO設定

當您選擇繼承中心帳戶的設定時，您會注意到所有欄位現在都已填入中心帳戶的資料(7)，並且單一登入會自動在您的主帳戶上啟用/停用(8)。 欄位中也不再有編輯連結，因為衛星帳戶的整個SSO設定現在是從您的中心帳戶設定和管理的。

![Satellite_Account_-_Inherited_SSO.png](assets/satellite-account---inherited-sso-350x99.png)

在您的Hub帳戶(9)中，[!UICONTROL SSO使用量]欄位會顯示此設定正由附屬帳戶(10)使用。\
![Hub_Account_-_Inherited_SSO.png](assets/hub-account---inherited-sso-350x275.png)

## 手動設定的SSO

如果已為衛星帳戶(1)選擇手動SSO設定，則需要手動輸入單一登入的資料。

1. 按一下「**[!UICONTROL 設定]**」>「**[!UICONTROL 帳戶設定]**」(1)。

1. 開啟&#x200B;**[!UICONTROL 單一登入]**&#x200B;標籤。
1. 按一下&#x200B;**[!UICONTROL 編輯]，**&#x200B;填入欄位，然後按一下&#x200B;**[!UICONTROL 儲存]** (2)。

1. 在&#x200B;**[!UICONTROL SSO]**&#x200B;資料列，按一下&#x200B;**[!UICONTROL 已啟用]** (3)。

![Satellite_Account_-_Manual_SSO.png](assets/satellite-account---manual-sso-350x280.png)

## sso登入

1. 按一下「**[!UICONTROL 設定]**」>「**[!UICONTROL 帳戶設定]**」(1)。

1. 開啟&#x200B;**[!UICONTROL 單一登入]**&#x200B;標籤。
1. 請確定已設定您的[!DNL Workfront Proof]網域/子網域(1)，且您的使用者可透過此自訂網域/子網域存取您的[!DNL Workfront Proof]帳戶。
   ![SAML_Subdomain.png](assets/saml-subdomain-350x150.png)
啟用「單一登入」後，子網域登入URL (例如yourcompany.proofhq.com/login)會顯示傳輸畫面(2)，可讓您直接前往SSO登入頁面。
   ![SSO_login_page.png](assets/sso-login-page-350x164.png)

1. 如果使用者透過頁面&#x200B;**([https://www.proofhq.com/login](https://www.proofhq.com/login))中的**&#x200B;預設記錄檔存取[!DNL Workfront Proof]，將有&#x200B;**兩個授權等級**。 首先要求使用者使用[!DNL Workfront Proof]存取資料（電子郵件和密碼）登入。 然後，使用者會透過SSO視窗(2)傳送到SSO登入頁面。\
   因此，啟用SSO服務後，建議您透過自己的[!DNL Workfront Proof]子網域/網域登入。

1. 目前，在您的Workfront Proof帳戶上啟用單一登入後，您將無法使用這些憑證登入iPhone應用程式。

## 關於新增使用者

當您的[!DNL Workfront Proof]帳戶已啟用單一登入功能時，新使用者將不會收到任何確認電子郵件，因為其帳戶將會自動啟動並準備使用。

從您的[!DNL Workfront Proof]登入頁面，按一下[!UICONTROL 登入]按鈕後，使用者會進入您的SSO登入頁面，並要求輸入您的Single Sign-On登入認證。

>[!IMPORTANT]
>
>在驗證過程中透過電子郵件地址識別使用者，這表示用於SSO登入的電子郵件帳戶必須是您的帳戶中註冊使用者的電子郵件地址。

## Active Directory同盟服務(AD FS)

Active Directory Federation Services (AD FS)是可安裝在Windows Server作業系統上的[!DNL Microsoft]軟體元件，可讓使用者透過單一登入存取跨組織界限的系統與應用程式。 如需詳細資訊，請參閱Microsoft Developer Network網站上的「Active Directory同盟服務」。

[!DNL Workfront Proof]系統支援SAML 2.0，而且只與AD FS 2.0或更新版本相容。

如需詳細指示，請參閱[在 [!DNL Workfront Proof]中的單一登入： AD FS組態](../../../workfront-proof/wp-acct-admin/account-settings/sso-in-wp-adfs-configuration.md)。
