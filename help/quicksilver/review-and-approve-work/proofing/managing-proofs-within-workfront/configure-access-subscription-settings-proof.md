---
product-area: documents;system-administration;setup
navigation-topic: manage-proofs-within-workfront
title: 設定校訂的存取權和訂閱設定
description: 您可以為個別校訂設定特定存取權和訂閱設定，例如是否要求使用者登入以及是否允許使用者訂閱校訂。 您可以在建立校訂時為其設定存取和訂閱設定，也可以為Workfront中已存在的校訂進行設定。
author: Courtney
feature: Digital Content and Documents
exl-id: f242887b-d768-4d56-b530-a1ac6294b2d4
source-git-commit: ac714bd5a5259d6f995ac445efbd0125e07022cb
workflow-type: tm+mt
source-wordcount: '860'
ht-degree: 0%

---

# 設定校訂的存取權和訂閱設定

您可以為個別校訂設定特定存取權和訂閱設定，例如是否要求使用者登入以及是否允許使用者訂閱校訂。 您可以在建立校訂時為其設定存取和訂閱設定，也可以為Workfront中已存在的校訂進行設定。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront套件</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td> 
   <p>標準</p>
   <p>工作或計畫</p> 
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">校樣權限設定檔 </td> 
   <td>經理或以上</td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>編輯檔案的存取權</p></td> 
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 建立校訂時進行存取和訂閱設定

若要在建立校樣時設定校樣的存取權和訂閱設定：

1. 前往您要校訂的專案、任務或問題，然後按一下「**檔案**」區段。
1. 按一下右上角區域的&#x200B;**新增**。
1. 捲動至&#x200B;**新校訂**&#x200B;頁面右下角的&#x200B;**校訂設定**&#x200B;區段。

1. 進行下列設定：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>允許透過公開URL或內嵌程式碼共用校訂</strong> </td> 
      <td>選取此選項時，可透過公用URL或內嵌程式碼共用校訂。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>允許透過公開URL或內嵌程式碼訂閱校訂</strong> </td> 
      <td>選取此選項時，未明確新增到校訂的人員可以訂閱校訂。 訂閱校訂的人員會獲得您在以下設定中定義的角色和電子郵件：
       <ul>
        <li><p><strong>訂閱者角色：</strong>指派給所有訂閱校訂的檢閱者的預設校訂角色。 </p><p>重要：如果Workfront Proof設定中的<strong>允許共用給</strong>設定為<strong>所有人</strong>以外的任何專案，則訂閱僅對組織內的人員有效。 如需詳細資訊，請參閱<a href="../../../workfront-proof/wp-work-proofsfiles/manage-your-work/configure-proof-settings.md" class="MCXref xref">在Workfront Proof中設定校訂設定</a>。</p></li>
        <li><strong>訂閱者的電子郵件警示設定：</strong>指派給所有訂閱校訂的稽核者的預設電子郵件警示。</li>
       </ul><p>
        <ul>
         <li><strong>需要透過電子郵件連結存取校訂：</strong>設定訂閱者是否收到包含校訂連結的電子郵件。 您可以選取<strong>無電子郵件</strong> （存取校訂不需要電子郵件連結）、<strong>僅校訂通知電子郵件</strong> （訂閱者會透過電子郵件收到校訂的連結，而不需要任何驗證）或<strong>驗證和校訂通知電子郵件</strong> （訂閱者會透過電子郵件收到校訂的連結，必須按一下連結才能存取校訂，此選項的目的是確保人員已輸入他們有權存取的正確電子郵件地址）。</li>
        </ul><p>注意：  如果校訂已附加自動化工作流程，則所有訂閱都將向校訂所有者產生確認電子郵件，以便他們決定應將人員新增到哪個階段。<br></p></p></td> 
     </tr> 
    </tbody> 
   </table>

1. 繼續建立您的校訂。

## 設定現有校訂的存取權和訂閱設定

若要針對Workfront中已存在的校訂設定存取權和訂閱設定：

1. 在[檔案]區域中，選取包含您要設定之校訂的檔案，然後按一下[檔案詳細資料] ****。
1. 在左側面板中，按一下&#x200B;**校訂檢視器設定**。
1. 進行下列設定：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>允許透過公開URL或內嵌程式碼共用校訂</strong><strong>e</strong> </td> 
      <td>選取此選項時，可透過公用URL或內嵌程式碼共用校訂。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>允許透過公開URL或內嵌程式碼訂閱校訂</strong> </td> 
      <td>選取此選項時，未明確新增到校訂的人員可以訂閱校訂。 訂閱校訂的人員會獲得您在以下設定中定義的角色和電子郵件：
       <ul>
        <li><p><strong>訂閱者角色：</strong>指派給所有訂閱校訂的檢閱者的預設校訂角色。 </p><p>重要：如果Workfront Proof設定中的<strong>允許共用給</strong>設定為<strong>所有人</strong>以外的任何專案，則訂閱僅對組織內的人員有效。 如需詳細資訊，請參閱<a href="../../../workfront-proof/wp-work-proofsfiles/manage-your-work/configure-proof-settings.md" class="MCXref xref">在Workfront Proof中設定校訂設定</a>。</p></li>
        <li><strong>訂閱者的電子郵件警示設定：</strong>指派給所有訂閱校訂的稽核者的預設電子郵件警示。</li>
       </ul><p>
        <ul>
         <li><strong>需要透過電子郵件連結存取校訂：</strong>設定訂閱者是否收到包含校訂連結的電子郵件。 您可以選取<strong>無電子郵件</strong> （存取校訂不需要電子郵件連結）、<strong>僅校訂通知電子郵件</strong> （訂閱者會透過電子郵件收到校訂的連結，而不需要任何驗證）或<strong>驗證和校訂通知電子郵件</strong> （訂閱者會透過電子郵件收到校訂的連結，必須按一下連結才能存取校訂，此選項的目的是確保人員已輸入他們有權存取的正確電子郵件地址）。</li>
        </ul><p>注意：  如果校訂已附加自動化工作流程，則所有訂閱都將向校訂所有者產生確認電子郵件，以便他們決定應將人員新增到哪個階段。<br></p></p></td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下「**儲存**」。
