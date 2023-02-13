---
product-previous: workfront-fusion
product-area: workfront-integrations;setup
navigation-topic: connections-annd-webhooks
title: Connect [!DNL Adobe Workfront Fusion] to [!DNL Google Services] 使用自訂OAuth用戶端
description: 您可以使用 [!DNL Adobe Workfront Fusion] 連接到 [!DNL Google Services] 使用自訂OAuth用戶端。 此程式需要現有 [!DNL Google] 帳戶。
author: Becky
feature: Workfront Fusion
exl-id: 5efc0001-a8cd-4ffc-b074-3536f095727b
source-git-commit: fcaa2136310cad8ef478020a9bae34bbe5520c6d
workflow-type: tm+mt
source-wordcount: '899'
ht-degree: 0%

---

# Connect [!DNL Adobe Workfront Fusion] to [!DNL Google Services] 使用自訂OAuth用戶端

## 存取需求

您必須具備下列存取權才能使用本文中的功能：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計劃*</td> 
   <td> <p>[!UICONTROL Pro]或更高版本</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權*</td> 
   <td> <p>[!UICONTROL計畫]、[!UICONTROL工作]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] 許可**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] （工作自動化和整合） </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>貴組織必須購買 [!DNL Adobe Workfront Fusion] 和 [!DNL Adobe Workfront] 以使用本文所述的功能。</td> 
  </tr> 
 </tbody> 
</table>

若要了解您擁有的計畫、授權類型或存取權，請聯絡您的 [!DNL Workfront] 管理員。

如需 [!DNL Adobe Workfront Fusion] 許可證，請參閱 [[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 必要條件

您需要現有 [!DNL Google] 帳戶進行此連線。

## 在上建立專案 [!DNL Google Cloud Platform]

下列程式的用途為：

* 個人用途([!DNL @gmail.com] 和 [!DNL @googlemail.com] 使用者)
* 內部使用([!DNL G Suite] 偏好使用自訂OAuth用戶端的使用者)

在上建立專案 [!DNL Google Cloud] 平台：

1. 登入 [[!DNL Google Cloud] 平台](https://console.developers.google.com/projectselector2/apis/dashboard?supportedpurview=project) 使用 [!DNL Google] 憑證。
1. 在左側面板中，按一下 **[!UICONTROL 控制面板]**.
1. 按一下 **[!UICONTROL 建立專案]** 在螢幕的右上角。
1. 輸入 **[!UICONTROL 專案名稱]**，然後按一下 **[!UICONTROL 建立]**.

1. 按一下 **[!UICONTROL 啟用API與服務]** 標籤。
1. 在 **[!UICONTROL 搜尋API與服務]** 欄位，輸入您要使用的服務名稱(例如 [!DNL Gmail] API或 [!DNL Google Drive] API)。
1. 顯示時，按一下您要連線的API或服務 [!DNL Workfront Fusion].
1. 按一下 **[!UICONTROL 啟用]** 啟用所選API。
1. 對要啟用的每個API重複步驟6至8。

   >[!NOTE]
   >
   >您必須啟用 [!DNL Google Drive] API以及所有的API [!DNL Google] 您要使用的應用程式(例如 [!DNL Google Sheets] API)。

1. 在顯示的畫面上，按一下 **[!UICONTROL 建立憑證]** 在右上角。
1. 繼續前往區段 [配置OAuth同意設定](#configure-oauth-consent-settings) 這篇文章。

## 設定 [!UICONTROL OAuth同意] 設定

1. 在左側面板中，按一下 **[!UICONTROL OAuth同意畫面]**.
1. 選擇 **[!UICONTROL 外部]**，然後按一下 **[!UICONTROL 建立]**.

   >[!NOTE]
   >
   >選取此選項時，系統不會向您收取費用。 如需詳細資訊，請參閱 [!DNL Google]關於驗證要求的例外的資訊。

1. 填寫必填欄位如下：

   <table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL應用程式名稱]</p> </td> 
      <td> <p>輸入要求同意的應用程式名稱。</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>範例: </b></span></span>[!DNL Adobe Workfront Fusion] </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL用戶支援電子郵件]</td> 
      <td>輸入使用者的電子郵件地址，以便在連線至此應用程式時，與您連絡，詢問其同意的問題。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL電子郵件地址]</td> 
      <td>輸入一或多個Google可用來通知您專案任何變更的電子郵件地址。</td> 
     </tr> 
    </tbody> 
   </table>

1. 在 [!UICONTROL 授權網域]，按一下 **[!UICONTROL 新增網域]**，然後輸入 `workfrontfusion.com`.

1. 按一下 **[!UICONTROL 保存並繼續]**.
1. 按一下 **[!UICONTROL 添加或刪除作用域]**.
1. 在右側面板中，啟用以下範圍：

<table style="table-layout:auto">
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>服務/API</th> 
      <th>所需範圍</th> 
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

您可能需要展開清單或前往清單的下一頁，才能查看全部內容。

1. 按一下 **[!UICONTROL 更新]**.
1. 按一下 **[!UICONTROL 保存並繼續]**.
1. （選用）將任何測試使用者新增至專案。
1. 按一下 **[!UICONTROL 保存並繼續]**.
1. 檢查資訊是否準確，然後按一下 **[!UICONTROL 返回控制面板]**.

   >[!NOTE]
   >
   >您不需要提交同意畫面和申請以供驗證 [!DNL Google].

1. 繼續 [建立OAuth憑證](#create-oauth-credentials).

## 建立OAuth憑證

1. 在左側面板中，按一下 **[!UICONTROL 憑證]**.

   >[!NOTE]
   >
   >如果這不是第一個API或服務([!DNL Gmail] 或 [!DNL Google Drive])，則您不必建立新憑證。

1. 按一下 **[!UICONTROL 建立憑證]** 在畫面頂端附近，選取 **[!UICONTROL OAuth用戶端ID]** 從下拉式功能表。

1. 填寫必填欄位如下：

   <table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL應用程式類型]</td> 
      <td> <p> [!UICONTROL Web應用程式]</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL名稱]</td> 
      <td>[!DNL Workfront Fusion] </td> 
     </tr> 
    </tbody> 
   </table>

