---
title: 透過 [!DNL Adobe Workfront Fusion] HTTP &amp；gt；呼叫MS Graph REST API；建立OAuth 2.0請求模組
description: 透過 [!DNL Adobe Workfront Fusion] HTTP &amp；gt；呼叫MS Graph REST API；建立OAuth 2.0請求模組
author: Becky
feature: Workfront Fusion
exl-id: adae390d-8b9e-4dab-8551-605e50af5a1e
source-git-commit: b90343eab40e91c6f5cddeaa960ce9c9c97b1d29
workflow-type: tm+mt
source-wordcount: '571'
ht-degree: 1%

---

# 透過[!DNL Adobe Workfront Fusion] [!UICONTROL HTTP] > [!UICONTROL 發出OAuth 2.0請求]模組呼叫[!UICONTROL  MS Graph REST API]

<!-- Audited: 3/2024-->

透過[!DNL Microsoft Graph API]存取許多[!DNL Microsoft]網站服務。 您可以使用[!DNL Workfront Fusion] [!DNL HTTP] > [!UICONTROL 發出OAuth 2.0請求]模組來建立與[!DNL Microsoft Graph API]的連線。

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

## 在[!DNL Microsoft Application Registration Portal]中註冊[!DNL Workfront Fusion]

若要建立與[!DNL Microsoft Graph REST API]的連線，您必須先註冊[!DNL Adobe Workfront Fusion]。

1. 開始註冊新的應用程式，如[在[!DNL Microsoft]檔案中註冊您的應用程式](https://docs.microsoft.com/en-us/graph/auth-register-app-v2)中所述。

   做為註冊的一部分，[!DNL Microsoft]需要下列資訊：

   <table style="table-layout:auto">
      <tr>
        <td>[！UICONTROL應用程式名稱]</td>
        <td>輸入應用程式的名稱，例如「我的[!DNL Workfront Fusion]應用程式」。</td>
      </tr>
      <tr>
        <td>[！UICONTROL重新導向URL]</td>
        <td><code>https://app.workfrontfusion.com/oauth/cb/oauth2</code></td>
      </tr>
    </table>

1. 完成應用程式註冊後，記下[!UICONTROL 應用程式識別碼]。

   >[!IMPORTANT]
   >
   >您需要應用程式ID才能在[!DNL Workfront Fusion]中設定連線。

1. 產生[!UICONTROL 應用程式密碼]。 記下此密碼。

   如需指示，請參閱[!DNL Microsoft]檔案中的[註冊您的應用程式](https://docs.microsoft.com/en-us/graph/auth-register-app-v2)。

   >[!IMPORTANT]
   >
   >您需要[!UICONTROL 應用程式密碼]才能在[!DNL Workfront Fusion]中設定連線。

1. 設定應用程式的許可權。

   如需尋找及設定這些欄位的詳細資訊，請參閱[!UICONTROL Microsoft]檔案中的[在沒有使用者身分的情況下取得存取權](https://docs.microsoft.com/en-us/graph/auth-v2-service)中的「設定Microsoft圖表的許可權」一節。

   <table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[！UICONTROL您的應用程式需要什麼型別的許可權？]</td> 
      <td>選取<code>[!UICONTROL Delegated permissions]</code>。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL選取許可權]</td> 
      <td> <p>選取下列許可權：</p> 
       <ul> 
        <li> <p><code>offline_access</code> </p> </li> 
        <li> <p><code>openid</code> </p> </li> 
        <li> <p>您的整合所需的任何其他許可權（範例： <code>User.Read</code>）</p> </li> 
       </ul> <p><b>重要</b>：您需要選取的許可權，才能在[!DNL Workfront Fusion]中設定您的連線。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 繼續進行[在 [!DNL Workfront Fusion]](#configure-your-ms-graph-api-connection-in-workfront-fusion)中設定您的 [!DNL MS Graph API] 連線。

## 在[!DNL Workfront Fusion]中設定您的[!DNL MS Graph API]連線

依照 [!DNL Microsoft Application Registration Portal]](#register-workfront-fusion-in-the-microsoft-application-registration-portal)中[註冊 [!DNL Workfront Fusion] 的說明註冊[!DNL Workfront Fusion]後，您可以在[!UICONTROL HTTP] > [!UICONTROL 建立Oauth 2.0]要求模組設定您的連線。

1. 新增[!UICONTROL HTTP] > [!UICONTROL 將OAuth 2.0呼叫]模組新增至您的情境。
1. 按一下[!UICONTROL 連線]欄位旁的&#x200B;**[!UICONTROL 新增]**。
1. 依照以下方式設定連線欄位：

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
      <td> <p>輸入您在[!DNL Microsoft Application Registration Portal]</a>中<a href="#register-workfront-fusion-in-the-microsoft-application-registration-portal" class="MCXref xref">登入[!DNL Workfront Fusion]的步驟4中所選取的許可權。</p> <p>對於每個範圍，按一下<b>[！UICONTROL新增]</b>並輸入許可權。</p> <p>範例： <code>offline_access</code>。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL範圍分隔符號]</td> 
      <td><code>SPACE</code> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL使用者端ID]</td> 
      <td>在[!DNL Microsoft Application Registration Portal]</a>的<a href="#register-workfront-fusion-in-the-microsoft-application-registration-portal" class="MCXref xref">登入[!DNL Workfront Fusion]中，從步驟2輸入[！UICONTROL應用程式識別碼]。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL使用者端密碼]</td> 
      <td>在[!DNL Microsoft Application Registration Portal]</a>的<a href="#register-workfront-fusion-in-the-microsoft-application-registration-portal" class="MCXref xref">登入[!DNL Workfront Fusion]中輸入您在步驟3產生的[！UICONTROL應用程式密碼]。</td> 
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
        <li value="1"> <p>按一下<b>[！UICONTROL新增]</b>。</p> </li> 
        <li value="2"> <p>在<b>[！UICONTROL Key]</b>欄位中，輸入<code>scope</code>。</p> </li> 
        <li value="3"> <p>在<b>[！UICONTROL值]</b>欄位中，輸入您輸入到範圍欄位中的所有[！UICONTROL範圍]，並以空格分隔。</p> <p>範例： <code>offline_access openid User.Read</code></p> </li> 
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

1. 按一下&#x200B;**[!UICONTROL 繼續]**。
1. 在出現的視窗中，按一下&#x200B;**[!UICONTROL 接受]**&#x200B;以完成連線並返回模組。
