---
product-previous: workfront-fusion
product-area: workfront-integrations;setup
navigation-topic: connections-annd-webhooks
title: 連線 [!DNL Adobe Workfront Fusion] 至 [!DNL Google Services] 使用自訂Oauth使用者端
description: 您可以使用 [!DNL Adobe Workfront Fusion] 以連線到 [!DNL Google Services] 使用自訂OAuth使用者端。 此程式需要現有的 [!DNL Google] 帳戶。
author: Becky
feature: Workfront Fusion
exl-id: 5efc0001-a8cd-4ffc-b074-3536f095727b
source-git-commit: 7d2b4a9940cb21de1b8b5f2955f53b3d88040e44
workflow-type: tm+mt
source-wordcount: '928'
ht-degree: 0%

---

# 連線 [!DNL Adobe Workfront Fusion] 至 [!DNL Google Services] 使用自訂Oauth使用者端

## 存取需求

您必須具有下列存取權才能使用本文中的功能：

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計劃</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權</td> 
   <td> <p>新增：[！UICONTROL Standard]</p><p>或</p><p>目前： [！UICONTROL Work]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] 授權**</td> 
   <td>
   <p>目前：否 [!DNL Workfront Fusion] 授權需求。</p>
   <p>或</p>
   <p>舊版：任何 </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>
   <p>新增：</p> <ul><li>[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Workfront] 計畫：您的組織必須購買 [!DNL Adobe Workfront Fusion].</li><li>[！UICONTROL Ultimate] [!DNL Workfront] 計畫： [!DNL Workfront Fusion] 已包括在內。</li></ul>
   <p>或</p>
   <p>目前：您的組織必須購買 [!DNL Adobe Workfront Fusion].</p>
   </td> 
  </tr>
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱 [Workfront檔案中的存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

有關的資訊 [!DNL Adobe Workfront Fusion] 授權，請參閱 [[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 先決條件

您需要現有的 [!DNL Google] 建立此連線的帳戶。

## 使用自訂OAuth使用者端連線Fusion至Google服務

若要建立此連線，您必須在Google Cloud平台上建立並設定專案，然後根據該專案在Fusion中設定連線。

* [建立專案於 [!DNL Google Cloud Platform]](#create-a-project-on-google-cloud-platform)
* [設定 [!UICONTROL OAuth同意] 設定](#configure-oauth-consent-settings)
* [建立OAuth認證](#create-oauth-credentials)
* [連線到 [!DNL Google] 在 [!DNL Workfront Fusion]](#connect-to-google-in-workfront-fusion)

>[!NOTE]
>
>此程式的用途為：
>
>* 個人使用([!DNL `@gmail.com`] 和 [!DNL `@googlemail.com`] 使用者)
>* 內部使用([!DNL G Suite] 偏好使用自訂OAuth使用者端的使用者)

### 建立專案於 [!DNL Google Cloud Platform]

建立專案的方式 [!DNL Google Cloud] 平台：

1. 登入 [[!DNL Google Cloud] Platform](https://console.developers.google.com/projectselector2/apis/dashboard?supportedpurview=project) 使用您的 [!DNL Google] 認證。
1. 在左側面板中，按一下 **[!UICONTROL 儀表板]**.
1. 按一下 **[!UICONTROL 建立專案]** 在畫面的右上角。
1. 輸入 **[!UICONTROL 專案名稱]**，然後按一下 **[!UICONTROL 建立]**.

1. 按一下 **[!UICONTROL 啟用API和服務]** 索引標籤靠近熒幕頂端。
1. 在 **[!UICONTROL 搜尋API和服務]** 在畫面頂端的欄位，輸入您要使用的服務名稱(例如 [!DNL Gmail] API或 [!DNL Google Drive] API)。
1. 當它顯示時，按一下您想要連線到的API或服務 [!DNL Workfront Fusion].
1. 按一下 **[!UICONTROL 啟用]** 以啟用選取的API。
1. 針對您要啟用的每個API，重複步驟6至8。

   >[!NOTE]
   >
   >您必須啟用 [!DNL Google Drive] API以及所有的API [!DNL Google] 您要使用的應用程式(例如 [!DNL Google Sheets] API)。

1. 在出現的畫面上，按一下 **[!UICONTROL 建立認證]** 位於右上角。
1. 繼續前往區段 [設定OAuth同意設定](#configure-oauth-consent-settings) 本文章內容。

### 設定 [!UICONTROL OAuth同意] 設定

1. 在左側面板中，按一下 **[!UICONTROL OAuth同意畫面]**.
1. 選取 **[!UICONTROL 外部]**，然後按一下 **[!UICONTROL 建立]**.

   >[!NOTE]
   >
   >選取此選項時不會向您收費。 如需詳細資訊，請參閱 [!DNL Google]的驗證需求例外相關資訊。

1. 依照以下說明填寫必填欄位：

   <table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[！UICONTROL應用程式名稱]</p> </td> 
      <td> <p>輸入要求同意的應用程式名稱。</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>範例： </b></span></span>[!DNL Adobe Workfront Fusion] </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL使用者支援電子郵件]</td> 
      <td>輸入電子郵件地址，讓使用者在連線至此應用程式時，針對同意問題聯絡您。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL電子郵件地址]</td> 
      <td>輸入一或多個電子郵件地址，Google可將其用於通知您專案的任何變更。</td> 
     </tr> 
    </tbody> 
   </table>

1. 在 [!UICONTROL 授權的網域]，按一下 **[!UICONTROL 新增網域]**，並輸入 `workfrontfusion.com`.

1. 按一下 **[!UICONTROL 儲存並繼續]**.
1. 按一下 **[!UICONTROL 新增或移除範圍]**.
1. 在右側面板中，啟用下列範圍：

<table style="table-layout:auto">
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>服務/API</th> 
      <th>必要的範圍</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td> <p>[!DNL Gmail]</p> </td> 
      <td> <p>https://mail.google.com/</p> <p>https://www.googleapis.com/auth/gmail.labels</p> <p>https://www.googleapis.com/auth/gmail.send</p> <p>https://www.googleapis.com/auth/gmail.readonly</p> <p>https://www.googleapis.com/auth/gmail.compose</p> <p>https://www.googleapis.com/auth/gmail.insert</p> <p>https://www.googleapis.com/auth/gmail.modify</p> <p>https://www.googleapis.com/auth/gmail.metadata</p> </td> 
     </tr> 
     <tr> 
      <td> <p>[!DNL Google Drive]</p> </td> 
      <td> <p>https://www.googleapis.com/auth/drive</p> <p>https://www.googleapis.com/auth/drive.readonly</p> </td> 
     </tr> 
    </tbody> 
   </table>

您可能需要展開清單或前往清單的下一頁檢視所有清單。

1. 按一下 **[!UICONTROL 更新]**.
1. 按一下 **[!UICONTROL 儲存並繼續]**.
1. （選用）將任何測試使用者新增至專案。
1. 按一下 **[!UICONTROL 儲存並繼續]**.
1. 檢查您的資訊是否準確，然後按一下 **[!UICONTROL 返回儀表板]**.

   >[!NOTE]
   >
   >您不需要提交同意畫面和申請以進行驗證 [!DNL Google].

1. 繼續至 [建立OAuth認證](#create-oauth-credentials).

### 建立OAuth認證

1. 在左側面板中，按一下 **[!UICONTROL 認證]**.

   >[!NOTE]
   >
   >如果這不是第一個API或服務([!DNL Gmail] 或 [!DNL Google Drive])已啟用，您不必建立新的認證。

1. 按一下 **[!UICONTROL 建立認證]** 在熒幕頂端附近，然後選取「 」 **[!UICONTROL OAuth使用者端ID]** （從下拉式功能表）。

1. 依照以下說明填寫必填欄位：

   <table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[！UICONTROL應用程式型別]</td> 
      <td> <p> [！UICONTROL Web應用程式]</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL名稱]</td> 
      <td>[!DNL Workfront Fusion] </td> 
     </tr> 
    </tbody> 
   </table>

1. 在 [!UICONTROL 授權的重新導向URI]，按一下 **[!UICONTROL 新增URI]** 並輸入 **一** 下列專案中的：

   * 的 [!DNL Gmail] 或 [!DNL Google Drive]： `https://app.workfrontfusion.com/oauth/cb/google-restricted`

   * 針對其他 [!DNL Google] 應用程式： `https://app.workfrontfusion.com/oauth/cb/google`

1. 按一下「**[!UICONTROL 建立]**」。

   此 [!UICONTROL 使用者端ID] 和 [!UICONTROL 使用者端密碼] 顯示。

1. 複製 [!UICONTROL 使用者端ID] 和 [!UICONTROL 使用者端密碼] 前往安全位置。 您將使用它們在中建立連線 [!DNL Workfront Fusion].
1. 繼續至 [連線到 [!DNL Google] 在 [!DNL Workfront Fusion]](#connect-to-google-in-workfront-fusion).

### 連線到 [!DNL Google] 在 [!DNL Workfront Fusion]

建立與的連線的程式 [!DNL Google] 視您使用的模組是否來自 [!DNL Google] 服務(例如 [!DNL Google Sheets] 或 [!DNL Google Docs])或如果您要連線至 [!DNL Google] 透過 [!UICONTROL HTTP] >[!UICONTROL 建立OAuth2.0] 要求模組。

* [連線到 [!DNL Google] 在 [!DNL Google] 服務](#connect-to-google-in-a-google-service)
* [連線到 [!DNL Google] 在 [!UICONTROL HTTP] > [!UICONTROL 提出OAuth2.0請求] 模組](#connect-to-google-in-the-http--make-an-oauth20-request-module)

#### 連線到 [!DNL Google] 在 [!DNL Google] 服務

1. 在 [!DNL Workfront Fusion]，找到 [!DNL Google] 建立連線所需的模組。
1. 按一下 **[!UICONTROL 建立連線]**，然後按一下 **[!UICONTROL 顯示進階設定]**.

1. 輸入 [!UICONTROL 使用者端ID] 和 [!UICONTROL 使用者端密碼] 您已擷取於 [[!UICONTROL 建立OAuth認證]](#create-oauth-credentials) 在個別欄位中，然後按一下 **[!UICONTROL 繼續]**.

1. 使用您的裝置登入 [!DNL Google] 帳戶。

   此 **[!UICONTROL 此應用程式未驗證]** 視窗隨即顯示。 請注意，視窗標題中提到的「應用程式」是您在上面建立的OAuth使用者端。

1. 按一下 **[!UICONTROL 進階]**，然後按一下 **[!UICONTROL 前往 [!DNL Workfront Fusion] （不安全）]** 以允許使用您的自訂OAuth使用者端進行存取。

1. 按一下 **[!UICONTROL 允許]** 授予 [!DNL Workfront Fusion] 許可權。
1. 在出現的視窗中，按一下 **[!UICONTROL 允許]** 再次確認您的選擇。

   所需專案的連線 [!DNL Google] 已建立使用自訂OAuth使用者端的服務。

#### 連線到 [!DNL Google] 在 [!UICONTROL HTTP] > [!UICONTROL 提出OAuth2.0請求] 模組 {#connect-to-google-in-the-http--make-an-oauth20-request-module}

有關連線說明 [!DNL Google] 在 [!UICONTROL HTTP] > [!UICONTROL 提出OAuth2.0請求] 模組，請參閱 [建立與的連線的指示 [!DNL Google] 在 [!UICONTROL HTTP] > [!UICONTROL 提出OAuth 2.0請求] 模組](../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-an-oauth-2-request.md#instructions-for-creating-a-connection-to-google-in-the-http-make-an-oauth-20-request-module) 在 [[!UICONTROL HTTP] > [!UICONTROL 提出OAuth 2.0請求] 模組](../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-an-oauth-2-request.md).

## 可能的錯誤訊息：[!UICONTROL [403] 未設定存取]

如果 [!UICONTROL `403 Access Not Configured`] 錯誤訊息顯示，您必須在Google Cloud平台中啟用對應的API。 若要啟用API，請依照一節中的步驟操作 [建立專案於 [!DNL Google Cloud Platform]](#create-a-project-on-google-cloud-platform) 本文章內容。
