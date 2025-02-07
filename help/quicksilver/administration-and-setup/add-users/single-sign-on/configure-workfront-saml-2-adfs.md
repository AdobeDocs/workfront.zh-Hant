---
user-type: administrator
product-area: system-administration;setup
navigation-topic: single-sign-on-in-workfront
title: 使用ADFS以SAML 2.0設定Adobe Workfront
description: 您可以使用SAML 2.0啟用對Workfront的驗證。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 9bc5987b-6e32-47df-90c8-08ea4b1b7451
source-git-commit: d2ca099e78d5adb707a0a5a53ccb2e6dd06698f8
workflow-type: tm+mt
source-wordcount: '882'
ht-degree: 0%

---

# 使用ADFS以SAML 2.0設定Adobe Workfront

{{important-admin-console-onboard}}

身為Adobe Workfront管理員，您可以將Workfront與安全性宣告標籤語言(SAML) 2.0解決方案整合，以便在使用Active Directory Federation Services (ADFS)時進行單一登入。

本指南著重於設定ADFS而不使用自動布建或屬性對應。 建議您在設定任何自動布建之前，先完成設定並進行測試。

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

## 啟用使用SAML 2.0對Workfront的驗證

若要啟用對Workfront Web應用程式和具有SAML 2.0的Workfront行動應用程式的驗證，請完成以下章節：

