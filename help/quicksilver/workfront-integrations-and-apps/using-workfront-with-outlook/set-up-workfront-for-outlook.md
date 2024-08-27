---
product-area: workfront-integrations
navigation-topic: workfront-for-outlook
title: 為 [!DNL Outlook]設定 [!DNL Adobe Workfront]
description: ' [!DNL Adobe Workfront] [!DNL Outlook]增益集可讓您直接從Outlook執行索引鍵 [!DNL Workfront] 工作。'
author: Becky
feature: Workfront Integrations and Apps
exl-id: 57f0560b-68c2-4654-863e-bd728e76da29
source-git-commit: bcf03609e0503a5db0384fd573066467a1feb341
workflow-type: tm+mt
source-wordcount: '682'
ht-degree: 0%

---

# 設定[!DNL Adobe Workfront for Outlook]

<!-- Audited: 12/2023 -->

[!DNL Adobe Workfront] [!DNL Outlook]增益集可讓您直接從Outlook執行下列主要的[!DNL Workfront]工作：

* 使用電子郵件中的資訊更新現有的專案、任務或問題。 如需詳細資訊，請參閱[從 [!DNL Outlook] 電子郵件](../../workfront-integrations-and-apps/using-workfront-with-outlook/update-an-existing-object-from-an-outlook-email.md)更新現有的物件。
* 根據[!DNL Outlook]內的電子郵件建立[!DNL Workfront]要求。 如需詳細資訊，請參閱[從 [!DNL Outlook] 電子郵件建立Adobe Workfront要求](../../workfront-integrations-and-apps/using-workfront-with-outlook/create-a-wf-request-from-an-outlook-email.md)。
* 新增電子郵件作為您[!UICONTROL 我的工作]區域中的工作。 如需詳細資訊，請參閱[將 [!DNL Outlook] 電子郵件新增為工作清單](../../workfront-integrations-and-apps/using-workfront-with-outlook/add-outlook-email-as-task-to-your-work-list.md)的工作。
* 透過[!DNL Outlook]的[!DNL Workfront]增益集回覆註解。 如需有關回覆[!DNL Outlook]來自Workfront的註解的資訊，請參閱[回覆來自 [!DNL Outlook]](../../workfront-integrations-and-apps/using-workfront-with-outlook/reply-to-a-comment-from-outlook.md)的註解。
* 從頭開始建立任務和問題，或從現有電子郵件建立（使用拖放功能）。 如需詳細資訊，請參閱[將 [!DNL Outlook] 電子郵件作為任務或問題新增至專案](../../workfront-integrations-and-apps/using-workfront-with-outlook/add-outlook-email-to-project-as-task-or-issue.md)。

您必須先將[!DNL Workfront]增益集新增至您的[!DNL Outlook]帳戶，才能使用[!DNL Workfront for Outlook]。

如果您無法使用您的[!DNL Outlook]帳戶安裝[!DNL Workfront]增益集，請連絡您的[!DNL Workfront]系統管理員，以確保您的組織已啟用[!DNL Outlook]增益集。

如需有關如何為您的組織啟用[!DNL Outlook]整合的資訊，請參閱[啟用 [!DNL Adobe Workfront for Outlook]](../../administration-and-setup/configure-integrations/enable-workfront-for-outlook.md)。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計劃</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權</td> 
   <td> 
   <p>新計畫： [！UICONTROL Standard]</p> 
   <p>目前計畫：[！UICONTROL Work]， [！UICONTROL Plan]</p> </td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 先決條件

您的[!DNL Workfront]管理員必須以[!DNL Workfront]啟用[!DNL Outlook for Office]，您才能使用此整合。

## 系統需求

下列應用程式可供使用：

* 在網頁上&#x200B;**[!DNL Outlook]：**&#x200B;在案頭或行動裝置上使用網頁瀏覽器中的[!DNL Outlook]時，可以使用[!DNL Workfront]增益集。 使用[!DNL Outlook]網頁應用程式時也可以使用此功能。
* **[!DNL Outlook]案頭應用程式：**&#x200B;使用[!DNL Office]套件所包含的[!DNL Outlook]的[!DNL Windows]和[!DNL Mac]案頭版本時，可以使用[!DNL Workfront]增益集。

符合下列需求的環境支援[!DNL Outlook]的[!DNL Workfront]增益集：

