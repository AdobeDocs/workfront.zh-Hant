---
title: 設定 [!DNL SharePoint] 整合
user-type: administrator
product-area: system-administration;workfront-integrations;setup
navigation-topic: administrator-integrations
description: 您可以整合 [!DNL Workfront] with [!DNL SharePoint] 線上，讓使用者能夠導覽、連結及新增 [!DNL SharePoint] 檔案。Workfront 提供的功能與其他功能類似 [!DNL Workfront] 整合，例如Google Drive、Box和Dropbox。
author: Becky, Caroline
feature: System Setup and Administration, [!DNL Workfront] Integrations and Apps, Digital Content and Documents
role: Admin
exl-id: fd45e1bc-9a35-4960-a73a-ff845216afe4
source-git-commit: 5292069412a73f824dbcd967d47737cff5ef58fa
workflow-type: tm+mt
source-wordcount: '2515'
ht-degree: 0%

---

# 設定舊版 [!DNL SharePoint] 整合

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

>[!IMPORTANT]
>
>新 [!DNL SharePoint] 透過22.3版本（2022年7月）發行整合以供生產。 雖然您的使用者仍可存取透過舊版連結的檔案 [!DNL SharePoint] 整合，他們必須使用新 [!DNL SharePoint] 整合以連結來自SharePoint的檔案。
>
>* 新的SharePoint整合不需要管理員進行設定，也可由個別使用者進行設定。 不過，為確保順利轉換至新的SharePoint整合，Workfront管理員必須在Workfront設定區域中進行一些小幅設定變更。
   >
   >    如需資訊和指示，請參閱 [設定舊版SharePoint整合，以繼續存取檔案](#configure-the-legacy-sharepoint-integration-for-continued-access-to-documents) 這篇文章。
>    
>* 建議使用者連結目前透過舊版連結的檔案 [!DNL SharePoint] 整合。
   >    
   >    有關連結文檔的說明，請參閱 [從外部應用程式連結文檔](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).


您可以整合 [!DNL Workfront] with [!DNL SharePoint Online]，讓使用者能導覽至、連結及新增 [!DNL SharePoint] 檔案。Workfront 提供的功能與其他功能類似 [!DNL Workfront] 整合，例如 [!DNL Google Drive], [!DNL Box]，和 [!DNL Dropbox].

此整合僅與 [!DNL SharePoint Online]. 內部部署的例項 [!DNL SharePoint] 不支援。

## 存取需求

您必須具備下列條件才能執行本文所述步驟：

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
   <td>[!UICONTROL計畫]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>您必須是 [!DNL Workfront] 管理員。 如需 [!DNL Workfront] 管理員請參閱 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予使用者完整的管理存取權</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的 [!DNL Workfront] 管理員。

## 必要條件

您必須擁有 [!DNL SharePoint] 修改或設定組織 [!DNL SharePoint].

## 透過新的SharePoint整合連結檔案

個別使用者可以透過新的 [!DNL SharePoint] 整合。 整合不需要管理員配置。 而是使用者登入 [!DNL Microsoft] 帳戶，這可讓整合存取使用者中可用的檔案 [!DNL SharePoint].

使用者首次連線 [!DNL Workfront] [!DNL SharePoint] 整合至 [!DNL SharePoint] 帳戶，他們會看到並同意 [!DNL Workfront] 與使用者互動時的使用 [!UICONTROL SharePoint] 帳戶。 讀取權限允許 [!DNL Workfront] 查看和訪問 [!DNL SharePoint]、和寫入權限可讓使用者將檔案上傳至 [!DNL SharePoint].

有關通過新 [!DNL SharePoint] 整合，請參閱 [將外部文檔連結到 [!DNL Workfront]](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#link-an-external-document-to-workfront)

>[!NOTE]
>
>* A [!DNL SharePoint] 整合可連線至單一 [!DNL SharePoint] 例項。 因此，使用者可為 [!DNL SharePoint]，但無法將整合設為秒 [!DNL SharePoint]，即使他們擁有第二個 [!DNL SharePoint].
>
>* 使用者可透過 [!DNL Workfront] [!DNL SharePoint] 與 [!DNL SharePoint] 帳戶。


## 設定舊版SharePoint整合，以繼續存取檔案

若要確保您的使用者能持續存取透過舊版SharePoint整合連結至Workfront的檔案，您必須重新設定舊版SharePoint整合的存取權，並保留SharePoint用戶端密碼為最新狀態。

* [重新配置對舊版的訪問 [!DNL SharePoint] 整合](#reconfigure-access-to-the-legacy-dnl-sharepoint-integration)
* [設定用戶端密碼以繼續存取舊版 [!DNL SharePoint] 整合](#configure-the-client-secret-for-continued-access-to-the-legacy-dnl-sharepoint-integration)

### 重新配置對舊版的訪問 [!DNL SharePoint] 整合

確保可以訪問通過舊版連結的文檔 [!DNL SharePoint] 整合，同時確保您的使用者無法透過該整合連結新檔案，請完成下列程式。

>[!NOTE]
>
> * 舊版 [!DNL SharePoint] 整合已標示為「[!DNL SharePoint].&quot;
> * 新 [!DNL SharePoint] 整合已標示為「[!UICONTROL [!DNL SharePoint] （圖表API）].&quot;


1. 按一下 **[!UICONTROL 主菜單]** 圖示 ![主菜單](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **[!UICONTROL 設定]** ![設定](../get-started-wf-administration/assets/gear-icon-settings.png).
1. 選擇 **[!UICONTROL 檔案]** 在左側導覽器中，然後選取 **[!UICONTROL 雲端提供者]**.
1. 請確定 **[!DNL SharePoint]** 選項和 **[!UICONTROL [!DNL SharePoint]（圖表API）]** 選項皆啟用。
1. 按一下&#x200B;**[!UICONTROL 儲存]**。
1. 選擇 **[!UICONTROL 檔案]** 在左側導覽器中，然後選取 **[!UICONTROL [!DNL SharePoint]整合]**.
1. 選取清單左側的勾選記號，然後選取 **[!UICONTROL 停用]**.


### 設定用戶端密碼以繼續存取舊版 [!DNL SharePoint] 整合

您的 [!DNL SharePoint] 用戶端密碼每年過期一次。 確保繼續訪問舊版中的文檔 [!DNL SharePoint] 整合，您必須保留 [!DNL SharePoint] 最新用戶端密碼。

>[!IMPORTANT]
>
> 因為 [!DNL SharePoint] 用戶端密碼由 [!DNL Microsoft]，用戶端密碼功能和程式可能會根據 [!DNL SharePoint] made by [!DNL Microsoft]. 請一律檢查 [!DNL Microsoft] 檔案，以取得 [!DNL SharePoint].

<!--1. Go to the site that your [!DNL SharePoint] integration uses. This may be a site that you created when setting up the integrations, or it may be your organization's root site.

1. Add `/_layouts/15/appregnew.aspx` to the end of the URL in the search bar at the top of your browser window.-->

1. 生成新的客戶端密碼，如 [在 [!DNL SharePoint] 附加元件](https://docs.microsoft.com/en-us/sharepoint/dev/sp-add-ins/replace-an-expiring-client-secret-in-a-sharepoint-add-in#generate-a-new-secret)
1. 將此客戶端密碼複製到安全位置。
1. 登入 [!DNL Workfront] 管理員。
1. 在Workfront中，按一下 **[!UICONTROL 主菜單]** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **[!UICONTROL 設定]** ![](assets/gear-icon-settings.png).
1. 在左側面板中，按一下 **[!UICONTROL 檔案]** > **[!UICONTROL [!DNL SharePoint]整合]**.
1. 按一下 [!DNL SharePoint] 要更新的整合，然後按一下 **[!UICONTROL 編輯]**.
1. 在 **[!UICONTROL 用戶端密碼]** 欄位。
1. 按一下&#x200B;**[!UICONTROL 儲存]**。



## 設定舊版SharePoint整合的指示

>[!IMPORTANT]
>
>此整合已淘汰。 此處的指示僅供參考，將於近期移除。


Workfront連線至 [!DNL SharePoint] 使用OAuth 2.0線上執行，此標準供大部分網頁型整合用於使用者驗證和授權。

若要設定OAuth，您需要建立 [!DNL SharePoint] 網站和網站應用程式 [!DNL SharePoint]. 以下幾節將說明此程式。

如需OAuth的詳細資訊，請參閱 [http://oauth.net](http://oauth.net/).

>[!TIP]
>
>讓您輕鬆複製和貼上資訊 [!DNL Workfront] 和 [!DNL SharePoint] 在這些步驟中，我們建議讓兩個應用程式在個別索引標籤中保持開啟。

* [建立和設定 [!DNL SharePoint] 網站](#create-and-configure-a-sharepoint-site)
* [將寫入權限授予網站應用程式](#grant-write-permissions-to-the-site-app)
* [建立 [!DNL Workfront] [!DNL SharePoint] 整合例項](#create-a-workfront-sharepoint-integration-instance)
* [完成整合](#complete-your-integration)
* [新增文件](#add-documents)

### 建立和設定 [!DNL SharePoint] 網站  {#create-and-configure-a-sharepoint-site}

為了 [!DNL Workfront] 驗證 [!DNL SharePoint], [!DNL Workfront] 可使用主網站，讓使用者擁有 [!UICONTROL 完全控制] 權限層級或特定管理權限。 此主體站點充當 [!DNL Workfront].

建立和設定 [!DNL SharePoint] 網站：

1. （選用）如果您不想使用組織的根網站，可以在 [!DNL SharePoint].

   如需指示，請造訪 [建立網站](https://docs.microsoft.com/en-us/sharepoint/create-site-collection) 在 [!DNL Microsoft] 檔案。

   * 選取 **[!UICONTROL 團隊網站]** 選項。

1. （條件性）如果您在步驟1建立網站，請前往您剛建立的網站。

   或

   如果您未在步驟1中建立網站，請前往貴組織的根網站。

1. 新增 `/_layouts/15/appregnew.aspx` 至瀏覽器視窗頂端搜尋列中URL的結尾。
1. 設定下列欄位：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL客戶端ID]</p> </td> 
      <td> <p>按一下 <strong>[!UICONTROL生成]</strong> 來產生用戶端ID。 將此ID複製到安全位置。 您稍後會在您設定 [!DNL SharePoint] 整合 [!DNL Workfront].</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL客戶端密碼]</p> </td> 
      <td> <p>按一下 <strong>[!UICONTROL生成]</strong> 來產生用戶端密碼。 將此密碼複製到安全位置。 您稍後會在您設定 [!DNL SharePoint] 整合 [!DNL Workfront].</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>標題</p> </td> 
      <td> <p>輸入標題，例如 [!DNL Workfront] 網站應用程式。 用戶在添加文檔時看到此標題……</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL應用域]</p> </td> 
      <td> <p><code>my.workfront.com</code> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL重定向URI]</p> </td> 
      <td> <p><code>https://oauth.my.workfront.com/oauth2/redirect</code> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下 **[!UICONTROL 建立]**
1. 繼續 [將寫入權限授予網站應用程式](#grant-write-permissions-to-the-site-app).

### 將寫入權限授予網站應用程式  {#grant-write-permissions-to-the-site-app}

此時，您已成功建立網站應用程式並在中註冊 [!DNL Workfront]. 此網站應用程式也稱為 [!DNL SharePoint]. 位於您的租用戶內。 新網站應用程式不會自動在租用戶記憶體取網站集合。 必須明確授予每個網站集的權限。 下列步驟將示範如何將寫入權限授予新網站應用程式的網站集合。 對您新增至下方的每個網站集合重複這些步驟 [!UICONTROL 可見網站集] 在上述步驟中。

此網站應用程式必須 [!UICONTROL 寫入] 任何網站集合的權限，使用者需透過 [!DNL Workfront].

1. 將&#39;/_layouts/15/appinv.aspx&#39;新增至 [!DNL Sharepoint].

   **範例:**

   ```
   https://mycompany.sharepoint.com/sites/mysite/_layouts/15/appinv.aspx
   ```

1. 設定下列欄位

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL應用程式ID]</td> 
      <td> <p>新增您在 <a href="#create-and-configure-a-sharepoint-site" class="MCXref xref">建立和設定 [!DNL SharePoint] 網站 </a>按一下 <strong>[!UICONTROL查閱]</strong>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL客戶端] / [!UICONTROL應用程式域] / [!UICONTROL重定向URL]</p> </td> 
      <td> <p>當您按一下[!UICONTROL查閱]時，這些會自動填入。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL權限請求XML]</td> 
      <td> <p>將以下XML複製到[!UICONTROL權限請求XML]欄位。 請確定新增的項目如所示，不含其他空格等。 以避免錯誤。</p> 
      <div></a> 
      <div style="mc-code-lang: XML;" class="codeSnippetBody" data-mc-continue="False" data-mc-line-number-start="1" data-mc-use-line-numbers="False"> 
       <pre></pre></div></div></td></tr></tbody></table>

1. 按一下 **[!UICONTROL 建立]**。
1. 在顯示的對話方塊中，按一下 **[!UICONTROL 相信它]**.
1. 按一下 **[!UICONTROL 網站集應用程式權限]** 連結 [!UICONTROL 網站設定].
1. 對其餘網站集重複上述步驟，然後繼續 [建立 [!DNL Workfront] [!DNL SharePoint] 整合例項](#create-a-workfront-sharepoint-integration-instance).

### 建立 [!DNL Workfront] [!DNL SharePoint] 整合例項 {#create-a-workfront-sharepoint-integration-instance}

當您在 [!DNL SharePoint]，您現在可以將資訊從網站應用程式複製到 [!DNL Workfront]. 網站應用程式是應用程式主體，是提出OAuth請求以存取網站集合內檔案的管道。

1. 登入 [!DNL Workfront] 管理員。
1. 按一下 **[!UICONTROL 主菜單]** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **[!UICONTROL 設定]** ![](assets/gear-icon-settings.png).

1. 在左側面板中，按一下 **[!UICONTROL 檔案]** > **[!UICONTROL [!DNL SharePoint]整合]**.
1. 按一下 **[!UICONTROL 新增[!DNL SharePoint]]**.
1. 設定下列欄位：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL名稱]</p> </td> 
      <td> <p>輸入 [!DNL SharePoint] 整合。 使用者在按一下[!UICONTROL新增] &gt; [!UICONTROL從] '整合名稱'時，會看到此名稱。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL [!DNL SharePoint] 主機實例]</p> </td> 
      <td> <p><code>&lt;YourDomain&gt;.sharepoint.com</code> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL [!DNL Azure] 訪問域]</p> </td> 
      <td> <p><code>&lt;YourDomain&gt;.onmicrosoft.com</code> </p> <p>這是指使用者用來透過驗證的主網站。 它可能與[!UICONTROL相同的域 [!DNL SharePoint] 主機實例]。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>
      </p> </td> 
      <td> <b>重要</b> 網站集僅用於舊版 [!DNL SharePoint] 整合。
       <ul> 
        <li> <p><b>如果您使用組織的根網站</b><b>:</b> </p> <p>輸入 <code>/</code></p> </li> 
        <li> <p><b>如果您使用主體網站和子網站：</b> </p> <p><b>重要</b>: [!DNL Microsoft SharePoint] 不再建議使用子網站。</p> <p>輸入您在上節中建立之網站集的URL主體。</p> <p>這是.com之後URL的區段。</p> <p>範例：URL <code>https://mycompany.sharepoint.com/sites/mysite</code>，莖 <code>/sites/mysite</code>.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL SharePoint] 客戶端ID]</td> 
      <td>輸入您在 <a href="#create-and-configure-a-sharepoint-site" class="MCXref xref">建立和設定 [!DNL SharePoint] 網站 </a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL SharePoint] 用戶端密碼]</td> 
      <td>輸入您在 <a href="#create-and-configure-a-sharepoint-site" class="MCXref xref">建立和設定 [!DNL SharePoint] 網站 </a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL可見網站集]</td> 
      <td> <b>重要</b> 網站集僅用於舊版 [!DNL SharePoint] 整合。
       <ul> 
        <li> <p><b> 如果您使用組織的根網站</b><b>:</b> </p> <p>輸入 <code>/</code></p> </li> 
        <li> <p><b>如果您使用主體網站和子網站：</b> </p> <p><b>重要</b>: [!DNL Microsoft SharePoint] 不再建議使用子網站。</p> <p>針對您要新增至 [!DNL SharePoint] 整合，輸入子站點的主體。</p> <p>範例：URL<code>https://mycompany.sharepoint.com/sites/mysite/mysubsite</code>，莖 <code>/sites/mysite/mysubsite</code>.</p> <p><b>附註</b>:   <p>如果僅要測試配置（無子網站），請輸入主網站的主體。 </p> <p>範例：URL <code> https://mycompany.sharepoint.com/sites/mysite</code>，莖 <code>/sites/mysite</code>.</p> <p>當您已依照 <a href="#complete-your-integration" class="MCXref xref">完成整合</a>，您必須刪除主體站點並輸入子站點。</p> 
          <ol> 
           <li value="1">按一下 <strong>[!UICONTROL主菜單]</strong> 圖示 <img src="assets/main-menu-icon.png"> 在 [!DNL Adobe Workfront]，然後按一下 <strong>[!UICONTROL設定]</strong> <img src="assets/gear-icon-settings.png">.<li><p>在左側面板中，按一下 <strong>[!UICONTROL文檔]</strong> &gt; <strong>[!UICONTROL [!DNL SharePoint] 整合]</strong>.</p></li><li><p>按一下 [!DNL SharePoint] 整合，然後按一下「編輯」 。</p></li><li><p>從[!UICONTROL可見站點集合]欄位中刪除主站點的主站點。</p></li><li><p>針對您要新增至 [!DNL SharePoint] 整合，輸入子站點的主體。</p></li><p>範例：URL<code>https://mycompany.sharepoint.com/sites/mysite/mysubsite</code>，莖 <code>/sites/mysite/mysubsite</code>.</p></li> 
          </ol> </p> </li> 
       </ul> <p> </p> <p> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下 **[!UICONTROL 儲存]**
1. 繼續 [完成整合](#complete-your-integration).

### 完成整合 {#complete-your-integration}

基本配置即將完成。

1. 在Workfront中，按一下 **[!UICONTROL 主菜單]** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **[!UICONTROL 檔案]** ![](assets/document-icon.png).
1. 按一下 **[!UICONTROL 新增]**.
1. 按一下 **[!UICONTROL 從]`<title of your [!DNL SharePoint] site>`** 中。

   此時將顯示一個邀請您信任此站點的對話框。

   >[!NOTE]
   >
   >如果此對話方塊未出現，則您的 [!DNL SharePoint] 整合未正確設定。

1. 按一下 **[!UICONTROL 相信它]**.

### 新增文件 {#add-documents}

您現在可以從 [!DNL SharePoint] 頁簽。

如需指示，請參閱 [將外部文檔連結到 [!DNL Workfront]](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#linking-existing-documents) in [從外部應用程式連結文檔](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md)

>[!IMPORTANT]
>
>如果連結資料夾的使用者無法再存取外部應用程式， [!DNL Workfront] 無法再存取資料夾的內容。 例如，如果原本連結資料夾的使用者離開公司，就可能會發生此情況。 若要確保持續存取，具有資料夾存取權的使用者必須重新連結資料夾。

## 疑難排解

* [問題：使用 [!DNL SharePoint] 整合。](#problem-users-experience-authentication-based-errors-when-using-the-sharepoint-integration)
* [問題：As a [!DNL Workfront] 用戶，我無法設定新 [!DNL SharePoint] 例項。 我嘗試做時，發現錯誤。](#problem-as-a-workfront-user-i-am-unable-to-provision-a-new-sharepoint-instance-when-i-attempt-to-do-i-see-an-error)
* [問題：嘗試瀏覽時 [!DNL SharePoint] 檔案 [!DNL Workfront]，我沒有看見任何或所有網站集合。](#problem-when-attempting-to-browse-sharepoint-files-in-workfront-i-do-not-see-any-or-all-of-my-site-collections)
* [問題：我無法訪問 [!DNL SharePoint].](#problem-i-cannot-access-previously-linked-folders-and-documents-in-sharepoint)

### 問題：使用 [!DNL SharePoint] 整合。 {#problem-users-experience-authentication-based-errors-when-using-the-sharepoint-integration}

解決方案：

使用者必須是群組的成員，且群組擁有 [!DNL SharePoint] 頁簽。

具有 [!UICONTROL 完全控制] 存取權 [!DNL SharePoint] 整合。 如果您不想授予使用者完全控制存取權，您必須授與下列權限：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL設計]</p> </td> 
   <td> <p>可以檢視、新增、更新、刪除、核准及自訂</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL編輯]</p> </td> 
   <td> <p>可以添加、編輯和刪除清單；可以查看、添加、更新和刪除清單項和文檔</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Contribute]</p> </td> 
   <td> <p>可以查看、添加、更新和刪除清單項和文檔</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL僅查看]</p> </td> 
   <td> <p>可以查看頁面、清單項和文檔（具有伺服器端檔案處理程式的文檔類型可以在瀏覽器中查看，但不能下載）</p> </td> 
  </tr> 
 </tbody> 
</table>

如需建立和編輯權限層級的指示，請參閱 [如何建立和編輯權限層級](https://docs.microsoft.com/en-us/sharepoint/how-to-create-and-edit-permission-levels) 在Microsoft檔案中。

### 問題：As a [!DNL Workfront] 用戶，我無法設定新 [!DNL SharePoint] 例項。 我嘗試做時，發現錯誤。 {#problem-as-a-workfront-user-i-am-unable-to-provision-a-new-sharepoint-instance-when-i-attempt-to-do-i-see-an-error}

解決方案：

這可能是因為若干原因所導致，原因為 [!DNL Workfront] 或 [!DNL SharePoint]的設定。 確認：

* 用戶端ID、用戶端密碼、傳回URL和其他設定欄位會正確對應至 [!DNL Workfront] [!DNL SharePoint] 整合例項和 [!DNL SharePoint] 網站應用程式。
* 使用者已 [!UICONTROL 完全控制] 對用於驗證的網站集合的權限。
* 網站應用程式列於 [!UICONTROL 網站應用程式權限] 針對 [!UICONTROL 網站集] 用於驗證。

### 問題：嘗試瀏覽時 [!DNL SharePoint] 檔案 [!DNL Workfront]，我沒有看見任何或所有網站集合。 {#problem-when-attempting-to-browse-sharepoint-files-in-workfront-i-do-not-see-any-or-all-of-my-site-collections}

解決方案：

若要在 [!DNL Workfront]，必須符合下列條件：

* 網站集必須註冊於 [!DNL Workfront] [!DNL SharePoint] 整合例項。

   若要在 [!DNL Workfront]:

   1. 前往 [!UICONTROL 設定] > [!UICONTROL 檔案] > [!UICONTROL [!DNL SharePoint] 整合].
   1. 編輯 [!DNL SharePoint] 整合例項資訊。
   1. 確認網站集列於 [!UICONTROL 可見網站集].

* 使用者必須擁有中網站集的檢視存取權 [!DNL SharePoint].
* 若要在 [!DNL SharePoint]，前往 [!DNL SharePoint]，然後開啟網站集> [!UICONTROL 設定] > [!UICONTROL 網站權限].
* 此 [!DNL SharePoint] 網站應用程式必須擁有網站集合的存取權。

   若要在 [!DNL SharePoint]:

   1. 前往網站集> [!UICONTROL 設定] > [!UICONTROL 網站應用程式權限].
   1. 確保 [!UICONTROL 網站應用程式] 使用者 [!DNL Workfront] 即可取得Advertising Cloud的說明。
   1. （條件性）如果未列出網站應用程式，請使用_layouts/15/appinv.aspx新增至網站集合。

      有關添加網站集的資訊，請參閱授予網站應用的寫權限。

### 問題：我無法訪問 [!DNL SharePoint]. {#problem-i-cannot-access-previously-linked-folders-and-documents-in-sharepoint}

解決方案：

如果連結 [!DNL SharePoint] 資料夾無法再驗證， [!DNL Workfront] 無法再存取資料夾的內容。 例如，如果原本連結資料夾的使用者離開公司，就可能會發生此情況。

若要確保持續存取，具有資料夾存取權的使用者必須重新連結資料夾。

有關從外部提供程式連結資料夾的資訊，請參見 [從外部應用程式連結文檔](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

### 問題：嘗試從 [!DNL Sharepoint]

#### 解決方案：

若 [!UICONTROL 可見網站集] 清單已在Sharepoint中刪除。 檢查 [!UICONTROL 可見網站集] 清單，並刪除已在Sharepoint中刪除的任何站點。
