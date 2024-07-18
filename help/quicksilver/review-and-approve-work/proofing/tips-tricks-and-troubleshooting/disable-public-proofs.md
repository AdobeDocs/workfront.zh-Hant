---
content-type: tips-tricks-troubleshooting
product-area: documents
keywords: 停用，公用，共用，校訂，公用，url
navigation-topic: tips-tricks-and-troubleshooting-proofing-within-workfront
title: 停用透過公開URL或內嵌程式碼共用校訂
description: 您可以關閉與公共URL共用校訂或根據校訂嵌入程式碼或為個別使用者共用校訂的功能。
author: Courtney
feature: Digital Content and Documents
exl-id: 73f08e12-f70d-4347-8a5b-441f94d24590
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '315'
ht-degree: 0%

---

# 停用透過公開URL或內嵌程式碼共用校訂

您可以關閉與公共URL共用校訂或根據校訂嵌入程式碼或為個別使用者共用校訂的功能。

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>目前計畫：Pro或更高版本</p> <p>或</p> <p>舊版計畫：選擇或Premium</p> <p>如需有關不同方案的校訂存取許可權的詳細資訊，請參閱<a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">存取Workfront中的校訂功能</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>目前計畫：工作或計畫</p> <p>舊版計畫：任何（您必須為使用者啟用校訂）</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>編輯檔案的存取權</p> <p>如需請求其他存取權的資訊，請參閱<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求物件</a>的存取權。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、角色或校訂許可權設定檔，請連絡您的Workfront或Workfront Proof管理員。

## 根據校訂停用

您必須是校訂擁有者或建立者，或您必須擁有作者或版主校訂角色。

1. 在包含校訂的專案中，按一下左側面板中的&#x200B;**檔案**。
1. 將滑鼠停留在校訂上，並選取&#x200B;**檔案詳細資訊**。
1. 在左側面板中，按一下&#x200B;**校訂檢視器設定**，然後停用&#x200B;**允許透過公用URL或內嵌程式碼共用校訂**&#x200B;核取方塊。

   ![](assets/proofing-viewer-settings-350x200.png)

1. 按一下「**儲存**」。

## 為每個使用者停用

您可以在Workfront執行個體中停用個別使用者的公開校訂設定。 您必須擁有管理員的校訂許可權設定檔，才能進行此變更。

1. 按一下Adobe Workfront右上角的&#x200B;**主要功能表**&#x200B;圖示![](assets/main-menu-icon.png)，然後按一下&#x200B;**校訂**。
1. 按一下右上角附近的&#x200B;**帳戶設定**。
1. 按一下&#x200B;**使用者**&#x200B;標籤，然後按一下使用者名稱。
1. 在&#x200B;**預設校訂設定**&#x200B;區段中，停用&#x200B;**公用共用**&#x200B;核取方塊。

   ![](assets/default-proof-settings--public-sharing-350x210.png)
