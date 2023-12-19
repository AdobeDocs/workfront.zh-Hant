---
title: 建立OAuth2應用程式 [!DNL Workfront] 整合
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: administrator-integrations
description: 作為 [!DNL Adobe Workfront] 管理員，您可以為您的執行個體建立OAuth2應用程式 [!DNL Workfront]，可讓其他應用程式存取Workfront。 接著，您的使用者可以授予這些其他應用程式存取其Workfront資料的許可權。 如此一來，您就可以將Workfront與您選擇的應用程式整合，包括您自己的內部應用程式。
author: Becky
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
exl-id: e13c7dda-8945-47ad-b6d3-4d6a62b368f5
source-git-commit: 59c3a57e334d1660e3e59da480a90060b1ba81b7
workflow-type: tm+mt
source-wordcount: '1945'
ht-degree: 6%

---

# 建立OAuth2應用程式 [!DNL Workfront] 整合

作為 [!DNL Adobe Workfront] 管理員，您可以為您的執行個體建立OAuth2應用程式 [!DNL Workfront]，可允許其他應用程式存取 [!DNL Workfront]. 接著，您的使用者就可以將許可權授予這些其他應用程式，以存取其 [!DNL Workfront] 資料。 如此一來，您就可以與您選擇的應用程式整合，包括您自己的內部應用程式。

當您建立 [!UICONTROL OAuth2] 應用程式時，您會產生使用者端ID和使用者端密碼。 接著，您的使用者便可在API呼叫中使用使用者端ID，將與您建立的應用程式整合。

>[!NOTE]
>
>在OAuth2的上下文中，「建立應用程式」是指在應用程式和伺服器之間建立此類存取連結的程式，例如 [!DNL Workfront].

* 如需有關設定和搭配使用者認證（授權碼流程）使用OAuth2應用程式的指示，請參閱 [使用授權程式碼流程設定及使用您組織的自訂OAuth 2應用程式](../../wf-api/api/oauth-app-code-token-flow.md).
* 如需使用伺服器驗證（JWT流程）設定和使用OAuth2應用程式的指示，請參閱 [使用JWT流程設定並使用您組織的自訂OAuth 2應用程式](../../wf-api/api/oauth-app-jwt-flow.md).
* 如需使用PKCE設定和使用OAuth2應用程式的指示，請參閱 [使用PKCE流程設定並使用您組織的自訂OAuth 2應用程式](../../wf-api/api/oauth-app-pkce-flow.md).

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計畫*</td> 
   <td> <p>[！UICONTROL Pro]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權*</td> 
   <td><p>新增：[！UICONTROL Standard]</p>
   或
   <p>目前：[！UICONTROL計畫]</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> 您必須是 [!DNL Workfront] 管理員。 </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的 [!DNL Workfront] 管理員。

## OAuth2總覽

假設應用程式必須從提取某些特定資訊 [!DNL Workfront]. 要求資訊的應用程式稱為使用者端。 在此範例中，使用者端名稱為ClientApp。 ClientApp需要存取特定使用者的資訊，因此必須存取 [!DNL Workfront] 作為該使用者。 如果您的使用者提供ClientApp的使用者名稱和密碼，ClientApp就可以存取使用者可存取的所有資料。 這是安全性風險，因為ClientApp只需要一小組特定資訊。

當您為ClientApp建立OAuth2應用程式時，基本上是告訴 [!DNL Workfront] 該ClientApp被允許存取 [!DNL Workfront]，但前提是ClientApp正在存取的使用者授予存取許可權。

## 建立Oauth2應用程式

建立OAuth2應用程式時，請選擇最符合整合需求的應用程式型別。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>應用程式型別</th> 
   <th>最適合</th> 
   <th>驗證方法</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>機器對機器應用程式</p> </td> 
   <td> <p>最適合伺服器上執行的CLI、精靈或指令碼</p> <p>範例：</p> 
    <ul> 
     <li> <p>[!DNL Shell] </p> </li> 
     <li> <p>[!DNL Python]</p> </li> 
    </ul> </td> 
   <td> <p>透過使用公開/私密金鑰組編碼的 JSON Web 權杖進行驗證。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>單頁網頁應用程式</p> </td> 
   <td> <p>最適合行動或單頁網頁應用程式</p> <p>範例：</p> 
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
   <td> <p>最適合在伺服器上處理認證和權杖的伺服器端應用程式</p> <p>範例：</p> 
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
>您一次最多可以有十個OAuth2應用程式。

