---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: security
title: 管理API金鑰
description: 為了將API安全性弱點降至最低，Adobe Workfront管理員可以管理用來讓應用程式代表使用者存取Workfront的API金鑰。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 1176d899-0585-430d-87f2-0823bda2f1be
source-git-commit: 5d36c2c959dbfd00920eaf0a16409102b99de042
workflow-type: tm+mt
source-wordcount: '1374'
ht-degree: 2%

---

# 管理API金鑰

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.</p>
-->

為了將API安全性弱點降至最低，Adobe Workfront管理員可以管理用來讓應用程式代表使用者存取Workfront的API金鑰。

您可以重設或移除目前的管理員API金鑰、設定API金鑰至過期，以及移除所有使用者的API金鑰。

運用Workfront API的應用程式範例如下：

* Dropbox、Google Drive和Workfront DAM等檔案整合
* Workfront行動應用程式

>[!IMPORTANT]
>
>重設或移除API金鑰時，任何採用Workfront API並透過此API金鑰驗證至Workfront的應用程式都必須重新設定，才能重新取得Workfront的存取權。

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

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
   <td>計劃</td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置</td> 
   <td> <p>您必須是Workfront管理員。</p> <p><b>注意</b>:如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Workfront API金鑰

Workfront中的每位使用者都有唯一的API金鑰。 此金鑰是在使用者存取採用Workfront API的整合(例如Workfront行動應用程式或檔案整合)時，根據每位使用者產生。

>[!NOTE]
>
> 您在生產環境中產生的API金鑰會在每週重新整理期間複製到您的預覽環境。 您在「預覽」環境中產生的任何API金鑰，都會在每週重新整理期間由生產API金鑰覆寫。

Workfront管理員也有唯一的API金鑰。 當應用程式使用管理員API金鑰來存取Workfront時，應用程式即具有Workfront的管理員存取權。

## 管理管理員API金鑰

您可以產生、重設或移除管理員使用者帳戶的API金鑰。

>[!NOTE]
>
>您也可以透過API產生API金鑰。 如需詳細資訊，請參閱 [事件訂閱API](../../../wf-api/general/event-subs-api.md) 區段 [事件訂閱API](../../../wf-api/general/event-subs-api.md).

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **設定** ![](assets/gear-icon-settings.png).

1. 按一下 **系統>** **客戶資訊。**
1. （條件性）執行下列其中一項動作：

   若要產生API金鑰：在 **API金鑰設定** ，按一下 **產生API金鑰**.

   或\
   重設API金鑰：在 **API金鑰設定** ，按一下 **重設**，然後&#x200B;**重設。**

   或

   若要移除API金鑰：在 **API金鑰設定** ，按一下 **移除**，然後 **移除**.

## 為非管理員使用者產生API金鑰

您可以為非Workfront管理員角色的使用者產生和管理API金鑰。

>[!NOTE]
>
>如果貴組織的Workfront執行個體已透過Adobe IMS啟用，則無法使用此功能。 如需詳細資訊，請洽詢您的網路或IT管理員。

1. （條件性）如果貴組織使用單一登入(SSO)存取管理，請暫時停用需要SSO驗證的選項。

   1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **設定** ![](assets/gear-icon-settings.png).

   1. 展開 **系統**，然後按一下 **單一登入(SSO)**.\
      ![](assets/sysadmin-security-sso-disable-31620-350x320.png)

   1. 禁用需要SSO驗證的複選框。

      例如，如果貴組織使用SAML 2.0，請停用 **僅允許SAML 2.0驗證**.

1. 在瀏覽器的位址列中，輸入下列API呼叫：

   `<domain>`**.my.workfront.com/attask/api/v7.0/user?action=generateApiKey&amp;username=**用戶名**&amp;password=**密碼**&amp;method=PUT

   取代 `<domain>` 使用您的Workfront網域名稱，以及使用者的Workfront憑證的使用者名稱和密碼。

1. （條件性）如果您在步驟1中停用了SSO驗證選項，請啟用此選項。

   1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **設定** ![](assets/gear-icon-settings.png).

   1. 展開 **系統**，然後按一下 **單一登入(SSO)**.

   1. 在 **類型** 下拉式功能表。
   1. 勾選需要SSO驗證的核取方塊。

## 設定API金鑰何時過期

您可以設定API金鑰，讓系統中的所有使用者都過期。 當使用者的API金鑰過期時，使用者必須對使用Workfront API存取Workfront的任何應用程式重新驗證。 您可以變更API金鑰過期的頻率。 您也可以設定當使用者的密碼過期時，API金鑰是否過期。

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **設定** ![](assets/gear-icon-settings.png).

