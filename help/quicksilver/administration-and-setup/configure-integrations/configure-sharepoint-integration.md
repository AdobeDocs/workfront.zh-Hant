---
title: 設定 [!DNL SharePoint] 整合
user-type: administrator
product-area: system-administration;workfront-integrations;setup
navigation-topic: administrator-integrations
description: 您可以將 [!DNL Workfront] 與 [!DNL SharePoint] 線上整合，讓使用者能夠在Workfront中導覽、連結及新增 [!DNL SharePoint] 檔案。 提供的功能與其他 [!DNL Workfront] 檔案整合的功能類似。
author: Becky
feature: System Setup and Administration, [!DNL Workfront] Integrations and Apps, Digital Content and Documents
role: Admin
exl-id: fd45e1bc-9a35-4960-a73a-ff845216afe4
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '1729'
ht-degree: 0%

---

# 設定[!DNL SharePoint]整合

<!--Audited: 12/2023-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

>[!IMPORTANT]
>
>新的[!DNL SharePoint]整合已在22.3版（2022年7月）中發佈至生產環境。
>
>* 雖然您的使用者仍然可以存取透過舊版[!DNL SharePoint]整合連結的檔案，但他們無法透過該整合連結檔案。 他們必須使用新的[!DNL SharePoint]整合以從SharePoint連結檔案。
>
>* 如果您尚未設定舊版SharePoint整合，則無法新增。 您必須使用新的SharePoint整合，將檔案連結至SharePoint。
>
>* 新的SharePoint整合可能不需要管理員進行設定，也可能由個別使用者進行設定。 不過，為確保順利轉換至新的SharePoint整合，Workfront管理員必須在Workfront設定區域中變更幾項設定。
>
>    如需相關資訊與指示，請參閱[設定舊版SharePoint整合以繼續存取本文中的檔案](#configure-the-legacy-sharepoint-integration-for-continued-access-to-documents)。
>    
>* 我們建議使用者連結目前透過舊版[!DNL SharePoint]整合透過新整合連結的檔案。
>    
>    如需連結檔案的指示，請參閱[從外部應用程式連結檔案](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md)。

您可以整合[!DNL Workfront]與[!DNL SharePoint Online]，讓使用者能夠在Workfront中導覽、連結及新增[!DNL SharePoint]份檔案。 提供的功能與其他[!DNL Workfront]整合（例如[!DNL Google Drive]、[!DNL Box]及[!DNL Dropbox]）的功能類似。

此整合僅與[!DNL SharePoint Online]相容。 不支援[!DNL SharePoint]的內部部署執行個體。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

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
   <td>您必須是[!DNL Workfront]管理員。 </td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 先決條件

您必須在[!DNL SharePoint]中擁有任何必要的存取權或許可權，才能修改或設定您的[!DNL SharePoint]整合。

## 透過新的SharePoint整合連結檔案

個別使用者可透過新的[!DNL SharePoint]整合連結檔案。 整合不需要管理員設定。 而是在連結檔案時，使用者登入其[!DNL Microsoft]帳戶，如此整合即可存取使用者[!DNL SharePoint]中可用的檔案。

使用者第一次將[!DNL Workfront] [!DNL SharePoint]整合連線至其[!DNL SharePoint]帳戶時，他們會看到並同意[!DNL Workfront]在與其[!UICONTROL SharePoint]帳戶互動時所使用的所有許可權，或能夠向其Microsoft管理員要求許可權。 讀取許可權允許[!DNL Workfront]檢視及存取[!DNL SharePoint]上的檔案，而寫入許可權允許使用者上傳檔案至[!DNL SharePoint]。

![Sharepoint許可權](assets/sharepoint-permissions.png)

如需透過新的[!DNL SharePoint]整合連結檔案的指示，請參閱[將外部檔案連結至 [!DNL Workfront]](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#link-an-external-document-to-workfront)

>[!NOTE]
>
>* 根據組織的Microsoft設定，使用者可能會看到「需要核准」頁面，而不是「要求的許可權」頁面。 在此情況下，使用者可以使用此頁面來要求組織的Microsoft管理員授與Sharepoint整合的許可權。
>
>* [!DNL SharePoint]整合可以連線至單一[!DNL SharePoint]執行個體。 因此，使用者可以設定一個[!DNL SharePoint]的整合，但無法設定第二個[!DNL SharePoint]的整合，即使他們擁有許可權存取和檔案在第二個[!DNL SharePoint]上。
>
>* 使用者透過[!DNL Workfront] [!DNL SharePoint]整合存取的網站、集合、資料夾、子資料夾和檔案與其[!DNL SharePoint]帳戶中的相同。

### 從SharePoint連結檔案

如需透過新的[!DNL SharePoint]整合從SharePoint連結檔案的指示，請參閱[將外部檔案連結至 [!DNL Workfront]](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#link-an-external-document-to-workfront)。

### 傳送檔案至SharePoint

若要傳送檔案至SharePoint：

1. 按一下&#x200B;**傳送至**&#x200B;圖示![傳送至](assets/send-to-icon.png)並選取SharePoint (Graph API)。
1. （選擇性）在搜尋列中搜尋您要傳送檔案的網站或資料夾。
1. 從清單中選取網站或資料夾。

   * 網站標示有![網站圖示](assets/site-icon.png)。

   * 資料夾標示為![資料夾圖示](assets/folder-icon.png)。

   * 檔案未標示圖示。

1. 按一下「**儲存**」。


## [!DNL SharePoint]整合的安全性、存取和授權資訊

### 驗證和授權

[!DNL Workfront]使用OAuth2來擷取存取權杖和重新整理權杖。 此存取權杖用於所有[!DNL SharePoint]區域的授權。

### 存取權和許可權

使用者第一次從[!DNL SharePoint]新增檔案至[!DNL Workfront]時，系統會將他們導向至許可權要求的頁面，他們可以在其中授與許可權給其SharePoint整合。

>[!NOTE]
>
>根據組織的Microsoft設定，使用者可能會看到「需要核准」頁面，而不是「要求的許可權」頁面。 在此情況下，使用者可以使用此頁面來要求組織的Microsoft管理員授與Sharepoint整合的許可權。

需要下列許可權：

| 存取 | 原因 |
|---|---|
| 擁有檔案的完整存取權 | 允許[!DNL Workfront]存取使用者的檔案以連結資產。 當檔案從[!DNL Workfront]傳送到[!DNL SharePoint]時，[!DNL Workfront]需要存取權才能建立資產。 |
| 讀取所有網站集合中的專案 | 允許[!DNL Workfront]讀取資產以啟用使用者導覽。 |
| 編輯或刪除所有網站集合中的專案 | 允許[!DNL Workfront]在網站和網站集合中建立資產。 刪除只會在不成功的連結嘗試後清除時使用。 |
| 維護您授予其資料存取權的資料存取權 | 允許[!DNL Workfront]產生重新整理權杖。 |
| 登入並讀取使用者設定檔 | 允許[!DNL Workfront]透過OAuth2登入流程使用存取權杖來代表使用者執行。 |

* 使用者第一次使用整合時就會授予此存取權，且可隨時撤銷。
* 此整合要求的許可權為&#x200B;**委派**&#x200B;許可權。
* [!DNL Workfront]要求執行整合中作業所需的最低存取許可權。
* 檢視、編輯或刪除連結至[!DNL SharePoint]的[!DNL Adobe Workfront]檔案的存取權是根據使用者在[!DNL Workfront]中的存取權。 但是，任何導覽、下載或編輯[!DNL SharePoint]檔案或資料夾都需要存取[!DNL SharePoint]，而且這些動作的存取權是由[!DNL SharePoint]所控制。
* 使用者可以檢視來源為[!DNL SharePoint]的縮圖及預覽影像，而且可以在[!DNL SharePoint]中檢視檔案和資料夾名稱，而不需要登入[!DNL SharePoint]。
* 只有當使用者離線且另一個使用者檢視連結至[!DNL Workfront]的資料夾內容時，才會使用使用者的存取權杖。 存取權杖用於探索資料夾中是否有任何檔案已新增、移除或編輯。

### 安全性

[!DNL Workfront]與[!DNL SharePoint]之間的所有通訊都是透過HTTPS進行，這會加密資訊。

[!DNL Workfront]未儲存、複製或複製[!DNL SharePoint]中的資料。 唯一的例外是[!DNL Workfront]儲存來自[!DNL SharePoint]的縮圖，以顯示在清單檢視和預覽中。

如果資產先上傳至[!DNL Workfront]，再傳送至[!DNL SharePoint]，[!DNL Workfront]會保留第一個檔案的資料，因為使用者可以下載舊版的[!DNL Workfront]檔案。 如果檔案是在[!DNL SharePoint]中建立，[!DNL Workfront]不會儲存該檔案資料。

## 設定舊版[!DNL SharePoint]整合以繼續存取檔案

若要確保您的使用者可透過舊版[!DNL SharePoint]整合繼續存取連結至Workfront的檔案，您必須重新設定舊版[!DNL SharePoint]整合的存取權，並維持SharePoint使用者端密碼為最新狀態。

* [重新設定舊版 [!DNL SharePoint] 整合的存取權](#reconfigure-access-to-the-legacy-sharepoint-integration)
* [設定使用者端密碼以繼續存取舊版 [!DNL SharePoint] 整合](#configure-the-client-secret-for-continued-access-to-the-legacy-sharepoint-integration)

### 重新設定舊版[!DNL SharePoint]整合的存取權

重新設定舊版[!DNL SharePoint]整合可讓您的使用者存取透過舊版[!DNL SharePoint]整合連結的檔案，同時確保您的使用者無法透過該整合連結新檔案。

>[!NOTE]
>
> * 舊版[!DNL SharePoint]整合已標籤為「[!DNL SharePoint]」。
> * 新的[!DNL SharePoint]整合已標籤為「[!UICONTROL [!DNL SharePoint] (Graph API)]」。

1. 按一下Adobe Workfront右上角的&#x200B;**[!UICONTROL 主功能表]**&#x200B;圖示![主功能表](assets/main-menu-icon.png)，或（如果有的話）按一下左上角的&#x200B;**[!UICONTROL 主功能表]**&#x200B;圖示![主功能表](/help/_includes/assets/main-menu-icon-left-nav.png)，然後按一下&#x200B;**[!UICONTROL 設定]** ![設定圖示](/help/_includes/assets/gear-icon-setup.png)。
1. 在左側導覽中選取&#x200B;**[!UICONTROL 檔案]**，然後選取&#x200B;**[!UICONTROL 雲端提供者]**。
1. 請確定&#x200B;**[!DNL SharePoint]**&#x200B;選項和&#x200B;**[!UICONTROL [!DNL SharePoint] (Graph API)]**&#x200B;選項皆已啟用。
1. 按一下「**[!UICONTROL 儲存]**」。
1. 在左側導覽中選取&#x200B;**[!UICONTROL 檔案]**，然後選取&#x200B;**[!UICONTROL [!DNL SharePoint]整合]**。
1. 選取清單左側的核取記號，以取得所有現有的整合，然後選取&#x200B;**[!UICONTROL 停用]**。



### 設定使用者端密碼以繼續存取舊版[!DNL SharePoint]整合

您的[!DNL SharePoint]使用者端密碼每年會過期一次。 若要確保持續存取您舊版[!DNL SharePoint]整合中的檔案，您必須將其[!DNL SharePoint]使用者端密碼保持在最新狀態。

>[!IMPORTANT]
>
> 因為[!DNL SharePoint]使用者端密碼是由[!DNL Microsoft]處理，所以使用者端密碼功能和程式可能會根據[!DNL Microsoft]對[!DNL SharePoint]所做的更新而變更。 請一律檢視[!DNL Microsoft]檔案，以瞭解[!DNL SharePoint]中程式和功能的最新資訊。

<!--1. Go to the site that your [!DNL SharePoint] integration uses. This may be a site that you created when setting up the integrations, or it may be your organization's root site.

1. Add `/_layouts/15/appregnew.aspx` to the end of the URL in the search bar at the top of your browser window.-->

1. 產生新的使用者端密碼，如[取代 [!DNL SharePoint] 增益集](https://docs.microsoft.com/en-us/sharepoint/dev/sp-add-ins/replace-an-expiring-client-secret-in-a-sharepoint-add-in#generate-a-new-secret)中即將到期的使用者端密碼。
1. 將此使用者端密碼複製到安全位置。
1. 以系統管理員身分登入[!DNL Workfront]。
1. 在Workfront中，按一下Adobe Workfront右上角的&#x200B;**[!UICONTROL 主功能表]**&#x200B;圖示![主功能表](assets/main-menu-icon.png)，或（如果可用）按一下左上角的&#x200B;**[!UICONTROL 主功能表]**&#x200B;圖示![主功能表](/help/_includes/assets/main-menu-icon-left-nav.png)，然後按一下&#x200B;**[!UICONTROL 設定]** ![設定圖示](/help/_includes/assets/gear-icon-setup.png)。
1. 在左側面板中，按一下&#x200B;**[!UICONTROL 檔案]** > **[!UICONTROL [!DNL SharePoint]整合]**。
1. 按一下要更新的[!DNL SharePoint]整合，然後按一下&#x200B;**[!UICONTROL 編輯]**。
1. 找出編輯視窗的&#x200B;**連線資訊**&#x200B;區段，然後在&#x200B;**[!UICONTROL SharePoint使用者端密碼]**&#x200B;欄位中輸入新的使用者端密碼。
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
1. Click the **[!UICONTROL Main Menu]** icon ![Main menu icon](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **[!UICONTROL Setup]** ![Gear settings icon](assets/gear-icon-settings.png).

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

1. In Workfront, Click the **[!UICONTROL Main Menu]** icon ![Main menu icon](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **[!UICONTROL Documents]** ![Document icon](assets/document-icon.png).
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

* [問題：使用者在使用 [!DNL SharePoint] 整合時遇到驗證錯誤。](#problem-users-experience-authentication-based-errors-when-using-the-sharepoint-integration)
* [問題：嘗試瀏覽 [!DNL Workfront]中的 [!DNL SharePoint] 個檔案時，我看不到任何或所有網站集合。](#problem-when-attempting-to-browse-sharepoint-files-in-workfront-i-do-not-see-any-or-all-of-my-site-collections)
* [問題：我無法存取 [!DNL SharePoint]中先前連結的資料夾和檔案。](#problem-i-cannot-access-previously-linked-folders-and-documents-in-sharepoint)

### 問題：使用者在使用[!DNL SharePoint]整合時遇到驗證錯誤。 {#problem-users-experience-authentication-based-errors-when-using-the-sharepoint-integration}

解決方案：

使用者必須擁有[!DNL SharePoint]網站的適當許可權。

擁有[!UICONTROL 完全控制]存取許可權的使用者擁有您[!DNL SharePoint]整合的所有必要許可權。 如果您不想要授與使用者的完全控制存取權，您必須授與下列許可權：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 設計]</p> </td> 
   <td> <p>可以檢視、新增、更新、刪除、核准和自訂</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 編輯]</p> </td> 
   <td> <p>可以新增、編輯和刪除清單；可以檢視、新增、更新和刪除清單專案和檔案</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Contribute]</p> </td> 
   <td> <p>可以檢視、新增、更新及刪除清單專案和檔案</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 檢視]</p> </td> 
   <td> <p>可以檢視頁面、清單專案和檔案（具有伺服器端檔案處理常式的檔案型別可以在瀏覽器中檢視，但不能下載）</p> </td> 
  </tr> 
 </tbody> 
</table>

如需建立和編輯許可權層級的指示，請參閱Microsoft檔案中的[如何建立和編輯許可權層級](https://docs.microsoft.com/en-us/sharepoint/how-to-create-and-edit-permission-levels)。

<!--

### Problem: As a [!DNL Workfront] user, I am unable to provision a new [!DNL SharePoint] instance. When I attempt to do I see an error. {#problem-as-a-workfront-user-i-am-unable-to-provision-a-new-sharepoint-instance-when-i-attempt-to-do-i-see-an-error}

Solutions:

This can be caused by a number of things, originating in either [!DNL Workfront] or [!DNL SharePoint]'s configuration. Verify that:

* The Client ID, Client Secret, return URL and other configuration fields are correctly mapped between the [!DNL Workfront] [!DNL SharePoint] Integration instance and the [!DNL SharePoint] Site App.
* The user has [!UICONTROL Full Control] permission to the Site Collection used for authentication.
* The Site App is listed under [!UICONTROL Site App Permissions] for the [!UICONTROL Site Collection] used for authentication.

-->

### 問題：嘗試瀏覽[!DNL Workfront]中的[!DNL SharePoint]個檔案時，我看不到任何或所有網站集合。 {#problem-when-attempting-to-browse-sharepoint-files-in-workfront-i-do-not-see-any-or-all-of-my-site-collections}

解決方案：

若要在[!DNL Workfront]中檢視網站集合，必須符合下列條件：

<!--

* The site collection must be registered in the [!DNL Workfront] [!DNL SharePoint] Integration instance.

  To verify this in [!DNL Workfront]:

   1. Go to [!UICONTROL Setup] > [!UICONTROL Documents] > [!UICONTROL [!DNL SharePoint] Integration].
   1. Edit the [!DNL SharePoint] Integration instance information.
   1. Verify that the site collection is listed under [!UICONTROL Visible Site Collections].
   -->

* 使用者必須擁有[!DNL SharePoint]中網站集合的檢視存取權。

  若要在[!DNL SharePoint]中驗證，請在SharePoint中檢查網站集合的許可權。

<!--* The [!DNL SharePoint] Site App must have access to the site collection.

  To verify this in [!DNL SharePoint]:

   1. Go to the site collection > [!UICONTROL Settings] > [!UICONTROL Site app permissions].
   1. Ensure that the [!UICONTROL Site App] used by [!DNL Workfront] is listed here.
   1. (Conditional) If the Site App is not listed, add to the site collection using _layouts/15/appinv.aspx.

      For information about adding the site collection, see Granting Write Permissions To The Site App.
      
-->

### 問題：我無法存取[!DNL SharePoint]中先前連結的資料夾和檔案。 {#problem-i-cannot-access-previously-linked-folders-and-documents-in-sharepoint}

解決方案：

如果連結[!DNL SharePoint]資料夾的使用者無法再驗證，[!DNL Workfront]就無法再存取資料夾的內容。 例如，如果最初連結資料夾的使用者離開公司，就可能發生這種情況。

為確保繼續存取，有權存取資料夾的使用者必須重新連結資料夾。

如需從外部提供者連結資料夾的資訊，請參閱[從外部應用程式連結檔案](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md)。

<!--

### Problem: I see a "404 not found" error when attempting to add a document from [!DNL Sharepoint]

#### Solution:

This error might occur if one of the sites configured in the [!UICONTROL Visible Site Collections] list has been deleted in Sharepoint. Check the [!UICONTROL Visible Site Collections] list, and remove any sites that have been deleted in Sharepoint.-->
