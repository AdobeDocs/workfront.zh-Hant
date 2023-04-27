---
product-area: workfront-integrations
navigation-topic: workfront-for-outlook
title: 設定 [!DNL Adobe Workfront] for [!DNL Outlook]
description: Adobe Workfront Fusion提供與Outlook的整合。 本文說明如何在自己的工作流程中開始使用此整合。
author: Becky
feature: Workfront Integrations and Apps
exl-id: 57f0560b-68c2-4654-863e-bd728e76da29
source-git-commit: 61a107e1ee8a415fd94e73fc65fa5f59f7de02d1
workflow-type: tm+mt
source-wordcount: '761'
ht-degree: 0%

---

# 設定 [!DNL Adobe Workfront for Outlook]

此 [!DNL Adobe Workfront] [!DNL Outlook] 增益集可讓您執行下列索引鍵 [!DNL Workfront] 直接從Outlook執行任務：

* 更新來自電子郵件的資訊的現有項目、任務或問題。 如需詳細資訊，請參閱 [從 [!DNL Outlook] 電子郵件](../../workfront-integrations-and-apps/using-workfront-with-outlook/update-an-existing-object-from-an-outlook-email.md).
* 建立 [!DNL Workfront] 根據內的電子郵件要求 [!DNL Outlook]. 如需詳細資訊，請參閱 [從 [!DNL Outlook] 電子郵件](../../workfront-integrations-and-apps/using-workfront-with-outlook/create-a-wf-request-from-an-outlook-email.md).
* 將電子郵件新增為 [!UICONTROL 我的工作] 的上界。 如需詳細資訊，請參閱 [新增 [!DNL Outlook] 將電子郵件作為工作清單的任務](../../workfront-integrations-and-apps/using-workfront-with-outlook/add-outlook-email-as-task-to-your-work-list.md).
* 透過 [!DNL Workfront] 用於 [!DNL Outlook]. 有關回覆Workfront意見的資訊，請參閱 [!DNL Outlook]，請參閱 [回復來自 [!DNL Outlook]](../../workfront-integrations-and-apps/using-workfront-with-outlook/reply-to-a-comment-from-outlook.md).
* 從草稿開始建立工作和問題，或從現有電子郵件建立工作和問題（使用拖放功能）。 如需詳細資訊，請參閱 [新增 [!DNL Outlook] 以任務或問題形式將電子郵件發送到項目](../../workfront-integrations-and-apps/using-workfront-with-outlook/add-outlook-email-to-project-as-task-or-issue.md).

您必須新增 [!DNL Workfront] 新增至 [!DNL Outlook] 帳戶，您才能使用 [!DNL Workfront for Outlook].

如果您無法安裝 [!DNL Workfront] 與 [!DNL Outlook] 帳戶，請連絡您的 [!DNL Workfront] 管理員確保 [!DNL Outlook] 已為貴組織啟用增益集。

如需如何啟用 [!DNL Outlook] 貴組織的整合，請參閱 [啟用 [!DNL Adobe Workfront for Outlook]](../../administration-and-setup/configure-integrations/enable-workfront-for-outlook.md).

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計劃*</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權*</td> 
   <td> <p>[!UICONTROL工作], [!UICONTROL計畫]</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的 [!DNL Workfront] 管理員。

## 必要條件

您的 [!DNL Workfront] 管理員必須啟用 [!DNL Outlook for Office] with [!DNL Workfront] 才能使用此整合。

## 系統需求

可使用下列應用程式：

* **[!DNL Outlook]在網上：** 此 [!DNL Workfront] 使用時可使用增益集 [!DNL Outlook] 在桌上型電腦或行動裝置上使用網頁瀏覽器。 使用 [!DNL Outlook] 網頁應用程式。
* **[!DNL Outlook]案頭應用程式：** 此 [!DNL Workfront] 使用時，可使用增益集 [!DNL Windows] 和 [!DNL Mac] 案頭版本 [!DNL Outlook] 隨附 [!DNL Office] 包。

此 [!DNL Workfront] 用於 [!DNL Outlook] 在符合下列需求的環境中支援：

