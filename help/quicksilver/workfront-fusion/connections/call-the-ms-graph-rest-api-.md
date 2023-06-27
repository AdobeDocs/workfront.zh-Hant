---
title: 透過呼叫MS Graph REST API [!DNL Adobe Workfront Fusion] HTTP &gt；建立OAuth 2.0請求模組
description: 透過呼叫MS Graph REST API [!DNL Adobe Workfront Fusion] HTTP &gt；建立OAuth 2.0請求模組
author: Becky
draft: Probably
feature: Workfront Fusion
exl-id: adae390d-8b9e-4dab-8551-605e50af5a1e
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '616'
ht-degree: 1%

---

# 呼叫[!UICONTROL  MS Graph REST API] 透過 [!DNL Adobe Workfront Fusion] [!UICONTROL HTTP] > [!UICONTROL 提出OAuth 2.0請求] 模組

許多 [!DNL Microsoft] 網路服務可透過 [!DNL Microsoft Graph API]. 本文會說明如何使用 [!DNL Workfront Fusion] [!DNL HTTP] > [!UICONTROL 提出OAuth 2.0請求] 模組。

## 存取需求

您必須具有下列存取權才能使用本文中的功能：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計劃*</td> 
   <td> <p>[！UICONTROL Pro]或更高版本</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權*</td> 
   <td> <p>[！UICONTROL計畫]，[！UICONTROL工作]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] 授權**</td> 
   <td>
   <p>目前授權需求：否 [!DNL Workfront Fusion] 授權需求。</p>
   <p>或</p>
   <p>舊版授權需求： [！UICONTROL [!DNL Workfront Fusion] 適用於工作自動化與整合] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>
   <p>目前產品需求：如果您有[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Adobe Workfront] 計畫，您的組織必須購買 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文所述功能。 [!DNL Workfront Fusion] 包含在[！UICONTROL Ultimate]中 [!DNL Workfront] 計畫。</p>
   <p>或</p>
   <p>舊版產品需求：貴組織必須購買 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文所述功能。</p>
   </td> 
  </tr>
 </tbody> 
</table>

若要瞭解您擁有哪些計畫、授權型別或存取權，請聯絡您的 [!DNL Workfront] 管理員。

