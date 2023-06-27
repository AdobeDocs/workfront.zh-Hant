---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 聯結器
navigation-topic: http-modules
title: HTTP &gt；建立OAuth 2.0請求模組
description: 為了進行 [!DNL Adobe Workfront Fusion] 向需要OAuth 2.0授權的伺服器發出HTTP(S)請求，您首先需要建立OAuth連線。 [!DNL Adobe Workfront Fusion] 請確定使用此連線進行的所有呼叫都有適當的授權標頭，並視需要自動重新整理關聯的權杖。
author: Becky
feature: Workfront Fusion
exl-id: 6c68c9b9-9f74-44a7-94ed-3785081b8331
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '2220'
ht-degree: 0%

---

# [!UICONTROL HTTP] > [!UICONTROL 提出OAuth 2.0請求] 模組

>[!NOTE]
>
>[!DNL Adobe Workfront Fusion] 需要 [!DNL Adobe Workfront Fusion] 除了授權外， [!DNL Adobe Workfront] 授權。

為了進行 [!DNL Adobe Workfront Fusion] 向需要OAuth 2.0授權的伺服器發出HTTP(S)請求，您首先需要建立OAuth連線。 [!DNL Adobe Workfront Fusion] 請確定使用此連線進行的所有呼叫都有適當的授權標頭，並視需要自動重新整理關聯的權杖。

[!DNL Workfront Fusion] 支援下列OAuth 2.0驗證流程：

* 授權代碼流程
* 隱含流量

其他流程（例如資源擁有者密碼認證流程和使用者端認證流程）不自動透過此模組支援。

