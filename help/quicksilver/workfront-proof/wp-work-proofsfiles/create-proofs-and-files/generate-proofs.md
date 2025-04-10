---
product-previous: workfront-proof
product-area: documents
navigation-topic: create-proofs-and-files
title: 在 [!DNL Workfront Proof]中產生校樣
description: Workfront Proof可讓您從檔案或網站建立校樣，並和其他人共用這些校樣。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 49657851-2948-4d3b-b2ce-c8359eeb315b
source-git-commit: de23513976d7bc4fe34cbf7b007a41c3b9797347
workflow-type: tm+mt
source-wordcount: '1889'
ht-degree: 1%

---

# 在[!DNL Workfront Proof]中產生校訂

<!-- Audited: 4/2025 -->

>[!IMPORTANT]
>
>本文提及獨立產品[!DNL Workfront Proof]中的功能。 有關[!DNL Adobe Workfront]內部校訂的資訊，請參閱[校訂](../../../review-and-approve-work/proofing/proofing.md)。

[!DNL Workfront Proof]可讓您從檔案或網站建立校樣，並與他人共用這些校樣。 下列步驟說明可用的各種設定選項：

## 從檔案產生校訂

1. 執行下列任一項作業以開啟&#x200B;**[!UICONTROL 新校訂]**&#x200B;頁面：

   * 按一下任何頁面左上角的&#x200B;**[!UICONTROL 新校訂]**&#x200B;按鈕。
   * 透過Dropzone提交（企業功能）。

1. 若要校訂一或多個檔案，請以下列其中一種方式新增要校訂的檔案（重複此程式以新增多個檔案）：

   * 將檔案從您的檔案系統拖放到&#x200B;**[!UICONTROL 新增檔案]**&#x200B;區域的拖放區域。
   * 在&#x200B;**[!UICONTROL 新增檔案]**&#x200B;區域中，按一下&#x200B;**瀏覽**&#x200B;連結，從工作站的檔案系統尋找並選取您要上傳的檔案。

     ![proof_document_upload.png](assets/proof-document-upload-350x64.png)