* [使用伺服器驗證（JWT流程）建立OAuth2應用程式](#create-an-oauth2-application-using-server-authentication-jwt-flow)
* [使用使用者認證建立OAuth2應用程式（授權代碼流程）](#create-an-oauth2-application-using-user-credentials-authorization-code-flow)
* [使用PKCE建立OAuth2單頁網頁應用程式](#create-an-oauth2-single-page-web-application-using-pkce)

### 使用伺服器驗證（JWT流程）建立OAuth2應用程式 {#create-an-oauth2-application-using-server-authentication-jwt-flow}

{{step-1-to-setup}}

1. 在左側導覽面板中，按一下 **[!UICONTROL 系統]**，然後選取 **[!UICONTROL Oauth2應用程式]**.
1. 按一下 **[!UICONTROL 建立應用程式整合]**.
此 **新OAuth2應用程式** 方塊隨即顯示。
1. 在 **新OAuth2應用程式** 方塊，選取 **[!UICONTROL 伺服器驗證]**.
1. 輸入新應用程式的名稱，例如&quot;[!DNL Workfront] 適用於ClientApp。」
1. 按一下「**[!UICONTROL 建立]**」。
1. 填寫新應用程式的欄位。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[！UICONTROL使用者端ID]</td> 
      <td> <p>此欄位會自動產生。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL使用者端密碼]</td> 
      <td> <p>此欄位會自動產生</p> <p><b>重要</b>：  <p>在關閉此頁面之前，請先將此欄位的內容複製到另一個安全檔案。 您將無法再看到此秘密金鑰。</p> <p>如果您遺失此金鑰，請刪除並建立使用者端密碼。</p> 
        <ol> 
         <li value="1"> <p>按一下 <b>[！UICONTROL Delete]</b> 圖示 <img src="assets/delete.png"> 刪除目前的使用者端密碼。</p> </li> 
         <li value="2"> <p>按一下 <b>[！UICONTROL新增使用者端密碼]</b> 產生新的使用者端密碼。</p> </li> 
        </ol> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL公開金鑰]</td> 
      <td> <p>伺服器對伺服器應用程式使用公開和私密金鑰進行驗證。 執行下列其中一項：</p> 
       <ul> 
        <li> <p>按一下 <b>[！UICONTROL新增公開金鑰]</b> 並輸入其他應用程式的公開金鑰。</p> </li> 
        <li> <p>按一下 <b>[！UICONTROL產生公用/私用金鑰組]</b>，然後與其他應用程式共用公開金鑰。</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL名稱]</td> 
      <td>此名稱與您提供應用程式的名稱相同。 此欄位不得為空白。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL說明]</td> 
      <td>輸入整合的說明。</td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下「**[!UICONTROL 儲存]**」。

如需有關設定和搭配使用者認證（授權碼流程）使用OAuth2應用程式的指示，請參閱 [使用JWT流程設定並使用您組織的自訂OAuth 2應用程式](../../wf-api/api/oauth-app-jwt-flow.md).

### 使用使用者認證建立OAuth2應用程式（授權代碼流程） {#create-an-oauth2-application-using-user-credentials-authorization-code-flow}

{{step-1-to-setup}}

1. 在左側導覽面板中，按一下 **[!UICONTROL 系統]**，然後選取 **[!UICONTROL Oauth2應用程式]**.
1. 按一下 **[!UICONTROL 建立應用程式整合]**.

   此 **新OAuth2應用程式** 顯示。
