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
source-git-commit: a25eb28800ca8bbeeffedb521b3d72c8df71c697
workflow-type: tm+mt
source-wordcount: '654'
ht-degree: 0%

---

# 續約Adobe Workfront SAML 2.0中繼資料憑證

>[!IMPORTANT]
>
>本頁所述的程式僅適用於尚未加入Admin Console的組織。 如果您的組織已上線Adobe Admin Console，則不需要採取任何動作。
>
>如需根據貴組織是否已加入Adobe Admin Console而有所差異的程式清單，請參閱[以平台為基礎的管理差異(Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md)。

Adobe Workfront伺服器利用SAML 2.0通訊協定進行驗證和授權。 更新後，新憑證的有效期為一年。 當您需要更新身分提供者上的憑證時，您會在Workfront中收到警告，提醒您必須進行此變更。 身為Workfront管理員，您可以在系統層級管理此變更。

<!--Use this Important note box in the last few weeks before each update.

You must take action to update the metadata in your identity provider with the information from the renewed certificate before the specified date. Mismatched certificates can keep your users from logging in to Workfront after November 22, 2022.
 
-->

>[!NOTE]
>
>如果您組織的Workfront執行個體已啟用Adobe IMS，便無法使用此功能。 如需詳細資訊，請洽詢您的網路或IT管理員。

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
  <td> <p>新增：標準 </p>
 <p>或</p> 
<p>目前：計畫 </p> 
</td> 
 </tr>   
 <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>您必須是Workfront管理員。</p> </td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 在Workfront中設定SAML 2.0

若要檢閱警告訊息並確認身分提供者中SAML 2.0中繼資料的更新：

{{step-1-to-setup}}

1. 按一下&#x200B;**系統** > **單一登入**。

1. 在&#x200B;**型別**&#x200B;下拉式功能表中，選取&#x200B;**SAML 2.0**。

1. 按一下&#x200B;**下載SAML 2.0中繼資料**。

   這將下載更新的Workfront SAML 2.0憑證，其中包含伺服器的正確中繼資料。

1. 在您的身分提供者中，將您目前的Assertion Consumer Service (ACS) URL （也稱為回覆URL）複製到安全的地方。

   >[!CAUTION]
   >
   >在步驟6中將Workfront中繼資料上傳至您的單一登入(SSO)提供者之前，請將您目前的Assertion Consumer Service (ACS) URL複製到安全的地方。 此URL （也稱為回覆URL）可在您的SSO提供者的Workfront設定頁面上找到。
   >
   >
   >如果您上傳Workfront中繼資料後ACS URL變更，表示中繼資料可能包含不正確的ACS URL。 您必須將其變回您複製的專案，以避免中斷您的單一登入連線。 更新後的憑證在執行此動作後仍會正確。

1. 在您的身分提供者伺服器中，更新您下載的新憑證。
1. （視條件而定）如果您的身分提供者中的判斷提示消費者服務(ACS) URL或回覆URL已變更，請將其變更回您在步驟5中複製的URL。
1. 在Workfront的&#x200B;**單一登入(SSO)頁面**&#x200B;上，確定已選取此選項： **新的Workfront憑證已上傳至身分提供者**。

   >[!NOTE]
   >
   >* 只有在下列所有條件都適用時，才會顯示此選項：
   >   * 您的組織已設定為SAML 2.0
   >   * 目前的憑證已準備好到期
   >   * 新憑證可供使用
   >* 選取此欄位時，Workfront管理員可使用其SSO憑證或Workfront憑證登入Workfront。

1. 按一下「**儲存**」。

   警告訊息不再顯示，因為您已確認身分提供者伺服器上的SAML 2.0憑證續約。

1. 按一下&#x200B;**測試連線**&#x200B;以測試您的組態。

   您應該會看到一則訊息，確認連線成功。

如需詳細資訊或手動設定中繼資料的協助，請連絡我們的支援團隊，如[連絡客戶支援](../../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md)中所述。
