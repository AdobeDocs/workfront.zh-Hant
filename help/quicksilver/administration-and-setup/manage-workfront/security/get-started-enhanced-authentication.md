---
title: 增強型驗證概述
description: 在搜尋和左側導覽中隱藏
hidefromtoc: true
hide: true
feature: System Setup and Administration
role: Admin
exl-id: bf3c6c6f-ddd5-42d0-9efe-b5eb94549f85
source-git-commit: c71c5c4a545f9256ecce123ae3513d01a7251ad7
workflow-type: tm+mt
source-wordcount: '13'
ht-degree: 0%

---

# 增強型驗證概述

<!-- enhanced authentication is no longer available for workfront customers -->

{{important-admin-console-onboard}}

<!--REMOVE ME MARCH 2026-->

<!--Adobe Workfront is changing the system management of users and passwords. These changes will roll out in a phased release called **Enhanced Authentication** experience. Enhanced Authentication offers users a more consistent and secure sign-in experience across all Workfront products and services.

The following table provides details about current and future functionality:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col data-mc-conditions=""> 
 <thead> 
  <tr> 
   <th> <p><strong>Feature</strong> </p> </th> 
   <th><strong>Legacy Authentication</strong> </th> 
   <th><strong>Enhanced Authentication 1.0</strong> </th> 
   <th> <p>Enhanced Authentication 2.0</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td colspan="3"> <p><strong>Login options</strong> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Enable a single username to be used for all Workfront products and services, including training, support, and others</p> </td> 
   <td>Not available</td> 
   <td> <p>Not available</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Allow using the same email address across Workfront instances</p> </td> 
   <td> <p>✓</p> <p>Available as of the 2019.3 release</p> </td> 
   <td> <p>✓</p> <p>Available as of the 2019.3 release</p> </td> 
   <td> <p>✓</p> <p>Available as of the 2019.3 release</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Email addresses are case-insensitive</p> </td> 
   <td> <p>✓</p> <p>Available as of the 2019.3 release</p> </td> 
   <td> <p>✓</p> <p>Multiple users cannot have the same email address if the address differs only by case. </p> </td> 
   <td> <p>✓</p> <p>Multiple users cannot have the same email address if the address differs only by case. </p> <p>Workfront administrators will be notified toward the end of 2019 to begin fixing duplicate email addresses.</p> </td> 
  </tr> 
  <tr> 
   <td colspan="3"> <p><strong>Password management options</strong> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Instigate a password reset email for a user as the Workfront administrator</p> </td> 
   <td> <p>Not available </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Set a temporary password for a user as the Workfront administrator</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>Not planned</p> <p>This functionality is not a security best practice</p> </td> 
   <td> <p>Not planned</p> <p>This functionality is not a security best practice</p> </td> 
  </tr> 
  <tr> 
   <td colspan="3"> <p><strong>Password policy requirements</strong> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Require users to reset passwords after a certain timeframe</p> </td> 
   <td>✓</td> 
   <td> <p>Not planned</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Restrict users from using a previous password </p> </td> 
   <td>✓</td> 
   <td>Not planned </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Safeguard against incorrect password entry attempts </p> </td> 
   <td> <p>✓ </p> <p>Locks the account after 5 incorrect password entry attempts. The wait time required after lockout is configured by the Workfront administrator</p> </td> 
   <td> <p>✓</p> <p>Wait time is exponentially increased after each successive incorrect password based on industry best practices; the time required is not configurable by the Workfront administrator</p> </td> 
   <td> <p>✓</p> <p>Uses a lock-out algorithm that proactively blocks a variety of suspicious behavior.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Require a mix of lowercase, uppercase, numbers, and special characters</p> </td> 
   <td>✓</td> 
   <td> <p>✓ </p> <p>Enhanced flexibility in choosing specific requirements</p> </td> 
   <td> <p>✓</p> <p> 
     </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Set a minimum password length </p> </td> 
   <td> Not available </td> 
   <td> ✓ </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td>Restrict users from using more than 2 identical characters in a row</td> 
    <td>Not available</td> 
    <td>Not available</td> 
    <td> <p>✓</p> </td> 
   </tr>
  -->
<!--<tr> 
   <td colspan="3"> <p><strong>Single Sign-On Protocol support</strong></p> </td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td> <p>Supports SSO integrations that are compliant with Active Directory and LDAP protocols</p> </td> 
   <td> ✓&nbsp;</td> 
   <td> <p> Deprecated</p> <p>Active Directory, Azure, and LDAP systems should use SAML 2.0</p> </td> 
   <td> <p>Deprecated</p> <p>Active Directory, Azure, and LDAP systems can be configured with encrypted SAML 2.0 or OpenID Connect.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Supports SSO protocols that are compliant with SAML 2.0&nbsp;</p> </td> 
   <td>✓</td> 
   <td> ✓&nbsp;</td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Supports Open ID Connect protocols</p> </td> 
   <td> <p>Not available</p> </td> 
   <td> <p>Not available</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p> Configure the Workfront login page to always redirect to the identity provider login page </p> </td> 
   <td> Enabled by default and cannot be disabled</td> 
   <td> <p>✓</p> <p>Workfront administrator can configure the login page to redirect to the identity provider login page, or can configure a login button or buttons.</p> </td> 
   <td> <p>✓</p> <p> Workfront administrators can configure the login page to redirect to the identity provider login page, or can configure a login button or buttons.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Allow each instance to enable multiple SSO providers</p> </td> 
   <td> <p>N/A</p> </td> 
   <td> <p>Not planned</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td colspan="3"> <p><strong>Environment support</strong> </p> </td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td> <p>A single username and password for Preview environments</p> </td> 
   <td> <p>Not available</p> </td> 
   <td> <p>Not available</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>A single username and password for Sandbox environments</p> </td> 
   <td> <p>Not available</p> </td> 
   <td> <p>Not available</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <!--
   <tr> 
    <td> <p>Available for Production environments</p> </td> 
    <td>✓</td> 
    <td> ✓&nbsp;</td> 
    <td> <p>✓</p> </td> 
   </tr>
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td> Available for Preview and Sandbox environments&nbsp;</td> 
    <td> ✓&nbsp;</td> 
    <td> ✓</td> 
    <td> <p>✓</p> </td> 
   </tr>
   </tbody> 
</table>-->
