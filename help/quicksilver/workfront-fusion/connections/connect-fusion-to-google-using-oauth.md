---
product-previous: workfront-fusion
product-area: workfront-integrations;setup
navigation-topic: connections-annd-webhooks
title: 使用自訂OAuth使用者端連線 [!DNL Adobe Workfront Fusion] 至 [!DNL Google Services]
description: 您可以使用 [!DNL Adobe Workfront Fusion] 使用自訂OAuth使用者端連線至 [!DNL Google Services] 。 此程式需要現有的 [!DNL Google] 帳戶。
author: Becky
feature: Workfront Fusion
exl-id: 5efc0001-a8cd-4ffc-b074-3536f095727b
source-git-commit: 84444753db0e5c496f013e0245988e62fddad585
workflow-type: tm+mt
source-wordcount: '928'
ht-degree: 0%

---

# 使用自訂OAuth使用者端連線[!DNL Adobe Workfront Fusion]至[!DNL Google Services]

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
   <p>目前：無[!DNL Workfront Fusion]授權需求。</p>
   <p>或</p>
   <p>舊版：任何 </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>
   <p>新增：</p> <ul><li>[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Workfront]計畫：您的組織必須購買[!DNL Adobe Workfront Fusion]。</li><li>已包含[！UICONTROL Ultimate] [!DNL Workfront]計畫： [!DNL Workfront Fusion]。</li></ul>
   <p>或</p>
   <p>目前：您的組織必須購買[!DNL Adobe Workfront Fusion]。</p>
   </td> 
  </tr>
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