1. 在 [!UICONTROL 授權的重定向URI]，按一下 **[!UICONTROL 添加URI]** 輸入 **one** （共以下）:

   * 針對 [!DNL Gmail] 或 [!DNL Google Drive]: `https://app.workfrontfusion.com/oauth/cb/google-restricted`

   * 其他 [!DNL Google] 應用程式： `https://app.workfrontfusion.com/oauth/cb/google`

1. 按一下 **[!UICONTROL 建立]**。

   此 [!UICONTROL 用戶端ID] 和 [!UICONTROL 用戶端密碼] 顯示。

1. 複製 [!UICONTROL 用戶端ID] 和 [!UICONTROL 用戶端密碼] 到安全的地方。 您會使用這些參數來建立 [!DNL Workfront Fusion].
1. 繼續 [連線至 [!DNL Google] in [!DNL Workfront Fusion]](#connect-to-google-in-workfront-fusion).

## 連線至 [!DNL Google] in [!DNL Workfront Fusion]

建立與 [!DNL Google] 視您是否使用 [!DNL Google] 服務(例如 [!DNL Google Sheets] 或 [!DNL Google Docs])，或如果您連線至 [!DNL Google] 透過 [!UICONTROL HTTP] >[!UICONTROL 建立OAuth2.0] 要求模組。

* [連線至 [!DNL Google] 在 [!DNL Google] 服務](#connect-to-google-in-a-google-service)
* [連線至 [!DNL Google] 在 [!UICONTROL HTTP] > [!UICONTROL 提出OAuth2.0請求] 模組](#connect-to-google-in-the-http--make-an-oauth20-request-module)

### 連線至 [!DNL Google] 在 [!DNL Google] 服務

1. 在 [!DNL Workfront Fusion]，找到 [!DNL Google] 您需要為建立連線的模組。
1. 按一下 **[!UICONTROL 建立連線]**，然後按一下 **[!UICONTROL 顯示高級設定]**.

1. 輸入 [!UICONTROL 用戶端ID] 和 [!UICONTROL 用戶端密碼] 在 [[!UICONTROL 建立OAuth憑證]](#create-oauth-credentials) 在個別欄位中，然後按一下 **[!UICONTROL 繼續]**.

1. 使用 [!DNL Google] 帳戶。

   此 **[!UICONTROL 未驗證此應用]** 視窗。 請注意，視窗標題中提及的「應用程式」是您在上面建立的OAuth用戶端。

1. 按一下 **[!UICONTROL 進階]**，然後按一下 **[!UICONTROL 前往 [!DNL Workfront Fusion] （不安全）]** 允許使用自訂OAuth用戶端存取。

1. 按一下 **[!UICONTROL 允許]** 授予 [!DNL Workfront Fusion] 權限。
1. 在顯示的視窗中，按一下 **[!UICONTROL 允許]** 再次確認您的選擇。

   與所需的連線 [!DNL Google] 已建立使用自訂OAuth用戶端的服務。

### 連線至 [!DNL Google] 在 [!UICONTROL HTTP] > [!UICONTROL 提出OAuth2.0請求] 模組 {#connect-to-google-in-the-http--make-an-oauth20-request-module}

有關連接到 [!DNL Google] 在 [!UICONTROL HTTP] > [!UICONTROL 提出OAuth2.0請求] 模組，請參閱 [建立與 [!DNL Google] 在 [!UICONTROL HTTP] > [!UICONTROL 提出OAuth 2.0請求] 模組](../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-an-oauth-2-request.md#instruct) in [[!UICONTROL HTTP] > [!UICONTROL 提出OAuth 2.0請求] 模組](../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-an-oauth-2-request.md).

## 可能的錯誤消息：[!UICONTROL [403] 未配置訪問]

若 [!UICONTROL [403] 未配置訪問] 錯誤訊息隨即顯示，您必須在Google雲端平台中啟用對應的API。 若要啟用API，請依照 [在上建立專案 [!DNL Google Cloud Platform]](#create-a-project-on-google-cloud-platform) 這篇文章。
