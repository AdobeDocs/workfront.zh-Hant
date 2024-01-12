---
product-area: workfront-integrations
navigation-topic: workfront-for-outlook
title: 設定 [!DNL Adobe Workfront] 的 [!DNL Outlook]
description: 此 [!DNL Adobe Workfront] [!DNL Outlook] 增益集可讓您執行金鑰 [!DNL Workfront] 直接從Outlook執行工作。
author: Becky
feature: Workfront Integrations and Apps
exl-id: 57f0560b-68c2-4654-863e-bd728e76da29
source-git-commit: 8382b69e6a55af69397dd8f566395143f3c1dcd3
workflow-type: tm+mt
source-wordcount: '727'
ht-degree: 0%

---

# 設定 [!DNL Adobe Workfront for Outlook]

<!-- Audited: 12/2023 -->

此 [!DNL Adobe Workfront] [!DNL Outlook] 增益集可讓您執行下列索引鍵 [!DNL Workfront] 直接從Outlook執行工作：

* 使用電子郵件中的資訊更新現有的專案、任務或問題。 如需詳細資訊，請參閱 [從更新現有物件 [!DNL Outlook] 電子郵件](../../workfront-integrations-and-apps/using-workfront-with-outlook/update-an-existing-object-from-an-outlook-email.md).
* 建立 [!DNL Workfront] 根據中的電子郵件提出請求 [!DNL Outlook]. 如需詳細資訊，請參閱 [從建立Adobe Workfront請求 [!DNL Outlook] 電子郵件](../../workfront-integrations-and-apps/using-workfront-with-outlook/create-a-wf-request-from-an-outlook-email.md).
* 將電子郵件新增為中的任務 [!UICONTROL 我的工作] 區域。 如需詳細資訊，請參閱 [新增 [!DNL Outlook] 以電子郵件傳送作為您工作清單的任務](../../workfront-integrations-and-apps/using-workfront-with-outlook/add-outlook-email-as-task-to-your-work-list.md).
* 回覆意見的方式： [!DNL Workfront] 的增益集 [!DNL Outlook]. 如需有關回覆Workfront註釋的資訊，請參閱 [!DNL Outlook]，請參閱 [回覆來自的評論 [!DNL Outlook]](../../workfront-integrations-and-apps/using-workfront-with-outlook/reply-to-a-comment-from-outlook.md).
* 從頭開始建立任務和問題，或從現有電子郵件建立（使用拖放功能）。 如需詳細資訊，請參閱 [新增 [!DNL Outlook] 以電子郵件將任務或問題傳送至專案](../../workfront-integrations-and-apps/using-workfront-with-outlook/add-outlook-email-to-project-as-task-or-issue.md).

您必須新增 [!DNL Workfront] 您的增益集 [!DNL Outlook] 帳戶，然後才能使用 [!DNL Workfront for Outlook].

如果您無法安裝 [!DNL Workfront] 增益集與您的 [!DNL Outlook] 帳戶，請聯絡您的 [!DNL Workfront] 管理員，確保 [!DNL Outlook] 您的組織已啟用增益集。

如需如何啟用 [!DNL Outlook] 與貴組織的整合，請參閱 [啟用 [!DNL Adobe Workfront for Outlook]](../../administration-and-setup/configure-integrations/enable-workfront-for-outlook.md).

## 存取需求

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

