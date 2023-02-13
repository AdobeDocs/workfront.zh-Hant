---
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: security
title: 配置用於身份驗證的密碼策略
description: 身為Adobe Workfront管理員，您可以設定密碼原則選項來自訂Workfront系統的驗證體驗。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 7832986b-a5e8-4f14-8802-d3b8e32b14bc
source-git-commit: fe399743ee495334face9d4d632686d9472bc8ef
workflow-type: tm+mt
source-wordcount: '713'
ht-degree: 2%

---

# 配置用於身份驗證的密碼策略

{{important-admin-console-onboard}}

身為Adobe Workfront管理員，您可以設定密碼原則選項來自訂Workfront系統的驗證體驗。

建議您在Workfront實作期間設定驗證偏好設定，並只在之後偶爾重新造訪。

改善的密碼管理功能即將推出，或已可供貴組織使用。 視您的組織是否擁有新驗證體驗的存取權而定，請使用下列其中一節。

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

## 配置身份驗證（所有客戶均可使用） {#configure-authentication-available-for-all-customers}

系統會為所有客戶顯示驗證選項。 改善的密碼管理功能即將推出，或可能已可供您的組織使用，如一節所述 [配置增強身份驗證（即將推出）](#configure-enhanced-authentication-coming-soon) 這篇文章。

要配置身份驗證首選項，請執行以下操作：

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **設定** ![](assets/gear-icon-settings.png).

1. 按一下 **系統** > **驗證**.

1. 選取下列任一欄位，以建立貴組織的驗證設定：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">強制使用者每次重設密碼 <em>&lt;value&gt;</em> 天數</td> 
      <td>如此可建立使用者重設其Workfront密碼的時間範圍。 依預設，此選項會停用。 啟用後，您可以選擇30、60、90、120、180天。 預設為30天。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">不允許用戶設定與以前任何用戶相同的密碼 <em>&lt;value&gt;</em> 密碼</td> 
      <td> <p>此欄位禁止用戶重複使用設定數量的重置的密碼。 此欄位預設為停用。 啟用此值時，您可以將此值設定為5、10或15，然後密碼才可重複使用。</p> <p>選取此選項時，使用者在指定的一天內無法多次重設密碼</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">如果連續輸入錯誤密碼五次，請鎖定帳戶 <em>&lt;value&gt;</em> 分鐘： </td> 
      <td> <p>連續輸入錯誤密碼5次後，選取將使用者鎖定在Workfront外的時間長度。 預設會啟用此選項，等待時間量為10分鐘。 您可以鎖定帳戶10分鐘、30分鐘、1小時、8小時或24小時。 </p> <p>手動重設使用者的密碼，以覆寫此預設等待值。 <br>使用者透過登入畫面鎖定時，可重設自己的密碼。 如需如何重設密碼的詳細資訊（如果忘記密碼），請參閱 <a href="../../../workfront-basics/manage-your-account-and-profile/managing-your-workfront-account/reset-your-password.md" class="MCXref xref">重設密碼</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">密碼至少必須包含 <em>&lt;value&gt;</em> 不同的字元類型：</td> 
      <td> <p>允許您選擇密碼中所需的不同類型字元的數量，從而確定需要多強的用戶密碼。</p> <p>可識別的字典詞不能用作密碼。<br>依預設，Workfront要求密碼中至少包含下列2個字元（您也可以要求有3個字元以顯示有效密碼）: </p> 
       <ul> 
        <li>大寫字元</li> 
        <li>小寫字元</li> 
        <li>數字</li> 
        <li>符號</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下&#x200B;**儲存**。

## 配置增強身份驗證（即將推出） {#configure-enhanced-authentication-coming-soon}

本節說明增強的驗證體驗，這些體驗可能尚未提供給您的組織使用。 如果您的組織尚未移轉至新的驗證體驗，您必須依照 [配置身份驗證（所有客戶均可使用）](#configure-authentication-available-for-all-customers).

要配置增強的身份驗證首選項：

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **設定** ![](assets/gear-icon-settings.png).

1. 按一下 **系統** > **增強驗證**.
1. 在 **密碼長度** 框中，輸入有效密碼所需的字元數下限。

   Workfront至少需要6個字元。

1. （選用）在 **密碼要求** 部分，選擇用戶密碼中所需的字元類型。

   通過要求「密碼要求」部分中的任何或所有類型的字元，可以增加用戶密碼的強度。 可使用下列選項：

   | 小寫字母 | 至少需要一個小寫字母 |
   |---|---|
   | 大寫字母 | 至少需要一個大寫字母 |
   | 數字 | 至少需要一個數字 |
   | 特殊字元 | 至少需要一個特殊字元 |

   {style=&quot;table-layout:auto&quot;}

1. 按一下&#x200B;**儲存**。
