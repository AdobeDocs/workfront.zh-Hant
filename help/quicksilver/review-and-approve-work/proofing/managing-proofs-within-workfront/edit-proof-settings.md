---
product-area: documents;user-management;resource-management
navigation-topic: manage-proofs-within-workfront
title: 編輯校樣設定
description: 建立校樣後，您隨時都可以編輯校樣設定。
author: Courtney
feature: Digital Content and Documents
exl-id: ee30ce2c-e3dc-4863-a69b-cbc1b8747362
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '622'
ht-degree: 2%

---

# 編輯校樣設定

建立校樣後，您隨時都可以編輯校樣設定。

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>當前計畫：Pro或更高</p> <p>或</p> <p>舊計畫：Premium</p> <p>如需使用不同計畫校對存取權限的詳細資訊，請參閱 <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">存取Workfront中的校對功能</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>當前計畫：工作或計畫</p> <p>舊計畫：任何（您必須為使用者啟用校對）</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">校訂權限設定檔 </td> 
   <td>管理員或更高</td> 
  </tr> 
  <tr> 
   <td role="rowheader">證明角色</td> 
   <td>作者或協調者</td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>編輯對文檔的訪問</p> <p>注意：如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、角色或校樣權限設定檔，請聯絡您的Workfront或Workfront Proof管理員。

## 編輯校樣設定

如果您的Workfront管理員在帳戶層級停用了某些設定，則這些設定可能會遭到鎖定。

1. 前往您要校樣的專案、任務或問題，然後按一下 **檔案** 標籤。
1. 將滑鼠移到校樣上，然後按一下 **文檔詳細資訊**.
1. 在左側面板中，按一下 **校對檢視器設定**.
1. 調整下列設定：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">需要登入. 此校樣無法與來賓用戶共用</td> 
      <td> <p>如果您的審核和審批流程需要更高級別的安全性，則可以使用要求登錄校樣。 這表示只能將Workfront使用者新增至校樣。 他們必須先輸入電子郵件和密碼，才能存取。</p> <p>注意： <em style="font-style: normal;">如果啟用「需要登入」，則無法啟用「訂閱」。</em> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">需要以電子方式簽署決策</td> 
      <td> <p>任何對證明做出決定的審核者都需要電子簽名。 審核者作出決定時，系統會出現提示，要求他們輸入電子郵件和密碼並確認其決定。 <!--
         <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
          For more information, see 
          <a href="../../../workfront-proof/wp-acct-admin/managing-security/electronic-sigs-in-wp.md" class="MCXref xref">Understanding electronic signatures in Workfront Proof</a>
         </MadCap:conditionalText>
        --></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">做出所有必要決策時鎖定校樣</td> 
      <td> <p>您可以設定在最終核准者做出決策時鎖定的校樣狀態。 如果您想要確定審核者無法返回校樣並新增其他意見或變更其決定，這個功能會很實用。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">允許下載原始檔案</td> 
      <td> <p>您可以允許校樣的審核者下載建立校樣的原始檔案。 預設會啟用。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">允許透過公用URL或內嵌程式碼共用校樣</td> 
      <td>您可以讓使用者與公用URL或內嵌程式碼共用校樣。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">允許透過公用URL或內嵌程式碼訂閱校樣</td> 
      <td> <p>啟用校樣的訂閱，可讓尚未明確新增至校樣的使用者訂閱校樣（即將自己新增至校樣）。 然後，系統會為使用者指派您在訂閱設定中為其選取的角色和電子郵件警報。</p> <p>如果已對校樣啟用訂閱，則下列欄位將會生效：</p> 
       <ul> 
        <li><strong>需要訂閱者驗證</strong>  — 訂閱者必須按一下電子郵件中的連結才能存取校樣<br>選取此選項表示訂閱者無法立即存取校樣，但會在電子郵件中取得校樣的連結。 訂閱者驗證的目的，是確保使用者輸入了其有權存取的正確電子郵件地址。</li> 
        <li><strong>新訂閱者的預設角色 — </strong> 這是將分配給所有訂閱校樣的審核者的預設校樣角色。</li> 
        <li><strong>新訂閱者的預設電子郵件警報</strong>  — 這是預設電子郵件警報，將分配給所有訂閱校樣的審核者。</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下&#x200B;**儲存**。

 
