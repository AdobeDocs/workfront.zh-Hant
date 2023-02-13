---
product-previous: workfront-proof
product-area: documents
navigation-topic: create-proofs-and-files
title: 在中產生校樣 [!DNL Workfront Proof]
description: Workfront校樣可讓您從檔案或網站建立校樣，並與其他人共用這些校樣。 以下步驟說明了各種可用的配置選項 — EDIT ME。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 49657851-2948-4d3b-b2ce-c8359eeb315b
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '2267'
ht-degree: 0%

---

# 在中產生校樣 [!DNL Workfront Proof]

>[!IMPORTANT]
>
>本文說明獨立產品中的功能 [!DNL Workfront Proof]. 有關內部校對的資訊 [!DNL Adobe Workfront]，請參閱 [校對](../../../review-and-approve-work/proofing/proofing.md).

[!DNL Workfront Proof] 可讓您從檔案或網站建立校樣，並與他人共用這些校樣。 下列步驟說明可用的各種設定選項：

## 生成文檔校樣

1. 執行下列任一操作以開始建立新校樣並顯示 [!UICONTROL 新校樣] 頁面：

   * 按一下綠色 **[!UICONTROL 新校樣]** 按鈕。
   * 在 **[!UICONTROL 控制面板]** 區域，在 **[!UICONTROL 概述]** ，按一下 **[!UICONTROL 新校樣]** 連結。

   * 透過Dropzone提交（企業功能）。
   * 此 **[!UICONTROL 新校樣]** 頁面。

1. 要校樣一個或多個文檔，請通過以下任一方式添加要校樣的文檔（重複此過程以添加要校樣的多個文檔）:

   * 將文檔從檔案系統拖放到 **[!UICONTROL 新增檔案]** 的上界。
   * 按一下 **[!UICONTROL 新增檔案]** 區域，然後瀏覽以查找並選擇要從工作站上的檔案系統上載的文檔。

      ![proof_document_upload.png](assets/proof-document-upload-350x64.png)

1. 若要校樣一或多個網站，請在 **[!UICONTROL 新增檔案]** 區域，然後按 **[!UICONTROL 輸入]**.

