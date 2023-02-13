---
content-type: tips-tricks-troubleshooting
product-area: documents
keywords: disable,public,sharing,proof,public,url
navigation-topic: tips-tricks-and-troubleshooting-proofing-within-workfront
title: 停用透過公用URL或內嵌程式碼共用校樣
description: 您可以關閉與公用URL共用校樣的功能，或以校樣方式或個別使用者的校樣內嵌程式碼。
author: Courtney
feature: Digital Content and Documents
exl-id: 73f08e12-f70d-4347-8a5b-441f94d24590
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '320'
ht-degree: 0%

---

# 停用透過公用URL或內嵌程式碼共用校樣

您可以關閉與公用URL共用校樣的功能，或以校樣方式或個別使用者的校樣內嵌程式碼。

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>當前計畫：Pro或更高</p> <p>或</p> <p>舊計畫：Select或Premium</p> <p>如需使用不同計畫校對存取權限的詳細資訊，請參閱 <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">存取Workfront中的校對功能</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>當前計畫：工作或計畫</p> <p>舊計畫：任何（您必須為使用者啟用校對）</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>編輯對文檔的訪問</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、角色或校樣權限設定檔，請聯絡您的Workfront或Workfront Proof管理員。

## 按校樣禁用

您必須是校樣擁有者或建立者，或必須擁有「作者」或「協調者」校樣角色。

1. 在包含校樣的專案中，按一下 **檔案** 中。
1. 將滑鼠移到校樣上並選取 **文檔詳細資訊** .
1. 在左側面板中，按一下 **校對檢視器設定**，然後停用 **允許透過公用URL或內嵌程式碼共用校樣** 核取方塊。

   ![](assets/proofing-viewer-settings-350x200.png)

1. 按一下&#x200B;**儲存**。

## 按用戶禁用

您可以停用Workfront例項中個別使用者的公開校樣設定。 您必須擁有管理員的「證明權限設定檔」才能進行此變更。

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **校對**.
1. 按一下 **帳戶設定** 靠近右上角。
1. 按一下 **使用者** ，然後按一下使用者的名稱。
1. 在 **預設校樣設定** 部分，禁用 **公共共用** 核取方塊。

   ![](assets/default-proof-settings--public-sharing-350x210.png)