如需有關此表格的詳細資訊，請參閱 [Workfront檔案中的存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## 先決條件

您的 [!DNL Workfront] 管理員必須啟用 [!DNL Outlook for Office] 替換為 [!DNL Workfront] 才能使用此整合。

## 系統需求

下列應用程式可供使用：

* **[!DNL Outlook]在網頁上：** 此 [!DNL Workfront] 使用時，可使用增益集 [!DNL Outlook] 從案頭或行動裝置上的網頁瀏覽器。 此功能也可在使用 [!DNL Outlook] 網頁應用程式。
* **[!DNL Outlook]案頭應用程式：** 此 [!DNL Workfront] 使用時，可使用增益集 [!DNL Windows] 和 [!DNL Mac] 案頭版本的 [!DNL Outlook] 包含在 [!DNL Office] 封裝。

此 [!DNL Workfront] 的增益集 [!DNL Outlook] 在符合下列需求的環境中受支援：

* [使用者端需求](#client-requirements-client-requirements)
* [郵件伺服器需求](#mail-server-requirements-mail-server-requirements)

### 使用者端需求 {#client-requirements}

Workfront支援下列版本 [!DNL Outlook]：

* [!DNL Outlook 2013] 或稍後 [!DNL Windows]
*[!DNL  Outlook 2016] 或稍後 [!DNL Windows]
* [!DNL Outlook] 於 [!DNL Mac] ([!DNL Microsoft 365])
* [!DNL Outlook] 於 [!DNL Windows] ([!DNL Microsoft 365])
* [!DNL Outlook] 在網頁上

您必須連線到 [!DNL Exchange Server] 或 [!DNL Office 365] 使用直接連線。

設定使用者端時，使用者必須選取下列其中一個帳戶型別：

* [!DNL Exchange]
* [!DNL Office 365]
* [!DNL Outlook.com]&#x200B;URL **&#x200B;URL**&#x200B;如&#x200B;果使用者端已設定為連線至POP3或IMAP，則 [!DNL Workfront] 增益集未載入。

### 郵件伺服器需求 {#mail-server-requirements}

當您連線到時，預設會符合郵件伺服器需求 [!DNL Office 365] 或 [!DNL Outlook.com]. 不過，如果您已連線至內部部署安裝， [!DNL Exchange Server]，則適用下列要求：

* Workfront支援所有 [!DNL Exchange On-Premise] 伺服器
* [!DNL Exchange Web Services] (EWS)必須已啟用，且必須公開至網際網路。
* 伺服器必須具備有效的驗證憑證，伺服器才能核發有效的身分識別權杖。 全新安裝 [!DNL Exchange Server] 包含預設的驗證憑證。

  <!--this used to be here but Dev asked for it to be taken out - logged issue for editing this article on 4-26-2023: For more information, see [Digital certificates and encryption in [!DNL Exchange 2016]](https://technet.microsoft.com/en-us/library/dd351044(v=exchg.160).aspx) and [Set-AuthConfig](https://technet.microsoft.com/en-us/library/jj215766(v=exchg.160).aspx).-->

* 若要存取 [!DNL Workfront] 來自的增益集 [[!DNL Office] 儲存](https://store.office.com/)，您的使用者端存取伺服器必須能夠與  [https://store.office.com](https://store.office.com/).

如需受支援環境的詳細資訊，請參閱 [[!DNL Microsoft Office 365] 首頁](https://products.office.com/en-us/office-365-home).

## 安裝增益集

您可以從取得適用於Outlook的Workfront增益集 [Microsoft商店](https://appsource.microsoft.com/en-us/product/office/WA104380943?tab=Overview).

### [!DNL Workfront] 的 [!DNL Outlook 365] {#workfront-for-outlook-365}

1. 在 [!DNL Outlook 365]，按一下 **[!UICONTROL 瀏覽增益集]** 圖示 ![](assets/outlook-add-in-26x26.png)在Office 365介面的頂端，然後按一下 **[!UICONTROL 管理增益集]**.

1. 在 **[!UICONTROL 搜尋增益集]** 方塊，搜尋 **[!DNL Workfront]** 然後按 [!UICONTROL 輸入].

1. 按一下 **[!UICONTROL 新增]**.

### [!DNL Workfront] 的 [!DNL Outlook] 在網頁上 {#workfront-for-outlook-on-the-web}

1. 開啟 [!DNL Microsoft Outlook] 在網頁瀏覽器中。
1. 按一下 **[!UICONTROL 瀏覽] 增益集** 圖示 ![](assets/outlook-add-in-web-version-20x20.png).

   若要尋找圖示，請參閱 [在中使用增益集 [!DNL Outlook] 在網頁上](https://support.microsoft.com/en-us/office/using-add-ins-in-outlook-on-the-web-8f2ce816-5df4-44a5-958c-f7f9d6dabdce#bkmk_addaddinsicon) (位於Microsoft檔案中)。

1. 搜尋 **[!DNL Workfront]** 在 **[!UICONTROL 搜尋增益集]** 欄位，然後按 **[!UICONTROL 輸入]**.

1. 當它出現在清單上時，按一下 **新增**.

### [!DNL Workfront for Outlook] 於 [!UICONTROL Windows] 或 [!DNL Mac] {#workfront-for-outlook-on-windows-or-mac}

1. 按一下 **[!UICONTROL 首頁]** > **[!UICONTROL 儲存]** 在功能區上。

1. 搜尋 **[!DNL Workfront]** 在 **[!UICONTROL 搜尋]** 欄位，然後按 **[!UICONTROL 輸入]**.

1. 按一下切換以啟用 **[!UICONTROL [!DNL Workfront]增益集]**.

## 登入 [!DNL Workfront] 從 [!DNL Outlook]

1. 在 [!DNL Outlook]，選取電子郵件訊息，然後按一下 **[!DNL Workfront]** 圖示來識別。
1. 依照提示登入 [!DNL Workfront] 使用增強式驗證、OAuth 2.0或您的安全性宣告標籤語言(SAML) URL。

   使用者登入之前 [!DNL Workfront] 使用SAML的增益集，a [!DNL Workfront] 管理員必須先啟用 [!DNL Office 365] 增益集以使用SAML 2.0解決方案進行驗證。 如需詳細資訊，請參閱區段 [設定 [!DNL Adobe Workfront] 使用SAML 2.0](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md#enable-saml-with-office-365) 在文章中 [設定 [!DNL Adobe Workfront] 使用SAML 2.0](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md).

   >[!NOTE]
   >
   >* 當提示您輸入您的網域時 [!DNL Workfront] 帳戶，請以此格式輸入： *yourCompany&#39;sDomain.my.workfront.com*. 您公司的網域通常是您公司的名稱。
   >* 增強式驗證必須等到 [!DNL Workfront] 管理員會為此整合啟用它。