如需OAuth 2.0驗證的詳細資訊，請參閱 [OAuth 2.0授權架構](https://tools.ietf.org/html/rfc6749).

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

有關以下專案的資訊： [!DNL Adobe Workfront Fusion] 授權，請參閱 [[!DNL Adobe Workfront Fusion] 授權](../../../workfront-fusion/get-started/license-automation-vs-integration.md)

## 為建立連線 [!DNL OAuth] 請求

* [在「HTTP >建立OAuth 2.0請求模組」中建立連線的一般指示](#general-instructions-for-creating-a-connection-in-the-http--make-an-oauth-20-request-module)
* [在HTTP中建立與Google連線的指示>[!UICONTROL 製作] OAuth 2.0要求模組](#instructions-for-creating-a-connection-to-google-in-the-http-make-an-oauth-20-request-module)
* [透過「HTTP >提出OAuth 2.0請求模組」連線Microsoft Graph API的指示](#instructions-for-connecting-to-microsoft-graph-api-via-the-http--make-an-oauth-20-request-module)

### 在中建立連線的一般指示 [!UICONTROL HTTP] > [!UICONTROL 提出OAuth 2.0請求] 模組

1. 在中建立OAuth使用者端 [!DNL target] 您想要使用的服務 [!DNL Adobe Workfront Fusion] 以進行通訊。 此選項最可能位於 [!UICONTROL 開發人員] 指定服務的區段。

   1. 建立使用者端時，請在 `[!UICONTROL Redirect URL]` 或 `[!UICONTROL Callback URL]` 欄位：

      | 美洲/APAC | https://app.workfrontfusion.com/oauth/cb/oauth2 |
      |---|---|
      | EMEA | https://app-eu.workfrontfusion.com/oauth/cb/oauth2 |

   1. 建立使用者端後，指定的服務會顯示2個金鑰： `[!UICONTROL Client ID]` 和 `[!UICONTROL Client Secret]`. 有些服務會呼叫這些專案 `[!UICONTROL App Key]` 和 `[!UICONTROL App Secret]` . 將金鑰和秘密儲存在安全位置，以便您在Workfront Fusion中建立連線時提供它們。

1. 尋找 `[!UICONTROL Authorize URI]` 和 `[!UICONTROL Token URI]` 在指定服務的API檔案中。 這些是URL位址， [!DNL Workfront Fusion] 與 [!DNL target] 服務。 這些位址可用於OAuth授權。

   >[!NOTE]
   >
   >如果服務使用隱含流量，則您只需要 `[!UICONTROL Authorize URI]`.

   >[!INFO]
   >
   >**範例：** Yahoo位址：
   >
   >* 授權URI：
   >
   >`https://api.login.yahoo.com/oauth2/request_auth`
   >
   >* 權杖URI：
   >
   >`https://api.login.yahoo.com/oauth2/get_token`

1. （條件式）如果目標服務使用範圍（存取許可權），請檢查服務如何分隔個別範圍，並確定您在進階設定中相應地設定分隔符號。 如果分隔符號未正確設定， [!DNL Workfront Fusion] 無法建立連線，而且您收到無效的範圍錯誤。
1. 完成上述步驟後，您就可以開始在中建立OAuth連線 [!DNL Workfront Fusion]. 將OAuth 2.0 HTTP(S)請求和回應處理模組新增至您的情境。
1. 在模組的「連線」欄位中，按一下 **[!UICONTROL 新增]**.

1. 填寫以下欄位以建立連線：

   <table style="table-layout:auto">  
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[！UICONTROL連線名稱] </td> 
      <td> <p>輸入連線的名稱。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[！UICONTROL流程型別]</p> </td> 
      <td> <p>選取取得Token的流程。</p> 
       <ul> 
        <li><strong>[！UICONTROL授權碼]</strong>：輸入 <code>[!UICONTROL Authorize URI]</code> 和 <code>[!UICONTROL Token URI]</code> 來自服務的API檔案。</li> 
        <li><strong>[！UICONTROL Implicit]</strong>：輸入 <code>[!UICONTROL Authorize URI]</code> 來自服務的API檔案。</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL範圍] </td> 
      <td> <p>新增個別範圍。 您可以在特定服務的開發人員(API)檔案中找到此資訊。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL範圍分隔符號] </td> 
      <td> <p>選取上面輸入的範圍應該用分隔符號來分隔。 您可以在特定服務的開發人員(API)檔案中找到此資訊。</p> <p>警告：如果分隔符號未正確設定， [!DNL Workfront Fusion] 無法建立連線，且您收到無效的範圍錯誤。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL使用者端ID] </td> 
      <td> <p>輸入使用者端ID。 您在要連線的服務中建立OAuth使用者端時，已取得使用者端ID。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL使用者端密碼]</td> 
      <td> <p> 輸入使用者端密碼。 您在要連線的服務中建立OAuth使用者端時，已取得使用者端密碼。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[！UICONTROL Authorize引數]</p> </td> 
      <td> <p>新增您要納入授權呼叫中的任何引數。 下列標準引數一律會自動納入，不需要新增。</p> <p>標準引數：</p> 
       <ul> 
        <li> <p><strong>[！UICONTROL response_type]</strong> </p> <p> <code>code </code>適用於[！UICONTROL授權碼流程]和 <code>token </code>適用於[！UICONTROL Implicit flow]</p> </li> 
        <li> <p><strong>[！UICONTROL redirect_uri]</strong> </p> 
         <table style="table-layout:auto">  
          <col> 
          <col> 
          <tbody> 
           <tr> 
            <td role="rowheader">美洲/APAC</td> 
            <td>https://app.workfrontfusion.com/oauth/cb/oauth2</td> 
           </tr> 
           <tr> 
            <td role="rowheader">EMEA </td> 
            <td>https://app-eu.workfrontfusion.com/oauth/cb/oauth2</td> 
           </tr> 
          </tbody> 
         </table> </li> 
        <li> <p><strong>[！UICONTROL client_id]</strong> </p> <p> 建立帳戶時收到的使用者端ID</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[！UICONTROL存取權杖引數]</p> </td> 
      <td> <p>新增您要包含在Token呼叫中的任何引數。 下列標準引數一律會自動納入，不需要新增。</p> <p>標準引數：</p> 
       <ul> 
        <li><strong>[！UICONTROL grant_type]</strong>： <code>authorization_code</code></li> 
        <li> <p><strong>[！UICONTROL redirect_uri]：</strong> </p> 
         <table style="table-layout:auto">  
          <col> 
          <col> 
          <tbody> 
           <tr> 
            <td role="rowheader">美洲/APAC</td> 
            <td>https://app.workfrontfusion.com/oauth/cb/oauth2</td> 
           </tr> 
           <tr> 
            <td role="rowheader">EMEA </td> 
            <td>https://app-eu.workfrontfusion.com/oauth/cb/oauth2</td> 
           </tr> 
          </tbody> 
         </table> </li> 
        <li><strong>[！UICONTROL client_id]</strong>：您在建立帳戶時收到的使用者端ID會自動包含在要求內文中</li> 
        <li><strong>client_secret</strong>：您在建立帳戶時收到的使用者端密碼會自動包含在要求內文中</li> 
        <li><strong>程式碼</strong>：授權請求傳回的代碼</li> 
       </ul> <p>備註:  <p>OAuth 2.0標準在此步驟中支援至少2種使用者端驗證方法(<code>[!UICONTROL client_secret_basic]</code> 和 <code>[!UICONTROL client_secret_post]</code>)。 [!DNL Workfront Fusion] 透過，自動傳送指定的使用者端ID和密碼 <code>[!UICONTROL client_secret_post]</code> 方法。 因此，這些引數會自動納入為權杖要求內文的一部分。 </p> <p>如需OAuth 2.0驗證的詳細資訊，請參閱 <a href="https://tools.ietf.org/html/rfc6749">OAuth 2.0授權架構</a>.</p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[！UICONTROL重新整理權杖引數]</p> </td> 
      <td> <p>新增您要包含在Token呼叫中的任何引數。 下列標準引數一律會自動納入，不需要新增。</p> <p>標準引數：</p> 
       <ul> 
        <li> <p><strong>[！UICONTROL grant_type]</strong>： <code>refresh_token</code></p> </li> 
        <li> <p><strong>[！UICONTROL refresh_token]</strong>：您所連線的服務所取得的最新重新整理Token</p> </li> 
        <li> <p><strong>[！UICONTROL client_id]</strong>：您在建立帳戶時收到的使用者端ID會自動包含在要求內文中</p> </li> 
        <li> <p><strong>[！UICONTROL client_secret]</strong>：您在建立帳戶時收到的使用者端密碼會自動包含在要求內文中</p> </li> 
       </ul> <p>備註:  <p>OAuth 2.0標準在此步驟中支援至少2種使用者端驗證方法(<code>[!UICONTROL client_secret_basic]</code> 和 <code>[!UICONTROL client_secret_post]</code>)。 [!DNL Workfront Fusion] 透過，自動傳送指定的使用者端ID和密碼 <code>[!UICONTROL client_secret_post]</code> 方法。 因此，這些引數會自動納入為權杖要求內文的一部分。 </p> <p>如需OAuth 2.0驗證的詳細資訊，請參閱 <a href="https://tools.ietf.org/html/rfc6749">OAuth 2.0授權架構</a>.</p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[！UICONTROL自訂標頭]</p> </td> 
      <td> <p>指定要包含在[！UICONTROL Token]和R[！UICONTROL Refresh Token]步驟的標頭中的任何其他金鑰和值。</p> <p>備註:  <p>OAuth 2.0標準在此步驟中支援至少2種使用者端驗證方法(<code>[!UICONTROL client_secret_basic]</code> 和 <code>[!UICONTROL client_secret_post]</code>)。 [!DNL Workfront Fusion] 不會自動支援 <code>[!UICONTROL client_secret_basic]</code> 方法。 如果您要連線的服務預期使用者端ID和使用者端密碼會合併為單一字串，然後將base64編碼為Authorization標頭，則您應該在此處新增該標頭與金鑰值。</p> <p> 如需OAuth 2.0驗證的詳細資訊，請參閱 <a href="https://tools.ietf.org/html/rfc6749">OAuth 2.0授權架構</a>.</p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[！UICONTROL權杖位置]</p> </td> 
      <td> <p>選取在連線至指定的URL時，是以[！UICONTROL標頭]、[！UICONTROL查詢字串]或兩者傳送Token。</p> <p>Token最常在請求標頭中傳送。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL標頭權杖名稱] </td> 
      <td> <p>在標頭中輸入授權權杖的名稱。 預設: <code>[!UICONTROL Bearer]</code>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL查詢字串引數名稱] </td> 
      <td> <p>在查詢字串中輸入授權權杖的名稱。 預設: <code>[!UICONTROL access_token]</code>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下 **[!UICONTROL 繼續]** 以儲存連線設定。
