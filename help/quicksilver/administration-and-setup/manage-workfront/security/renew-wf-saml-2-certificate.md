---
user-type: administrator
product-area: system-administration
keywords: SAML 2.0，安全性，憑證，管理員，免除，設定，中繼資料
navigation-topic: security
title: 續約Adobe Workfront SAML 2.0中繼資料憑證
description: 本頁面上描述的程式僅適用於尚未上線至Admin Console的組織。 如果貴組織已上線至Adobe Admin Console，您必須透過Adobe Admin Console執行此動作。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 4b481215-36a1-4945-828a-1598502529d8
source-git-commit: 3f84f6b8d6cb36fdb23ff332c4078ac1da4a8745
workflow-type: tm+mt
source-wordcount: '571'
ht-degree: 0%

---

# 續約Adobe Workfront SAML 2.0中繼資料憑證

>[!IMPORTANT]
>
>本頁面上描述的程式僅適用於尚未上線至Admin Console的組織。 如果貴組織已上線至Adobe Admin Console，則不需執行任何動作。
>
>如需依貴組織是否已上線至Adobe Admin Console而有所不同的程式清單，請參閱 [平台管理差異(Adobe Workfront/Adobe業務平台)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

Adobe Workfront伺服器會利用SAML 2.0通訊協定進行驗證和授權。 更新後，新憑證的有效期為一年。 當您是時候在身分提供者上續約憑證時，Workfront會警告您必須進行此變更。 身為Workfront管理員，您可以在系統層級管理此變更。

<!--Use this Important note box in the last few weeks before each update.

You must take action to update the metadata in your identity provider with the information from the renewed certiﬁcate before the speciﬁed date. Mismatched certiﬁcates can keep your users from logging in to Workfront after November 22, 2022.
 
-->

>[!NOTE]
>
>如果貴組織的Workfront執行個體已透過Adobe IMS啟用，則無法使用此功能。 如需詳細資訊，請洽詢您的網路或IT管理員。

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

## 在Workfront中設定SAML 2.0

若要檢閱警告訊息並確認身分提供者中SAML 2.0中繼資料的更新：

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **設定** ![](assets/gear-icon-settings.png).

1. 按一下 **系統** > **單一登入**.

1. 在 **類型** 下拉式功能表，選取 **SAML 2.0**.

1. 按一下 **下載SAML 2.0中繼資料**.

   這會下載SAML 2.0的續約Workfront憑證，其中包含您伺服器的正確中繼資料。

   >[!CAUTION]
   >
   >在步驟5中將Workfront中繼資料上傳至單一登入(SSO)提供者之前，請將您目前的斷言使用者服務(ACS)URL複製到安全的位置。 此URL也稱為回覆URL，可在您SSO提供者的Workfront設定頁面上找到。
   >
   >
   >如果上傳Workfront中繼資料後ACS URL變更，這表示中繼資料可能包含錯誤的ACS URL。 您必須將其變更回您複製的連線，以避免中斷單一登入連線。 完成此操作後，更新的證書仍然正確。

1. 前往您的身分提供者伺服器，並更新您下載的新憑證。
1. 在Workfront **單一登入(SSO)頁面**，請確定已選取此選項： **新的Workfront憑證已上傳至Identity Provider**.

   選取此欄位時，Workfront管理員可使用其SSO憑證或Workfront憑證登入Workfront。

1. 按一下&#x200B;**儲存**。

   警告訊息不再顯示，因為您已確認身分提供者伺服器上的SAML 2.0憑證已續約。

1. 按一下 **測試連線** 來測試您的設定。

   您應會看到訊息，確認連線成功。

如需詳細資訊或手動配置中繼資料的協助，請連絡我們的支援團隊，如 [聯絡客戶支援](../../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).
