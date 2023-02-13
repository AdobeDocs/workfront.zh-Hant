---
user-type: administrator
product-area: system-administration;setup
navigation-topic: single-sign-on-in-workfront
title: 使用ADFS以SAML 2.0設定Adobe Workfront
description: 您可以使用SAML 2.0啟用Workfront驗證。
author: Becky, Caroline
feature: System Setup and Administration
role: Admin
exl-id: 9bc5987b-6e32-47df-90c8-08ea4b1b7451
source-git-commit: 02191d80ea58f80de2e7be2ff55f43663e415e31
workflow-type: tm+mt
source-wordcount: '870'
ht-degree: 0%

---

# 使用ADFS以SAML 2.0設定Adobe Workfront

{{important-admin-console-onboard}}

作為Adobe Workfront管理員，您可以將Workfront與安全斷言標籤語言(SAML)2.0解決方案整合，以便在使用Active Directory聯合身份驗證服務(ADFS)時進行單一登入。

本指南著重於設定ADFS而不自動布建或屬性對應。 建議您在設定任何自動布建之前，先完成設定並進行測試。

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

## 使用SAML 2.0啟用Workfront驗證

若要使用SAML 2.0啟用Workfront Web應用程式和Workfront行動應用程式的驗證，請完成下列章節：

* [擷取Workfront SSO中繼資料檔案](#retrieve-the-workfront-sso-metadata-file)
* [配置信賴方信託](#configure-relying-party-trusts)
* [配置聲明規則](#configure-claim-rules)
* [上傳中繼資料檔案並測試連線](#upload-the-metadata-file-and-test-the-connection)

### 擷取Workfront SSO中繼資料檔案 {#retrieve-the-workfront-sso-metadata-file}

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **設定** ![](assets/gear-icon-settings.png).
1. 在左側面板中，按一下 **系統** > **單一登入(SSO)**.
1. 在 **類型** 下拉式功能表，按一下 **SAML 2.0** 以顯示其他資訊和選項。
1. 複製在 **中繼資料URL**.
1. 繼續下列章節： [配置信賴方信託](#configure-relying-party-trusts).

### 配置信賴方信託 {#configure-relying-party-trusts}

1. 開啟 **ADFS管理器** 使用Windows server 2008 R2（版本可能有所不同）。
1. 前往 **開始。**
1. 按一下 **管理工具。**
1. 按一下 **ADFS 2.0管理。**
1. 選擇 **ADFS** 擴展 **信任關係**.
1. 按一下右鍵 **信賴方信託**，然後選取 **添加信賴方信任** 啟動「添加信賴方信任嚮導」。
1. 從 **歡迎頁面**，選取 **開始**.
1. 在 **選擇日期來源** 區段中，貼上來自Workfront的中繼資料URL。
1. 按一下 **下一個**.
1. 按一下 **確定** 確認警告消息。
1. 在 **指定顯示名稱** 區段，新增 **顯示名稱** 和 **附註** 要區分信任，請按一下 **下一個**.
1. 選擇 **允許所有用戶訪問此信賴方** (或 **無** 如果您稍後想要設定)。
1. 按一下 **下一個**.

   這會將您帶至 **準備添加信任** 區段。

1. 繼續下一節 [配置聲明規則](#configure-claim-rules).

### 配置聲明規則 {#configure-claim-rules}

1. 按一下 **下一個** 在 **準備添加信任** 區段，然後確定 **開啟「編輯聲明規則」對話框** 選項。

   這允許您在以後的步驟中編輯「聲明規則」。

1. 按一下 **關閉**。
1. 按一下 **新增規則。**
1. 選擇 **將LDAP屬性發送為聲明**.
1. 按一下 **下一個** 顯示 **配置聲明規則** 步驟。
1. 指定以下最低要求以配置聲明規則：(這會進入 **聯合ID** （在使用者設定中），用於區分登入的使用者。


   <table >                
      <tbody>
            <tr>
               <td>聲明規則名稱
               </td>
               <td>指定聲明規則的名稱。 例如，「Workfront」。</td>
            </tr>
            <tr>
               <td>屬性儲存</td>
               <td >選擇 <b>Active Directory</b> 從下拉式功能表。</td>
            </tr>
            <tr>
               <td>LDAP屬性</td>
               <td>這可以是任何類型的屬性。 建議您使用 <b>SAM-Account-Name</b> 的URL。</td>
            </tr>
            <tr>
               <td>傳出聲明類型</td>
               <td>您必須選取 <b>名稱ID</b> 作為傳出的聲明類型</td>
            </tr>
      </tbody>
   </table>

1. （可選）要建立自動置備，請在「LDAP屬性」和「傳出聲明類型」中添加以下附加聲明：

   * 指定名稱
   * 姓氏
   * 電子郵件地址

1. 按一下 **完成**，然後按一下 **確定** 在下一個畫面。
1. 以滑鼠右鍵按一下新 **信賴方信任**，然後選取 **屬性**.
1. 選取&#x200B;**進階標籤**. 和底下 **安全哈希算法** 選擇SHA-1或SHA-256。

   >[!NOTE]
   >
   >您在「安全雜湊演算法」下選取的選項，必須符合Workfront中「設定>系統>單一登入(SSO)」下的「安全雜湊演算法」欄位。

1. 繼續下一節 [上傳中繼資料檔案並測試連線](#upload-the-metadata-file-and-test-the-connection).

### 上傳中繼資料檔案並測試連線 {#upload-the-metadata-file-and-test-the-connection}

1. 開啟瀏覽器並導覽至 `https://<yourserver>/FederationMetadata/2007-06/FederationMetadata.xml` .

   這應該會下載中繼資料檔案FederationMetadata.xml檔案。

1. 按一下 **選擇檔案** 在 **從身分提供者中繼資料填入欄位**，然後選取 **FederationMetadata.xml** 檔案。

1. （選用）如果憑證資訊未填入中繼資料檔案，您可以個別上傳檔案。 選擇 **選擇檔案** 在 **憑證** 區段。

1. 按一下 **測試連線**. 如果設定正確，您應該會看到類似下列頁面的頁面：

   ![](assets/success-saml-2.png)

   >[!NOTE]
   >
   >如果要設定屬性映射，請確保將屬性從測試連接複製到目錄屬性。 如需詳細資訊，請參閱對應使用者屬性。

1. 選擇 **管理員豁免** 允許Workfront管理員使用具有略過url的Workfront憑證登入。

   指向的書籤 `<yourdomain>`.my.workfront.com/login會略過重新導向。

1. 選取 **啟用** 方塊啟用設定。
1. 按一下&#x200B;**儲存**。

## 關於更新SSO的使用者

依照本指南， **SSO用戶名** 將是他們 **Active Directory用戶名**.

身為Workfront管理員，您可以大量更新SSO的使用者。 如需更新SSO使用者的詳細資訊，請參閱 [更新單一登入的使用者](../../../administration-and-setup/add-users/single-sign-on/update-users-sso.md).

身為Workfront管理員，您也可以手動指派同盟ID，編輯使用者的設定檔並填寫同盟ID欄位。 如需編輯使用者的詳細資訊，請參閱 [編輯使用者的設定檔](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

>[!NOTE]
>
>編輯使用者的設定檔以包含同盟ID時，請選取 **僅允許SAML 2.0驗證** 移除使用略過url(`<yourdomain>`.my.workfront.com/login)。