1. 在 **新OAuth2應用程式** 方塊，選取 **[!UICONTROL 使用者驗證]**.
1. 輸入新OAuth2應用程式的名稱，例如&quot;[!DNL Workfront] 適用於ClientApp。」
1. 按一下「**[!UICONTROL 建立]**」。
1. 填寫新應用程式的欄位。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[！UICONTROL使用者端ID]</td> 
      <td> <p>此欄位會自動產生。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL使用者端密碼]</td> 
      <td> <p>此欄位會自動產生</p> <p><b>重要</b>：  <p>在關閉此頁面之前，請先將此欄位的內容複製到另一個安全檔案。 您將無法再看到此秘密金鑰。</p> <p>如果您遺失此金鑰，請刪除並建立使用者端密碼。</p> 
        <ol> 
         <li value="1"> <p>按一下 <b>[！UICONTROL Delete]</b> 圖示 <img src="assets/delete.png"> 刪除目前的使用者端密碼。</p> </li> 
         <li value="2"> <p>按一下 <b>[！UICONTROL新增使用者端密碼]</b> 產生新的使用者端密碼。</p> </li> 
        </ol> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL重新導向URL]</td> 
      <td>使用者在透過進行驗證後，將會重新導向至此路徑 [!DNL Workfront].</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[！UICONTROL重新整理權杖輪換]</td> 
      <td>啟用此選項以在每次使用重新整理權杖時，發出新的重新整理權杖。您的應用程式必須在每次重新整理後，儲存新的重新整理權杖。</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[！UICONTROL絕對重新整理權杖到期]</td> 
      <td> <p>選取您希望在重新整理權杖過期之前存在的時間。 當它過期時，您的使用者必須再次登入整合。 如果您不希望重新整理權杖過期，請選取「[！UICONTROL無過期]」。</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">非使用狀態重新整理權杖過期</td> 
      <td> <p>選取多長時間，如果使用者未在使用您的系統中，其重新整理Token就會過期。 </p> <p>例如，如果非使用狀態重新整理權杖到期日為6個月，而使用者已有6個月未登入，則重新整理權杖將會到期，即使絕對重新整理權杖到期日可能設定的時間更長。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL標誌]</td> 
      <td>您可以新增標誌，讓此應用程式更具識別性。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL名稱]</td> 
      <td>此名稱與您提供應用程式的名稱相同。 此欄位不得為空白。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL說明]</td> 
      <td>輸入整合的說明。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL應用程式說明URL]</td> 
      <td>這可以是「關於我們」頁面的連結，或包含整合詳細資訊的頁面。</td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下「**[!UICONTROL 儲存]**」。

如需有關設定和搭配使用者認證（授權碼流程）使用OAuth2應用程式的指示，請參閱 [使用授權程式碼流程設定及使用您組織的自訂OAuth 2應用程式](../../wf-api/api/oauth-app-code-token-flow.md).

### 使用PKCE建立OAuth2單頁網頁應用程式 {#create-an-oauth2-single-page-web-application-using-pkce}

{{step-1-to-setup}}

1. 在左側導覽面板中，按一下 **[!UICONTROL 系統]**，然後選取 **[!UICONTROL Oauth2應用程式]**.
1. 按一下 **[!UICONTROL 建立應用程式整合]**.

   此 **新OAuth2應用程式** 方塊隨即顯示。
1. 在 **新OAuth2應用程式** 方塊，選取 **[!UICONTROL 單頁網頁應用程式]**.
1. 輸入新專案的名稱 [!UICONTROL OAuth2] 應用程式，例如&quot;[!DNL Workfront] 適用於ClientApp。」
1. 按一下「**[!UICONTROL 建立]**」。
1. 填寫新應用程式的欄位。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[！UICONTROL使用者端ID]</td> 
      <td> <p>此欄位會自動產生。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL重新導向URL]</td> 
      <td>使用者透過Workfront驗證後，系統會將使用者重新導向至此路徑。</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[！UICONTROL每次使用時都輪換重新整理權杖]</td> 
      <td>啟用此選項以在每次使用重新整理權杖時，發出新的重新整理權杖。您的應用程式必須在每次重新整理後，儲存新的重新整理權杖。</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[！UICONTROL絕對期限]</td> 
      <td> <p>選取您希望在重新整理權杖過期之前存在的時間。 當它過期時，您的使用者必須再次登入整合。 如果您不希望重新整理權杖過期，請選取「[！UICONTROL無過期]」。</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[！UICONTROL非使用狀態到期日]</td> 
      <td> <p>選取多長時間，如果使用者未在使用您的系統中，其重新整理Token就會過期。 </p> <p>例如，如果非使用狀態重新整理權杖到期日為6個月，而使用者已有6個月未登入，則重新整理權杖將會到期，即使絕對重新整理權杖到期日可能設定的時間更長。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL標誌]</td> 
      <td>您可以新增標誌，讓此應用程式更具識別性。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL名稱]</td> 
      <td>此名稱與您提供應用程式的名稱相同。 此欄位不得為空白。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL說明]</td> 
      <td>輸入整合的說明。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL開發人員姓名]</td> 
      <td>這是設定OAuth2應用程式的開發人員名稱。</td> 
     </tr> 
   <tr> 
      <td role="rowheader">[！UICONTROL開發人員電子郵件地址]</td> 
      <td>這是設定OAuth2應用程式的開發人員電子郵件地址。</td> 
     </tr> 
   <tr> 
      <td role="rowheader">[！UICONTROL隱私權原則UTL]</td> 
      <td>這是貴組織儲存隱私權原則的連結。</td> 
     </tr>


   </tbody> 
   </table>

   <!-- removed this from the table, and added "Developer name" and following rows:
   [!UICONTROL App Description URL]</td> 
      <td>This can be a link to an "About us" page or a page with more information about the integration.> -->

