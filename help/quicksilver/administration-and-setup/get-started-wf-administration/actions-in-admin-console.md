---
user-type: administrator
product-area: system-administration;setup
navigation-topic: start-with-workfront-administration
title: 平台管理差異(Adobe Workfront/Adobe業務平台)
description: 如果您的組織已上線至Adobe業務平台，則您的使用者會使用Adobe業務平台來存取Adobe Workfront。 這表示使用者管理主要是透過Adobe Admin Console完成，而單一登入(SSO)是透過Adobe業務平台處理，而非透過Workfront。 身為Adobe Workfront管理員，您的管理職責和程式會因貴組織是否已上線至Adobe業務平台而有所不同。 本文列出必須以不同方式處理的程式，以及Workfront和Adobe Admin Console指示的連結。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: a84a5a8d-7c2a-4b51-a614-91a6dc9aa4ed
source-git-commit: 137165deb0c0e9172224e810c82bc651bb0adfc0
workflow-type: tm+mt
source-wordcount: '526'
ht-degree: 1%

---

# 平台管理差異(Adobe Workfront/Adobe業務平台)

如果您的組織已上線至Adobe業務平台，則您的使用者會使用Adobe業務平台來存取Adobe Workfront。 這表示：

* 使用者管理主要透過Adobe Admin Console完成
* 單一登入(SSO)是透過Adobe業務平台處理，而非透過Workfront

身為Adobe Workfront管理員，您的管理職責和程式會因貴組織是否已上線至Adobe業務平台而有所不同。 本文列出必須以不同方式處理的程式，以及Workfront和Adobe Admin Console指示的連結。

## 使用者

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>動作</th> 
   <th>如需Workfront的指示，請參閱</th> 
   <th>如需AdobeAdmin Console的指示，請參閱</th> 
  </tr> 
 </thead> 
 <tbody> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">View information about access levels and licenses for your users</td> 
    <td> 
     <ul> 
      <li> <p><a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/list-access-levels-and-licenses-for-your-users.md" class="MCXref xref">List your users' access levels and licenses</a> </p> </li> 
     </ul> </td> 
    <td> 
     <ul> 
      <li> <p>The section "View user list" in <a href="https://helpx.adobe.com/enterprise/using/manage-users-individually.html">Manage users individually</a></p> </li> 
     </ul> </td> 
   </tr>
  --> 
  <tr> 
   <td role="rowheader">授予使用者管理員存取權</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予使用者完整的管理存取權</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>在 <a href="https://helpx.adobe.com/enterprise/using/manage-users-individually.html">個別管理使用者</a></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">新增使用者至Adobe Workfront</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/add-users.md" class="MCXref xref">新增使用者</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/admin-console.md" class="MCXref xref">在Adobe Admin Console中管理使用者</a> </p> </li> 
     <li> <p>在 <a href="https://helpx.adobe.com/enterprise/using/manage-users-individually.html">個別管理使用者</a></p> </li> 
    </ul> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Add a user to Adobe Workfront Fusion</td> 
    <td> 
     <ul> 
      <li> <p><a href="../../workfront-fusion/organizations/add-user-to-an-organization.md" class="MCXref xref">Add a user to an organization in Adobe Workfront Fusion</a> </p> </li> 
     </ul> </td> 
    <td> 
     <ul> 
      <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/admin-console.md" class="MCXref xref">Manage users in the Adobe Admin Console</a> </p> </li> 
      <li> <p>The section "Add users" in in <a href="https://helpx.adobe.com/enterprise/using/manage-users-individually.html">Manage users individually</a></p> </li> 
     </ul> </td> 
   </tr>
  --> 
  <tr> 
   <td role="rowheader">停用使用者</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">停用或重新啟用使用者</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>在 <a href="https://helpx.adobe.com/enterprise/using/manage-users-individually.html">個別管理使用者</a></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">刪除使用者</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/delete-a-user.md" class="MCXref xref">刪除使用者</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>中的「永久刪除使用者」一節 <a href="https://helpx.adobe.com/enterprise/using/manage-directory-users.html">管理目錄用戶</a>
     </p><p>注意：從 [!DNL Adobe Admin Console] 停用 [!DNL Workfront]，但不會從 [!DNL Workfront].</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">編輯使用者設定檔</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">編輯使用者的設定檔</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>在 <a href="https://helpx.adobe.com/enterprise/using/manage-users-individually.html">個別管理使用者</a></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">大量編輯使用者設定檔</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/edit-user-profiles-in-bulk.md" class="MCXref xref">大量編輯使用者設定檔</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>在 <a href="https://helpx.adobe.com/enterprise/using/bulk-upload-users.html">大量CSV上傳</a></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">匯入使用者 </td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/import-users.md" class="MCXref xref">匯入使用者</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>在 <a href="https://helpx.adobe.com/enterprise/using/bulk-upload-users.html">大量CSV上傳</a></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">以其他使用者身分登入</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/log-in-as-another-user.md" class="MCXref xref">以其他使用者身分登入</a> </p> </li> 
    </ul> </td> 
   <td>不可用</td> 
  </tr> 
  <tr> 
   <td role="rowheader">續約SAML憑證</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/manage-workfront/security/renew-wf-saml-2-certificate.md" class="MCXref xref">續約Adobe Workfront SAML 2.0中繼資料憑證</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>「SAML回應中的數位簽章未驗證……」 in <a href="https://helpx.adobe.com/enterprise/kb/tshoot-fed-id.html">疑難排解Federated ID</a></p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## SSO（單一登入）

由於Adobe業務平台控制用戶的單一登錄(SSO)，因此以下操作和功能將通過Adobe業務平台自動處理。 如果您的組織尚未上線至Adobe業務平台，您必須在Workfront中執行這些動作。


* [使用SAML 2.0設定Adobe Workfront](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md)
* [使用ADFS以SAML 2.0設定Adobe Workfront](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2-adfs.md)
* [在Adobe Workfront中停用單一登入](../../administration-and-setup/add-users/single-sign-on/deactivate-sso.md)
* [在您的身分提供者中更新SAML 2.0中繼資料](../../administration-and-setup/add-users/single-sign-on/update-saml-2-metadata-ip.md)
* [更新單一登入的使用者](../../administration-and-setup/add-users/single-sign-on/update-users-sso.md)
* [配置用於身份驗證的密碼策略](../../administration-and-setup/manage-workfront/security/configure-password-policies-authentication.md)
* [配置系統安全首選項](../../administration-and-setup/manage-workfront/security/configure-security-preferences.md)
