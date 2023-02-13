---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 連接器
navigation-topic: http-modules
title: HTTP &gt;提出OAuth 2.0要求模組
description: 為了讓 [!DNL Adobe Workfront Fusion] 向需要OAuth 2.0授權的伺服器發出HTTP(S)要求，您必須先建立OAuth連線。 [!DNL Adobe Workfront Fusion] 確保使用此連線進行的所有呼叫都具有適當的授權標題，並在需要時自動重新整理相關的Token。
author: Becky
feature: Workfront Fusion
exl-id: 6c68c9b9-9f74-44a7-94ed-3785081b8331
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '2172'
ht-degree: 0%

---

# [!UICONTROL HTTP] > [!UICONTROL 提出OAuth 2.0請求] 模組

>[!NOTE]
>
>[!DNL Adobe Workfront Fusion] 要求 [!DNL Adobe Workfront Fusion] 除 [!DNL Adobe Workfront] 授權。

為了讓 [!DNL Adobe Workfront Fusion] 向需要OAuth 2.0授權的伺服器發出HTTP(S)要求，您必須先建立OAuth連線。 [!DNL Adobe Workfront Fusion] 確保使用此連線進行的所有呼叫都具有適當的授權標題，並在需要時自動重新整理相關的Token。

[!DNL Workfront Fusion] 支援下列OAuth 2.0驗證流程：

* 授權碼流
* 隱式流

其他流（如資源所有者密碼憑據流和客戶端憑據流）不會通過此模組自動受支援。

如需OAuth 2.0驗證的詳細資訊，請參閱 [OAuth 2.0授權架構](https://tools.ietf.org/html/rfc6749).

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] （工作自動化和整合） </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>貴組織必須購買 [!DNL Adobe Workfront Fusion] 和 [!DNL Adobe Workfront] 以使用本文所述的功能。</td> 
  </tr>
 </tbody> 
</table>

若要了解您擁有的計畫、授權類型或存取權，請聯絡您的 [!DNL Workfront] 管理員。

如需 [!DNL Adobe Workfront Fusion] 許可證，請參閱 [[!DNL Adobe Workfront Fusion] 授權](../../../workfront-fusion/get-started/license-automation-vs-integration.md)

## 為 [!DNL OAuth] 請求

