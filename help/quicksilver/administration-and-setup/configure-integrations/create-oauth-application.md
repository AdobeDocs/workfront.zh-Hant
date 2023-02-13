---
title: 為建立OAuth2應用程式 [!DNL Workfront] 整合
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: administrator-integrations
description: 作為 [!DNL Adobe Workfront] 管理員，您可以為執行個體建立OAuth2應用程式 [!DNL Workfront]，可讓其他應用程式存取Workfront。 接著，您的使用者就可授予其他應用程式存取其Workfront資料的權限。 如此一來，您就能將Workfront與您所選擇的應用程式整合，包括您自己的內部應用程式。
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
exl-id: e13c7dda-8945-47ad-b6d3-4d6a62b368f5
source-git-commit: f7e3182776e6b62103cd755b2fbd5057efc95394
workflow-type: tm+mt
source-wordcount: '1917'
ht-degree: 6%

---

# 為建立OAuth2應用程式 [!DNL Workfront] 整合

作為 [!DNL Adobe Workfront] 管理員，您可以為執行個體建立OAuth2應用程式 [!DNL Workfront]，允許其他應用程式存取 [!DNL Workfront]. 然後，您的使用者就可以授予其他應用程式存取其 [!DNL Workfront] 資料。 這樣，您就可以與您所選擇的應用程式整合，包括您自己的內部應用程式。

當您建立 [!UICONTROL OAuth2] 應用程式時，您會產生用戶端ID和用戶端密碼。 然後，您的使用者就可以在API呼叫中使用用戶端ID，與您建立的應用程式整合。