* [使用者端需求](#client-requirements-client-requirements)
* [郵件伺服器需求](#mail-server-requirements-mail-server-requirements)

### 使用者端需求 {#client-requirements}

Workfront支援下列[!DNL Outlook]版本：

* [!DNL Outlook 2013]或更新於[!DNL Windows]
* [!DNL Outlook 2016]或更新於[!DNL Windows]
* [!DNL Outlook]於[!DNL Mac] ([!DNL Microsoft 365])
* [!DNL Outlook]於[!DNL Windows] ([!DNL Microsoft 365])
* 網路[!DNL Outlook]

您必須使用直接連線來連線至[!DNL Exchange Server]或[!DNL Office 365]。

設定使用者端時，使用者必須選取下列其中一個帳戶型別：

* [!DNL Exchange]
* [!DNL Office 365]
* [!DNL Outlook.com]如果使用者端設定為連線至POP3或IMAP，則無法載入[!DNL Workfront]增益集。

### 郵件伺服器需求 {#mail-server-requirements}

當您連線到[!DNL Office 365]或[!DNL Outlook.com]時，預設會符合郵件伺服器需求。 但是，如果您已連線到內部部署安裝的[!DNL Exchange Server]，則適用下列要求：

* Workfront支援所有[!DNL Exchange On-Premise]伺服器
* [!DNL Exchange Web Services] (EWS)必須已啟用，且必須公開至網際網路。
* 伺服器必須具備有效的驗證憑證，伺服器才能核發有效的身分識別權杖。 [!DNL Exchange Server]的新安裝包含預設的驗證憑證。

  <!--this used to be here but Dev asked for it to be taken out - logged issue for editing this article on 4-26-2023: For more information, see [Digital certificates and encryption in [!DNL Exchange 2016]](https://technet.microsoft.com/en-us/library/dd351044(v=exchg.160).aspx) and [Set-AuthConfig](https://technet.microsoft.com/en-us/library/jj215766(v=exchg.160).aspx).-->

* 若要從[[!DNL Office] 存放區](https://store.office.com/)存取[!DNL Workfront]增益集，您的使用者端存取伺服器必須能夠與[https://store.office.com](https://store.office.com/)通訊。

如需支援環境的詳細資訊，請參閱[[!DNL Microsoft Office 365] 首頁](https://products.office.com/en-us/office-365-home)。

## 安裝增益集

您可以從[Microsoft市集](https://appsource.microsoft.com/en-us/product/office/WA104380943?tab=Overview)取得適用於Outlook的Workfront增益集。

### [!DNL Outlook 365]的[!DNL Workfront] {#workfront-for-outlook-365}

1. 在[!DNL Outlook 365]中，按一下Office 365介面頂端的&#x200B;**[!UICONTROL 瀏覽增益集]**&#x200B;圖示![](assets/outlook-add-in-26x26.png)，然後按一下&#x200B;**[!UICONTROL 管理增益集]**。

1. 在&#x200B;**[!UICONTROL 搜尋增益集]**&#x200B;方塊中，搜尋&#x200B;**[!DNL Workfront]**，然後按下[!UICONTROL Enter]。

1. 按一下&#x200B;**[!UICONTROL 新增]**。

### 網路上的[!DNL Outlook]的[!DNL Workfront] {#workfront-for-outlook-on-the-web}

1. 在網頁瀏覽器中開啟[!DNL Microsoft Outlook]。
1. 按一下&#x200B;**[!UICONTROL 瀏覽]增益集**&#x200B;圖示![](assets/outlook-add-in-web-version-20x20.png)。

   若要尋找圖示，請參閱Microsoft檔案中的[在網頁上 [!DNL Outlook] 使用增益集](https://support.microsoft.com/en-us/office/using-add-ins-in-outlook-on-the-web-8f2ce816-5df4-44a5-958c-f7f9d6dabdce#bkmk_addaddinsicon)。

1. 在&#x200B;**[!UICONTROL 搜尋增益集]**&#x200B;欄位中搜尋&#x200B;**[!DNL Workfront]**，然後按&#x200B;**[!UICONTROL Enter]**。

1. 當它出現在清單中時，按一下&#x200B;**新增**。

### [!UICONTROL Windows]或[!DNL Mac]上的[!DNL Workfront for Outlook] {#workfront-for-outlook-on-windows-or-mac}

1. 按一下功能區上的&#x200B;**[!UICONTROL 首頁]** > **[!UICONTROL 商店]**。

1. 在&#x200B;**[!UICONTROL 搜尋]**&#x200B;欄位中搜尋&#x200B;**[!DNL Workfront]**，然後按&#x200B;**[!UICONTROL Enter]**。

1. 按一下切換即可啟用&#x200B;**[!UICONTROL [!DNL Workfront]增益集]**。

## 從[!DNL Outlook]登入[!DNL Workfront]

1. 在[!DNL Outlook]中，選取電子郵件訊息，然後按一下電子郵件標題中的&#x200B;**[!DNL Workfront]**&#x200B;圖示。
1. 在登入頁面上，按一下&#x200B;**登入Workfront**。
1. 依照提示使用OAuth 2.0登入[!DNL Workfront]。<!--Enhanced Authentication or your Security Assertion Markup Language (SAML) URL.-->

   <!--Before users can log in to the [!DNL Workfront] add-in using SAML, a [!DNL Workfront] administrator must first enable [!DNL Office 365] add-ins to authenticate using a SAML 2.0 solution. For more information, see the section [Configure [!DNL Adobe Workfront] with SAML 2.0](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md#enable-saml-with-office-365) in the article [Configure [!DNL Adobe Workfront] with SAML 2.0](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md).-->

   >[!NOTE]
   >
   >* 如果系統提示您輸入[!DNL Workfront]帳戶的網域，請以此格式輸入： *yourCompany&#39;sDomain.my.workfront.com*。 您公司的網域通常是您公司的名稱。

<!--ADDITIONAL BULLET REMOVED FROM NOTE BOX: Enhanced Authentication is not available until a Workfront administrator enables it for this integration.-->