* [在HTTP >建立OAuth 2.0要求模組中建立連線的一般指示](#general-instructions-for-creating-a-connection-in-the-http--make-an-oauth-20-request-module)
* [在HTTP >中建立與Google連線的指示[!UICONTROL Make] OAuth 2.0要求模組](#instructions-for-creating-a-connection-to-google-in-the-http-make-an-oauth-20-request-module)
* [透過「HTTP >建立OAuth 2.0請求模組」連線至Microsoft Graph API的指示](#instructions-for-connecting-to-microsoft-graph-api-via-the-http--make-an-oauth-20-request-module)

### 在 [!UICONTROL HTTP] > [!UICONTROL 提出OAuth 2.0請求] 模組

1. 在 [!DNL target] 服務 [!DNL Adobe Workfront Fusion] 進行溝通。 此選項很可能位於 [!UICONTROL 開發人員] 部分。

   1. 建立用戶端時，請在 `[!UICONTROL Redirect URL]` 或 `[!UICONTROL Callback URL]` 欄位：

      | 美洲/亞太地區 | https://app.workfrontfusion.com/oauth/cb/oauth2 |
      |---|---|
      | 歐洲、中東和非洲 | https://app-eu.workfrontfusion.com/oauth/cb/oauth2 |

   1. 建立用戶端後，指定服務會顯示2個索引鍵： `[!UICONTROL Client ID]` 和 `[!UICONTROL Client Secret]`. 有些服務稱為 `[!UICONTROL App Key]` 和 `[!UICONTROL App Secret]` . 將金鑰和機密儲存在安全位置，以便在Workfront Fusion中建立連線時提供這些金鑰和機密。

1. 尋找 `[!UICONTROL Authorize URI]` 和 `[!UICONTROL Token URI]` （位於指定服務的API檔案中）。 這些是URL位址，可透過 [!DNL Workfront Fusion] 與 [!DNL target] 服務。 地址用於OAuth授權。

   >[!NOTE]
   >
   >如果服務使用隱式流，則您只需要 `[!UICONTROL Authorize URI]`.

   >[!INFO]
   >
   >**範例：** Yahoo地址：
   >
   >* 授權URI:
   >
   >`https://api.login.yahoo.com/oauth2/request_auth`
   >
   >* 令牌URI:
   >
   >`https://api.login.yahoo.com/oauth2/get_token`

1. （條件性）如果目標服務使用範圍（存取權限），請檢查服務如何分隔個別範圍，並務必在進階設定中據以設定分隔符號。 如果分隔符號未正確設定， [!DNL Workfront Fusion] 無法建立連接，並且您收到無效的作用域錯誤。
1. 完成上述步驟後，您就可以開始在 [!DNL Workfront Fusion]. 將OAuth 2.0 HTTP(S)要求和回應處理模組新增至您的案例。
1. 在模組的「連線」欄位中，按一下 **[!UICONTROL 新增]**.

1. 填寫下列欄位以建立連線：

   <table style="table-layout:auto">  
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL連接名] </td> 
      <td> <p>輸入連線的名稱。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL流類型]</p> </td> 
      <td> <p>選取用於取得Token的流程。</p> 
       <ul> 
        <li><strong>[!UICONTROL授權代碼]</strong>:輸入 <code>[!UICONTROL Authorize URI]</code> 和 <code>[!UICONTROL Token URI]</code> 從服務的API檔案。</li> 
        <li><strong>[!UICONTROL隱式]</strong>:輸入 <code>[!UICONTROL Authorize URI]</code> 從服務的API檔案。</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL範圍] </td> 
      <td> <p>添加單個作用域。 您可以在指定服務的開發人員(API)檔案中找到此資訊。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL範圍分隔符] </td> 
      <td> <p>選擇上面輸入的範圍應用於分隔的範圍。 您可以在指定服務的開發人員(API)檔案中找到此資訊。</p> <p>警告：如果分隔符號未正確設定， [!DNL Workfront Fusion] 無法建立連接，您會收到無效的作用域錯誤。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL客戶端ID] </td> 
      <td> <p>輸入客戶端ID。 在您要連線的服務中建立OAuth用戶端時，您已取得用戶端ID。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL客戶端密碼]</td> 
      <td> <p> 輸入用戶端密碼。 在您要連線的服務中建立OAuth用戶端時，您已取得用戶端密碼。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL授權參數]</p> </td> 
      <td> <p>新增您要納入授權呼叫的任何參數。 一律會自動加入下列標準參數，不需要新增。</p> <p>標準參數：</p> 
       <ul> 
        <li> <p><strong>[!UICONTROL response_type]</strong> </p> <p> <code>code </code>適用於[!UICONTROL授權碼流程]和 <code>token </code>適用於[!UICONTROL隱式流]</p> </li> 
        <li> <p><strong>[!UICONTROL redirect_uri]</strong> </p> 
         <table style="table-layout:auto">  
          <col> 
          <col> 
          <tbody> 
           <tr> 
            <td role="rowheader">美洲/亞太地區</td> 
            <td>https://app.workfrontfusion.com/oauth/cb/oauth2</td> 
           </tr> 
           <tr> 
            <td role="rowheader">歐洲、中東和非洲 </td> 
            <td>https://app-eu.workfrontfusion.com/oauth/cb/oauth2</td> 
           </tr> 
          </tbody> 
         </table> </li> 
        <li> <p><strong>[!UICONTROL client_id]</strong> </p> <p> 建立帳戶時收到的用戶端ID</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL訪問令牌參數]</p> </td> 
      <td> <p>新增您要納入Token呼叫的任何參數。 一律會自動加入下列標準參數，不需要新增。</p> <p>標準參數：</p> 
       <ul> 
        <li><strong>[!UICONTROL grant_type]</strong>: <code>authorization_code</code></li> 
        <li> <p><strong>[!UICONTROL redirect_uri]:</strong> </p> 
         <table style="table-layout:auto">  
          <col> 
          <col> 
          <tbody> 
           <tr> 
            <td role="rowheader">美洲/亞太地區</td> 
            <td>https://app.workfrontfusion.com/oauth/cb/oauth2</td> 
           </tr> 
           <tr> 
            <td role="rowheader">歐洲、中東和非洲 </td> 
            <td>https://app-eu.workfrontfusion.com/oauth/cb/oauth2</td> 
           </tr> 
          </tbody> 
         </table> </li> 
        <li><strong>[!UICONTROL client_id]</strong>:您建立帳戶時收到的用戶端ID會自動包含在請求內文中</li> 
        <li><strong>client_secret</strong>:您建立帳戶時收到的用戶端密碼會自動包含在請求內文中</li> 
        <li><strong>代碼</strong>:授權請求傳回的代碼</li> 
       </ul> <p>備註:  <p>OAuth 2.0標準在此步驟中至少支援兩種用戶端驗證方法(<code>[!UICONTROL client_secret_basic]</code> 和 <code>[!UICONTROL client_secret_post]</code>)。 [!DNL Workfront Fusion] 會透過 <code>[!UICONTROL client_secret_post]</code> 方法。 因此，這些參數會自動納入代號要求內文中。 </p> <p>如需OAuth 2.0驗證的詳細資訊，請參閱 <a href="https://tools.ietf.org/html/rfc6749">OAuth 2.0授權架構</a>.</p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL刷新令牌參數]</p> </td> 
      <td> <p>新增您要納入Token呼叫的任何參數。 一律會自動加入下列標準參數，不需要新增。</p> <p>標準參數：</p> 
       <ul> 
        <li> <p><strong>[!UICONTROL grant_type]</strong>: <code>refresh_token</code></p> </li> 
        <li> <p><strong>[!UICONTROL refresh_token]</strong>:您要連線的服務所取得的最新重新整理Token</p> </li> 
        <li> <p><strong>[!UICONTROL client_id]</strong>:您建立帳戶時收到的用戶端ID會自動包含在請求內文中</p> </li> 
        <li> <p><strong>[!UICONTROL client_secret]</strong>:您建立帳戶時收到的用戶端密碼會自動包含在請求內文中</p> </li> 
       </ul> <p>備註:  <p>OAuth 2.0標準在此步驟中至少支援兩種用戶端驗證方法(<code>[!UICONTROL client_secret_basic]</code> 和 <code>[!UICONTROL client_secret_post]</code>)。 [!DNL Workfront Fusion] 會透過 <code>[!UICONTROL client_secret_post]</code> 方法。 因此，這些參數會自動納入代號要求內文中。 </p> <p>如需OAuth 2.0驗證的詳細資訊，請參閱 <a href="https://tools.ietf.org/html/rfc6749">OAuth 2.0授權架構</a>.</p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL自訂標題]</p> </td> 
      <td> <p>指定要包含在[!UICONTROL Token]和R[!UICONTROL刷新Token]步驟的標題中的任何其他鍵和值。</p> <p>備註:  <p>OAuth 2.0標準在此步驟中至少支援兩種用戶端驗證方法(<code>[!UICONTROL client_secret_basic]</code> 和 <code>[!UICONTROL client_secret_post]</code>)。 [!DNL Workfront Fusion] 不會自動支援 <code>[!UICONTROL client_secret_basic]</code> 方法。 如果您要連線的服務預期會將用戶端ID和用戶端密碼合併為單一字串，然後將base64編碼為授權標題，則您應在此新增該標題和金鑰值。</p> <p> 如需OAuth 2.0驗證的詳細資訊，請參閱 <a href="https://tools.ietf.org/html/rfc6749">OAuth 2.0授權架構</a>.</p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL代號放置]</p> </td> 
      <td> <p>選取連線至指定的URL時，要在[!UICONTROL標題]、[!UICONTROL查詢字串]中還是兩者中傳送代號。</p> <p>Token最常在請求標題中傳送。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL標頭令牌名稱] </td> 
      <td> <p>在標題中輸入授權Token的名稱。 預設: <code>[!UICONTROL Bearer]</code>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL查詢字串參數名稱] </td> 
      <td> <p>在查詢字串中輸入授權Token的名稱。 預設: <code>[!UICONTROL access_token]</code>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下 **[!UICONTROL 繼續]** 保存連接設定。