* [擷取Workfront SSO中繼資料檔案](#retrieve-the-workfront-sso-metadata-file)
* [設定信賴方信任](#configure-relying-party-trusts)
* [設定宣告規則](#configure-claim-rules)
* [上傳中繼資料檔案並測試連線](#upload-the-metadata-file-and-test-the-connection)

### 擷取Workfront SSO中繼資料檔案 {#retrieve-the-workfront-sso-metadata-file}

{{step-1-to-setup}}

1. 在左側面板中，按一下&#x200B;**系統** > **單一登入(SSO)**。
1. 在&#x200B;**型別**&#x200B;下拉式功能表中，按一下&#x200B;**SAML 2.0**&#x200B;以顯示其他資訊和選項。
1. 複製&#x200B;**中繼資料URL**&#x200B;之後顯示的URL。
1. 繼續下列章節，[設定信賴方信任](#configure-relying-party-trusts)。

### 設定信賴方信任 {#configure-relying-party-trusts}

1. 使用Windows Server 2008 R2 （版本可能有所不同）開啟&#x200B;**ADFS管理員**。
1. 移至&#x200B;**開始。**
1. 按一下&#x200B;**管理工具。**
1. 按一下&#x200B;**ADFS 2.0管理。**
1. 選取&#x200B;**ADFS**&#x200B;並展開&#x200B;**信任關係**。
1. 用滑鼠右鍵按一下&#x200B;**信賴方信任**，然後選取&#x200B;**新增信賴方信任**&#x200B;以啟動[新增信賴方信任]精靈。
1. 從&#x200B;**歡迎頁面**，選取&#x200B;**開始**。
1. 在&#x200B;**選取日期Source**&#x200B;區段中，貼上Workfront的中繼資料URL。
1. 按一下&#x200B;**下一步**。
1. 按一下&#x200B;**確定**&#x200B;認可警告訊息。
1. 在&#x200B;**指定顯示名稱**&#x200B;區段中，新增&#x200B;**顯示名稱**&#x200B;和&#x200B;**附註**&#x200B;以區分信任，然後按一下&#x200B;**下一步**。
1. 選取&#x200B;**允許所有使用者存取此信賴方** （或若您稍後要設定，請選取&#x200B;**無**）。
1. 按一下&#x200B;**下一步**。

   這會將您帶往&#x200B;**準備新增信任**&#x200B;區段。

1. 繼續下列章節[設定宣告規則](#configure-claim-rules)。

### 設定宣告規則 {#configure-claim-rules}

1. 按一下&#x200B;**準備新增信任**&#x200B;區段中的&#x200B;**下一步**，然後確定已選取&#x200B;**開啟[編輯宣告規則]對話方塊**&#x200B;選項。

   這可讓您在未來的步驟中編輯宣告規則。

1. 按一下 **關閉**。
1. 按一下&#x200B;**新增規則。**
1. 選取&#x200B;**傳送LDAP屬性作為宣告**。
1. 按一下&#x200B;**下一步**&#x200B;以顯示&#x200B;**設定宣告規則**&#x200B;步驟。
1. 指定設定宣告規則的下列最低需求： （這會進入使用者設定的&#x200B;**同盟ID**，用來區分登入者。）


   <table >                
      <tbody>
            <tr>
               <td>宣告規則名稱
               </td>
               <td>指定宣告規則的名稱。 例如，「Workfront」。</td>
            </tr>
            <tr>
               <td>屬性存放區</td>
               <td >從下拉式功能表中選取<b>Active Directory</b>。</td>
            </tr>
            <tr>
               <td>LDAP屬性</td>
               <td>這可以是任何型別的屬性。 我們建議對此屬性使用<b>SAM-Account-Name</b>。</td>
            </tr>
            <tr>
               <td>連出宣告型別</td>
               <td>您必須選取<b>名稱ID</b>做為傳出宣告型別</td>
            </tr>
      </tbody>
   </table>

1. （選擇性）若要建立自動布建，請在LDAP屬性和傳出宣告型別中新增下列其他宣告：

   * 名字
   * 姓氏
   * 電子郵件地址

1. 按一下[完成]****，然後在下一個畫面中按一下[確定]****。
1. 用滑鼠右鍵按一下新的&#x200B;**信賴方信任**，然後選取&#x200B;**內容**。
1. 選取&#x200B;**進階索引標籤**。 在&#x200B;**安全雜湊演演算法**&#x200B;下，選取SHA-1或SHA-256。

   >[!NOTE]
   >
   >您在「安全雜湊演演算法」下選取的選項，必須與Workfront中「設定>系統>單一登入(SSO)」下的「安全雜湊演演算法」欄位相符。

1. 繼續下列區段[上傳中繼資料檔並測試連線](#upload-the-metadata-file-and-test-the-connection)。

### 上傳中繼資料檔案並測試連線 {#upload-the-metadata-file-and-test-the-connection}

1. 開啟瀏覽器並導覽至`https://<yourserver>/FederationMetadata/2007-06/FederationMetadata.xml` 。

   這應該會下載中繼資料檔案FederationMetadata.xml檔案。

1. 按一下&#x200B;**從識別提供者中繼資料**&#x200B;填入欄位&#x200B;**選擇檔案**，然後選取&#x200B;**FederationMetadata.xml**&#x200B;檔案。

1. （選擇性）如果憑證資訊未填入中繼資料檔案，您可以另外上傳檔案。 在&#x200B;**憑證**&#x200B;區段中選取&#x200B;**選擇檔案**。

1. 按一下&#x200B;**測試連線**。 如果設定正確，您應該會看到類似以下所示的頁面：

   ![SAML 2成功訊息](assets/success-saml-2.png)

   >[!NOTE]
   >
   >如果要設定屬性對應，請確定您將屬性從「測試連線」複製到「目錄屬性」。 如需詳細資訊，請參閱對應使用者屬性。

1. 選取&#x200B;**管理劐免**&#x200B;以允許Workfront管理員使用略過URL的Workfront憑證登入。

   指向`<yourdomain>`.my.workfront.com/login的書籤略過重新導向。

1. 選取&#x200B;**啟用**&#x200B;方塊以啟用組態。
1. 按一下「**儲存**」。

## 關於更新SSO的使用者

依照本指南，**SSO使用者名稱**&#x200B;將是他們的&#x200B;**Active Directory使用者名稱**。

身為Workfront管理員，您可以大量更新SSO的使用者。 如需更新SSO使用者的詳細資訊，請參閱[更新單一登入的使用者](../../../administration-and-setup/add-users/single-sign-on/update-users-sso.md)。

身為Workfront管理員，您也可以手動指派同盟ID，以編輯使用者的設定檔並完成「同盟ID」欄位。 如需編輯使用者的詳細資訊，請參閱[編輯使用者的設定檔](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)。

>[!NOTE]
>
>編輯使用者的設定檔以包含Federation ID時，選取&#x200B;**僅允許SAML 2.0驗證**&#x200B;會移除使用略過URL (`<yourdomain>`.my.workfront.com/login)登入Workfront的功能。
