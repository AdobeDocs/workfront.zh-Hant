---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 聯結器
navigation-topic: apps-and-their-modules
title: AWS S3模組
description: 此 [!DNL Adobe Workfront Fusion AWS] S3模組可讓您對S3儲存貯體執行操作。
author: Becky
feature: Workfront Fusion
exl-id: 33623b5d-d9ff-4d41-b938-33378f50539e
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1429'
ht-degree: 1%

---

# AWS S3模組

此 [!DNL Adobe Workfront Fusion AWS] S3模組可讓您對S3儲存貯體執行操作。

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

有關以下專案的資訊： [!DNL Adobe Workfront Fusion] 授權，請參閱 [[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 必要條件

使用 [!UICONTROL AWS S3] 模組，您必須擁有 [!DNL Amazon Web Service] 帳戶。

## Connect [!DNL AWS] 至 [!DNL Workfront Fusion] {#connect-aws-to-workfront-fusion}

若要連線 [!DNL AWS S3] 至 [!DNL Workfront Fusion] 您必須連線 [!DNL AWS] 帳戶至 [!DNL Workfront Fusion]. 若要這麼做，您首先需要在以下位置建立API使用者： [!DNL AWS] [!UICONTROL IAM].

1. 登入您的 [!DNL AWS] [!UICONTROL IAM] 帳戶。
1. 導覽至 **[!UICONTROL Identity and Access Management]** > **[!UICONTROL 存取管理]** > **[!UICONTROL 使用者]**.

1. 按一下 **[!UICONTROL 新增使用者]**.
1. 輸入新使用者的名稱，然後選取 **[!UICONTROL 程式化存取]** 中的選項 [!UICONTROL 存取型別] 區段。
1. 按一下 **[!UICONTROL 直接附加現有原則]**，然後搜尋 **[!UICONTROL AmazonS3FullAccess]** 在搜尋列中。 當它出現時，按一下它，然後按一下 **[!UICONTROL 下一個]**.

1. 繼續瀏覽其他對話方塊畫面，然後按一下 **[!UICONTROL 建立使用者]**.
1. 複製提供的 **[!UICONTROL 存取金鑰ID]** 和 **[!UICONTROL 秘密存取金鑰]**.

1. 前往 [!DNL Workfront Fusion] 並開啟 [!DNL AWS S3] 模組的 **[!UICONTROL 建立連線]** 對話方塊。
1. 輸入 [!UICONTROL 存取金鑰ID] 和 [!UICONTROL 秘密存取金鑰] 從步驟7至個別欄位，然後按一下 **[!UICONTROL 繼續]** 以建立連線。

已建立連線。 您可以繼續設定模組。

## [!DNL AWS S3] 模組及其欄位

當您設定 [!DNL AWS S3] 模組， [!DNL Workfront Fusion] 顯示下列欄位。 除了這些以外， [!DNL AWS S3] 視您在應用程式或服務中的存取層級等因素而定，可能會顯示欄位。 模組中的粗體標題表示必填欄位。

如果您在欄位或函式上方看到對應按鈕，則可以使用它來設定該欄位的變數和函式。 如需詳細資訊，請參閱 [將資訊從一個模組對應至中的另一個模組 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [動作](#actions)
* [搜尋](#searches)

### 動作

* [[!UICONTROL 建立貯體]](#create-bucket)
* [[!UICONTROL 取得檔案]](#get-file)
* [[!UICONTROL 上傳檔案]](#upload-file)
* [[!UICONTROL 進行API呼叫]](#make-an-api-call)

#### [!UICONTROL 建立貯體]

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[！UICONTROL連線] </td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL AWS] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-aws-to-workfront-fusion" class="MCXref xref">Connect [!DNL AWS] 至 [!DNL Workfront Fusion]</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL名稱] </td> 
   <td> <p>輸入新儲存貯體的名稱。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL區域] </td> 
   <td> <p>選取您的區域端點。 如需詳細資訊，請參閱 <a href="https://docs.aws.amazon.com/general/latest/gr/rande.html">區域端點</a> (位於AWS檔案中)。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 取得檔案]

從貯體下載檔案。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL連線] </td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL AWS] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-aws-to-workfront-fusion" class="MCXref xref">Connect [!DNL AWS] 至 [!DNL Workfront Fusion]</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL區域] </td> 
   <td> <p>選取您的區域端點。 如需詳細資訊，請參閱 <a href="https://docs.aws.amazon.com/general/latest/gr/rande.html">區域端點</a> 在 [!DNL AWS] 說明檔案。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL貯體] </td> 
   <td> <p>選取要從中下載檔案的儲存貯體。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL路徑]</p> </td> 
   <td> <p>輸入檔案的路徑。 範例: <code>/photos/2019/February/image023.jpg</code>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 上傳檔案]

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[！UICONTROL連線] </td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL AWS] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-aws-to-workfront-fusion" class="MCXref xref">Connect [!DNL AWS] 至 [!DNL Workfront Fusion]</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL區域] </td> 
   <td> <p>選取您的區域端點。 如需詳細資訊，請參閱 <a href="https://docs.aws.amazon.com/general/latest/gr/rande.html">區域端點</a> 在 [!DNL AWS] 說明檔案。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL資料夾] （選擇性） </p> </td> 
   <td> <p>指定您要上傳檔案的目標資料夾。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL來源檔案]</td> 
   <td> <p>從先前的模組中選取來源檔案，或對應來源檔案的名稱和資料。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Headers] （選用）</p> </td> 
   <td> <p> 插入請求標頭。 可用的標頭可在以下網址找到： <a href="https://docs.aws.amazon.com/AmazonS3/latest/API/API_PutObject.html">[!DNL AWS S3] 檔案 — [！UICONTROLPUT]物件</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 進行API呼叫]