>[!NOTE]
>
>在OAuth2的內容中，「建立應用程式」是指在應用程式和伺服器(例如 [!DNL Workfront].

* 如需使用者認證（授權程式碼流程）設定和使用OAuth2應用程式的相關指示，請參閱 [使用授權碼流程設定及使用貴組織的自訂OAuth 2應用程式](../../wf-api/api/oauth-app-code-token-flow.md).
* 如需使用伺服器驗證（JWT流程）設定和使用OAuth2應用程式的指示，請參閱 [使用JWT流程設定及使用貴組織的自訂OAuth 2應用程式](../../wf-api/api/oauth-app-jwt-flow.md).
* 有關使用PKCE配置和使用OAuth2應用程式的說明，請參見 [使用PKCE流配置和使用貴組織的自定義OAuth 2應用程式](../../wf-api/api/oauth-app-pkce-flow.md).

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計劃*</td> 
   <td> <p>[!UICONTROL Pro]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權*</td> 
   <td>[!UICONTROL計畫]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> 您必須是 [!DNL Workfront] 管理員。 </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的 [!DNL Workfront] 管理員。

## OAuth2概觀

假設應用程式需要從 [!DNL Workfront]. 請求資訊的應用程式稱為客戶端。 在此範例中，用戶端名稱為ClientApp。 ClientApp需要訪問特定用戶的資訊，因此需要訪問 [!DNL Workfront] 作為該使用者。 如果您的用戶向ClientApp提供其用戶名和密碼，則ClientApp可以訪問用戶可以訪問的所有資料。 這是一種安全風險，因為ClientApp只需要一組小的特定資訊。

當您為ClientApp建立OAuth2應用程式時，您實際上會告訴 [!DNL Workfront] 允許ClientApp訪問 [!DNL Workfront]，但僅限於其帳戶ClientApp正在存取的使用者授予存取權限時。

## 建立OAuth2應用程式

建立OAuth2應用程式時，請選擇最符合整合需求的應用程式類型。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>應用程式類型</th> 
   <th>最佳</th> 
   <th>驗證方法</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>機器對機器應用程式</p> </td> 
   <td> <p>最適合在伺服器上運行的CLI、守護程式或指令碼</p> <p>範例:</p> 
    <ul> 
     <li> <p>[!DNL Shell] </p> </li> 
     <li> <p>[!DNL Python]</p> </li> 
    </ul> </td> 
   <td> <p>透過使用公開/私密金鑰組編碼的 JSON Web 權杖進行驗證。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>單頁網頁應用程式</p> </td> 
   <td> <p>最適合行動或單頁Web應用程式</p> <p>範例:</p> 
    <ul> 
     <li> <p>[!DNL Javascript]</p> </li> 
     <li> <p>[!DNL Angular]</p> </li> 
     <li> <p>[!DNL React]</p> </li> 
     <li> <p>[!DNL Vue]</p> </li> 
    </ul> </td> 
   <td> <p>透過使用 Proof Key for Code Exchange (PKCE) 的 OAuth 2.0 授權代碼流程進行驗證。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>網頁應用程式</p> </td> 
   <td> <p>最適合在伺服器上處理憑證和代號的伺服器端應用程式</p> <p>範例:</p> 
    <ul> 
     <li> <p>[!DNL Go]</p> </li> 
     <li> <p>[!DNL Java]</p> </li> 
     <li> <p>[!DNL ASP.Net]</p> </li> 
     <li> <p>[!DNL Node.js]</p> </li> 
     <li> <p>[!DNL PHP]</p> </li> 
    </ul> </td> 
   <td> <p>透過 OAuth 2.0 授權代碼流程進行驗證。</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>一次最多可以有10個OAuth2應用程式。

* [使用伺服器驗證（JWT流程）建立OAuth2應用程式](#create-an-oauth2-application-using-server-authentication-jwt-flow)
* [使用使用者憑證建立OAuth2應用程式（授權程式碼流程）](#create-an-oauth2-application-using-user-credentials-authorization-code-flow)
* [使用PKCE建立OAuth2單頁Web應用程式](#create-an-oauth2-single-page-web-application-using-pkce)

### 使用伺服器驗證（JWT流程）建立OAuth2應用程式 {#create-an-oauth2-application-using-server-authentication-jwt-flow}

1. 按一下 **[!UICONTROL 主菜單]** 圖示 ![](assets/main-menu-icon.png) 在 [!DNL Adobe Workfront]，然後按一下 **[!UICONTROL 設定]** ![](assets/gear-icon-settings.png).

1. 在左側導覽面板中，按一下 **[!UICONTROL 系統]**，然後選取 **[!UICONTROL OAuth應用程式]**.
1. 按一下 **[!UICONTROL 建立應用程式整合]**.
1. 在顯示的視窗中，選取 **[!UICONTROL 伺服器驗證]**.
1. 輸入新應用程式的名稱，例如「[!DNL Workfront] 」
1. 按一下 **[!UICONTROL 建立]**。
1. 填寫新應用程式的欄位。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL客戶端ID]</td> 
      <td> <p>此欄位會自動產生。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL客戶端密碼]</td> 
      <td> <p>此欄位會自動產生</p> <p><b>重要</b>:  <p>關閉此頁之前，將此欄位的內容複製到另一個安全檔案。 您將無法再看到此密鑰。</p> <p>如果您遺失此金鑰，請刪除該金鑰並建立新的用戶端密碼。</p> 
        <ol> 
         <li value="1"> <p>按一下 <b>[!UICONTROL刪除]</b> 圖示 <img src="assets/delete.png"> 刪除當前客戶端密碼。</p> </li> 
         <li value="2"> <p>按一下 <b>[!UICONTROL添加客戶端密碼]</b> 來產生新的用戶端密碼。</p> </li> 
        </ol> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL公鑰]</td> 
      <td> <p>伺服器到伺服器應用使用公開和私鑰進行身份驗證。 執行下列任一項作業：</p> 
       <ul> 
        <li> <p>按一下 <b>[!UICONTROL新增公開金鑰]</b> 並從其他應用程式中輸入公鑰。</p> </li> 
        <li> <p>按一下 <b>[!UICONTROL產生公開/私用密鑰對]</b>，然後將公開金鑰與其他應用程式共用。</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL名稱]</td> 
      <td>此名稱與您為應用程式提供的名稱相同。 此欄位不能為空。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL描述]</td> 
      <td>輸入整合的說明。</td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下&#x200B;**[!UICONTROL 儲存]**。

如需使用者認證（授權程式碼流程）設定和使用OAuth2應用程式的相關指示，請參閱 [使用JWT流程設定及使用貴組織的自訂OAuth 2應用程式](../../wf-api/api/oauth-app-jwt-flow.md).

### 使用使用者憑證建立OAuth2應用程式（授權程式碼流程） {#create-an-oauth2-application-using-user-credentials-authorization-code-flow}