有關以下專案的資訊： [!DNL Adobe Workfront Fusion] 授權，請參閱 [[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 註冊 [!DNL Workfront Fusion] 在 [!DNL Microsoft Application Registration Portal]

若要建立與的連線 [!DNL Microsoft Graph REST API]，您必須先註冊 [!DNL Adobe Workfront Fusion].

1. 開始註冊新的應用程式，如中所述 [註冊您的應用程式](https://docs.microsoft.com/en-us/graph/auth-register-app-v2) 在 [!DNL Microsoft] 說明檔案。

   註冊時， [!DNL Microsoft] 需要下列資訊：

   <table style="table-layout:auto">
      <tr>
        <td>[！UICONTROL應用程式名稱]</td>
        <td>輸入應用程式的名稱，例如「我的」 [!DNL Workfront Fusion] 應用程式。」</td>
      </tr>
      <tr>
        <td>[！UICONTROL重新導向URL]</td>
        <td><code>https://app.workfrontfusion.com/oauth/cb/oauth2</code></td>
      </tr>
    </table>

1. 完成應用程式註冊後，請記下 [!UICONTROL 應用程式ID].

   >[!IMPORTANT]
   >
   >您需要應用程式ID才能在中設定您的連線 [!DNL Workfront Fusion].

1. 產生 [!UICONTROL 應用程式密碼]. 記下此密碼。

   如需指示，請參閱 [註冊您的應用程式](https://docs.microsoft.com/en-us/graph/auth-register-app-v2) 在 [!DNL Microsoft] 說明檔案。

   >[!IMPORTANT]
   >
   >您將需要 [!UICONTROL 應用程式密碼] 以設定您的連線 [!DNL Workfront Fusion].

1. 設定應用程式的許可權。

   如需尋找和設定這些欄位的詳細資訊，請參閱以下的「設定Microsoft Graph的許可權」一節： [取得存取權而不需要使用者](https://docs.microsoft.com/en-us/graph/auth-v2-service) 在 [!UICONTROL Microsoft] 說明檔案。

   <table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[！UICONTROL您的應用程式需要哪種型別的許可權？]</td> 
      <td>選取 <code>[!UICONTROL Delegated permissions]</code>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL選取許可權]</td> 
      <td> <p>選取下列許可權：</p> 
       <ul> 
        <li> <p><code>offline_access</code> </p> </li> 
        <li> <p><code>openid</code> </p> </li> 
        <li> <p>您的整合所需的任何其他許可權(例如： <code>User.Read</code>)</p> </li> 
       </ul> <p>重要：您需要選取的許可權才能在中設定您的連線 [!DNL Workfront Fusion].</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 繼續前往 [設定您的 [!DNL MS Graph API] 中的連線 [!DNL Workfront Fusion]](#configure-your-ms-graph-api-connection-in-workfront-fusion).

## 設定您的 [!DNL MS Graph API] 中的連線 [!DNL Workfront Fusion]

註冊之後 [!DNL Workfront Fusion] 如中所述 [註冊 [!DNL Workfront Fusion] 在 [!DNL Microsoft Application Registration Portal]](#register-workfront-fusion-in-the-microsoft-application-registration-portal)，您可在以下位置設定連線： [!UICONTROL HTTP] >[!UICONTROL 建立Oauth 2.0] 要求模組。

1. 新增 [!UICONTROL HTTP] >[!UICONTROL 進行OAuth 2.0呼叫] 模組至您的情境。
1. 按一下 **[!UICONTROL 新增]** 旁邊 [!UICONTROL 連線] 欄位。
1. 設定連線欄位，如下所示：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[！UICONTROL連線名稱]</td> 
      <td>輸入連線的名稱。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">[！UICONTROL流程型別]</p> </td> 
      <td><code>[!UICONTROL Authorization Code]</code> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL授權URI]</td> 
      <td><code>https://login.microsoftonline.com/common/oauth2/v2.0/authorize</code> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL權杖URI]</td> 
      <td><code>https://login.microsoftonline.com/common/oauth2/v2.0/token</code> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL範圍]</td> 
      <td> <p>輸入您在的步驟4中選擇的許可權 <a href="#register-workfront-fusion-in-the-microsoft-application-registration-portal" class="MCXref xref">註冊 [!DNL Workfront Fusion] 在 [!DNL Microsoft Application Registration Portal]</a>.</p> <p>對於每個範圍，按一下 <b>[！UICONTROL新增]</b> 並輸入許可權。</p> <p>範例: <code>offline_access</code>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL範圍分隔符號]</td> 
      <td><code>SPACE</code> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL使用者端ID]</td> 
      <td>在中步驟2輸入[！UICONTROL應用程式ID] <a href="#register-workfront-fusion-in-the-microsoft-application-registration-portal" class="MCXref xref">註冊 [!DNL Workfront Fusion] 在 [!DNL Microsoft Application Registration Portal]</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL使用者端密碼]</td> 
      <td>輸入您在步驟2產生的[！UICONTROL應用程式密碼] <a href="#register-workfront-fusion-in-the-microsoft-application-registration-portal" class="MCXref xref">註冊 [!DNL Workfront Fusion] 在 [!DNL Microsoft Application Registration Portal]</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL Authorize引數]</td> 
      <td> <p>新增下列Authorize引數：</p> 
       <ul> 
        <li> <p>[！UICONTROL索引鍵]：<code> response_mode</code> [！UICONTROL值]： <code>query</code></p> </li> 
        <li> <p>[！UICONTROL索引鍵]： <code>prompt </code>[！UICONTROL值]： <code>consent</code></p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL存取權杖引數]</td> 
      <td>您不需要在此欄位中輸入任何內容。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL重新整理權杖引數]</td> 
      <td> 
       <ol> 
        <li value="1"> <p>按一下 <b>[！UICONTROL新增]</b>.</p> </li> 
        <li value="2"> <p>在 <b>[！UICONTROL索引鍵]</b> 欄位，輸入 <code>scope</code>.</p> </li> 
        <li value="3"> <p>在 <b>[！UICONTROL值]</b> 欄位，輸入您輸入到範圍欄位中的所有[！UICONTROL範圍]，以空格分隔。</p> <p>範例: <code>offline_access openid User.Read</code></p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL自訂標頭]</td> 
      <td>您不需要在此欄位中輸入任何內容。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL權杖位置]</td> 
      <td><code>[!UICONTROL In the header]</code> </td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下 **[!UICONTROL 繼續]**.
1. 在出現的視窗中，按一下 **[!UICONTROL Accept]** 以完成連線並返回模組。