如需 [!DNL Amazon S3] API，請參閱 [[!DNL Amazon S3] [!UICONTROL REST] API簡介](https://docs.aws.amazon.com/AmazonS3/latest/API/Welcome.html).

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL連線] </td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL AWS] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-aws-to-workfront-fusion" class="MCXref xref">Connect [!DNL AWS] 至 [!DNL Workfront Fusion]</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL區域] </td> 
   <td> <p>選取您的區域端點。 如需詳細資訊，請參閱 <a href="https://docs.aws.amazon.com/general/latest/gr/rande.html">區域端點</a> 在 [!DNL AWS] 說明檔案。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL URL]</td> 
   <td> <p>url輸入主機URL。 路徑必須相對於<code> https://s3.&lt;selected-region>.amazonaws.com/</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL方法]</td> 
   <td> <p>選取設定API呼叫所需的[！UICONTROL HTTP]要求方法。 如需詳細資訊，請參閱 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">中的[！UICONTROL HTTP]要求方法 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL標頭]</td> 
   <td> <p>新增請求標頭。 您可以使用以下常見請求標頭。 如需更多請求標頭，請參閱 <a href="https://docs.aws.amazon.com/AmazonS3/latest/API/RESTCommonRequestHeaders.html">[!DNL AWS S3] API檔案</a>.</p> <p>[!DNL Workfront Fusion] 自動新增授權標頭。</p> 
    <table style="table-layout:auto">
     <col> 
     <col> 
     <thead> 
      <tr> 
       <th>頁首名稱</th> 
       <th> <p> 說明</p> </th> 
      </tr> 
     </thead> 
     <tbody> 
      <tr> 
       <td role="rowheader"> <p>[！UICONTROL Content-Length]</p> </td> 
       <td> <p>根據RFC 2616的訊息長度（沒有標頭）。 載入XML的[！UICONTROLPUT]和作業（例如記錄和ACL）需要此標頭。</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[！UICONTROL Content-Type]</p> </td> 
       <td> <p>資源的內容型別，以備要求內容位於內文時使用。 範例: <code>text/plain</code>.</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[！UICONTROL Content-MD5]</p> </td> 
       <td> <p>根據RFC 1864，訊息的base64已編碼128位元MD5摘要（沒有標頭）。 此標頭可用作訊息完整性檢查，以確認資料與最初傳送的資料相同。 雖然這是選擇性的，但建議您使用[！UICONTROL Content-MD5]機製作為端對端的完整性檢查。 如需[！UICONTROL REST]要求驗證的詳細資訊，請前往 <a href="https://docs.aws.amazon.com/AmazonS3/latest/dev/RESTAuthentication.html?r=1821">[！UICONTROL REST]驗證</a> 在 <i>[!DNL Amazon] Simple Storage Service開發人員指南</i>.</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[！UICONTROL日期]</p> </td> 
       <td> <p>根據請求者的目前日期和時間。 範例: <code>Wed, 01 Mar 2006 12:00:00 GMT</code>. 當您指定 <code>Authorization </code>標頭，您必須指定 <code>x-amz-date</code> 或 <code>Date </code>標頭。</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[！UICONTROL Expect]</p> </td> 
       <td> <p>當您的應用程式使用[！UICONTROL 100-continue]時，它會在收到確認後才傳送要求內文。 如果郵件根據標頭被拒絕，則不會傳送郵件正文。 此標頭只有在傳送內文時才能使用。</p> <p>有效值： [！UICONTROL 100-continue]</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[！UICONTROL主機]</p> </td> 
       <td> <p>對於路徑樣式請求，值為 <code>s3.amazonaws.com</code>. 對於虛擬樣式請求，值為 <code>BucketName.s3.amazonaws.com</code>. 如需詳細資訊，請參閱 <a href="https://docs.aws.amazon.com/AmazonS3/latest/dev/VirtualHosting.html">虛擬託管</a> 在 <i>[!DNL Amazon] Simple Storage Service開發人員指南</i>.</p> <p>HTTP 1.1需要此標頭（大部分的Toolkit會自動新增此標頭）；HTTP/1.0要求則選填。</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[！UICONTROL x-amz-content-sha256]</p> </td> 
       <td> <p>使用簽名版本4驗證請求時，此標頭會提供請求承載的雜湊。 以區塊上傳物件時，將值設為 <code>STREAMING-AWS4-HMAC-SHA256-PAYLOAD</code> 以指出簽名僅涵蓋標題且沒有裝載。 如需詳細資訊，請參閱 <a href="https://docs.aws.amazon.com/AmazonS3/latest/API/sigv4-streaming.html">授權標頭的簽名計算：以多個區塊傳輸裝載（區塊上傳） ([!DNL AWS] 簽章第4版)</a>.</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[！UICONTROL x-amz-date]</p> </td> 
       <td> <p>根據請求者的目前日期和時間。 範例: <code>Wed, 01 Mar 2006 12:00:00 GMT</code>. 當您指定 <code>Authorization </code>標頭，您必須指定 <code>x-amz-date</code> 或 <code>Date </code>標頭。 如果您同時指定兩者，則為指定的值 <code>x-amz-date</code> 標題優先。</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[！UICONTROL x-amz-security-token]</p> </td> 
       <td> <p>此標頭可用於下列情況：</p> 
        <ul> 
         <li>提供安全性權杖 [!DNL Amazon DevPay] 作業。 使用的每個請求 [!DNL Amazon DevPay] 需要兩個 <code>x-amz-security-token</code> 標頭：一個用於產品權杖，一個用於使用者權杖。 時間 [!DNL Amazon S3] 會收到驗證過的要求，並將計算的簽章與提供的簽章進行比較。 不正確格式化用於計算簽名的多值標頭可能會導致驗證問題。</li> 
         <li>使用臨時安全性憑證時提供安全性權杖。 使用您從IAM取得的臨時安全性憑證提出請求時，您必須使用此標頭提供安全性權杖。 若要進一步瞭解臨時安全性認證，請前往提出請求。</li> 
        </ul> <p>使用的請求需要此標頭 [!DNL Amazon DevPay] 和使用臨時安全性憑證簽署的要求。</p> </td> 
      </tr> 
     </tbody> 
    </table> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL查詢字串]</td> 
   <td> <p>新增所需的查詢字串，例如引數或表單欄位。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL內文]</td> 
   <td> <p>以標準JSON物件的形式新增API呼叫的正文內容。</p> <p>備註:   <p>使用條件陳述式時，例如 <code>if</code> 在JSON中，將引號放在條件陳述式之外。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>">  
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