1. 繼續 [OAuth 2.0要求模組設定](#oauth-20-request-module-setup).

### 建立與 [!DNL Google] 在 [!UICONTROL HTTP] >[!UICONTROL 提出OAuth 2.0要求模組]

下列範例說明如何使用 [!UICONTROL HTTP] > [!UICONTROL 建立OAuth 2.0] 要求模組連線至 [!DNL Google].

1. 請確定您已建立專案、設定OAuth設定，並產生憑證，如 [Connect [!DNL Adobe Workfront Fusion] to [!DNL Google Services] 使用自訂OAuth用戶端](../../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).
1. 開啟 [!UICONTROL HTTP] >[!UICONTROL 提出OAuth 2.0請求] 模組。
1. 按一下 **[!UICONTROL 新增]** 連線方塊旁邊。
1. 輸入下列值：

   <table style="table-layout:auto">  
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL連接名] </td> 
      <td> <p>輸入連線的名稱。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL流類型]</p> </td> 
      <td> <p>[!UICONTROL授權代碼]</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL授權URI]</td> 
      <td><code>https://accounts.google.com/o/oauth2/v2/auth</code> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL令牌URI]</td> 
      <td><code>https://www.googleapis.com/oauth2/v4/token</code> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL範圍] </td> 
      <td> <p>添加單個作用域。 有關作用域的詳細資訊，請參見 <a href="https://developers.google.com/identity/protocols/oauth2/scopes">OAuth 2.O範圍 [!DNL Google] API</a> 在 [!DNL Google] 檔案。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL範圍分隔符] </td> 
      <td> <p>[!UICONTROL空間]</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL客戶端ID] </td> 
      <td> <p>輸入 [!DNL Google] 用戶端ID。 </p> <p>若要建立用戶端ID，請參閱 <a href="../../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md#create2" class="MCXref xref">建立OAuth憑證</a> in <a href="../../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md" class="MCXref xref">[!DNL Connect Adobe Workfront Fusion] to [!DNL Google Services] 使用自訂OAuth用戶端</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL客戶端密碼]</td> 
      <td> <p>輸入 [!DNL Google] 用戶端密碼。 </p> <p>若要建立用戶端密碼，請參閱 <a href="../../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md#create2" class="MCXref xref">建立OAuth憑證</a> in <a href="../../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md" class="MCXref xref">[!DNL Connect Adobe Workfront Fusion] to [!DNL Google] 使用自訂OAuth用戶端的服務</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL授權參數]</p> </td> 
      <td> <p>新增 <code>[!UICONTROL access_type]</code> - <code>[!UICONTROL offline] </code>機碼值組。</p> <p> <img src="assets/google-authentication-http.png"> </p> <p>注意：如果您遇到驗證問題（例如，令牌重新整理），請嘗試新增 <code>[!UICONTROL prompt] </code>- <code>[!UICONTROL consent] </code>機碼值組。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下 **[!UICONTROL 繼續]** 保存連接設定。