1. 按一下「**[!UICONTROL 儲存]**」。

## 設定並使用建立的OAuth2應用程式

進一步設定及使用已建立的OAuth2應用程式需要一些技術知識，包括API呼叫。

* 如需有關設定和搭配使用者認證（授權碼流程）使用OAuth2應用程式的指示，請參閱 [使用授權程式碼流程設定及使用您組織的自訂OAuth 2應用程式](../../wf-api/api/oauth-app-code-token-flow.md).
* 如需使用伺服器驗證（JWT流程）設定和使用OAuth2應用程式的指示，請參閱 [使用JWT流程設定並使用您組織的自訂OAuth 2應用程式](../../wf-api/api/oauth-app-jwt-flow.md).
* 如需使用PKCE設定和使用OAuth2應用程式的指示，請參閱 [使用PKCE流程設定並使用您組織的自訂OAuth 2應用程式](../../wf-api/api/oauth-app-pkce-flow.md).

## 授權代碼流程的OAuth2流程

>[!NOTE]
>
>您的使用者存取 [!UICONTROL OAuth2] 應用程式透過API。 本節以一般術語說明功能，僅供參考。
>
>如需使用OAuth2應用程式的特定指示，包括特定API呼叫，請參閱 [使用授權程式碼流程設定及使用您組織的自訂OAuth 2應用程式](../../wf-api/api/oauth-app-code-token-flow.md).

### 以授權代碼和存取權杖授權 {#authorizing-with-an-authorization-code-and-access-token}

1. ClientApp需要一些資訊，來自 [!DNL Workfront]，因此會傳送要求至 [!DNL Workfront] API `/authorize` 端點。 此請求包括 [!UICONTROL response_type] `code`，這表示要求應傳回授權碼。
1. 此觸發程式 [!DNL Workfront] 傳送驗證提示給使用者。 使用者可以在提示中輸入其認證，這會 [!DNL Workfront] 與ClientApp通訊的許可權。 如果使用者已登入 [!DNL Workfront]，此步驟可能會略過。
1. 此 [!DNL Workfront] API傳送授權代碼給ClientApp。
1. ClientApp會在要求中將下列資訊傳送至 [!DNL Workfront] API `/token`   端點：

   * 在步驟3中傳送至ClientApp的授權代碼。 這會識別使用者許可權的特定執行個體。
   * 當您在中設定ClientApp OAuth2應用程式時所產生的使用者端密碼 [!DNL Workfront]. 這允許 [!DNL Workfront] 以確認要求來自ClientApp。

1. 如果授權代碼和使用者端密碼正確， [!DNL Workfront] 傳送存取權杖給ClientApp。 此存取Token會直接從傳送 [!DNL Workfront] 至ClientApp，且任何其他使用者或使用者端應用程式均無法檢視、複製或使用。
1. ClientApp傳送存取權杖到 [!DNL Workfront] 以及特定的資訊要求。
1. 因為存取權杖正確， [!DNL Workfront] 傳送資訊至ClientApp。

#### 正在重新整理存取權杖

為了安全起見，存取權杖會在短時間內過期。 若要取得新的存取權杖，而不需每次都輸入認證， [!DNL OAuth2] 使用重新整理權杖。 重新整理Token會由使用者端儲存。

取得重新整理權杖的程式與區段中討論的程式相同 [以授權代碼和存取權杖授權](#authorizing-with-an-authorization-code-and-access-token). 授權碼要求包含範圍 `offline_access`，這表示請求應傳回請求權杖以及授權代碼。
