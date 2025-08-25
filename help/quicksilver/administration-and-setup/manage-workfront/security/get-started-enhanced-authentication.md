---
title: 增強型驗證概述
description: 在搜尋和左側導覽中隱藏
hidefromtoc: true
hide: true
feature: System Setup and Administration
role: Admin
exl-id: bf3c6c6f-ddd5-42d0-9efe-b5eb94549f85
source-git-commit: d585b698b6c7900d861a30dc6b5e0bff6bd6d13a
workflow-type: tm+mt
source-wordcount: '537'
ht-degree: 4%

---

# 增強型驗證概述

<!-- enhanced authentication is no longer available for workfront customers -->

{{important-admin-console-onboard}}

Adobe Workfront正在變更使用者和密碼的系統管理。 這些變更將以稱為&#x200B;**增強式驗證**&#x200B;體驗的分階段發行推出。 增強型驗證可在所有Workfront產品和服務中，為使用者提供更一致且安全的登入體驗。

下表提供有關目前和未來功能的詳細資訊：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col data-mc-conditions=""> 
 <thead> 
  <tr> 
   <th> <p><strong>功能</strong> </p> </th> 
   <th><strong>舊版驗證</strong> </th> 
   <th><strong>增強式驗證1.0</strong> </th> 
   <th> <p>增強型驗證2.0</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td colspan="3"> <p><strong>登入選項</strong> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>啟用用於所有Workfront產品和服務的單一使用者名稱，包括訓練、支援和其他</p> </td> 
   <td>未提供</td> 
   <td> <p>未提供</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>允許在Workfront執行個體中使用相同的電子郵件地址</p> </td> 
   <td> <p>✓</p> <p>自2019.3版起提供</p> </td> 
   <td> <p>✓</p> <p>自2019.3版起提供</p> </td> 
   <td> <p>✓</p> <p>自2019.3版起提供</p> </td> 
  </tr> 
  <tr> 
   <td> <p>電子郵件地址區分大小寫</p> </td> 
   <td> <p>✓</p> <p>自2019.3版起提供</p> </td> 
   <td> <p>✓</p> <p>如果地址僅依大小寫不同，則多位使用者不能擁有相同的電子郵件地址。 </p> </td> 
   <td> <p>✓</p> <p>如果地址僅依大小寫不同，則多位使用者不能擁有相同的電子郵件地址。 </p> <p>Workfront管理員將會在2019年底收到通知，開始修正重複的電子郵件地址。</p> </td> 
  </tr> 
  <tr> 
   <td colspan="3"> <p><strong>密碼管理選項</strong> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>為身為Workfront管理員的使用者啟動密碼重設電子郵件</p> </td> 
   <td> <p>未提供 </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>為身為Workfront管理員的使用者設定暫時密碼</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>未計畫</p> <p>此功能不是安全性最佳實務</p> </td> 
   <td> <p>未計畫</p> <p>此功能不是安全性最佳實務</p> </td> 
  </tr> 
  <tr> 
   <td colspan="3"> <p><strong>密碼原則需求</strong> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>要求使用者在特定時間範圍後重設密碼</p> </td> 
   <td>✓</td> 
   <td> <p>未計畫</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>限制使用者使用先前的密碼 </p> </td> 
   <td>✓</td> 
   <td>未計畫 </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>防止錯誤密碼輸入嘗試 </p> </td> 
   <td> <p>✓ </p> <p>在5次密碼輸入嘗試不正確後鎖定帳戶。 Workfront管理員設定鎖定後所需的等待時間</p> </td> 
   <td> <p>✓</p> <p>根據業界最佳實務，在每次出現連續錯誤密碼後，等待時間都會以指數方式增加；Workfront管理員無法設定所需的時間</p> </td> 
   <td> <p>✓</p> <p>使用鎖定演演算法，主動封鎖各種可疑行為。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>需要混合小寫、大寫、數字和特殊字元</p> </td> 
   <td>✓</td> 
   <td> <p>✓ </p> <p>更靈活地選擇特定需求</p> </td> 
   <td> <p>✓</p> <p> 
     </p> </td> 
  </tr> 
  <tr> 
   <td> <p>設定密碼長度下限 </p> </td> 
   <td> 未提供 </td> 
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
  <tr> 
   <td colspan="3"> <p><strong>單一登入通訊協定支援</strong></p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>支援與Active Directory和LDAP通訊協定相容的SSO整合</p> </td> 
   <td> ✓ </td> 
   <td> <p> 已棄用</p> <p>Active Directory、Azure和LDAP系統應該使用SAML 2.0</p> </td> 
   <td> <p>已棄用</p> <p>Active Directory、Azure和LDAP系統可設定為加密的SAML 2.0或OpenID Connect。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>支援符合SAML 2.0的SSO通訊協定 </p> </td> 
   <td>✓</td> 
   <td> ✓ </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>支援Open ID連線通訊協定</p> </td> 
   <td> <p>未提供</p> </td> 
   <td> <p>未提供</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p> 設定Workfront登入頁面，一律重新導向至身分提供者登入頁面 </p> </td> 
   <td> 預設為啟用，無法停用</td> 
   <td> <p>✓</p> <p>Workfront管理員可以設定登入頁面，以重新導向至身份提供者登入頁面，也可以設定登入按鈕。</p> </td> 
   <td> <p>✓</p> <p> Workfront管理員可以設定登入頁面，以重新導向至身份提供者登入頁面，也可以設定登入按鈕。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>允許每個執行個體啟用多個SSO提供者</p> </td> 
   <td> <p>不適用</p> </td> 
   <td> <p>未計畫</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td colspan="3"> <p><strong>環境支援</strong> </p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>預覽環境的單一使用者名稱和密碼</p> </td> 
   <td> <p>未提供</p> </td> 
   <td> <p>未提供</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>沙箱環境的單一使用者名稱和密碼</p> </td> 
   <td> <p>未提供</p> </td> 
   <td> <p>未提供</p> </td> 
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
  --> 
 </tbody> 
</table>