1. 繼續至 [OAuth 2.0要求模組設定](#oauth-20-request-module-setup).

### 建立與的連線的指示 [!DNL Google] 在 [!UICONTROL HTTP] >[!UICONTROL 建立OAuth 2.0請求模組]

以下範例說明如何使用 [!UICONTROL HTTP] > [!UICONTROL 建立OAuth 2.0] 要連線的要求模組 [!DNL Google].

1. 請確定您已建立專案、設定OAuth設定，並產生您的認證，如所述 [Connect [!DNL Adobe Workfront Fusion] 至 [!DNL Google Services] 使用自訂OAuth使用者端](../../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).
1. 開啟 [!UICONTROL HTTP] >[!UICONTROL 提出OAuth 2.0請求] 模組。
1. 按一下 **[!UICONTROL 新增]** 連線方塊旁邊。
1. 輸入下列值：

   <table style="table-layout:auto">  
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[！UICONTROL連線名稱] </td> 
      <td> <p>輸入連線的名稱。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[！UICONTROL流程型別]</p> </td> 
      <td> <p>[！UICONTROL授權碼]</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL授權URI]</td> 
      <td><code>https://accounts.google.com/o/oauth2/v2/auth</code> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL權杖URI]</td> 
      <td><code>https://www.googleapis.com/oauth2/v4/token</code> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL範圍] </td> 
      <td> <p>新增個別範圍。 如需有關範圍的詳細資訊，請參閱 <a href="https://developers.google.com/identity/protocols/oauth2/scopes">OAuth 2.O範圍 [!DNL Google] API</a> 在 [!DNL Google] 說明檔案。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL範圍分隔符號] </td> 
      <td> <p>[！UICONTROL空格]</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL使用者端ID] </td> 
      <td> <p>輸入您的 [!DNL Google] 使用者端ID。 </p> <p>若要建立使用者端ID，請參閱 <a href="../../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md#create2" class="MCXref xref">建立OAuth認證</a> 在 <a href="../../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md" class="MCXref xref">[!DNL Connect Adobe Workfront Fusion] 至 [!DNL Google Services] 使用自訂OAuth使用者端</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL使用者端密碼]</td> 
      <td> <p>輸入您的 [!DNL Google] 使用者端密碼。 </p> <p>若要建立使用者端密碼，請參閱 <a href="../../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md#create2" class="MCXref xref">建立OAuth認證</a> 在 <a href="../../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md" class="MCXref xref">[!DNL Connect Adobe Workfront Fusion] 至 [!DNL Google] 使用自訂OAuth使用者端的服務</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[！UICONTROL Authorize引數]</p> </td> 
      <td> <p>新增 <code>[!UICONTROL access_type]</code> - <code>[!UICONTROL offline] </code>機碼值組。</p> <p> <img src="assets/google-authentication-http.png"> </p> <p>注意：如果您遇到驗證問題（例如重新整理權杖），請嘗試新增 <code>[!UICONTROL prompt] </code>- <code>[!UICONTROL consent] </code>機碼值組。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下 **[!UICONTROL 繼續]** 以儲存連線設定。
