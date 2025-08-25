---
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: security
title: 設定用於驗證的密碼原則
description: 身為Adobe Workfront管理員，您可以設定密碼原則選項，以自訂Workfront系統的驗證體驗。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 7832986b-a5e8-4f14-8802-d3b8e32b14bc
source-git-commit: d585b698b6c7900d861a30dc6b5e0bff6bd6d13a
workflow-type: tm+mt
source-wordcount: '705'
ht-degree: 3%

---

# 設定用於驗證的密碼原則

{{important-admin-console-onboard}}

身為Adobe Workfront管理員，您可以設定密碼原則選項，以自訂Workfront系統的驗證體驗。

我們建議您在Workfront實作期間設定驗證偏好設定，之後僅偶爾重新造訪一次。

改進的密碼管理功能即將推出，或可能已經提供給您的組織使用。 視您的組織是否具備新驗證體驗的存取權而定，請使用下列任一章節。

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

## 設定驗證（適用於所有客戶） {#configure-authentication-available-for-all-customers}

所有客戶皆會顯示驗證選項。 已改善的密碼管理功能即將推出，或可能已經提供給您的組織使用，如本文的[設定增強驗證)](#configure-enhanced-authentication-coming-soon)一節所述。

若要設定驗證偏好設定：

{{step-1-to-setup}}

1. 按一下&#x200B;**系統** > **驗證**。

1. 選取下列任一欄位，為您的組織建立驗證設定：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">強制使用者每<em>&lt;value&gt;</em>天重設密碼</td> 
      <td>這會建立使用者重設Workfront密碼的時間範圍。 此選項預設為停用。 啟用後，您可以選擇30、60、90、120、180天。 預設值為30天。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">不允許使用者將密碼設定為與其先前<em>&lt;value&gt;</em>個密碼相同的密碼</td> 
      <td> <p>此欄位禁止使用者針對設定的重設次數重複使用密碼。 依預設，此欄位為停用。 啟用後，您可以將此值設定為5、10或15重設，然後才能重複使用密碼。</p> <p>選取此選項時，使用者無法在指定時間內多次重設密碼</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">如果連續5次輸入密碼不正確，請鎖定帳戶<em>&lt;value&gt;</em>分鐘： </td> 
      <td> <p>選取連續5次輸入錯誤密碼後，使用者將被鎖定在Workfront中的時間。 依預設，此選項已啟用，等待時間為10分鐘。 您可以鎖定帳戶10分鐘、30分鐘、1小時、8小時或24小時。 </p> <p>手動重設使用者的密碼將會覆寫此預設等待值。 <br>使用者透過登入畫面鎖定時，可以重設自己的密碼。 如需有關如何重設密碼的詳細資訊（若忘記密碼），請參閱<a href="../../../workfront-basics/manage-your-account-and-profile/managing-your-workfront-account/reset-your-password.md" class="MCXref xref">重設密碼</a>。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">密碼必須包含至少<em>&lt;value&gt;</em>個不同型別的字元：</td> 
      <td> <p>可讓您選取密碼中所需的不同字元型別數目，以決定需要多強使用者密碼。</p> <p>可辨識的字典單字無法當做密碼使用。<br>依預設，Workfront要求密碼中至少要有2個下列字元（您也可以要求有效密碼中要有3個字元）： </p> 
       <ul> 
        <li>大寫字</li> 
        <li>小寫字母</li> 
        <li>數字</li> 
        <li>符號</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下「**儲存**」。

## 設定增強式驗證{#configure-enhanced-authentication-coming-soon}

本節說明增強型驗證體驗，您的組織可能尚未提供此體驗。 如果貴組織尚未移轉至新的驗證體驗，您必須依照[設定驗證（適用於所有客戶）](#configure-authentication-available-for-all-customers)中的說明來設定驗證設定。

若要設定增強的驗證偏好設定：

{{step-1-to-setup}}

1. 按一下&#x200B;**系統** > **增強式驗證**。
1. 在&#x200B;**密碼長度**&#x200B;方塊中，輸入有效密碼所需的最小字元數。

   Workfront至少需要6個字元。

1. （選擇性）在&#x200B;**密碼需求**&#x200B;區段中，選取使用者密碼所需的字元型別。

   您可以在「密碼要求」區段中要求任何或所有型別的字元，以增加使用者密碼的強度。 提供下列選項：

   | 小寫字母 | 至少需要一個小寫字母 |
   |---|---|
   | 大寫字母 | 至少需要一個大寫字母 |
   | 數字 | 至少需要一個數字 |
   | 特殊字元 | 至少需要一個特殊字元 |

   {style="table-layout:auto"}

1. 按一下「**儲存**」。