1. 按一下 **[!UICONTROL 主菜單]** 圖示 ![](assets/main-menu-icon.png) 在 [!DNL Adobe Workfront]，然後按一下 **[!UICONTROL 設定]** ![](assets/gear-icon-settings.png).
1. 在左側導覽面板中，按一下 **[!UICONTROL 系統]**，然後選取 **[!UICONTROL OAuth應用程式]**.
1. 按一下 **[!UICONTROL 建立應用程式整合]**.
1. 在顯示的視窗中，選取 **[!UICONTROL 使用者驗證]**.
1. 輸入新OAuth2應用程式的名稱，例如「[!DNL Workfront] 」
1. 按一下 **[!UICONTROL 建立]**。
1. 填寫新應用程式的欄位。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL客戶端ID]</td> 
      <td> <p>此欄位會自動產生。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL客戶端密碼]</td> 
      <td> <p>此欄位會自動產生</p> <p><b>重要</b>:  <p>關閉此頁之前，將此欄位的內容複製到另一個安全檔案。 您將無法再看到此密鑰。</p> <p>如果您遺失此金鑰，請刪除該金鑰並建立新的用戶端密碼。</p> 
        <ol> 
         <li value="1"> <p>按一下 <b>[!UICONTROL刪除]</b> 圖示 <img src="assets/delete.png"> 刪除當前客戶端密碼。</p> </li> 
         <li value="2"> <p>按一下 <b>[!UICONTROL添加客戶端密碼]</b> 來產生新的用戶端密碼。</p> </li> 
        </ol> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL重新導向URL]</td> 
      <td>使用者通過驗證後，系統會將其重新導向至此路徑 [!DNL Workfront].</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL刷新令牌輪換]</td> 
      <td>啟用此選項以在每次使用重新整理權杖時，發出新的重新整理權杖。您的應用程式必須在每次重新整理後，儲存新的重新整理權杖。</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL絕對刷新令牌過期]</td> 
      <td> <p>選取您希望在重新整理Token過期之前存在的時間長度。 過期時，您的使用者必須重新登入整合。 如果您不想讓重新整理代號過期，請選取「[!UICONTROL無過期]」。</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">非使用狀態重新整理權杖過期</td> 
      <td> <p>如果使用者在您的系統中尚未處於作用中狀態，則選取其重新整理權杖過期的時間長度。 </p> <p>例如，如果閒置重新整理Token過期為6個月，而使用者未登入6個月，則重新整理Token過期，即使絕對重新整理Token過期時間可能已設定得更長。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL徽標]</td> 
      <td>您可以新增標誌，讓此應用程式更具可識別性。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL名稱]</td> 
      <td>此名稱與您為應用程式提供的名稱相同。 此欄位不能為空。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL描述]</td> 
      <td>輸入整合的說明。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL應用程式說明URL]</td> 
      <td>這可以是「關於我們」頁面的連結，或是包含整合詳細資訊的頁面。</td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下&#x200B;**[!UICONTROL 儲存]**。

如需使用者認證（授權程式碼流程）設定和使用OAuth2應用程式的相關指示，請參閱 [使用授權碼流程設定及使用貴組織的自訂OAuth 2應用程式](../../wf-api/api/oauth-app-code-token-flow.md).

### 使用PKCE建立OAuth2單頁Web應用程式 {#create-an-oauth2-single-page-web-application-using-pkce}

1. 按一下 **[!UICONTROL 主菜單]** 圖示 ![](assets/main-menu-icon.png) 在 [!DNL Adobe Workfront]，然後按一下 **[!UICONTROL 設定]** ![](assets/gear-icon-settings.png).
1. 在左側導覽面板中，按一下 **[!UICONTROL 系統]**，然後選取 **[!UICONTROL OAuth應用程式]**.
1. 按一下 **[!UICONTROL 建立應用程式整合]**.
1. 在顯示的視窗中，選取 **[!UICONTROL 單頁Web應用程式]**.
1. 輸入新名稱 [!UICONTROL OAuth2] 應用程式，例如「[!DNL Workfront] 」
1. 按一下 **[!UICONTROL 建立]**。
1. 填寫新應用程式的欄位。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL客戶端ID]</td> 
      <td> <p>此欄位會自動產生。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL重新導向URL]</td> 
      <td>使用者通過Workfront驗證後，會重新導向至此路徑。</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL刷新令牌輪換]</td> 
      <td>啟用此選項以在每次使用重新整理權杖時，發出新的重新整理權杖。您的應用程式必須在每次重新整理後，儲存新的重新整理權杖。</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL絕對刷新令牌過期]</td> 
      <td> <p>選取您希望在重新整理Token過期之前存在的時間長度。 過期時，您的使用者必須重新登入整合。 如果您不想讓重新整理代號過期，請選取「[!UICONTROL無過期]」。</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL閒置刷新令牌過期]</td> 
      <td> <p>如果使用者在您的系統中尚未處於作用中狀態，則選取其重新整理權杖過期的時間長度。 </p> <p>例如，如果閒置重新整理Token過期為6個月，而使用者未登入6個月，則重新整理Token過期，即使絕對重新整理Token過期時間可能已設定得更長。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL徽標]</td> 
      <td>您可以新增標誌，讓此應用程式更具可識別性。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL名稱]</td> 
      <td>此名稱與您為應用程式提供的名稱相同。 此欄位不能為空。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL描述]</td> 
      <td>輸入整合的說明。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL應用程式說明URL]</td> 
      <td>這可以是「關於我們」頁面的連結，或是包含整合詳細資訊的頁面。</td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下&#x200B;**[!UICONTROL 儲存]**。