1. 繼續 [OAuth 2.0要求模組設定](#oauth-20-request-module-setup).

### 連接到 [!DNL Microsoft Graph API] 透過 [!UICONTROL HTTP] > [!UICONTROL 提出OAuth 2.0請求] 模組

有關 [!DNL Microsoft Graph API]，請參閱 [呼叫 [!DNL MS Graph REST API] 透過 [!DNL Adobe Workfront Fusion] [!UICONTROL HTTP] > [!UICONTROL 提出OAuth 2.0請求] 模組](../../../workfront-fusion/connections/call-the-ms-graph-rest-api-.md).

## OAuth 2.0要求模組設定

當您建立 [!DNL Oauth 2].0連接，如 [為 [!DNL OAuth] 請求](#creating-a-connection-for-an-oauth-request)，視需要繼續設定模組。 所有授權Token都會自動包含在此請求中，以及包含在使用相同連線的任何其他請求中。

當您設定 [!UICONTROL HTTP] >[!UICONTROL 提出OAuth 2.0請求] 模組， [!DNL Workfront Fusion] 顯示下列欄位。 模組中的粗體標題表示必填欄位。

如果您在欄位或函式上方看到對應按鈕，則可使用它來設定該欄位的變數和函式。 如需詳細資訊，請參閱 [將資訊從一個模組對應到 [!DNL Adobe Workfront Fusion]](../../../workfront-fusion/mapping/map-information-between-modules.md).

<!--
<img src="assets/map-toggle-350x74.png" style="width: 350;height: 74;" data-mc-conditions="QuicksilverOrClassic.Draft mode">
-->

<table style="table-layout:auto">  
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關設定連接的資訊，請參閱 <a href="#creating-a-connection-for-an-oauth-request" class="MCXref xref">為OAuth請求建立連線</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL將所有狀態評估為錯誤（2xx和3xx除外） </td> 
   <td> <p>使用此選項可設定錯誤處理。</p> <p>如需詳細資訊，請參閱 <a href="../../../workfront-fusion/errors/error-handling.md" class="MCXref xref">錯誤處理 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL] </td> 
   <td> <p>輸入您要傳送要求的URL，例如API端點、網站等。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL方法]</p> </td> 
   <td> <p>選取設定API呼叫所需的HTTP要求方法。 如需詳細資訊，請參閱 <a href="../../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">中的HTTP要求方法 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL標題] </td> 
   <td> <p>以標準JSON物件的形式新增請求的標題。 例如， <code>{"Content-type":"application/json"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL查詢字串]</td> 
   <td> <p> 輸入所需的查詢索引鍵值配對。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL主體類型]</p> </td> 
   <td> <p>HTTP Body是在HTTP交易訊息中傳送的資料位元組，若有需要使用，則緊接在標題後。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Raw]</strong> </p> <p>原始內文類型通常適用於大部分HTTP內文要求，即使在開發人員檔案未指定要傳送的資料的情況下亦然。</p> <p>在[!UICONTROL內容類型]欄位中指定解析資料的形式。</p> <p>儘管已選取內容類型，但資料會以開發人員檔案所規定或要求的任何格式輸入。</p> </li> 
     <li> <p><strong>[!UICONTROL Application/x-www-form-urlencoded]</strong> </p> <p>此內文類型是用來POST資料 <code>[!UICONTROL application/x-www-form-urlencoded]</code>.</p> <p>針對 <code>[!UICONTROL application/x-www-form-urlencoded]</code>，則傳送至伺服器的HTTP訊息內文基本上是一個查詢字串。 索引鍵和值會以由 <code>&amp;</code> 和 <code>=</code> 在索引鍵和值之間。 </p> <p>對於二進位資料， <code>use [!UICONTROL multipart/form-data]</code> 。</p> 
      <div class="example" data-mc-autonum="<b>Example: </b>">
       <span class="autonumber"><span><b>範例: </b></span></span> 
       <p>產生的HTTP要求格式範例：</p> 
       <p><code>field1=value1&amp;field2=value2</code> </p> 
      </div> </li> 
     <li> <p><strong>[!UICONTROL多部分/表單資料]</strong> </p> <p>[!UICONTROL Multipart/form-data]是用於傳送檔案和資料的HTTP多部分請求。 它通常用於將檔案上傳至伺服器。</p> <p>新增要在請求中傳送的欄位。 每個欄位都必須包含機碼值組。</p> 
      <ul> 
       <li> <p><strong>[!UICONTROL文本]</strong> </p> <p>輸入要在請求內文中傳送的索引鍵和值。</p> </li> 
       <li> <p><strong>[!UICONTROL檔案]</strong> </p> <p>輸入索引鍵，並在請求內文中指定您要傳送的來源檔案。</p> <p>映射要從前一個模組上載的檔案(如[!UICONTROL HTTP] &gt;[!UICONTROL Get a File]或[!UICONTROL Google Drive] &gt;[!UICONTROL Download a File)]，或手動輸入檔案名和檔案資料。</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Parse響應]</p> </td> 
   <td> <p>啟用此選項可自動剖析回應並轉換JSON和XML回應，因此您不需要使用[!UICONTROL JSON] &gt; [!UICONTROL Parse JSON]或[!UICONTROL XML] &gt; [!UICONTROL Parse XML]模組。</p> <p>您必須先手動執行模組一次，以便模組能辨識回應內容，並允許您在後續模組中對應該內容，才能使用剖析好的JSON或XML內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL超時] </td> 
   <td> <p>以秒為單位輸入請求逾時(1-300)。 預設為40秒。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL與其他HTTP模組共用Cookie]</td> 
   <td> <p> 啟用此選項，可將伺服器上的Cookie與您案例中的所有HTTP模組共用。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL自簽名證書]</td> 
   <td> <p> 如果您想使用自行簽署的憑證使用TLS，請上傳憑證。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL拒絕使用未驗證（自簽名）證書的連接] </td> 
   <td> <p>啟用此選項可拒絕使用未驗證TLS證書的連接。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL遵循重新導向]</td> 
   <td> <p> 啟用此選項，以使用3xx回應遵循URL重新導向。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL遵循所有重新導向] </td> 
   <td> <p>啟用此選項，使用所有回應代碼遵循URL重新導向。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL禁用與陣列相同的多個查詢字串鍵的序列化]</p> </td> 
   <td> <p>依預設， [!DNL Workfront Fusion] 處理與陣列相同之URL查詢字串參數索引鍵的多個值。 例如， <code>www.test.com?foo=bar&amp;foo=baz</code> 將轉換為 <code>www.test.com?foo[0]=bar&amp;foo[1]=baz</code>. 啟用此選項以停用此功能。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL請求壓縮內容]</td> 
   <td> <p> 啟用此選項可要求壓縮版本的網站。</p> <p>這會新增 <code>[!UICONTROL Accept-Encoding]</code> 要求壓縮內容的標題。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL使用相互TLS]</td> 
   <td> <p>啟用此選項，可在HTTP要求中使用相互TLS。</p> <p>如需相互TLS的詳細資訊，請參閱 <a href="../../../workfront-fusion/apps-and-their-modules/http-modules/use-mtls-in-http-modules.md" class="MCXref xref">在的HTTP模組中使用相互TLS [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
