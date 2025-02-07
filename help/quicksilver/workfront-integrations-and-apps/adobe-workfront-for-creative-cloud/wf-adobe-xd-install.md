---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-for-creative-cloud
title: 安裝並開啟適用於XD的Adobe Workfront
description: 您可以從Adobe市集安裝適用於XD的Adobe Workfront外掛程式。
author: Courtney
feature: Workfront Integrations and Apps, Digital Content and Documents
exl-id: d4971977-b5bd-4bb4-a1c2-44829a67d32d
source-git-commit: 494c7bf8aaf3570d4a01b5e88b85410ee3f52f18
workflow-type: tm+mt
source-wordcount: '474'
ht-degree: 1%

---

# 安裝並開啟[!DNL Adobe Workfront for XD]

您可以從Adobe市集安裝[!DNL Adobe Workfront for XD]外掛程式。 外掛程式支援下列語言：

* 英文
* 法文
* 德文
* 義大利文
* 西班牙文
* 葡萄牙文
* 日文
* 簡體中文
* 繁體中文
* 韓文

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
 <!-- <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!UICONTROL Pro] or higher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!UICONTROL Work] or [!UICONTROL Plan]</p> </td> 
  </tr> -->
  <tr> 
   <td role="rowheader">產品</td> 
   <td><p>除了[!DNL Workfront]授權之外，您還必須有[!DNL Adobe Creative Cloud]授權。</p><p>如需詳細資訊，請參閱<a href="https://helpx.adobe.com/support/programs/cc-support-policy.html#cce" class="MCXref xref" xrefformat="{para}">Creative Cloud支援政策</a>。</p></td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的[!DNL Workfront]管理員。

+++

## 先決條件

* 您必須先安裝[!DNL Adobe XD]應用程式才能安裝Workfront外掛程式。

## 為您的組織安裝[!DNL Adobe Workfront for XD]外掛程式

如果您是[!DNL Adobe Admin Console]管理員，可以在[!DNL Creative Cloud]部署套件中包含外掛程式。 如需詳細資訊，請參閱[在套件中包含外掛程式](https://helpx.adobe.com/in/enterprise/using/manage-extensions.html)。

[在此觀看教學課程影片](https://www.youtube.com/watch?v=zzvXNLIBzrc){target=_blank}。

[!DNL Adobe Admin Console]管理員也可以建立僅含外掛程式的套件，以分發給使用者。 如需詳細資訊，請參閱 [!DNL Adobe Admin Console]](/help/quicksilver/administration-and-setup/configure-integrations/create-plugin-only-packages.md)中的[為您的使用者建立 [!DNL Creative Cloud]] 套裝的[！UICONTROL [!DNL Adobe Workfront] 

## 個別安裝[!DNL Adobe Workfront for XD]外掛程式

您可以從[!DNL Adobe Exchange]自行安裝[!DNL Adobe Workfront for XD]外掛程式。

1. 前往Adobe Exchange上的[Adobe Workfront for XD安裝頁面](https://exchange.adobe.com/apps/cc/4c3566f9?pluginId=4c3566f9&amp;workflow=share)。
1. 在出現的對話方塊中，按一下&#x200B;**開啟[!DNL Adobe Creative Cloud]案頭應用程式**。
1. 在[!DNL Adobe XD]外掛程式管理員開啟後，按一下&#x200B;**[!UICONTROL 安裝]**。
1. 讀取對話方塊中的資訊，然後按一下[確定]。****
1. 請繼續參閱下節，瞭解如何開啟外掛程式的詳細資訊。

## 開啟[!DNL Adobe Workfront for XD]外掛程式

1. 開啟[!DNL Adobe XD]。

1. 建立新檔案，或開啟現有檔案。

1. 在左下角，按一下&#x200B;**外掛程式**&#x200B;圖示。

![XD外掛程式視窗](assets/xd-plugin-window-350x620.png)

1. 在&#x200B;**[!UICONTROL 外掛程式面板]**&#x200B;中，找到&#x200B;**[!UICONTROL 適用於XD]**&#x200B;的Adobe Workfront。

1. 請繼續參閱下節，瞭解如何登入外掛程式的詳細資訊。

## 登入[!DNL Adobe Workfront for XD]

1. 確定外掛程式面板已開啟，然後按一下&#x200B;**[!DNL Adobe Workfront for XD]**。
1. 輸入您的網域，然後按一下&#x200B;**[!UICONTROL 登入]**。 瀏覽器頁面隨即開啟。

   >[!TIP]
   >
   >* 若要尋找您的網域，請開啟瀏覽器、導覽至您的[!DNL Workfront]執行個體，並複製URL的第一個部分：\
   >![尋找網域](assets/domain-350x50.png)
   >
   > * 如果您的Workfront執行個體已與Experience Cloud整合，請要求您的管理員提供您Admin Console中「產品> Workfront」底下的Workfront網域。

1. 在瀏覽器中輸入您的[!DNL Workfront]認證，然後按一下&#x200B;**[!DNL Log in]**。 如果貴公司使用單一登入(SSO)，系統會將您導向至SSO提供者的頁面以登入。

   >[!NOTE]
   >
   >如果您最近登入，系統可能不會提示您輸入您的[!DNL Workfront]認證。

   依照提示登入[!DNL Workfront]。

   >[!NOTE]
   >
   >* [!DNL Workfront]使用OAuth 2.0連線至[!DNL Adobe Creative Cloud]，這是大部分網頁式整合所使用的安全標準，用於驗證及授權使用者。
   >* 當系統提示您輸入[!DNL Workfront]帳戶的[網域或主機]時，請使用下列格式輸入它： *yourCompany&#39;sDomain.my.workfront.com*。 您公司的網域通常是您公司的名稱。

1. 按一下&#x200B;**[!UICONTROL 允許存取]**&#x200B;以完成登入，然後返回[!DNL Adobe XD]檢視您的工作。

 