1. （選用）重複此程式，新增多個網站以進行校樣。

   如需校對網站的詳細資訊，請參閱 [產生URL的校樣](#generate-a-proof-for-a-url).

   ![](assets/proof-website-350x65.png)

1. （可選）修改任何已上載檔案的檔案名：

   1. 將滑鼠移到要修改的文檔名稱上 **[!UICONTROL 新增檔案]** ，然後按一下 **[!UICONTROL 編輯]** 表徵圖。

      ![proof_edit.png](assets/proof-edit-350x53.png)

   1. 在 **[!UICONTROL 校樣名稱]** 欄位，指定新名稱，然後按一下 **[!UICONTROL 完成]**.

   1. （可選）要刪除要上載的任何檔案，請將滑鼠移到要刪除的文檔清單中的 **[!UICONTROL 新增檔案]** ，然後按一下 **[!UICONTROL 刪除]** 表徵圖。

      ![proof_delete.png](assets/proof-delete-350x53.png)

   1. （選用）啟用選項， **[!UICONTROL 將所有相容的檔案合併為單一校樣]**.

      **啟用此選項時：** 所有靜態檔案和網站都可透過單一校樣取得，而且您一次最多可上傳50個檔案。

      >[!NOTE]
      >
      >互動式檔案（包括影片和互動式網站）無法結合為單一校樣。

      **禁用此選項時：** 所有檔案和網站都會以個別校樣的形式產生，您一次最多可上傳20個檔案。

      若要將所有上傳的檔案和網站合併成單一校樣：

      1. 啟用選項， **[!UICONTROL 將所有相容的檔案合併為單一校樣]**.
      1. 在 **[!UICONTROL 校樣名稱]** 欄位中，指定組合校樣的新名稱。
      1. 在 **[!UICONTROL 新增檔案]** 區域中，將檔案拖動到所需順序以重新排序包含的檔案。 檔案的順序是組合校樣的頁面順序。 如需建立合併校樣的詳細資訊，請參閱 [建立多頁校樣](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-multi-page-proof.md).

1. （選用）如果您想要使用包含多個階段的自動化工作流程，請在 **[!UICONTROL 工作流程]** ，請從以下選項中選擇：

   * **基本：** 選擇此選項可指定在建立校樣後立即擁有校樣存取權的使用者。 您可以與多個使用者共用校樣。

      如需共用校樣的詳細資訊，請參閱 [在內共用校樣 [!DNL Adobe Workfront]](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md).

   * **自動化：** 選擇此選項可在您有複雜的審核流程時管理內容審核和批准，或者如果您定期將內容發送給相同的人員組進行審核。 透過自動化工作流程，校樣會從階段移至階段，直到最終核准。 需要批准時，會通知相關用戶。

      如需建立自動化工作流程的詳細資訊，請參閱 [在 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/automated-workflow/set-up-proof-auto-workflow.md#create2).

1. 選取是否要傳送電子郵件通知和自訂訊息給您在上一個步驟中選取的使用者：

   * **將此校樣通知收件者：** 選取此選項可傳送電子郵件通知給使用者。 當 **[!UICONTROL 基本共用]** 在 **[!UICONTROL 工作流程]** 區段中，建立校樣時會傳送電子郵件通知。 當 **[!UICONTROL 自動化工作流程]** 在 **[!UICONTROL 工作流程]** 區段中，當校樣進入使用者相關聯的自動化工作流程階段時，會傳送電子郵件通知。

   * **新增自訂訊息：** 選取此選項，在通知中加入自訂訊息。 您可以指定主旨和訊息內文。 訊息內文可包含RTF格式，例如粗體、項目符號和超連結。

1. 選取下列任何校樣設定：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">需要登入 — 校樣只能與其他使用者共用</td> 
      <td> <p><strong>需要登入 — 校樣只能與其他使用者共用：</strong> 選取此選項時，僅 [!DNL Workfront Proof] 使用者可檢視校樣。</p> <p>預設會停用此選項；任何具有URL的人都能檢視校樣。</p> <p>選取此選項時：</p> 
       <ul> 
        <li>除非使用者已新增至校樣，否則無法登入校樣。</li> 
        <li>無法啟用訂閱。</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">此證明只需要一個決定</td> 
      <td> <p>當選擇此選項時，在某個決策者作出決定後完成審查。</p> <p>預設會停用此選項。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">需要以電子方式簽署決策</td> 
      <td>使用者在決定校樣時，必須指定其使用者名稱和密碼。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">做出所有必要決策時鎖定校樣</td> 
      <td> <p><strong></strong> 啟用此設定後，在做出所有決策後，會鎖定校樣狀態。 當最終批准者作出決定時，狀態會自動從解除鎖定變更為鎖定。</p> <p>預設會停用此選項。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">下載原始檔案</td> 
      <td> <p><strong></strong> 選取此選項時，審閱者將能夠下載建立校樣的原始檔案。</p> <p>取消選取此選項時，「下載」圖示將不再顯示。<br>預設會啟用此選項。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">透過公用URL或內嵌程式碼共用校樣</td> 
      <td>選取此選項時，可透過公用URL或內嵌程式碼來共用校樣。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">透過公開URL或內嵌程式碼訂閱校樣</td> 
      <td> <p>選取此選項時，尚未明確新增至校樣的人員可訂閱校樣。 訂閱校樣的人員會獲得您在下列設定中定義的角色和電子郵件：</p> 
       <ul> 
        <li><strong>訂閱者角色</strong>:分配給訂閱校樣的所有審核者的預設校樣角色。</li> 
        <li><strong>訂閱者的電子郵件警報設定</strong>:指派給訂閱校樣之所有審核者的預設電子郵件警報。</li> 
        <li> <p><strong>透過電子郵件連結進行校樣存取</strong>:設定訂閱者是否收到包含校樣連結的電子郵件。 您可以選取 <strong>無電子郵件</strong> （存取校樣不需要電子郵件連結）, <strong>僅校樣通知電子郵件</strong> （訂閱者會透過電子郵件收到校樣的連結，無需任何驗證），或 <strong>驗證和校樣通知電子郵件</strong> (訂閱者會透過電子郵件收到校樣的連結，且必須按一下連結才能存取校樣；此選項的目的是確保人員輸入了他們有權訪問的正確電子郵件地址)。</p> <p>注意：如果校樣已附加「自動化工作流程」，所有訂閱都會產生確認電子郵件給校樣擁有者，讓他們決定應將人員新增至哪個階段。</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下 **[!UICONTROL 建立校樣]**.

   Workfront會開始產生所選檔案或網站的證明。 視檔案大小和類型而定，檔案上傳的延遲時間會有所不同。 請耐心等待，因為較大的檔案需要更長的時間才能產生。 您可以離開頁面，Workfront會繼續產生您的檔案。 檔案上傳大小上限為4GB。

   產生校樣後，按一下 **[!UICONTROL 前往校樣]** 啟動校對工具。

   ![螢幕截圖2018-05-16_08-59-34.png](assets/screenshot-2018-05-16-08-59-34-350x134.png)

   文檔將出現在校對工具中。

   帳戶上未啟用校樣的使用者仍可檢視檔案，並對校樣發表意見。

## 產生URL的校樣 {#generate-a-proof-for-a-url}

您可以首次產生URL的校樣。 或者，您也可以產生先前已產生校樣的URL校樣新版本。

>[!NOTE]
>
>只有在 [!DNL Workfront] 環境與 [!DNL Workfront Proof] 高級帳戶。 如果您無法使用本節所述的校對功能，請與系統管理員聯繫。

若要產生URL的校樣：

1. 執行下列任一操作以開始建立新校樣並顯示 [!UICONTROL 新校樣] 頁面：

   * 按一下綠色 **[!UICONTROL 新校樣]** 按鈕。
   * 在 **[!UICONTROL 控制面板]** 區域，在 **[!UICONTROL 概述]** ，按一下 **[!UICONTROL 新校樣]** 連結。

   * 透過Dropzone提交（企業功能）。

1. （有條件）在 **[!UICONTROL 新校樣]** 頁面，以建立現有校樣的新版本：

   1. 選取您要新增版本的URL校樣。
   1. 按一下 **[!UICONTROL 新版本]** 按鈕。

      ![螢幕截圖2018-05-15_10-59-56.png](assets/screenshot-2018-05-15-10-59-56-350x80.png)

1. 在顯示的「新校樣版本」頁面中，指定您要在 **[!UICONTROL 新增檔案]** 區域，然後按 **[!UICONTROL 輸入]**.

1. （選用）重複此程式，新增多個網站以進行校樣。

   ![proof_website.png](assets/proof-website-350x65.png)

1. 按一下 **[!UICONTROL 新增檔案]** 的上界。

   ![proof_upload_website_modify.png](assets/proof-upload-website-modify-350x185.png)

1. 指定 **[!UICONTROL 校樣名稱]** 來證明。

   依預設，校樣名稱與網站URL相同。

1. 選擇 **[!UICONTROL 處理網站內容]** 選項：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">擷取螢幕擷圖</td> 
      <td>建立URL首頁的靜態影像校樣。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">互動</td> 
      <td> <p>建立校樣，讓審核者導覽網站、檢視HTML5影像、Flash元素等。</p> <p>若要建立互動式校樣，網站必須使用安全通訊協定(https)托管。 此外，無法內嵌於iframe的網站無法產生為互動式校樣（iframe內嵌限制是由您嘗試內嵌的網站所控制）。</p> <p>建立初始校樣後，建立後續版本時無法變更此設定。</p> <p>如需互動式測試的詳細資訊，請參閱 <a href="#generate-a-proof-for-interactive-content" class="MCXref xref">產生互動式內容的校樣</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">螢幕截圖解析度</td> 
      <td> <p>（此選項不適用於互動式校樣）。 您可以調整內容顯示的解析度，也可以選取多個解析度。</p> <p>這可讓檢閱校樣的使用者檢視內容在不同裝置（例如各種大小的手機、平板電腦和顯示器）上的顯示方式。</p> <p>如果您選取多個解析度，則會針對您選取的每個解析度建立個別的校樣。</p> <p>當使用者對校樣留言時，目前的螢幕解析度會自動顯示在留言中，以確保其他使用者知道留言相關聯的解析度。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">尋找子頁面</td> 
      <td>（此選項不適用於互動式校樣）。 選取此選項可導覽網站的頁面。 您可以將網站從主要頁面深度展開至2個層級。 將滑鼠移至頁面上以檢視頁面的URL。 僅選取您要校樣的頁面。 依預設，您選取的每個頁面都會以個別校樣的形式建立；或，啟用 <strong>合併為單一校樣</strong> 選項，將所有選取的頁面合併為單一校樣。</td> 
     </tr> 
    </tbody> 
   </table>

1. （選用）設定任何進階校對選項，例如共用校樣、新增自動化工作流程或設定存取權和訂閱設定。 如需這些選項的詳細資訊，請參閱下列文章：

   * [在內共用校樣 [!DNL Adobe Workfront]](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md)
   * [在 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/automated-workflow/set-up-proof-auto-workflow.md)
   * [配置校樣的訪問和訂閱設定](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/configure-access-subscription-settings-proof.md)

1. 按一下 **[!UICONTROL 完成]**.

   如果您要將新版本添加到現有URL校樣，則在原始校樣或先前版本上配置的任何選項都將保留在此版本中。如果您要將新版本添加到現有URL校樣，則在原始校樣或先前版本上配置的任何選項都將保留在此版本中。

1. 按一下 **[!UICONTROL 建立校樣]**.

## 產生互動式內容的校樣 {#generate-a-proof-for-interactive-content}

使用此功能需要Pro Workfront計畫或更高版本。 如需各種可用計畫的詳細資訊，請參閱 [Workfront計畫](https://www.workfront.com/plans).

如需互動式內容的詳細資訊，請參閱 [互動式內容校樣概觀](../../../review-and-approve-work/proofing/proofing-overview/interactive-content-proofs.md).

* [將互動式內容新增為URL](#add-interactive-content-as-a-url)
* [將互動式內容新增為ZIP檔案](#add-interactive-content-as-a-zip-file)

### 將互動式內容新增為URL {#add-interactive-content-as-a-url}

如需如何新增互動式URL校樣的詳細資訊，請參閱  [產生URL的校樣](#generate-a-proof-for-a-url).

### 將互動式內容新增為ZIP檔案 {#add-interactive-content-as-a-zip-file}

1. 建立.zip套件檔案，以準備您的內容。

   如需.zip套件檔案規格的相關資訊，請參閱 [關於準備ZIP檔案中的互動式內容以進行校對](../../../review-and-approve-work/proofing/proofing-overview/interactive-content-proofs.md#howtoprepareaninteractiveziparchive) 在文章中 [互動式內容校樣概觀](../../../review-and-approve-work/proofing/proofing-overview/interactive-content-proofs.md).

1. 執行下列任一操作以開始建立新校樣並顯示 [!UICONTROL 新校樣] 頁面：

   * 按一下綠色 **[!UICONTROL 新校樣]** 按鈕。
   * 在 **[!UICONTROL 控制面板]** 區域，在 **[!UICONTROL 概述]** ，按一下 **[!UICONTROL 新校樣]** 連結。

   * 透過Dropzone提交（企業功能）。

1. 在 **[!UICONTROL 新校樣]** 頁面，將您的互動式.zip套件組合拖放至 **[!UICONTROL 新增檔案]** 的上界。

1. （可選）設定任何進階校對選項，例如共用校樣、新增自動化工作流程或設定存取權和訂閱設定。 如需這些選項的詳細資訊，請參閱下列文章：

   * [在內共用校樣 [!DNL Adobe Workfront]](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md)
   * 在文章中
   * [配置校樣的訪問和訂閱設定](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/configure-access-subscription-settings-proof.md)

1. 按一下 **[!UICONTROL 建立校樣]**.

   Workfront開始產生.zip套件組合的證明。 檔案上傳的延遲時間會因套件大小而異。 產生較大的檔案需要較長的時間。 您可以離開頁面，Workfront會繼續產生您的檔案。 檔案上傳大小上限為4GB。

   校樣產生後，您可以按一下 **[!UICONTROL 前往校樣]** 按鈕開啟校樣。