如需[!DNL Adobe Workfront Fusion]授權的相關資訊，請參閱[[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md)。

## 先決條件

您需要現有的[!DNL Google]帳戶才能建立此連線。

## 使用自訂OAuth使用者端連線Fusion至Google服務

若要建立此連線，您必須在Google Cloud平台上建立並設定專案，然後根據該專案在Fusion中設定連線。

* [在 [!DNL Google Cloud Platform]上建立專案](#create-a-project-on-google-cloud-platform)
* [設定[!UICONTROL OAuth同意]設定](#configure-oauth-consent-settings)
* [建立OAuth認證](#create-oauth-credentials)
* [連線到 [!DNL Workfront Fusion]中的 [!DNL Google] ](#connect-to-google-in-workfront-fusion)

>[!NOTE]
>
>此程式的用途為：
>
>* 個人使用（[!DNL `@gmail.com`]和[!DNL `@googlemail.com`]位使用者）
>* 內部使用（偏好使用自訂OAuth使用者端的[!DNL Google Workspace]位使用者）

### 在[!DNL Google Cloud Platform]上建立專案

若要在[!DNL Google Cloud]平台上建立專案：

1. 使用您的[!DNL Google]認證登入[[!DNL Google Cloud] 平台](https://console.developers.google.com/projectselector2/apis/dashboard?supportedpurview=project)。
1. 在左側面板中，按一下&#x200B;**[!UICONTROL 儀表板]**。
1. 按一下畫面右上角的&#x200B;**[!UICONTROL 建立專案]**。
1. 輸入&#x200B;**[!UICONTROL 專案名稱]**，然後按一下&#x200B;**[!UICONTROL 建立]**。

1. 按一下熒幕上方附近的&#x200B;**[!UICONTROL 啟用API和服務]**&#x200B;標籤。
1. 在熒幕上方的&#x200B;**[!UICONTROL 搜尋API和服務]**&#x200B;欄位中，輸入您要使用的服務名稱（例如[!DNL Gmail] API或[!DNL Google Drive] API）。
1. 當它顯示時，按一下您要連線到[!DNL Workfront Fusion]的API或服務。
1. 按一下&#x200B;**[!UICONTROL 啟用]**&#x200B;以啟用選取的API。
1. 針對您要啟用的每個API，重複步驟6至8。

   >[!NOTE]
   >
   >您必須啟用[!DNL Google Drive] API以及您要使用的所有[!DNL Google]應用程式的API （例如[!DNL Google Sheets] API）。

1. 在出現的畫面上，按一下右上角的&#x200B;**[!UICONTROL 「建立認證」]**。
1. 繼續閱讀本文章[設定OAuth同意設定](#configure-oauth-consent-settings)一節。

### 設定[!UICONTROL OAuth同意]設定

1. 在左側面板中，按一下&#x200B;**[!UICONTROL OAuth同意畫面]**。
1. 選取&#x200B;**[!UICONTROL 外部]**，然後按一下&#x200B;**[!UICONTROL 建立]**。

   >[!NOTE]
   >
   >選取此選項時不會向您收費。 如需詳細資訊，請參閱[!DNL Google]關於驗證需求例外的資訊。

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

1. 在[!UICONTROL 授權的網域]下，按一下&#x200B;**[!UICONTROL 新增網域]**，然後輸入`workfrontfusion.com`。

1. 按一下&#x200B;**[!UICONTROL 儲存並繼續]**。
1. 按一下&#x200B;**[!UICONTROL 新增或移除領域]**。
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

1. 按一下&#x200B;**[!UICONTROL 更新]**。
1. 按一下&#x200B;**[!UICONTROL 儲存並繼續]**。
1. （選用）將任何測試使用者新增至專案。
1. 按一下&#x200B;**[!UICONTROL 儲存並繼續]**。
1. 檢查您的資訊是否準確，然後按一下&#x200B;**[!UICONTROL 返回儀表板]**。

   >[!NOTE]
   >
   >您不需要提交同意畫面與申請以由[!DNL Google]驗證。

1. 繼續[建立OAuth認證](#create-oauth-credentials)。

### 建立OAuth認證

1. 在左側面板中，按一下&#x200B;**[!UICONTROL 認證]**。

   >[!NOTE]
   >
   >如果這不是您啟用的第一個API或服務（[!DNL Gmail]或[!DNL Google Drive]），您就不需要建立新的認證。

1. 按一下熒幕上方附近的&#x200B;**[!UICONTROL 建立認證]**，然後從下拉式功能表中選取&#x200B;**[!UICONTROL OAuth使用者端識別碼]**。

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

1. 在[!UICONTROL 授權的重新導向URI]下，按一下&#x200B;**[!UICONTROL 新增URI]**，然後輸入下列&#x200B;**一個**：

   * 針對[!DNL Gmail]或[!DNL Google Drive]： `https://app.workfrontfusion.com/oauth/cb/google-restricted`

   * 其他[!DNL Google]應用程式： `https://app.workfrontfusion.com/oauth/cb/google`

1. 按一下「**[!UICONTROL 建立]**」。

   顯示[!UICONTROL 使用者端識別碼]和[!UICONTROL 使用者端密碼]。

1. 將[!UICONTROL 使用者端識別碼]和[!UICONTROL 使用者端密碼]複製到安全位置。 您將使用這些工具在[!DNL Workfront Fusion]中建立連線。
1. 繼續[連線至 [!DNL Workfront Fusion]](#connect-to-google-in-workfront-fusion)中的 [!DNL Google] 。

### 在[!DNL Workfront Fusion]中連線到[!DNL Google]

建立與[!DNL Google]的連線的程式會有所不同，這取決於您是使用來自[!DNL Google]服務（例如[!DNL Google Sheets]或[!DNL Google Docs]）的模組，或是您是透過[!UICONTROL HTTP] >[!UICONTROL 建立OAuth2.0]要求模組來連線到[!DNL Google]。

* [連線到 [!DNL Google] 服務中的 [!DNL Google] ](#connect-to-google-in-a-google-service)
* [連線到[!UICONTROL HTTP] > [!UICONTROL 發出OAuth2.0請求]模組中的 [!DNL Google] ](#connect-to-google-in-the-http--make-an-oauth20-request-module)

#### 在[!DNL Google]服務中連線到[!DNL Google]

1. 在[!DNL Workfront Fusion]中，找出您需要建立連線的[!DNL Google]模組。
1. 按一下[建立連線]****，然後按一下[顯示進階設定]****。

1. 在個別欄位中輸入您在[[!UICONTROL 建立OAuth認證]](#create-oauth-credentials)中擷取的[!UICONTROL 使用者端識別碼]和[!UICONTROL 使用者端密碼]，然後按一下&#x200B;**[!UICONTROL 繼續]**。

1. 使用您的[!DNL Google]帳戶登入。

   **[!UICONTROL 此應用程式未驗證]**&#x200B;視窗會顯示。 請注意，視窗標題中提到的「應用程式」是您在上面建立的OAuth使用者端。

1. 按一下&#x200B;**[!UICONTROL 進階]**，然後按一下&#x200B;**[!UICONTROL 移至[!DNL Workfront Fusion] （不安全）]**&#x200B;以允許使用您的自訂OAuth使用者端進行存取。

1. 按一下&#x200B;**[!UICONTROL 允許]**&#x200B;以授予[!DNL Workfront Fusion]許可權。
1. 在出現的視窗中，再按一下&#x200B;**[!UICONTROL 允許]**&#x200B;以確認您的選擇。

   已使用自訂OAuth使用者端建立與所需[!DNL Google]服務的連線。

#### 連線到[!UICONTROL HTTP] > [!UICONTROL 發出OAuth2.0請求]模組中的[!DNL Google] {#connect-to-google-in-the-http--make-an-oauth20-request-module}

如需在[!UICONTROL HTTP] > [!UICONTROL 發出OAuth2.0要求]模組中連線[!DNL Google]的指示，請參閱[在[!UICONTROL HTTP] > [!UICONTROL 在[[!UICONTROL HTTP] > [!UICONTROL 發出OAuth 2.0要求]模組](../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-an-oauth-2-request.md)中發出OAuth 2.0要求 [!DNL Google] 的指示。]](../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-an-oauth-2-request.md#instructions-for-creating-a-connection-to-google-in-the-http-make-an-oauth-20-request-module)

## 可能的錯誤訊息：[!UICONTROL [403]未設定存取]

如果顯示[!UICONTROL `403 Access Not Configured`]錯誤訊息，您必須在Google Cloud平台中啟用對應的API。 若要啟用API，請依照本文中[在 [!DNL Google Cloud Platform]](#create-a-project-on-google-cloud-platform)上建立專案一節中的步驟操作。