* [用戶端需求](#client-requirements-client-requirements)
* [郵件伺服器需求](#mail-server-requirements-mail-server-requirements)

### 用戶端需求 {#client-requirements}

我們支援下列版本 [!DNL Outlook]:

* [!DNL Outlook 2013] 或更新版本 [!DNL Windows]
*[!DNL  Outlook 2016] 或更新版本 [!DNL Windows]
* [!DNL Outlook] on [!DNL Mac] ([!DNL Microsoft 365])
* [!DNL Outlook] on [!DNL Windows] ([!DNL Microsoft 365])
* [!DNL Outlook] 在網路上

您必須連線至 [!DNL Exchange Server] 或 [!DNL Office 365] 使用直接連線。

配置客戶端時，用戶必須選擇以下帳戶類型之一：

* [!DNL Exchange]
* [!DNL Office 365]
* [!DNL Outlook.com]&#x200B;**&#x200B;**&#x200B;如果客戶端配置為與POP3或IMAP連接，則 [!DNL Workfront] 載入項未載入。

### 郵件伺服器需求 {#mail-server-requirements}

當您連接到 [!DNL Office 365] 或 [!DNL Outlook.com]. 不過，如果您已連線至內部部署的 [!DNL Exchange Server]，則適用下列要求：

* 我們支援所有 [!DNL Exchange On-Premise] 伺服器
* [!DNL Exchange Web Services] (EWS)必須啟用，並且必須向Internet公開。
* 伺服器必須具有有效的驗證證書，伺服器才能發出有效的身份令牌。 新安裝 [!DNL Exchange Server] 包含預設驗證憑證。

   <!--this used to be here but Dev asked for it to be taken out - logged issue for editing this article on 4-26-2023: For more information, see [Digital certificates and encryption in [!DNL Exchange 2016]](https://technet.microsoft.com/en-us/library/dd351044(v=exchg.160).aspx) and [Set-AuthConfig](https://technet.microsoft.com/en-us/library/jj215766(v=exchg.160).aspx).-->

* 若要存取 [!DNL Workfront] 從 [[!DNL Office] 商店](https://store.office.com/)，您的用戶端存取伺服器必須能夠與  [https://store.office.com](https://store.office.com/).

如需支援環境的詳細資訊，請參閱 [[!DNL Microsoft Office 365] 首頁](https://products.office.com/en-us/office-365-home).

## 安裝載入項

如需設定 [!DNL Workfront] 用於 [!DNL Outlook]，請參閱 [[!DNL Workfront]  — 協作工作管理。](https://appsource.microsoft.com/en-us/product/office/WA104380943?tab=Overview)

* [[!DNL Workfront] 針對 [!DNL Outlook 365]](#workfront-for-outlook-365-workfront-for-outlook-365)
* [[!DNL Workfront] for [!DNL Outlook] 在網路上](#workfront-for-outlook-on-the-web-workfront-for-outlook-on-the-web)
* [[!DNL Workfront] for [!DNL Outlook] on [!DNL Windows] 或 [!DNL Mac]](#workfront-for-outlook-on-windows-or-mac-workfront-for-outlook-on-windows-or-mac)

### [!DNL Workfront] 針對 [!DNL Outlook 365] {#workfront-for-outlook-365}

1. 在 [!DNL Outlook 365]，按一下 **[!UICONTROL 瀏覽載入項]** 圖示 ![](assets/outlook-add-in-26x26.png)在Office 365介面頂部，按一下 **[!UICONTROL 管理載入項]**.

1. 在 **[!UICONTROL 搜尋增益集]** 框，搜索 **[!DNL Workfront]** 然後按下 [!UICONTROL 輸入].

1. 按一下 **[!UICONTROL 新增]**.

### [!DNL Workfront] for [!DNL Outlook] 在網路上 {#workfront-for-outlook-on-the-web}

1. 開啟 [!DNL Microsoft Outlook] 在網頁瀏覽器中。
1. 按一下 **[!UICONTROL 瀏覽] 增益集** 圖示 ![](assets/outlook-add-in-web-version-20x20.png).

   若要尋找圖示，請參閱 [在中使用增益集 [!DNL Outlook] 在網路上](https://support.microsoft.com/en-us/office/using-add-ins-in-outlook-on-the-web-8f2ce816-5df4-44a5-958c-f7f9d6dabdce#bkmk_addaddinsicon) 在Microsoft檔案中。

1. 搜尋 **[!DNL Workfront]** 在 **[!UICONTROL 搜尋增益集]** 欄位，然後按 **[!UICONTROL 輸入]**.

1. 當它出現在清單上時，按一下 **新增**.

### [!DNL Workfront for Outlook] on [!UICONTROL Windows] 或 [!DNL Mac] {#workfront-for-outlook-on-windows-or-mac}

1. 按一下 **[!UICONTROL 首頁]** > **[!UICONTROL 商店]** 在絲帶上。

1. 搜尋 **[!DNL Workfront]** 在 **[!UICONTROL 搜尋]** 欄位，然後按 **[!UICONTROL 輸入]**.

1. 按一下切換以啟用 **[!UICONTROL [!DNL Workfront]載入項]**.

## 登入 [!DNL Workfront] 從 [!DNL Outlook]

1. 在 [!DNL Outlook]，請選取電子郵件訊息，然後按一下 **[!DNL Workfront]** 圖示。
1. 按照提示登錄 [!DNL Workfront] 使用增強驗證、OAuth 2.0或您的安全斷言標籤語言(SAML)URL。

   使用者登入之前 [!DNL Workfront] 使用SAML的增益集， [!DNL Workfront] 管理員必須先啟用 [!DNL Office 365] 使用SAML 2.0解決方案進行驗證的增益集。 如需詳細資訊，請參閱 [設定 [!DNL Adobe Workfront] 搭配SAML 2.0](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md#enable-saml-with-office-365) 在文章中 [設定 [!DNL Adobe Workfront] 搭配SAML 2.0](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md).

   >[!NOTE]
   >
   >* 當系統提示您輸入 [!DNL Workfront] 帳戶，請使用此格式輸入： *yourCompany&#39;sDomain.my.workfront.com*. 您公司的網域通常是您公司的名稱。
   >* 增強驗證必須在 [!DNL Workfront] 管理員會啟用此整合。


