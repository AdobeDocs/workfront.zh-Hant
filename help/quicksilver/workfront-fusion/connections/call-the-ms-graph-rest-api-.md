---
title: 透過呼叫MS Graph REST API [!DNL Adobe Workfront Fusion] HTTP &gt;提出OAuth 2.0要求模組
description: 透過呼叫MS Graph REST API [!DNL Adobe Workfront Fusion] HTTP &gt;提出OAuth 2.0要求模組
author: Becky
draft: Probably
feature: Workfront Fusion
exl-id: adae390d-8b9e-4dab-8551-605e50af5a1e
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '568'
ht-degree: 1%

---

# 呼叫[!UICONTROL  MS圖表重置API] 透過 [!DNL Adobe Workfront Fusion] [!UICONTROL HTTP] > [!UICONTROL 提出OAuth 2.0請求] 模組

許多 [!DNL Microsoft] 網站服務可透過 [!DNL Microsoft Graph API]. 本文說明如何使用 [!DNL Workfront Fusion] [!DNL HTTP] > [!UICONTROL 提出OAuth 2.0請求] 模組。

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

## 註冊 [!DNL Workfront Fusion] 在 [!DNL Microsoft Application Registration Portal]

若要建立與 [!DNL Microsoft Graph REST API]，您必須先註冊 [!DNL Adobe Workfront Fusion].

1. 開始註冊新應用程式，如 [註冊您的應用](https://docs.microsoft.com/en-us/graph/auth-register-app-v2) 在 [!DNL Microsoft] 檔案。

   作為登記的一部分， [!DNL Microsoft] 需要下列資訊：

   <table style="table-layout:auto">
      <tr>
        <td>[!UICONTROL應用程式名稱]</td>
        <td>輸入應用程式的名稱，例如「My [!DNL Workfront Fusion] 應用程式。」</td>
      </tr>
      <tr>
        <td>[!UICONTROL重新導向URL]</td>
        <td><code>https://app.workfrontfusion.com/oauth/cb/oauth2</code></td>
      </tr>
    </table>

1. 完成應用程式註冊後，請記下 [!UICONTROL 應用程式ID].

   >[!IMPORTANT]
   >
   >您需要應用程式ID，才能在 [!DNL Workfront Fusion].

1. 產生 [!UICONTROL 應用程式密碼]. 記下這個秘密。

   如需指示，請參閱 [註冊您的應用](https://docs.microsoft.com/en-us/graph/auth-register-app-v2) 在 [!DNL Microsoft] 檔案。

   >[!IMPORTANT]
   >
   >您需要 [!UICONTROL 應用程式密碼] 若要在 [!DNL Workfront Fusion].

1. 設定應用程式的權限。

   如需找到和設定這些欄位的詳細資訊，請參閱以下章節： [無須使用者即可存取](https://docs.microsoft.com/en-us/graph/auth-v2-service) 在 [!UICONTROL Microsoft] 檔案。

   <table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL您的應用程式需要什麼類型的權限？]</td> 
      <td>選取 <code>[!UICONTROL Delegated permissions]</code>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL選擇權限]</td> 
      <td> <p>選取下列權限：</p> 
       <ul> 
        <li> <p><code>offline_access</code> </p> </li> 
        <li> <p><code>openid</code> </p> </li> 
        <li> <p>整合所需的任何其他權限(範例： <code>User.Read</code>)</p> </li> 
       </ul> <p>重要：您需要選取的權限，才能在 [!DNL Workfront Fusion].</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 繼續 [設定您的 [!DNL MS Graph API] 連接 [!DNL Workfront Fusion]](#configure-your-ms-graph-api-connection-in-workfront-fusion).

## 設定您的 [!DNL MS Graph API] 連接 [!DNL Workfront Fusion]

註冊之後 [!DNL Workfront Fusion] 如 [註冊 [!DNL Workfront Fusion] 在 [!DNL Microsoft Application Registration Portal]](#register-workfront-fusion-in-the-microsoft-application-registration-portal)，您可以在 [!UICONTROL HTTP] >[!UICONTROL 建立Oauth 2.0] 要求模組。

1. 新增 [!UICONTROL HTTP] >[!UICONTROL 進行OAuth 2.0呼叫] 模組至您的案例。
1. 按一下 **[!UICONTROL 新增]** 旁邊 [!UICONTROL 連接] 欄位。
1. 按如下方式配置連接欄位：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL連接名]</td> 
      <td>輸入連線的名稱。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">[!UICONTROL流類型]</p> </td> 
      <td><code>[!UICONTROL Authorization Code]</code> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL授權URI]</td> 
      <td><code>https://login.microsoftonline.com/common/oauth2/v2.0/authorize</code> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL令牌URI]</td> 
      <td><code>https://login.microsoftonline.com/common/oauth2/v2.0/token</code> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL範圍]</td> 
      <td> <p>輸入您在的步驟4中選取的權限 <a href="#register-workfront-fusion-in-the-microsoft-application-registration-portal" class="MCXref xref">註冊 [!DNL Workfront Fusion] 在 [!DNL Microsoft Application Registration Portal]</a>.</p> <p>對於每個範圍，按一下 <b>[!UICONTROL添加]</b> 並輸入權限。</p> <p>範例: <code>offline_access</code>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL範圍分隔符]</td> 
      <td><code>SPACE</code> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL客戶端ID]</td> 
      <td>在 <a href="#register-workfront-fusion-in-the-microsoft-application-registration-portal" class="MCXref xref">註冊 [!DNL Workfront Fusion] 在 [!DNL Microsoft Application Registration Portal]</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL客戶端密碼]</td> 
      <td>輸入您在 <a href="#register-workfront-fusion-in-the-microsoft-application-registration-portal" class="MCXref xref">註冊 [!DNL Workfront Fusion] 在 [!DNL Microsoft Application Registration Portal]</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL授權參數]</td> 
      <td> <p>新增下列授權參數：</p> 
       <ul> 
        <li> <p>[!UICONTROL密鑰]:<code> response_mode</code> [!UICONTROL值]: <code>query</code></p> </li> 
        <li> <p>[!UICONTROL密鑰]: <code>prompt </code>[!UICONTROL值]: <code>consent</code></p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL訪問令牌參數]</td> 
      <td>您不需要在此欄位中輸入任何項目。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL刷新令牌參數]</td> 
      <td> 
       <ol> 
        <li value="1"> <p>按一下 <b>[!UICONTROL添加]</b>.</p> </li> 
        <li value="2"> <p>在 <b>[!UICONTROL密鑰]</b> 欄位，輸入 <code>scope</code>.</p> </li> 
        <li value="3"> <p>在 <b>[!UICONTROL值]</b> 欄位，輸入您在作用域欄位中輸入的所有[!UICONTROL作用域]，以空格分隔。</p> <p>範例: <code>offline_access openid User.Read</code></p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL自訂標題]</td> 
      <td>您不需要在此欄位中輸入任何項目。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL代號放置]</td> 
      <td><code>[!UICONTROL In the header]</code> </td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下 **[!UICONTROL 繼續]**.
1. 在顯示的視窗中，按一下 **[!UICONTROL 接受]** 完成連線並返回模組。
