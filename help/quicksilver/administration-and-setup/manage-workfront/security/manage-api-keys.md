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
source-git-commit: 99113ac4f2ceca6bd50f078916e33cec7f577362
workflow-type: tm+mt
source-wordcount: '1207'
ht-degree: 2%

---

# 管理 API 金鑰

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.</p>
-->

為了將API安全性弱點降至最低，Adobe Workfront管理員可以管理API金鑰，讓應用程式能夠代表使用者存取Workfront。

您可以重設或移除目前的管理員API金鑰、設定API金鑰過期時間，以及移除所有使用者的API金鑰。

以下是運用Workfront API的應用程式範例：

* 檔案整合，例如Dropbox、Google Drive和Workfront DAM
* Workfront行動應用計畫

>[!IMPORTANT]
>
>重設或移除API金鑰時，任何運用Workfront API並透過此API金鑰向Workfront驗證的應用程式都必須重新設定，才能重新取得Workfront的存取許可權。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td>規劃</td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>您必須是Workfront管理員。</p> <p><b>注意</b>：如果您還是沒有存取權，請詢問您的Workfront管理員是否對您的存取層級設定了其他限制。 如需Workfront管理員如何修改存取層級的詳細資訊，請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Workfront API金鑰

Workfront中的每個使用者都有唯一的API金鑰。 使用者存取運用Workfront API (例如Workfront行動應用程式或檔案整合)的整合時，系統會為每個使用者產生此金鑰。

>[!NOTE]
>
> 您在生產環境中產生的API金鑰會在每週重新整理期間複製到您的預覽環境。 在每週重新整理期間，您在預覽環境中產生的任何API金鑰都會被生產API金鑰覆寫。

Workfront管理員也有唯一的API金鑰。 當應用程式使用管理員API金鑰存取Workfront時，該應用程式將可存取Workfront的管理員存取權。

## 管理管理員API金鑰

您可以為管理員使用者帳戶產生、重設或移除API金鑰。

>[!NOTE]
>
>您也可以透過API產生API金鑰。 如需詳細資訊，請參閱[事件訂閱API](../../../wf-api/general/event-subs-api.md)中的[事件訂閱API](../../../wf-api/general/event-subs-api.md)區段。

{{step-1-to-setup}}

1. 按一下&#x200B;**系統>** **客戶資訊。**
1. （視條件而定）執行下列其中一項動作：

   若要產生API金鑰：在&#x200B;**API金鑰設定**&#x200B;區段中，按一下&#x200B;**產生API金鑰**。

   或\
   若要重設API金鑰：在&#x200B;**API金鑰設定**&#x200B;區段中，按一下&#x200B;**重設**，然後按一下&#x200B;**重設。**

   或

   若要移除API金鑰：在&#x200B;**API金鑰設定**&#x200B;區段中，按一下&#x200B;**移除**，然後按&#x200B;**移除**。

## 為非管理員使用者產生API金鑰 — >

<!--DELETE THIS SECTION MARCH 2026-->

>[!IMPORTANT]
>
>本節中說明的程式已移除，因為它僅適用於尚未加入Adobe Admin Console的組織。
>
>所有Workfront組織現在都已上線Adobe Admin Console。

<!--You can generate and manage API Keys for users in roles other than Workfront administrator.

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
   1. Check the checkbox requiring SSO authentication.-->

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

## 使用X.509憑證限制API登入

>[!IMPORTANT]
>
>本節中說明的程式僅適用於尚未加入Adobe Business Platform的組織。 如果您的組織已加入Workfront Business Platform，就無法透過Workfront API登入Adobe。
>
>如需根據貴組織是否已加入Adobe Business Platform而有所差異的程式清單，請參閱[以平台為基礎的管理差異(Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md)。

>[!NOTE]
>
>如果您組織的Workfront執行個體已啟用Adobe IMS，便無法使用此功能。 如需詳細資訊，請洽詢您的網路或IT管理員。

協力廠商應用程式可透過API與Workfront通訊。 為了提高Workfront網站的安全性，您可以將Workfront設定為透過將X.509憑證上傳到Workfront來限制API登入請求。 啟用後，所有透過API的登入請求都必須包含使用者端憑證以及使用者名稱和密碼。

* [取得X.509憑證](#obtain-the-x-509-certificate)
* [將憑證上傳至Workfront](#upload-the-certificate-to-workfront)
* [驗證API登入呼叫是否受到限制](#verify-api-login-calls-are-restricted)

### 取得X.509憑證 {#obtain-the-x-509-certificate}

從受信任的憑證授權單位（例如Verisign）取得有效的X.509憑證，並將其儲存至工作站上的暫存位置。

### 將憑證上傳至Workfront {#upload-the-certificate-to-workfront}

從憑證授權單位取得X.509憑證後，您需要將它上傳到Workfront。

1. 按一下Adobe Workfront右上角的&#x200B;**主功能表**&#x200B;圖示![主功能表圖示](assets/main-menu-icon.png)，然後按一下&#x200B;**設定** ![齒輪設定圖示](assets/gear-icon-settings.png)。

1. 展開&#x200B;**系統**，然後按一下&#x200B;**客戶資訊**。

1. 在&#x200B;**API金鑰設定**&#x200B;區域中，選取&#x200B;**API登入需要X.509憑證**。
1. 按一下&#x200B;**變更憑證**。
1. 在您的工作站上，瀏覽並選取您先前下載的X.509憑證。
1. （選擇性）按一下憑證名稱旁的&#x200B;**檢視詳細資料**&#x200B;以檢視憑證的下列詳細資料：

   * 主題一般名稱
   * 主題組織
   * 主題組織單位
   * 發行者一般名稱
   * 發行者組織
   * 發行者組織單位
   * 序號
   * 發行日期
   * 過期日期

1. 按一下「**儲存**」。

### 驗證API登入呼叫是否受到限制 {#verify-api-login-calls-are-restricted}

在設定您的Workfront執行個體以要求X.509憑證之前，請使用有效的使用者名稱和密碼引數對`/login`端點執行API要求。 您將會收到包含sessionID的200回應。

在透過您Workfront例項中的客戶資訊頁面要求X.509憑證後，請再次嘗試登入。 這次您會收到500錯誤回應，並出現下列訊息：「Untrusted request. 請連絡您的系統管理員並附加憑證。」

確認需要X.509憑證後，使用設為您的憑證值的額外apiCertificate引數，執行相同的登入要求。 如果正確執行此作業，您將會收到包含有效sessionID的200回應。