1. 繼續至 [OAuth 2.0要求模組設定](#oauth-20-request-module-setup).

### 連線說明 [!DNL Microsoft Graph API] 透過 [!UICONTROL HTTP] > [!UICONTROL 提出OAuth 2.0請求] 模組

如需相關指示 [!DNL Microsoft Graph API]，請參閱 [呼叫 [!DNL MS Graph REST API] 透過 [!DNL Adobe Workfront Fusion] [!UICONTROL HTTP] > [!UICONTROL 提出OAuth 2.0請求] 模組](../../../workfront-fusion/connections/call-the-ms-graph-rest-api-.md).

## OAuth 2.0要求模組設定

當您建立 [!DNL Oauth 2].0連線，如中所述 [為建立連線 [!DNL OAuth] 請求](#creating-a-connection-for-an-oauth-request)，繼續視需要設定模組。 所有授權權杖會自動包含在此請求中，以及使用相同連線的任何其他請求中。

當您設定 [!UICONTROL HTTP] >[!UICONTROL 提出OAuth 2.0請求] 模組， [!DNL Workfront Fusion] 顯示下列欄位。 模組中的粗體標題表示必填欄位。

如果您在欄位或函式上方看到對應按鈕，則可以使用它來設定該欄位的變數和函式。 如需詳細資訊，請參閱 [將資訊從一個模組對應至中的另一個模組 [!DNL Adobe Workfront Fusion]](../../../workfront-fusion/mapping/map-information-between-modules.md).

<!--
<img src="assets/map-toggle-350x74.png" style="width: 350;height: 74;" data-mc-conditions="QuicksilverOrClassic.Draft mode">
-->

<table style="table-layout:auto">  
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[！UICONTROL連線]</td> 
   <td> <p>如需設定連線的詳細資訊，請參閱 <a href="#creating-a-connection-for-an-oauth-request" class="MCXref xref">建立OAuth要求的連線</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL將所有狀態評估為錯誤（2xx和3xx除外） </td> 
   <td> <p>使用此選項可設定錯誤處理。</p> <p>如需詳細資訊，請參閱 <a href="../../../workfront-fusion/errors/error-handling.md" class="MCXref xref">中的錯誤處理 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL URL] </td> 
   <td> <p>輸入您要傳送請求的URL，例如API端點、網站等。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL方法]</p> </td> 
   <td> <p>選取設定API呼叫所需的HTTP要求方法。 如需詳細資訊，請參閱 <a href="../../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">中的HTTP要求方法 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL標頭] </td> 
   <td> <p>以標準JSON物件的形式新增請求的標頭。 例如， <code>{"Content-type":"application/json"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL查詢字串]</td> 
   <td> <p> 輸入所需的查詢索引鍵值配對。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL主體型別]</p> </td> 
   <td> <p>HTTP內文是HTTP交易訊息中傳輸的資料位元組，緊接在標題之後（如果有任何要使用的話）。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL Raw]</strong> </p> <p>Raw內文型別通常適用於大多數HTTP內文要求，即使開發人員檔案未指定要傳送的資料亦然。</p> <p>在[！UICONTROL內容型別]欄位中指定剖析資料的表單。</p> <p>儘管選取了內容型別，但資料仍會以開發人員檔案規定或要求的任何格式輸入。</p> </li> 
     <li> <p><strong>[！UICONTROL Application/x-www-form-urlencoded]</strong> </p> <p>此內文型別使用來POST資料 <code>[!UICONTROL application/x-www-form-urlencoded]</code>.</p> <p>對象 <code>[!UICONTROL application/x-www-form-urlencoded]</code>，傳送至伺服器的HTTP訊息內文基本上是一個查詢字串。 索引鍵和值會以索引鍵/值組編碼，並以以下方式分隔 <code>&amp;</code> 和 <code>=</code> 介於鍵和值之間。 </p> <p>針對二進位資料， <code>use [!UICONTROL multipart/form-data]</code> 而非。</p> 
      <div class="example" data-mc-autonum="<b>Example: </b>">
       <span class="autonumber"><span><b>範例: </b></span></span> 
       <p>產生的HTTP要求格式範例：</p> 
       <p><code>field1=value1&amp;field2=value2</code> </p> 
      </div> </li> 
     <li> <p><strong>[！UICONTROL Multipart/form-data]</strong> </p> <p>[！UICONTROL Multipart/form-data]是用於傳送檔案和資料的HTTP多部分要求。 它通常用於將檔案上傳到伺服器。</p> <p>新增要在請求中傳送的欄位。 每個欄位都必須包含一個索引鍵/值組。</p> 
      <ul> 
       <li> <p><strong>[！UICONTROL文字]</strong> </p> <p>輸入要在要求內文中傳送的索引鍵和值。</p> </li> 
       <li> <p><strong>[！UICONTROL檔案]</strong> </p> <p>輸入金鑰，並指定您要在要求內文中傳送的來源檔案。</p> <p>對應您要從上一個模組上傳的檔案(例如[！UICONTROL HTTP] &gt;[！UICONTROL Get a File]或[！UICONTROL Google Drive] &gt;[！UICONTROL Download a File)]，或手動輸入檔案名稱和檔案資料。</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL剖析回應]</p> </td> 
   <td> <p>啟用此選項可自動剖析回應並轉換JSON和XML回應，因此您不需要使用[！UICONTROL JSON] &gt; [！UICONTROL Parse JSON]或[！UICONTROL XML] &gt; [！UICONTROL Parse XML]模組。</p> <p>在使用剖析的JSON或XML內容之前，請先手動執行一次模組，讓模組可以識別回應內容，並允許您將其對應到後續模組中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL逾時] </td> 
   <td> <p>以秒為單位輸入請求逾時(1-300)。 預設值為40秒。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL與其他HTTP模組共用Cookie]</td> 
   <td> <p> 啟用此選項即可將伺服器的Cookie與您情境中的所有HTTP模組共用。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL自我簽署憑證]</td> 
   <td> <p> 如果您想要使用自我簽署憑證的TLS，請上傳憑證。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL拒絕使用未驗證（自我簽署）憑證的連線] </td> 
   <td> <p>啟用此選項可拒絕使用未驗證TLS憑證的連線。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL遵循重新導向]</td> 
   <td> <p> 啟用此選項可在URL重新導向之後附帶3xx回應。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL遵循所有重新導向] </td> 
   <td> <p>啟用此選項後，URL會重新導向並帶有所有回應代碼。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL停用將多個相同的查詢字串索引鍵序列化為陣列]</p> </td> 
   <td> <p>依預設， [!DNL Workfront Fusion] 處理作為陣列的同一URL查詢字串引數索引鍵的多個值。 例如， <code>www.test.com?foo=bar&amp;foo=baz</code> 將轉換為 <code>www.test.com?foo[0]=bar&amp;foo[1]=baz</code>. 啟動此選項以停用此功能。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL要求壓縮內容]</td> 
   <td> <p> 啟用此選項可請求網站的壓縮版本。</p> <p>這會新增 <code>[!UICONTROL Accept-Encoding]</code> 標頭以請求壓縮內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL使用雙向TLS]</td> 
   <td> <p>啟用此選項可在HTTP請求中使用雙向TLS。</p> <p>如需雙向TLS的詳細資訊，請參閱 <a href="../../../workfront-fusion/apps-and-their-modules/http-modules/use-mtls-in-http-modules.md" class="MCXref xref">在HTTP模組中使用雙向TLS [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