1. 按一下 **系統** > **客戶資訊**.
1. 在 **API金鑰設定** 區域，在 **建立後**, **API金鑰的過期時間為** 下拉式清單中，選取您希望API金鑰過期的時間範圍。

   當您變更此選項時，新的時間範圍將從您進行變更的時間開始。 例如，如果您將此選項從 *1個月* to *6個月*，則API金鑰會從您進行變更之日起6個月過期。

   依預設，API金鑰每月到期。

1. 若要設定API金鑰在使用者密碼過期時到期，請選取 **使用者密碼過期時移除API金鑰**.

   依預設，不會選取此選項。

   如需如何設定使用者密碼以過期的詳細資訊，請參閱 [配置系統安全首選項](../../../administration-and-setup/manage-workfront/security/configure-security-preferences.md).

1. 按一下&#x200B;**儲存**。

## 移除所有使用者的API金鑰

若您對Workfront系統的特定安全性違反行為有所顧慮，可同時為所有使用者移除API金鑰。

>[!IMPORTANT]
>
>移除所有使用者的API金鑰，會使系統中所有使用者的所有API金鑰失效。 此動作會導致您在Workfront中的所有整合失敗，直到您在Workfront中產生新API金鑰並更新所有整合為止。

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **設定** ![](assets/gear-icon-settings.png).

1. 展開 **系統**，然後按一下 **客戶資訊。**

1. 在 **API金鑰設定** 按一下 **移除所有API金鑰**，然後按一下 **移除** **全部**.

## 限制X.509憑證的API登入

>[!IMPORTANT]
>
>本節所述的程式僅適用於尚未上架到Adobe業務平台的組織。 如果貴組織已上線至Workfront Business Platform，便無法透過Workfront API登入Adobe。
>
>有關根據貴組織是否已上架到AdobeBusiness Platform而有所不同的過程清單，請參見 [平台管理差異(Adobe Workfront/Adobe業務平台)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

協力廠商應用程式可透過API與Workfront通訊。 若要提高Workfront網站的安全性，您可以將X.509憑證上傳至Workfront，以限制Workfront登入請求。 啟用後，除了使用者名稱和密碼外，API的所有登入請求都必須包含用戶端憑證。

>[!NOTE]
>
>如果貴組織的Workfront執行個體已透過Adobe IMS啟用，則無法使用此功能。 如需詳細資訊，請洽詢您的網路或IT管理員。

* [取得X.509憑證](#obtain-the-x-509-certificate)
* [上傳憑證至Workfront](#upload-the-certificate-to-workfront)
* [驗證API登入呼叫是否受限](#verify-api-login-calls-are-restricted)

### 取得X.509憑證 {#obtain-the-x-509-certificate}

從受信任的證書頒發機構（如Verisign）獲取有效的X.509證書，並將其置於工作站上的臨時位置。

### 上傳憑證至Workfront {#upload-the-certificate-to-workfront}

從憑證授權單位取得X.509憑證後，您必須將其上傳至Workfront。

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **設定** ![](assets/gear-icon-settings.png).

1. 展開 **系統**，然後按一下 **客戶資訊**.

1. 在 **API金鑰設定** 區域，選擇 **啟用X.509證書**.
1. 在工作站上，瀏覽並選取您先前下載的X.509憑證。
1. （選用）按一下 **檢視詳細資料** 位於憑證名稱旁，以檢視憑證的下列詳細資訊：

   * 主題一般名稱
   * 主題組織
   * 主題組織單位
   * 發行者一般名稱
   * 發行者組織
   * 發行者組織單位
   * 序號
   * 發行日期
   * 到期日期

1. 按一下&#x200B;**儲存**。

### 驗證API登入呼叫是否受限 {#verify-api-login-calls-are-restricted}

在將Workfront例項設定為需要X.509憑證之前，請向 `/login` 使用有效的用戶名和密碼參數的端點。 您將收到包含sessionID的200回應。

透過Workfront執行個體中的客戶資訊頁面要求X.509憑證後，請再次嘗試登入。 這次您會收到500錯誤回應，並顯示下列訊息：「不受信任的請求。 請聯繫您的系統管理員並附加證書。」

確認需要X.509憑證後，請使用將apiCertificate設為憑證值的其他參數，執行相同的登入要求。 如果正確執行此操作，您將收到包含有效sessionID的200回應。
