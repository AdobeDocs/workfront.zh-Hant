---
title: 增強驗證概觀
description: 在搜尋和左側導覽中隱藏
hidefromtoc: true
hide: true
exl-id: bf3c6c6f-ddd5-42d0-9efe-b5eb94549f85
source-git-commit: ab329085fae35fdda28dc8db70e3b47d9d6c28ea
workflow-type: tm+mt
source-wordcount: '580'
ht-degree: 3%

---

# 增強驗證概觀

<!-- enhanced authentication is no longer available for workfront customers -->

{{important-admin-console-onboard}}

Adobe Workfront正在更改用戶和密碼的系統管理。 這些變更將在以下分階段發行中推出： **增強驗證** 體驗。 增強驗證可為使用者提供跨所有Workfront產品和服務更一致且安全的登入體驗。

下表提供目前和未來功能的詳細資訊：

>[!IMPORTANT]
>
>大部分客戶目前都使用舊版驗證，部分客戶則使用增強驗證1.0。
> 
>要驗證您當前使用的身份驗證類型，請轉到 *your_domain*.my.workfront.com/login。 如果您被重新導向至/auth/login，表示您使用的是增強驗證1.0。
> 
>如果系統根據您的位置/平台將您重新導向至https://login-a-xx.workfront.com/ ，其中「xx」可能是美國（美國）、歐盟（歐洲）或GCP(Google雲端平台)，則您使用的是增強驗證2.0。
>
>到2021年底，所有客戶都將改用增強身份驗證2.0。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col data-mc-conditions=""> 
 <thead> 
  <tr> 
   <th> <p><strong>功能</strong> </p> </th> 
   <th><strong>舊版驗證</strong> </th> 
   <th><strong>增強的驗證1.0</strong> </th> 
   <th> <p>增強的驗證2.0</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td colspan="3"> <p><strong>登入選項</strong> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>啟用單一使用者名稱，以用於所有Workfront產品和服務，包括訓練、支援等</p> </td> 
   <td>不可用</td> 
   <td> <p>不可用</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>允許在各Workfront執行個體使用相同的電子郵件地址</p> </td> 
   <td> <p>✓</p> <p>自2019.3版本起提供</p> </td> 
   <td> <p>✓</p> <p>自2019.3版本起提供</p> </td> 
   <td> <p>✓</p> <p>自2019.3版本起提供</p> </td> 
  </tr> 
  <tr> 
   <td> <p>電子郵件地址不區分大小寫</p> </td> 
   <td> <p>✓</p> <p>自2019.3版本起提供</p> </td> 
   <td> <p>✓</p> <p>如果地址僅因個案而不同，則多個使用者無法擁有相同的電子郵件地址。 </p> </td> 
   <td> <p>✓</p> <p>如果地址僅因個案而不同，則多個使用者無法擁有相同的電子郵件地址。 </p> <p>Workfront管理員將於2019年底收到通知，以開始修正重複的電子郵件地址。</p> </td> 
  </tr> 
  <tr> 
   <td colspan="3"> <p><strong>密碼管理選項</strong> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>以Workfront管理員身分為使用者指派密碼重設電子郵件</p> </td> 
   <td> <p>不可用 </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>為使用者設定作為Workfront管理員的暫時密碼</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>未計畫</p> <p>此功能不是安全性最佳實務</p> </td> 
   <td> <p>未計畫</p> <p>此功能不是安全性最佳實務</p> </td> 
  </tr> 
  <tr> 
   <td colspan="3"> <p><strong>密碼策略要求</strong> </p> </td> 
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
   <td> <p>防止密碼輸入嘗試錯誤 </p> </td> 
   <td> <p>✓ </p> <p>嘗試5次錯誤密碼後鎖定帳戶。 Workfront管理員配置了鎖定後所需的等待時間</p> </td> 
   <td> <p>✓</p> <p>根據行業最佳實踐，在每個連續的錯誤密碼後，等待時間都呈指數級增加；Workfront管理員無法設定所需時間</p> </td> 
   <td> <p>✓</p> <p>使用鎖定算法，主動阻止各種可疑行為。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>需要混合使用小寫、大寫、數字和特殊字元</p> </td> 
   <td>✓</td> 
   <td> <p>✓ </p> <p>增強選擇特定需求的靈活性</p> </td> 
   <td> <p>✓</p> <p> 
     </p> </td> 
  </tr> 
  <tr> 
   <td> <p>設定最小密碼長度 </p> </td> 
   <td> 不可用 </td> 
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
   <td> <p>支援與Active Directory和LDAP協定相容的SSO整合</p> </td> 
   <td> ✓ </td> 
   <td> <p> 已棄用</p> <p>Active Directory、Azure和LDAP系統應使用SAML 2.0</p> </td> 
   <td> <p>已棄用</p> <p>Active Directory、Azure和LDAP系統可以配置加密的SAML 2.0或OpenID Connect。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>支援符合SAML 2.0的SSO通訊協定 </p> </td> 
   <td>✓</td> 
   <td> ✓ </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>支援開放ID連接協定</p> </td> 
   <td> <p>不可用</p> </td> 
   <td> <p>不可用</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p> 設定Workfront登入頁面，一律重新導向至身分提供者登入頁面 </p> </td> 
   <td> 預設為啟用，無法停用</td> 
   <td> <p>✓</p> <p>Workfront管理員可以設定登入頁面以重新導向至身分提供者登入頁面，或可以設定登入按鈕或按鈕。</p> </td> 
   <td> <p>✓</p> <p> Workfront管理員可以設定登入頁面以重新導向至身分提供者登入頁面，或設定登入按鈕或按鈕。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>允許每個實例啟用多個SSO提供程式</p> </td> 
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
   <td> <p>不可用</p> </td> 
   <td> <p>不可用</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>沙箱環境的單一使用者名稱和密碼</p> </td> 
   <td> <p>不可用</p> </td> 
   <td> <p>不可用</p> </td> 
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
