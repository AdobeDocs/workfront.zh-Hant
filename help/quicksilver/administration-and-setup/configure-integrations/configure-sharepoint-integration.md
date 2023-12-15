---
title: 設定 [!DNL SharePoint] 整合
user-type: administrator
product-area: system-administration;workfront-integrations;setup
navigation-topic: administrator-integrations
description: 您可以整合 [!DNL Workfront] 替換為 [!DNL SharePoint] 線上，讓使用者能夠導覽至、連結及新增 [!DNL SharePoint] Workfront中的檔案。 提供的功能與其他功能類似 [!DNL Workfront] 檔案整合。
author: Becky
feature: System Setup and Administration, [!DNL Workfront] Integrations and Apps, Digital Content and Documents
role: Admin
exl-id: fd45e1bc-9a35-4960-a73a-ff845216afe4
source-git-commit: b090983de417cf6a4dd36c9398da7dcc0296766a
workflow-type: tm+mt
source-wordcount: '1591'
ht-degree: 0%

---

# 設定 [!DNL SharePoint] 整合

<!--Audited: 12/2023-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

>[!IMPORTANT]
>
>新的 [!DNL SharePoint] 整合隨22.3版（2022年7月）發佈到生產環境。 雖然您的使用者仍可存取透過舊版連結的檔案 [!DNL SharePoint] 整合，他們必須使用新的 [!DNL SharePoint] 整合以從SharePoint連結檔案。
>
>* 新的SharePoint整合不需要管理員進行設定，可由個別使用者進行設定。 不過，為確保順利轉換至新的SharePoint整合，Workfront管理員必須在Workfront設定區域中變更幾項設定。
>
>    如需詳細資訊與指示，請參閱 [設定舊版SharePoint整合，以便持續存取檔案](#configure-the-legacy-sharepoint-integration-for-continued-access-to-documents) 本文章內容。
>    
>* 我們建議使用者連結目前透過舊版連結的檔案 [!DNL SharePoint] 透過新的整合進行整合。
>    
>    如需連結檔案的指示，請參閱 [從外部應用程式連結檔案](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

您可以整合 [!DNL Workfront] 替換為 [!DNL SharePoint Online]，讓使用者能導覽至、連結及新增 [!DNL SharePoint] Workfront中的檔案。 提供的功能與其他功能類似 [!DNL Workfront] 整合，例如 [!DNL Google Drive]， [!DNL Box]、和 [!DNL Dropbox].

此整合僅與相容 [!DNL SharePoint Online]. 的內部部署例項 [!DNL SharePoint] 不受支援。

## 存取需求

您必須具備下列專案才能執行本文所述的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計劃</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權</td> 
   <td>新增：標準 <p>或</p><p>目前：計畫</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td>您必須是 [!DNL Workfront] 管理員。 有關的資訊 [!DNL Workfront] 管理員，請參閱 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予使用者完整管理存取權</a>. </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的 [!DNL Workfront] 管理員。

## 先決條件

您必須擁有中任何必要的存取權或許可權 [!DNL SharePoint] 若要修改或設定您的 [!DNL SharePoint] 整合。

## 透過新的SharePoint整合連結檔案

個別使用者可透過新檔案連結檔案 [!DNL SharePoint] 整合。 整合不需要管理員設定。 相反地，使用者會登入 [!DNL Microsoft] 連結檔案時的帳戶，可讓整合功能存取使用者檔案中可用的檔案。 [!DNL SharePoint].

使用者第一次連線 [!DNL Workfront] [!DNL SharePoint] 整合至其 [!DNL SharePoint] 帳戶，他們將看到並同意以下所有許可權： [!DNL Workfront] 在與以下專案互動時使用 [!UICONTROL SharePoint] 帳戶。 讀取許可權允許 [!DNL Workfront] 若要檢視及存取檔案，請執行下列動作： [!DNL SharePoint]、和寫入許可權可讓使用者上傳檔案到 [!DNL SharePoint].

![Sharepoint許可權](assets/sharepoint-permissions.png)

有關透過新檔案連結檔案的指示 [!DNL SharePoint] 整合，請參閱 [連結外部檔案至 [!DNL Workfront]](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#link-an-external-document-to-workfront)

>[!NOTE]
>
>* A [!DNL SharePoint] 整合可連線至單一 [!DNL SharePoint] 執行個體。 因此，使用者可以為其中一個設定整合 [!DNL SharePoint]，但無法將整合設定到秒 [!DNL SharePoint]，即使他們擁有和檔案的許可權(在 [!DNL SharePoint].
>
>* 使用者可以透過存取相同的網站、集合、資料夾、子資料夾和檔案。 [!DNL Workfront] [!DNL SharePoint] 整合，如同他們在 [!DNL SharePoint] 帳戶。

### 從SharePoint連結檔案

如需透過新檔案從SharePoint連結檔案的指示 [!DNL SharePoint] 整合，請參閱 [連結外部檔案至 [!DNL Workfront]](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#link-an-external-document-to-workfront).

### 傳送檔案至SharePoint

若要傳送檔案至SharePoint：

1. 按一下 **傳送至** 圖示 ![傳送至](assets/send-to-icon.png) 並選取SharePoint (Graph API)。
1. （選擇性）在搜尋列中搜尋您要傳送檔案的網站或資料夾。
1. 從清單中選取網站或資料夾。

   * 網站標示為 ![網站圖示](assets/site-icon.png).

   * 資料夾標有 ![資料夾圖示](assets/folder-icon.png).

   * 檔案未標示圖示。

1. 按一下「**儲存**」。


## 的安全性、存取和授權資訊 [!DNL SharePoint] 整合

### 驗證和授權

[!DNL Workfront] 使用OAuth2來擷取存取權杖和重新整理權杖。 此存取權杖用於向所有 [!DNL SharePoint] 區域。

### 存取權和許可權

使用者第一次將檔案新增至時 [!DNL Workfront] 從 [!DNL SharePoint]，系統會將使用者導向至要求下列許可權的畫面：

| 存取 | 原因 |
|---|---|
| 擁有檔案的完整存取權 | 允許 [!DNL Workfront] 以存取使用者檔案來連結資產。 當檔案從以下來源傳送時 [!DNL Workfront] 至 [!DNL SharePoint]， [!DNL Workfront] 需要存取權才能建立資產。 |
| 讀取所有網站集合中的專案 | 允許 [!DNL Workfront] 以讀取資產並啟用使用者導覽。 |
| 編輯或刪除所有網站集合中的專案 | 允許 [!DNL Workfront] 在網站和網站集合中建立資產。 刪除只會在不成功的連結嘗試後清除時使用。 |
| 維護您授予其資料存取權的資料存取權 | 允許 [!DNL Workfront] 產生重新整理權杖。 |
| 登入並讀取使用者設定檔 | 允許 [!DNL Workfront] 以透過OAuth2登入流程使用存取權杖來代表使用者行事。 |

* 使用者第一次使用整合時就會授予此存取權，且可隨時撤銷。
* 要求對此整合的許可權為 **已委派** 許可權。
* [!DNL Workfront] 要求執行整合中作業所需的最低存取權。
* 存取「 」以檢視、編輯或刪除 [!DNL Adobe Workfront] 連結到的檔案 [!DNL SharePoint] 根據使用者在中的存取權 [!DNL Workfront]. 但是，任何導覽、下載或編輯 [!DNL SharePoint] 檔案或資料夾需要存取 [!DNL SharePoint]，這些動作的存取權則由 [!DNL SharePoint].
* 使用者可以檢視縮圖及預覽來源為的影像 [!DNL SharePoint]，並可以在以下位置檢視檔案和資料夾名稱： [!DNL SharePoint]，無需登入 [!DNL SharePoint].
* 只有當使用者離線且另一個使用者檢視連結至的資料夾內容時，才會使用使用者的存取權杖 [!DNL Workfront]. 存取權杖用於探索資料夾中是否有任何檔案已新增、移除或編輯。

### 安全性

所有通訊，介於 [!DNL Workfront] 和 [!DNL SharePoint] 會透過HTTPS執行，這會加密資訊。

[!DNL Workfront] 不會儲存、複製或複製下列來源的資料： [!DNL SharePoint]. 唯一的例外是 [!DNL Workfront] 儲存縮圖，從 [!DNL SharePoint] 以顯示在清單檢視和預覽中。

如果資產首次上傳至 [!DNL Workfront]，然後傳送至 [!DNL SharePoint]， [!DNL Workfront] 會保留第一個檔案的資料，因為使用者可以下載舊版的 [!DNL Workfront] 檔案。 若檔案是在中建立 [!DNL SharePoint]， [!DNL Workfront] 不會儲存該檔案資料。

## 設定舊版 [!DNL SharePoint] 整合以繼續存取檔案

為確保您的使用者能繼續存取透過舊版連結至Workfront的檔案 [!DNL SharePoint] 整合，您必須重新設定舊版的存取權 [!DNL SharePoint] 整合併保持SharePoint使用者端密碼為最新狀態。

* [重新設定舊版的存取權 [!DNL SharePoint] 整合](#reconfigure-access-to-the-legacy-sharepoint-integration)
* [設定使用者端密碼以繼續存取舊版 [!DNL SharePoint] 整合](#configure-the-client-secret-for-continued-access-to-the-legacy-sharepoint-integration)

### 重新設定舊版的存取權 [!DNL SharePoint] 整合

重新設定舊版 [!DNL SharePoint] 整合可讓您的使用者存取透過舊版連結的檔案 [!DNL SharePoint] 整合，同時確保您的使用者無法透過該整合連結新檔案。

>[!NOTE]
>
> * 舊版 [!DNL SharePoint] 整合已標籤為&quot;[!DNL SharePoint].」
> * 新的 [!DNL SharePoint] 整合已標籤為&quot;[!UICONTROL [!DNL SharePoint] (Graph API)].」

1. 按一下 **[!UICONTROL 主要功能表]** 圖示 ![主要功能表](assets/main-menu-icon.png) 在Adobe Workfront的右上角，或（如果有的話）按一下 **[!UICONTROL 主要功能表]** 圖示 ![主要功能表](/help/_includes/assets/main-menu-icon-left-nav.png) 然後按一下「 」 **[!UICONTROL 設定]** ![「設定」圖示](/help/_includes/assets/gear-icon-setup.png).
1. 選取 **[!UICONTROL 檔案]** 在左側導覽中，然後選取 **[!UICONTROL 雲端服務供應商]**.
1. 確定 **[!DNL SharePoint]** 選項和 **[!UICONTROL [!DNL SharePoint](Graph API)]** 選項皆已啟用。
1. 按一下「**[!UICONTROL 儲存]**」。
1. 選取 **[!UICONTROL 檔案]** 在左側導覽中，然後選取 **[!UICONTROL [!DNL SharePoint]整合]**.
1. 選取清單左側的核取記號，取得所有現有整合，然後選取「 」 **[!UICONTROL 停用]**.
   ![](assets/disable-old-sharepoint.png)


### 設定使用者端密碼以繼續存取舊版 [!DNL SharePoint] 整合

您的 [!DNL SharePoint] 使用者端密碼每年會過期一次。 為確保持續存取舊版中的檔案 [!DNL SharePoint] 整合，您必須保留其 [!DNL SharePoint] 最新使用者端密碼。

>[!IMPORTANT]
>
> 因為 [!DNL SharePoint] 使用者端密碼的處理者為 [!DNL Microsoft]，使用者端密碼功能和程式可能會因以下專案的更新而變更： [!DNL SharePoint] 製作者 [!DNL Microsoft]. 請務必檢查 [!DNL Microsoft] 檔案以取得中程式和功能的最新資訊 [!DNL SharePoint].

<!--1. Go to the site that your [!DNL SharePoint] integration uses. This may be a site that you created when setting up the integrations, or it may be your organization's root site.

1. Add `/_layouts/15/appregnew.aspx` to the end of the URL in the search bar at the top of your browser window.-->

1. 產生新的使用者端密碼，如所述 [在中取代即將到期的使用者端密碼 [!DNL SharePoint] 增益集](https://docs.microsoft.com/en-us/sharepoint/dev/sp-add-ins/replace-an-expiring-client-secret-in-a-sharepoint-add-in#generate-a-new-secret).
1. 將此使用者端密碼複製到安全位置。
1. 登入 [!DNL Workfront] 作為管理員。
1. 在Workfront中，按一下 **[!UICONTROL 主要功能表]** 圖示 ![主要功能表](assets/main-menu-icon.png) 在Adobe Workfront的右上角，或（如果有的話）按一下 **[!UICONTROL 主要功能表]** 圖示 ![主要功能表](/help/_includes/assets/main-menu-icon-left-nav.png) 然後按一下「 」 **[!UICONTROL 設定]** ![「設定」圖示](/help/_includes/assets/gear-icon-setup.png).
1. 在左側面板中，按一下 **[!UICONTROL 檔案]** > **[!UICONTROL [!DNL SharePoint]整合]**.
1. 按一下 [!DNL SharePoint] 要更新的整合，然後按一下 **[!UICONTROL 編輯]**.
1. 找到 **連線資訊** 編輯視窗的區段，然後將新的使用者端密碼輸入到 **[!UICONTROL SharePoint使用者端密碼]** 欄位。
1. 按一下「**[!UICONTROL 儲存]**」。

<!--

## Instructions for setting up the legacy SharePoint integration

>[!IMPORTANT]
>
>This integration has been deprecated. The instructions here are for information only and will be removed in the near future.


Workfront connects to [!DNL SharePoint] Online using OAuth 2.0, a standard used by most web-based integrations for the authentication and authorization of users.

To configure OAuth, you need to create a [!DNL SharePoint] site and a Site App within [!DNL SharePoint]. This process is described in the following sections.

For more information about OAuth, see [http://oauth.net](http://oauth.net/).

>[!TIP]
>
>To make it easy to copy and paste information between [!DNL Workfront] and [!DNL SharePoint] in these steps, we recommend keeping both applications open in separate tabs.

* [Create and configure a [!DNL SharePoint] site](#create-and-configure-a-sharepoint-site) 
* [Grant write permissions to the site app](#grant-write-permissions-to-the-site-app) 
* [Create a [!DNL Workfront] [!DNL SharePoint] integration instance](#create-a-workfront-sharepoint-integration-instance) 
* [Complete your integration](#complete-your-integration) 
* [Add documents](#add-documents)

### Create and configure a [!DNL SharePoint] site  {#create-and-configure-a-sharepoint-site}

In order for [!DNL Workfront] to authenticate with [!DNL SharePoint], [!DNL Workfront] ca use a master site where users have the [!UICONTROL Full Control] permission level or specific Manage permissions. This master site acts as an Authentication Entry Point for [!DNL Workfront].

To create and configure a [!DNL SharePoint] Site:

1. (Optional) If you do not want to use your organization's root site, you can create a master site in [!DNL SharePoint].

   For instructions, visit [Create a site](https://docs.microsoft.com/en-us/sharepoint/create-site-collection) in the [!DNL Microsoft] Documentation.

   * Select the **[!UICONTROL Team Site]** option when creating the site.

1. (Conditional) If you created a site in step 1, go to the site you just created.

   Or

   If you did not create a site in step 1, go to your organization's root site.

1. Add `/_layouts/15/appregnew.aspx` to the end of the URL in the search bar at the top of your browser window.
1. Configure the following fields:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Client ID]</p> </td> 
      <td> <p>Click <strong>[!UICONTROL Generate]</strong> to generate a Client ID. Copy this ID to a secure location. You will use it later when you set up the [!DNL SharePoint] integration in [!DNL Workfront].</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Client Secret]</p> </td> 
      <td> <p>Click <strong>[!UICONTROL Generate]</strong> to generate a Client Secret. Copy this Secret to a secure location. You will use it later when you set up the [!DNL SharePoint] integration in [!DNL Workfront].</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Title</p> </td> 
      <td> <p>Enter a title, such as [!DNL Workfront] Site App. Users see this title when adding documents..</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL App Domain]</p> </td> 
      <td> <p><code>my.workfront.com</code> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Redirect URI]</p> </td> 
      <td> <p><code>https://oauth.my.workfront.com/oauth2/redirect</code> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Click **[!UICONTROL Create]**
1. Continue to [Grant write permissions to the site app](#grant-write-permissions-to-the-site-app).

### Grant write permissions to the site app  {#grant-write-permissions-to-the-site-app}

At this point, you have successfully created a Site App and registered it within [!DNL Workfront]. This site app is also known as an app principal in [!DNL SharePoint]. It resides within your tenant. New site apps do not automatically have access to site collections within the tenant. Permissions must be granted explicitly, for each site collection. The steps below will show you how to grant Write permission to the new Site App a site collection. Repeat these steps for each of the site collections you added under [!UICONTROL Visible Site Collections] in the steps above.

This site app must have [!UICONTROL Write] permission to any site collections that users need to access through [!DNL Workfront].

1. Add '/_layouts/15/appinv.aspx' to the URL in [!DNL Sharepoint].

   **Example:**

   ```
   https://mycompany.sharepoint.com/sites/mysite/_layouts/15/appinv.aspx
   ```

1. Configure the following fields

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL App ID]</td> 
      <td> <p>Add the Client ID that you created in <a href="#create-and-configure-a-sharepoint-site" class="MCXref xref">Create and configure a [!DNL SharePoint] site </a>and click <strong>[!UICONTROL Lookup]</strong>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Client] / [!UICONTROL App Domain] / [!UICONTROL Redirect URL]</p> </td> 
      <td> <p>These automatically fill when you click [!UICONTROL Lookup].</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Permission Request XML]</td> 
      <td> <p>Copy the following XML to the [!UICONTROL Permission Request XML] field. Make sure that it is added exactly as shown without additional spaces etc. in order to avoid errors.</p> 
      <div></a> 
      <div style="mc-code-lang: XML;" class="codeSnippetBody" data-mc-continue="False" data-mc-line-number-start="1" data-mc-use-line-numbers="False"> 
       <pre><code><span style="color: #63a35c; ">&lt;AppPermissionRequests&gt;</span><br><span style="color: #63a35c; ">&lt;AppPermissionRequest <span style="color: #795da3; ">Scope</span><span style="color: #df5000; ">="http://sharepoint/content/sitecollection/web"</span> <span style="color: #795da3; ">Right</span><span style="color: #df5000; ">="Write"</span>/&gt;</span><br><span style="color: #63a35c; ">&lt;/AppPermissionRequests&gt;</span></code></pre> 
      </div> 
      </div> </td> 
     </tr> 
    </tbody> 
   </table>

1. Click **[!UICONTROL Create]**. 
1. In the dialog that appears, click **[!UICONTROL Trust it]**.
1. Verify that the site app has access to the site collection by clicking the **[!UICONTROL Site collection app permissions]** link in [!UICONTROL Site Settings].
1. Repeat the steps above for the remaining site collections, then continue with [Create a [!DNL Workfront] [!DNL SharePoint] integration instance](#create-a-workfront-sharepoint-integration-instance).

### Create a [!DNL Workfront] [!DNL SharePoint] integration instance {#create-a-workfront-sharepoint-integration-instance}

When you have created a site app in [!DNL SharePoint], you can now copy information from the site app into [!DNL Workfront]. The site app is an app principal and acts as the conduit through which OAuth requests are made to access documents within site collections.

1. Log into [!DNL Workfront] as an administrator.
1. Click the **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **[!UICONTROL Setup]** ![](assets/gear-icon-settings.png).

1. In the left panel, click **[!UICONTROL Documents]** > **[!UICONTROL [!DNL SharePoint] Integration]**.
1. Click **[!UICONTROL Add [!DNL SharePoint]]**.
1. Configure the following fields:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Name]</p> </td> 
      <td> <p>Enter a name for the [!DNL SharePoint] integration. Users see this name when they click [!UICONTROL Add] &gt; [!UICONTROL From] 'name of integration'. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL [!DNL SharePoint] Host Instance]</p> </td> 
      <td> <p><code>&lt;YourDomain&gt;.sharepoint.com</code> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL [!DNL Azure] Access Domain]</p> </td> 
      <td> <p><code>&lt;YourDomain&gt;.onmicrosoft.com</code> </p> <p>This refers to the Master Site that users will use to authenticate through. It is likely the same domain as the [!UICONTROL [!DNL SharePoint] Host Instance].</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>
      </p> </td> 
      <td> <b>Important</b> Site collections are used only in the Legacy [!DNL SharePoint] Integration.
       <ul> 
        <li> <p><b>If you are using your organization's root site</b><b>:</b> </p> <p>Enter <code>/</code></p> </li> 
        <li> <p><b>If you are using a master site and subsites:</b> </p> <p><b>IMPORTANT</b>: [!DNL Microsoft SharePoint] no longer recommends the use of subsites.</p> <p>Enter the URL stem for the site collection that you created in the section above.</p> <p>This is the section of the URL after .com.</p> <p>Example: for the URL <code>https://mycompany.sharepoint.com/sites/mysite</code>, the stem would be <code>/sites/mysite</code>.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL SharePoint] Client ID]</td> 
      <td>Enter the Client ID that you generated in <a href="#create-and-configure-a-sharepoint-site" class="MCXref xref">Create and configure a [!DNL SharePoint] site </a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL SharePoint] Client Secret]</td> 
      <td>Enter the Client Secret that you generated in <a href="#create-and-configure-a-sharepoint-site" class="MCXref xref">Create and configure a [!DNL SharePoint] site </a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Visible Site Collections]</td> 
      <td> <b>Important</b> Site collections are used only in the Legacy [!DNL SharePoint] integration.
       <ul> 
        <li> <p><b> If you are using your organization's root site</b><b>:</b> </p> <p>Enter <code>/</code></p> </li> 
        <li> <p><b>If you are using a master site and subsites:</b> </p> <p><b>IMPORTANT</b>: [!DNL Microsoft SharePoint] no longer recommends the use of subsites.</p> <p>For each subsite you want to add to your [!DNL SharePoint] integration, enter the stem of the subsite.</p> <p>Example: for the URL<code>https://mycompany.sharepoint.com/sites/mysite/mysubsite</code>, the stem would be <code>/sites/mysite/mysubsite</code>.</p> <p><b>NOTE</b>:   <p>If you want to test your configuration only (no subsites), enter the stem of the master site. </p> <p>Example: for the URL <code> https://mycompany.sharepoint.com/sites/mysite</code>, the stem would be <code>/sites/mysite</code>.</p> <p>When you have tested your configuration as described in <a href="#complete-your-integration" class="MCXref xref">Complete your integration</a>, you must remove the master site and enter the subsites.</p> 
          <ol> 
           <li value="1">Click the <strong>[!UICONTROL Main Menu]</strong> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of [!DNL Adobe Workfront], then click <strong>[!UICONTROL Setup]</strong> <img src="assets/gear-icon-settings.png">.<li><p>In the left panel, click <strong>[!UICONTROL Documents]</strong> &gt; <strong>[!UICONTROL [!DNL SharePoint] Integration]</strong>.</p></li><li><p>Click the [!DNL SharePoint] integration you are setting up, then click Edit.</p></li><li><p>Delete the stem for the master site from the [!UICONTROL Visible Site Collections] field.</p></li><li><p>For each subsite you want to add to your [!DNL SharePoint] integration, enter the stem of the subsite.</p></li><p>Example: for the URL<code>https://mycompany.sharepoint.com/sites/mysite/mysubsite</code>, the stem would be <code>/sites/mysite/mysubsite</code>.</p></li> 
          </ol> </p> </li> 
       </ul> <p> </p> <p> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Click **[!UICONTROL Save]**
1. Continue to [Complete your integration](#complete-your-integration).

### Complete your integration {#complete-your-integration}

The basic configuration is almost complete.

1. In Workfront, Click the **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **[!UICONTROL Documents]** ![](assets/document-icon.png).
1. Click **[!UICONTROL Add new]**.
1. Click **[!UICONTROL From] `<title of your [!DNL SharePoint] site>`** in the dropdown.

   A dialog that invites you to Trust this site appears.

   >[!NOTE]
   >
   >If this dialog does not appear, your [!DNL SharePoint] integration is not configured correctly.

1. Click **[!UICONTROL Trust it]**.

### Add documents {#add-documents}

You can now add documents from your [!DNL SharePoint] site.

For instructions, see [Link an external document to [!DNL Workfront]](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#linking-existing-documents) in [Link documents from external applications](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md)

>[!IMPORTANT]
>
>If the user who linked a folder no longer has access to the external application, [!DNL Workfront] can no longer access the contents of the folder. This may happen, for example, if the user who originally linked the folder leaves the company. To ensure continued access, a user with access to the folder must re-link the folder.
> 

-->

## 疑難排解

* [問題：使用者在使用時遇到驗證型錯誤 [!DNL SharePoint] 整合。](#problem-users-experience-authentication-based-errors-when-using-the-sharepoint-integration)
* [問題：嘗試瀏覽時 [!DNL SharePoint] 中的檔案 [!DNL Workfront]，我沒有看見任何或全部的網站集合。](#problem-when-attempting-to-browse-sharepoint-files-in-workfront-i-do-not-see-any-or-all-of-my-site-collections)
* [問題：我無法存取中先前連結的資料夾和檔案 [!DNL SharePoint].](#problem-i-cannot-access-previously-linked-folders-and-documents-in-sharepoint)

### 問題：使用者在使用時遇到驗證型錯誤 [!DNL SharePoint] 整合。 {#problem-users-experience-authentication-based-errors-when-using-the-sharepoint-integration}

解決方案：

使用者必須擁有適當的許可權， [!DNL SharePoint] 網站。

使用者 [!UICONTROL 完全控制] 存取擁有您的所有必要許可權 [!DNL SharePoint] 整合。 如果您不想要授與使用者的完全控制存取權，您必須授與下列許可權：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL設計]</p> </td> 
   <td> <p>可以檢視、新增、更新、刪除、核准和自訂</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL編輯]</p> </td> 
   <td> <p>可以新增、編輯和刪除清單；可以檢視、新增、更新和刪除清單專案和檔案</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Contribute]</p> </td> 
   <td> <p>可以檢視、新增、更新及刪除清單專案和檔案</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL檢視]</p> </td> 
   <td> <p>可以檢視頁面、清單專案和檔案（具有伺服器端檔案處理常式的檔案型別可以在瀏覽器中檢視，但不能下載）</p> </td> 
  </tr> 
 </tbody> 
</table>

如需建立和編輯許可權層級的指示，請參閱 [如何建立及編輯許可權層級](https://docs.microsoft.com/en-us/sharepoint/how-to-create-and-edit-permission-levels) (位於Microsoft檔案中)。

<!--

### Problem: As a [!DNL Workfront] user, I am unable to provision a new [!DNL SharePoint] instance. When I attempt to do I see an error. {#problem-as-a-workfront-user-i-am-unable-to-provision-a-new-sharepoint-instance-when-i-attempt-to-do-i-see-an-error}

Solutions:

This can be caused by a number of things, originating in either [!DNL Workfront] or [!DNL SharePoint]'s configuration. Verify that:

* The Client ID, Client Secret, return URL and other configuration fields are correctly mapped between the [!DNL Workfront] [!DNL SharePoint] Integration instance and the [!DNL SharePoint] Site App.
* The user has [!UICONTROL Full Control] permission to the Site Collection used for authentication.
* The Site App is listed under [!UICONTROL Site App Permissions] for the [!UICONTROL Site Collection] used for authentication.

-->

### 問題：嘗試瀏覽時 [!DNL SharePoint] 中的檔案 [!DNL Workfront]，我沒有看見任何或全部的網站集合。 {#problem-when-attempting-to-browse-sharepoint-files-in-workfront-i-do-not-see-any-or-all-of-my-site-collections}

解決方案：

若要在中檢視網站集合 [!DNL Workfront]，下列條件必須符合：

<!--

* The site collection must be registered in the [!DNL Workfront] [!DNL SharePoint] Integration instance.

  To verify this in [!DNL Workfront]:

   1. Go to [!UICONTROL Setup] > [!UICONTROL Documents] > [!UICONTROL [!DNL SharePoint] Integration].
   1. Edit the [!DNL SharePoint] Integration instance information.
   1. Verify that the site collection is listed under [!UICONTROL Visible Site Collections].
   -->

* 使用者必須擁有中網站集合的檢視存取權 [!DNL SharePoint].

  若要在中驗證此專案，請執行下列動作： [!DNL SharePoint]，請檢查SharePoint中的網站集合許可權。

<!--* The [!DNL SharePoint] Site App must have access to the site collection.

  To verify this in [!DNL SharePoint]:

   1. Go to the site collection > [!UICONTROL Settings] > [!UICONTROL Site app permissions].
   1. Ensure that the [!UICONTROL Site App] used by [!DNL Workfront] is listed here.
   1. (Conditional) If the Site App is not listed, add to the site collection using _layouts/15/appinv.aspx.

      For information about adding the site collection, see Granting Write Permissions To The Site App.
      
-->

### 問題：我無法存取中先前連結的資料夾和檔案 [!DNL SharePoint]. {#problem-i-cannot-access-previously-linked-folders-and-documents-in-sharepoint}

解決方案：

如果連結的使用者 [!DNL SharePoint] 資料夾無法再驗證， [!DNL Workfront] 無法再存取資料夾的內容。 例如，如果最初連結資料夾的使用者離開公司，就可能發生這種情況。

為確保繼續存取，有權存取資料夾的使用者必須重新連結資料夾。

如需從外部提供者連結資料夾的資訊，請參閱 [從外部應用程式連結檔案](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

<!--

### Problem: I see a "404 not found" error when attempting to add a document from [!DNL Sharepoint]

#### Solution:

This error might occur if one of the sites configured in the [!UICONTROL Visible Site Collections] list has been deleted in Sharepoint. Check the [!UICONTROL Visible Site Collections] list, and remove any sites that have been deleted in Sharepoint.-->