1. 若要校訂網站，請在&#x200B;**[!UICONTROL 新增檔案]**&#x200B;區域中輸入網站的URL，然後按&#x200B;**[!UICONTROL Enter]**。 重複此步驟以新增多個網站進行校訂。

   如需校訂網站的詳細資訊，請參閱[產生URL的校訂](#generate-a-proof-for-a-url)。

   ![校訂網站](assets/proof-website-350x65.png)

1. （可選）修改任何已上傳檔案的檔案名稱：

   1. 在檔案清單中，將滑鼠停留在您要修改的檔名稱上，然後按一下&#x200B;**[!UICONTROL 編輯]**&#x200B;圖示。

      ![proof_edit.png](assets/proof-edit-350x53.png)

   1. 在&#x200B;**[!UICONTROL 校訂名稱]**&#x200B;欄位中，指定新名稱，然後按一下&#x200B;**[!UICONTROL 完成]**。

   1. （選擇性）若要從上傳中刪除任何檔案，請將游標移至檔案清單中您要刪除的檔案上，然後按一下&#x200B;**[!UICONTROL 刪除]**&#x200B;圖示。

      ![proof_delete.png](assets/proof-delete-350x53.png)

   1. （選擇性）啟用&#x200B;**[!UICONTROL 將所有相容的檔案合併為單一校訂]**&#x200B;選項。

      **啟用此選項時：**&#x200B;所有靜態檔案和網站都可在單一校訂中使用，您一次最多可上傳50個檔案。

      >[!NOTE]
      >
      >互動式檔案（包括視訊和互動式網站）無法合併為單一校訂。

      **停用此選項時：**&#x200B;所有檔案和網站都會產生為個別校訂，您一次最多可上傳20個檔案。

      若要將所有上傳的檔案和網站合併為單一校訂：

      1. 啟用&#x200B;**[!UICONTROL 將所有相容檔案合併為單一校訂]**&#x200B;選項。
      1. 在&#x200B;**[!UICONTROL 校訂名稱]**&#x200B;欄位中，輸入合併校訂的新名稱。
      1. 在&#x200B;**[!UICONTROL 新增檔案]**&#x200B;區域中，將檔案拖曳到所要的順序來重新排序包含的檔案。 檔案的順序是合併校訂的頁面順序。 如需有關建立合併校訂的詳細資訊，請參閱[建立多頁校訂](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-multi-page-proof.md)。

1. （選擇性）如果要使用包含多個階段的自動化工作流程，請從&#x200B;**[!UICONTROL 工作流程]**&#x200B;區段中的下列選項中選取：

   * **基本：**&#x200B;選取此選項可指定您要在校訂建立後立即存取校訂的使用者。 您可以與多位使用者共用校訂。

     如需共用校訂的詳細資訊，請參閱[在 [!DNL Adobe Workfront]](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md)內共用校訂。

   * **自動化：**&#x200B;選取此選項，可在您有複雜的稽核程式，或您定期傳送內容給相同群組人員稽核時，管理內容稽核與核准。 使用自動化工作流程時，校樣會從不同階段移至不同階段，直到最後核准為止。 任何時候相關使用者都需要進行核準時，都會收到通知。

     如需有關建立自動化工作流程的詳細資訊，請參閱[在 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/automated-workflow/set-up-proof-auto-workflow.md#create2)中使用自動化工作流程設定校訂。

1. 選取是否將電子郵件通知和自訂訊息傳送給您在上一步驟中選取的使用者：

   * **將此校訂通知收件者：**&#x200B;選取此選項即可傳送電子郵件通知給使用者。 在&#x200B;**[!UICONTROL 工作流程]**&#x200B;區段中選取&#x200B;**[!UICONTROL 基本共用]**&#x200B;時，會在建立校訂時傳送電子郵件通知。 在&#x200B;**[!UICONTROL 工作流程]**&#x200B;區段中選取&#x200B;**[!UICONTROL 自動化工作流程]**&#x200B;時，當校訂進入使用者關聯的自動化工作流程階段時，會傳送電子郵件通知。

   * **新增自訂訊息：**&#x200B;選取此選項以在通知中包含自訂訊息。 您可以指定主旨和訊息內文。 訊息內文可包含RTF格式，例如粗體、專案符號和超連結。

1. 選取下列任一校訂設定：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">需要登入。 此校訂無法與其他使用者共用</td> 
      <td> <p>選取此選項時：</p> 
       <ul> 
        <li>使用者無法登入校訂進行檢視，除非他們已新增到校訂中。</li> 
        <li>無法啟用訂閱。</li> 
       </ul> 
       <p>此選項預設為停用。</p> 
       </td> 
     </tr> 
     <tr> 
      <td role="rowheader">需要以電子方式簽署決策</td> 
      <td><p>選取此選項時，使用者必須在就校訂做出決定時指定其使用者名稱和密碼。</p>
      <p>此選項預設為停用。</p>
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">完成所有必要的決定時鎖定校訂</td> 
      <td> <p>啟用此設定時，完成所有決定後才會鎖定校訂狀態。 當最終核准者做出決定時，狀態會自動從已解除鎖定變更為已鎖定。</p> 
      <p>此選項預設為停用。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">允許下載原始檔案</td> 
      <td> <p><strong></strong> 選取此選項時，稽核者可下載從中建立校訂的原始檔案。</p> <p>取消選取此選項時，不再顯示「下載」圖示。</p>
      <p>此選項預設為啟用。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">允許透過公開URL或內嵌代碼共用校訂</td> 
      <td><p>選取此選項時，可透過公用URL或內嵌程式碼共用校訂。</p>
       <p>此選項預設為啟用。</p>
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">允許透過公開URL或內嵌程式碼訂閱校訂</td> 
      <td> <p>選取此選項時，尚未新增到校訂的人員可以訂閱校訂。 訂閱校訂的人員會獲得您在以下設定中定義的角色和電子郵件：</p> 
       <ul> 
        <li><strong>訂閱者角色</strong>：指派給所有訂閱校訂的檢閱者的預設校訂角色。</li> 
        <li><strong>訂閱者的電子郵件警示設定</strong>：指派給所有訂閱校訂的稽核者的預設電子郵件警示。</li> 
        <li> <p><strong>需要透過電子郵件連結存取校訂</strong>：設定訂閱者是否收到包含校訂連結的電子郵件。 您可以選取<strong>無電子郵件</strong> （存取校訂不需要電子郵件連結）、<strong>僅校訂通知電子郵件</strong> （訂閱者會透過電子郵件收到校訂的連結，而不需要任何驗證）或<strong>驗證和校訂通知電子郵件</strong> (訂閱者會透過電子郵件收到校訂的連結，必須按一下連結才能存取校訂。 此選項的目的是確保人員已輸入他們有權存取的正確電子郵件地址)。</p> <p>注意：如果校訂附加了自動化工作流程，則所有訂閱都會向校訂所有者產生確認電子郵件，以便他們決定應將該人員新增到哪個階段。</p> </li> 
       </ul> 
        <p>此選項預設為停用。</p>
       </td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下&#x200B;**[!UICONTROL 建立校訂]**。 Workfront會產生所選檔案或網站的校訂。

   檔案上傳的延遲時間視檔案大小和型別而異。 產生大型檔案需要更長的時間。 您可以在Workfront持續產生檔案時離開頁面。 檔案上傳大小上限為4GB。

## 使用URL產生靜態校訂 {#generate-a-proof-for-a-url}

您可以使用網站URL產生靜態校樣。

>[!NOTE]
>
>您必須在[!DNL Workfront]環境與[!DNL Workfront Proof] Premium帳戶整合時，才能產生URL的互動式校訂。 如果您無法使用本節中討論的校訂，請聯絡Workfront管理員。

1. 執行下列任一項作業以開啟&#x200B;**[!UICONTROL 新校訂]**&#x200B;頁面：

   * 按一下任何頁面左上角的&#x200B;**[!UICONTROL 新校訂]**&#x200B;按鈕。
   * 透過Dropzone提交（企業功能）。

1. 在&#x200B;**新校訂**&#x200B;頁面中，在&#x200B;**[!UICONTROL 新增檔案]**&#x200B;區域輸入您要建立校訂的網站URL，然後在您的鍵盤上按&#x200B;**[!UICONTROL Enter]**&#x200B;或&#x200B;**[!UICONTROL Return]**。

1. （選用）重複此程式，將多個網站新增至校樣中。

   ![proof_website.png](assets/proof-website-350x65.png)

1. 在&#x200B;**[!UICONTROL 新增檔案]**&#x200B;區域中，按一下URL右側的&#x200B;**編輯**&#x200B;圖示以開啟網站校訂詳細資訊。

   ![proof_upload_website_modify.png](assets/proof-upload-website-modify-350x185.png)

1. 輸入&#x200B;**[!UICONTROL 校訂名稱]**。 依預設，校訂名稱與網站URL相同。

1. 選取下列任一&#x200B;**[!UICONTROL 處理網站內容]**&#x200B;選項：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">擷取熒幕擷圖</td> 
      <td>建立URL首頁靜態影像的校訂。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">互動</td> 
      <td> <p>建立校訂，讓檢閱者導覽網站、檢視HTML5影像、Flash元素等。</p> <p>若要建立互動式校樣，網站必須以安全通訊協定(https)代管。 此外，無法內嵌於iframe的網站無法產生為互動式校樣（iframe內嵌限制由您嘗試內嵌的網站控制）。</p> <p>建立初始校訂後，建立後續版本時無法變更此設定。</p> <p>如需互動式校訂的詳細資訊，請參閱<a href="#generate-a-proof-for-interactive-content" class="MCXref xref">產生互動式內容的校訂</a>。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">熒幕擷圖解析度</td> 
      <td> <p>（此選項不適用於互動式校樣。） 您可以調整內容顯示的解析度，也可以選取多個解析度。</p> <p>這可讓使用者檢視校訂以檢視內容在不同裝置上的顯示方式，例如各種尺寸的電話、平板電腦和顯示器。</p> <p>如果您選取多個解析度，則會為您選取的每個解析度建立個別的校樣。</p> <p>當使用者對校訂進行評論時，目前的熒幕解析度會自動顯示在評論中，以確保其他使用者知道評論關聯的解析度。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">尋找子頁面</td> 
      <td>（此選項不適用於互動式校樣。） 選取此選項可瀏覽網站的各個頁面。 您可將網站從首頁面展開至最多2層深。 將滑鼠懸停在頁面上，可檢視頁面的URL，並僅選取您要校訂的頁面。 依預設，您選取的每個頁面都會建立為個別校樣。 或者，您可以啟用<strong>將所有相容的檔案合併為單一校訂</strong>選項。</td> 
     </tr> 
    </tbody> 
   </table>

1. （選用）設定任何進階校訂選項，例如共用校訂、新增「自動化工作流程」或設定存取和訂閱設定。 如需這些選項的詳細資訊，請參閱下列文章：

   * [在 [!DNL Adobe Workfront]內共用校訂](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md)
   * [在 [!DNL Workfront Proof]中使用自動化工作流程設定校訂](../../../workfront-proof/wp-work-proofsfiles/automated-workflow/set-up-proof-auto-workflow.md)
   * [設定校訂的存取權和訂閱設定](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/configure-access-subscription-settings-proof.md)

1. 按一下&#x200B;**[!UICONTROL 完成]**。

1. 按一下&#x200B;**[!UICONTROL 建立校訂]**。

## 產生互動式內容的校訂 {#generate-a-proof-for-interactive-content}

<!--A Pro Workfront Plan or higher is required to use this feature. For more information about the various plans available, see [Workfront Plans](https://www.workfront.com/plans).-->

如需互動式內容的詳細資訊，請參閱[互動式內容校訂總覽](../../../review-and-approve-work/proofing/proofing-overview/interactive-content-proofs.md)。

* [將互動式內容新增為URL](#add-interactive-content-as-a-url)
* [將互動式內容新增為ZIP檔案](#add-interactive-content-as-a-zip-file)

### 將互動式內容新增為URL {#add-interactive-content-as-a-url}

如需如何新增互動式URL校訂的相關資訊，請參閱[產生URL的校訂](#generate-a-proof-for-a-url)。

### 將互動式內容新增為ZIP檔案 {#add-interactive-content-as-a-zip-file}

1. 建立.zip隨附檔案，準備您的內容。

   如需有關.zip套件檔案規格的資訊，請參閱[互動式內容校訂總覽](../../../review-and-approve-work/proofing/proofing-overview/interactive-content-proofs.md)。

1. 執行下列任一項作業以開啟&#x200B;**[!UICONTROL 新校訂]**&#x200B;頁面：

   * 按一下任何頁面左上角的&#x200B;**[!UICONTROL 新校訂]**&#x200B;按鈕。
   * 透過Dropzone提交（企業功能）。

1. 在&#x200B;**[!UICONTROL 新校訂]**&#x200B;頁面中，將互動式.zip套件組合拖放至&#x200B;**[!UICONTROL 新增檔案]**&#x200B;區域。

1. （選用）設定任何進階校訂選項，例如共用校訂、新增自動化工作流程，或設定存取權和訂閱設定。 如需這些選項的詳細資訊，請參閱下列文章：

   * [在 [!DNL Adobe Workfront]內共用校訂](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md)
   * [設定校訂的存取權和訂閱設定](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/configure-access-subscription-settings-proof.md)

1. 按一下&#x200B;**[!UICONTROL 建立校訂]**。 Workfront會產生zip檔案的校樣。

   檔案上傳的延遲時間視壓縮檔案大小而定。 您可以在Workfront持續產生檔案時離開頁面。 檔案上傳大小上限為4GB。