## 設定及使用已建立的OAuth2應用程式

若要進一步設定及使用已建立的OAuth2應用程式，需要一些技術知識，包括API呼叫。

* 如需使用者認證（授權程式碼流程）設定和使用OAuth2應用程式的相關指示，請參閱 [使用授權碼流程設定及使用貴組織的自訂OAuth 2應用程式](../../wf-api/api/oauth-app-code-token-flow.md).
* 如需使用伺服器驗證（JWT流程）設定和使用OAuth2應用程式的指示，請參閱 [使用JWT流程設定及使用貴組織的自訂OAuth 2應用程式](../../wf-api/api/oauth-app-jwt-flow.md).
* 有關使用PKCE配置和使用OAuth2應用程式的說明，請參見 [使用PKCE流配置和使用貴組織的自定義OAuth 2應用程式](../../wf-api/api/oauth-app-pkce-flow.md).

## OAuth2處理授權程式碼流程

>[!NOTE]
>
>您的使用者可存取 [!UICONTROL OAuth2] 應用程式。 本節以一般術語說明功能，僅供參考。
>
>如需使用OAuth2應用程式的特定指示，包括特定API呼叫，請參閱 [使用授權碼流程設定及使用貴組織的自訂OAuth 2應用程式](../../wf-api/api/oauth-app-code-token-flow.md).

### 使用授權碼和存取權杖進行授權 {#authorizing-with-an-authorization-code-and-access-token}

1. ClientApp需要 [!DNL Workfront]，因此會傳送要求至 [!DNL Workfront] API `/authorize` 端點。 請求包含 [!UICONTROL response_type] `code`，表示要求應傳回授權碼。
1. 這會觸發 [!DNL Workfront] 向用戶發送驗證提示。 用戶可以在提示中輸入其憑據，該提示提供 [!DNL Workfront] 與ClientApp通信的權限。 如果使用者已登入 [!DNL Workfront]，可以跳過此步驟。
1. 此 [!DNL Workfront] API會將授權碼傳送至ClientApp。
1. ClientApp會在要求中傳送下列資訊至 [!DNL Workfront] API `/token`   端點：

   * 在步驟3中傳送至ClientApp的授權代碼。 這可識別使用者權限的特定例項。
   * 在中設定ClientApp OAuth2應用程式時產生的用戶端密碼 [!DNL Workfront]. 這允許 [!DNL Workfront] 以知道要求來自ClientApp。

1. 如果授權碼和用戶端密碼正確， [!DNL Workfront] 傳送存取權杖至ClientApp。 此存取權杖會直接從 [!DNL Workfront] ，且無法供任何其他使用者或用戶端應用程式檢視、複製或使用。
1. ClientApp將存取權杖傳送至 [!DNL Workfront] 以及特定的資訊要求。
1. 因為存取權杖正確， [!DNL Workfront] 將資訊傳送至ClientApp。

#### 正在刷新訪問令牌

為了安全起見，存取權杖會在短時間內過期。 若要取得新的存取權杖，而不必每次都輸入憑證， [!DNL OAuth2] 使用重新整理Token。 刷新令牌由客戶端儲存。

取得重新整理代號的程式與區段中討論的程式相同 [使用授權碼和存取權杖進行授權](#authorizing-with-an-authorization-code-and-access-token). 授權碼的要求包含範圍 `offline_access`，指出要求應傳回要求Token以及授權代碼。
