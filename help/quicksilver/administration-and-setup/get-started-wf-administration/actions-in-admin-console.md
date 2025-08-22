---
user-type: administrator
product-area: system-administration;setup
navigation-topic: start-with-workfront-administration
title: 平台型管理差異(Adobe Workfront/Adobe Business Platform)
description: 如果您的組織已上線Adobe商業平台，您的使用者會使用Adobe商業平台來存取Adobe Workfront。 這表示使用者管理主要透過Adobe Admin Console完成，且單一登入(SSO)是透過Adobe Business Platform處理，而非透過Workfront。 作為Adobe Workfront管理員，您的管理責任和程式會因您的組織是否已上線到Adobe Business Platform而異。 本文列出必須以不同方式處理的程式，以及Workfront和Adobe Admin Console指示的連結。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: a84a5a8d-7c2a-4b51-a614-91a6dc9aa4ed
source-git-commit: c71c5c4a545f9256ecce123ae3513d01a7251ad7
workflow-type: tm+mt
source-wordcount: '426'
ht-degree: 0%

---

# 平台型管理差異(Adobe Workfront/Adobe Business Platform)

<!--DELETE ME MARCH 2026-->

>[!IMPORTANT]
>
>所有Workfront組織現在都已上線Adobe Admin Console。
>
>本文將於近期移除。

作為Adobe Workfront管理員，您的管理責任和程式可能會因您的組織是否已上線到Adobe Business Platform而異。 本文列出以不同方式處理的程式，以及Workfront和Adobe Admin Console指示的連結。

如果您的組織已上線Adobe商業平台，您的使用者會使用Adobe商業平台來存取Adobe Workfront。 這表示：

* 系統管理員是透過Adobe Admin Console建立的
* SAML憑證的續約已透過Adobe Admin Console處理。
* 單一登入(SSO)是透過Adobe商業平台處理，而非透過Workfront處理

## 在Adobe Admin Console中建立Workfront系統管理員

>[!NOTE]
>
>我們建議直接在Workfront中新增非系統管理員使用者。 您可以在Adobe Admin Console中新增使用者，但若在Workfront中新增使用者，您可於建立使用者時設定其存取層級，藉此節省您的時間。

如需建立Workfront系統管理員的指示，請參閱[在Adobe Admin Console中管理使用者](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/admin-console.md)。

<!--
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Action</th> 
   <th>For instructions in Workfront, see</th> 
   <th>For instructions in the Adobe Admin console, see</th> 
  </tr> 
 </thead> 
 <tbody> 
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">View information about access levels and licenses for your users</td> 
    <td> 
     <ul> 
      <li> <p><a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/list-access-levels-and-licenses-for-your-users.md" class="MCXref xref">List your users' access levels and licenses</a> </p> </li> 
     </ul> </td> 
    <td> 
     <ul> 
      <li> <p>The section "View user list" in <a href="https://helpx.adobe.com/tw/enterprise/using/manage-users-individually.html">Manage users individually</a></p> </li> 
     </ul> </td> 
   </tr>
  <tr> 
   <td role="rowheader">Grant a user admin access</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>The section "Edit user details" in <a href="https://helpx.adobe.com/tw/enterprise/using/manage-users-individually.html">Manage users individually</a></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Add a user to Adobe Workfront</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/add-users.md" class="MCXref xref">Add users</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/admin-console.md" class="MCXref xref">Manage users in the Adobe Admin Console</a> </p> </li> 
     <li> <p>The section "Add users" in in <a href="https://helpx.adobe.com/tw/enterprise/using/manage-users-individually.html">Manage users individually</a></p> </li> 
    </ul> </td> 
  </tr> 
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Add a user to Adobe Workfront Fusion</td> 
    <td> 
     <ul> 
      <li> <p><a href="../../workfront-fusion/organizations/add-user-to-an-organization.md" class="MCXref xref">Add a user to an organization in Adobe Workfront Fusion</a> </p> </li> 
     </ul> </td> 
    <td> 
     <ul> 
      <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/admin-console.md" class="MCXref xref">Manage users in the Adobe Admin Console</a> </p> </li> 
      <li> <p>The section "Add users" in in <a href="https://helpx.adobe.com/tw/enterprise/using/manage-users-individually.html">Manage users individually</a></p> </li> 
     </ul> </td> 
   </tr>
  <tr> 
   <td role="rowheader">Deactivate a user</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Deactivate or reactivate a user</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>The section "Remove users" in in <a href="https://helpx.adobe.com/tw/enterprise/using/manage-users-individually.html">Manage users individually</a></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Delete a user</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/delete-a-user.md" class="MCXref xref">Delete users</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>The section "Permanently delete users" in <a href="https://helpx.adobe.com/tw/enterprise/using/manage-directory-users.html">Manage directory users</a>
     </p><p>Note: Deleting a user from the [!DNL Adobe Admin Console] deactivates the user in [!DNL Workfront], but does not delete them from [!DNL Workfront].</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Edit a user profile</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Edit a user's profile</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>The section "Edit user details" in in <a href="https://helpx.adobe.com/tw/enterprise/using/manage-users-individually.html">Manage users individually</a></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Bulk edit user profiles</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/edit-user-profiles-in-bulk.md" class="MCXref xref">Edit user profiles in bulk</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>The section "Edit user details" in <a href="https://helpx.adobe.com/tw/enterprise/using/bulk-upload-users.html">Bulk CSV upload</a></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Import users </td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/import-users.md" class="MCXref xref">Import users</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>The section "Add users" in <a href="https://helpx.adobe.com/tw/enterprise/using/bulk-upload-users.html">Bulk CSV upload</a></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Log in as another user</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/log-in-as-another-user.md" class="MCXref xref">Log in as another user</a> </p> </li> 
    </ul> </td> 
   <td>Not available</td> 
  </tr> 
  <tr> 
    -->

## 更新SAML憑證

如需在Adobe Admin Console上續約SAML憑證的說明，請參閱[Federated ID疑難排解](https://helpx.adobe.com/tw/enterprise/kb/tshoot-fed-id.html)中的「SAML回應中的數位簽章未驗證……」一節

<!--

   <td role="rowheader">Renew SAML certificate</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/manage-workfront/security/renew-wf-saml-2-certificate.md" class="MCXref xref">Renew the Adobe Workfront SAML 2.0 metadata certificate</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>The section "The digital signature in the SAML response did not validate..." in <a href="https://helpx.adobe.com/tw/enterprise/kb/tshoot-fed-id.html">Troubleshooting Federated ID</a></p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

-->

## SSO （單一登入）

由於Adobe Business Platform可控制使用者的單一登入(SSO)，因此下列動作和功能會透過Adobe Business Platform自動處理。 如果您的組織尚未上線Adobe Business Platform，您必須在Workfront中執行這些動作。


* [使用SAML 2.0設定Adobe Workfront](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md)
* [使用ADFS設定Adobe Workfront的SAML 2.0](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2-adfs.md)
* [在Adobe Workfront中停用單一登入](../../administration-and-setup/add-users/single-sign-on/deactivate-sso.md)
* [更新您的身分提供者中的SAML 2.0中繼資料](../../administration-and-setup/add-users/single-sign-on/update-saml-2-metadata-ip.md)
* [更新單一登入的使用者](../../administration-and-setup/add-users/single-sign-on/update-users-sso.md)
* [設定驗證的密碼原則](../../administration-and-setup/manage-workfront/security/configure-password-policies-authentication.md)
* [設定系統安全性偏好設定](../../administration-and-setup/manage-workfront/security/configure-security-preferences.md)