### 搜尋

* [[!UICONTROL 清單檔案]](#list-files)
* [[!UICONTROL 清單資料夾]](#list-folders)

#### [!UICONTROL 清單檔案]

傳回指定位置的檔案清單。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[！UICONTROL連線] </td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL AWS] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-aws-to-workfront-fusion" class="MCXref xref">Connect [!DNL AWS] 至 [!DNL Workfront Fusion]</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL區域] </td> 
   <td> <p>選取您的區域端點。 如需詳細資訊，請參閱 <a href="https://docs.aws.amazon.com/general/latest/gr/rande.html">區域端點</a> 在 [!DNL AWS] 說明檔案。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL貯體] </td> 
   <td> <p>選取 [!DNL Amazon S3] 要搜尋檔案的儲存貯體。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL首碼] （選擇性）</p> </td> 
   <td> <p> 要在其中查閱檔案的資料夾路徑，例如： <code>workfrontfusion/work.</code></p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 清單資料夾]

從指定位置傳回資料夾清單。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[！UICONTROL連線] </td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL AWS] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-aws-to-workfront-fusion" class="MCXref xref">Connect [!DNL AWS] 至 [!DNL Workfront Fusion]</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL區域] </td> 
   <td> <p>選取您的區域端點。 如需詳細資訊，請參閱 <a href="https://docs.aws.amazon.com/general/latest/gr/rande.html">區域端點</a> (位於AWS檔案中)。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL貯體] </td> 
   <td> <p>選取 [!DNL Amazon S3] 要搜尋資料夾的儲存貯體。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL首碼] （選擇性）</p> </td> 
   <td> <p> 要在其中查閱資料夾的資料夾路徑，例如： <code>workfrontfusion/work.</code></p> </td> 
  </tr> 
 </tbody> 
</table>
