---
product-area: documents;system-administration;setup
navigation-topic: manage-proofs-within-workfront
title: 配置校樣的訪問和訂閱設定
description: 您可以為個別校樣設定特定的存取和訂閱設定，例如是否要求使用者登入，以及是否允許使用者訂閱校樣。 您可以在建立校樣時，為校樣設定存取權和訂閱設定，或為已存在於Workfront中的校樣設定校樣。
author: Courtney
feature: Digital Content and Documents
exl-id: f242887b-d768-4d56-b530-a1ac6294b2d4
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '949'
ht-degree: 0%

---

# 配置校樣的訪問和訂閱設定

您可以為個別校樣設定特定的存取和訂閱設定，例如是否要求使用者登入，以及是否允許使用者訂閱校樣。 您可以在建立校樣時，為校樣設定存取權和訂閱設定，或為已存在於Workfront中的校樣設定校樣。

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
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>編輯對文檔的訪問</p> <p>注意：如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、角色或校樣權限設定檔，請聯絡您的Workfront或Workfront Proof管理員。

## 建立校樣時配置存取和訂閱設定

若要在建立校樣時設定校樣的存取權和訂閱設定：

1. 前往您要校樣的專案、任務或問題，然後按一下 **檔案** 區段。
1. 按一下 **新增** 在右上角。
1. 捲動至 **校樣設定** 區段 **新校樣** 頁面。

1. 配置下列設定：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>允許透過公用URL或內嵌程式碼共用校樣</strong> </td> 
      <td>選取此選項時，可透過公用URL或內嵌程式碼來共用校樣。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>允許透過公用URL或內嵌程式碼訂閱校樣</strong> </td> 
      <td>選取此選項時，尚未明確新增至校樣的人員可訂閱校樣。 訂閱校樣的人員會獲得您在下列設定中定義的角色和電子郵件：
       <ul>
        <li><p><strong>訂閱者角色：</strong> 分配給訂閱校樣的所有審核者的預設校樣角色。 </p><p>重要：若 <strong>允許與共用</strong> 設為 <strong>每個人</strong> 在Workfront校樣設定中，訂閱僅適用於組織內的人員。 如需詳細資訊，請參閱 <a href="../../../workfront-proof/wp-work-proofsfiles/manage-your-work/configure-proof-settings.md" class="MCXref xref">在Workfront校樣中設定校樣設定</a>.</p></li>
        <li><strong>訂閱者的電子郵件警報設定：</strong> 指派給訂閱校樣之所有審核者的預設電子郵件警報。</li>
       </ul><p>
        <ul>
         <li><strong>下列項目需要透過電子郵件連結進行校樣存取：</strong> 設定訂閱者是否收到包含校樣連結的電子郵件。 您可以選取 <strong>無電子郵件</strong> （存取校樣不需要電子郵件連結）, <strong>僅校樣通知電子郵件</strong> （訂閱者會透過電子郵件收到校樣的連結，無需任何驗證），或 <strong>驗證和校樣通知電子郵件</strong> （訂閱者會透過電子郵件收到校樣的連結，且必須按一下連結才能存取校樣，此選項的目的是確保使用者已輸入其有權存取的正確電子郵件地址）。</li>
        </ul><p>注意： 如果校樣已附加「自動化工作流程」 ，則所有訂閱都會產生確認電子郵件給校樣擁有者，讓他們決定應將人員新增至哪個階段。<br></p></p></td> 
     </tr> 
    </tbody> 
   </table>

1. 繼續建立校樣。

## 配置現有校樣的訪問和訂閱設定

若要設定已存在於Workfront中校樣的存取權和訂閱設定：

1. 在「文檔」區域中，選擇包含要配置設定的校樣的文檔，然後按一下 **文檔詳細資訊**.
1. 在左側面板中，按一下 **校對檢視器設定**.
1. 配置下列設定：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>允許透過公用URL或內嵌程式碼共用校樣</strong><strong>e</strong> </td> 
      <td>選取此選項時，可透過公用URL或內嵌程式碼來共用校樣。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>允許透過公用URL或內嵌程式碼訂閱校樣</strong> </td> 
      <td>選取此選項時，尚未明確新增至校樣的人員可訂閱校樣。 訂閱校樣的人員會獲得您在下列設定中定義的角色和電子郵件：
       <ul>
        <li><p><strong>訂閱者角色：</strong> 分配給訂閱校樣的所有審核者的預設校樣角色。 </p><p>重要：若 <strong>允許與共用</strong> 設為 <strong>每個人</strong> 在Workfront校樣設定中，訂閱僅適用於組織內的人員。 如需詳細資訊，請參閱 <a href="../../../workfront-proof/wp-work-proofsfiles/manage-your-work/configure-proof-settings.md" class="MCXref xref">在Workfront校樣中設定校樣設定</a>.</p></li>
        <li><strong>訂閱者的電子郵件警報設定：</strong> 指派給訂閱校樣之所有審核者的預設電子郵件警報。</li>
       </ul><p>
        <ul>
         <li><strong>下列項目需要透過電子郵件連結進行校樣存取：</strong> 設定訂閱者是否收到包含校樣連結的電子郵件。 您可以選取 <strong>無電子郵件</strong> （存取校樣不需要電子郵件連結）, <strong>僅校樣通知電子郵件</strong> （訂閱者會透過電子郵件收到校樣的連結，無需任何驗證），或 <strong>驗證和校樣通知電子郵件</strong> （訂閱者會透過電子郵件收到校樣的連結，且必須按一下連結才能存取校樣，此選項的目的是確保使用者已輸入其有權存取的正確電子郵件地址）。</li>
        </ul><p>注意： 如果校樣已附加「自動化工作流程」 ，則所有訂閱都會產生確認電子郵件給校樣擁有者，讓他們決定應將人員新增至哪個階段。<br></p></p></td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下&#x200B;**儲存**。
