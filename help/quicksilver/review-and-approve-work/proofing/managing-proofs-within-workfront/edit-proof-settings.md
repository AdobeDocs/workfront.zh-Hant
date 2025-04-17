---
product-area: documents;user-management;resource-management
navigation-topic: manage-proofs-within-workfront
title: 編輯校訂設定
description: 在建立校訂後，您可以隨時編輯校訂設定。
author: Courtney
feature: Digital Content and Documents
exl-id: ee30ce2c-e3dc-4863-a69b-cbc1b8747362
source-git-commit: a036a99c13d80a2ba2305ebcdc799ad6e5b62b39
workflow-type: tm+mt
source-wordcount: '633'
ht-degree: 2%

---

# 編輯校訂設定

在建立校訂後，您可以隨時編輯校訂設定。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>目前計畫：Pro或更高版本</p> <p>或</p> <p>舊版計畫：Premium</p> <p>如需有關不同方案的校訂存取許可權的詳細資訊，請參閱<a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">存取Workfront中的校訂功能</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>目前計畫：工作或計畫</p> <p>舊版計畫：任何（您必須為使用者啟用校訂）</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">校樣權限設定檔 </td> 
   <td>經理或以上</td> 
  </tr> 
  <tr> 
   <td role="rowheader">校樣角色</td> 
   <td>作者或版主</td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>編輯檔案的存取權</p> <p>注意：如果您還是沒有存取權，請詢問您的Workfront管理員，他們是否在您的存取層級中設定其他限制。 如需Workfront管理員如何修改存取層級的詳細資訊，請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、角色或校訂許可權設定檔，請連絡您的Workfront或Workfront Proof管理員。

+++

## 編輯校訂設定

如果您的Workfront管理員在帳戶層級停用某些設定，這些設定可能會遭到鎖定。

1. 前往您要校訂的專案、任務或問題，然後按一下「**檔案**」標籤。
1. 將滑鼠移到校訂上，然後按一下&#x200B;**檔案詳細資料**。
1. 在左側面板中，按一下&#x200B;**校訂檢視器設定**。
1. 調整下列設定：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">需要登入。 此校訂無法與訪客使用者共用</td> 
      <td> <p>如果您的稽核和核准流程需要更高的安全性級別，則可以使用需要登入到校訂。 這表示只有Workfront使用者可以新增到校訂中。 使用者必須先輸入電子郵件和密碼，才能存取。</p> <p>注意： <em style="font-style: normal;">如果必須登入，則無法啟用訂閱。</em> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">需要以電子方式簽署決策</td> 
      <td> <p>您可以要求任何對校樣做出決定的稽核者的電子簽章。 當稽核者做出決定時，會出現提示，要求他們輸入電子郵件和密碼並確認其決定。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">完成所有必要的決定時鎖定校訂</td> 
      <td> <p>您可以設定校訂狀態，以在最終核准者做出決定時鎖定。 如果您想要確保檢閱者無法返回校樣並新增其他評論或變更其決定，這將很有用。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">允許下載原始檔案</td> 
      <td> <p>您可以允許校訂上的檢閱者下載建立校訂的原始檔案。 這預設為啟用。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">允許透過公開URL或內嵌代碼共用校訂</td> 
      <td>您可以允許使用者與公共URL或內嵌程式碼共用校訂。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">允許透過公開URL或內嵌程式碼訂閱校訂</td> 
      <td> <p>對校訂啟用訂閱可讓未明確新增到校訂的人員訂閱校訂（也就是將自己新增到校訂中）。 接著，系統會為您指派在訂閱設定中為其選取的角色和電子郵件警示。</p> <p>如果已在校訂上啟用訂閱，則下列欄位將變為使用中：</p> 
       <ul> 
        <li><strong>需要訂閱者驗證</strong> — 訂閱者必須按一下電子郵件中的連結才能存取校訂<br>選取此選項表示訂閱者不會立即存取校訂，但會透過電子郵件取得校訂的連結。 訂閱者驗證的目的是確保該人員輸入了他們有權存取的正確電子郵件地址。</li> 
        <li><strong>新訂閱者的預設角色 — </strong>這是將指派給訂閱校訂的所有檢閱者的預設校訂角色。</li> 
        <li><strong>新訂閱者的預設電子郵件警示</strong> — 這是將指派給所有自行訂閱校訂的稽核者的預設電子郵件警示。</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下「**儲存**」。

 
