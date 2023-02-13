---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 連接器
navigation-topic: apps-and-their-modules
title: AWS S3模組
description: 此 [!DNL Adobe Workfront Fusion AWS] S3模組可讓您對S3儲存貯體執行作業。
author: Becky
feature: Workfront Fusion
exl-id: 33623b5d-d9ff-4d41-b938-33378f50539e
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1381'
ht-degree: 0%

---

# AWS S3模組

此 [!DNL Adobe Workfront Fusion AWS] S3模組可讓您對S3儲存貯體執行作業。

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] （工作自動化和整合） </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>貴組織必須購買 [!DNL Adobe Workfront Fusion] 和 [!DNL Adobe Workfront] 以使用本文所述的功能。</td> 
  </tr> 
 </tbody> 
</table>

若要了解您擁有的計畫、授權類型或存取權，請聯絡您的 [!DNL Workfront] 管理員。

如需 [!DNL Adobe Workfront Fusion] 許可證，請參閱 [[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 必要條件

使用 [!UICONTROL AWS S3] 模組，您必須 [!DNL Amazon Web Service] 帳戶。

## Connect [!DNL AWS] to [!DNL Workfront Fusion] {#connect-aws-to-workfront-fusion}

連接 [!DNL AWS S3] to [!DNL Workfront Fusion] 您必須連接 [!DNL AWS] 帳戶 [!DNL Workfront Fusion]. 若要這麼做，您必須先在 [!DNL AWS] [!UICONTROL IAM].

1. 登入 [!DNL AWS] [!UICONTROL IAM] 帳戶。
1. 導覽至 **[!UICONTROL 身分與存取管理]** > **[!UICONTROL 存取管理]** > **[!UICONTROL 使用者]**.

1. 按一下 **[!UICONTROL 添加用戶]**.
1. 輸入新用戶的名稱並選擇 **[!UICONTROL 程式存取]** 選項 [!UICONTROL 存取類型] 區段。
1. 按一下 **[!UICONTROL 直接附加現有策略]**，然後搜尋 **[!UICONTROL AmazonS3FullAccess]** 的下一頁。 出現時按一下，然後按一下 **[!UICONTROL 下一個]**.

1. 繼續瀏覽其他對話方塊畫面，然後按一下 **[!UICONTROL 建立使用者]**.
1. 複製提供的 **[!UICONTROL 訪問密鑰ID]** 和 **[!UICONTROL 秘密訪問密鑰]**.

1. 前往 [!DNL Workfront Fusion] 然後開啟 [!DNL AWS S3] 模組 **[!UICONTROL 建立連線]** 對話框。
1. 輸入 [!UICONTROL 訪問密鑰ID] 和 [!UICONTROL 秘密訪問密鑰] 從步驟7到個別欄位，然後按一下 **[!UICONTROL 繼續]** 建立連接。

已建立連接。 您可以繼續設定模組。

## [!DNL AWS S3] 模組及其欄位

設定時 [!DNL AWS S3] 模組， [!DNL Workfront Fusion] 顯示下列欄位。 此外， [!DNL AWS S3] 視您在應用程式或服務中的存取層級等因素而定，可能會顯示欄位。 模組中的粗體標題表示必填欄位。

如果您在欄位或函式上方看到對應按鈕，則可使用它來設定該欄位的變數和函式。 如需詳細資訊，請參閱 [將資訊從一個模組對應到 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

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
    <td role="rowheader">[!UICONTROL連接] </td> 
   <td> <p>有關連接 [!DNL AWS] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-aws-to-workfront-fusion" class="MCXref xref">Connect [!DNL AWS] to [!DNL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL名稱] </td> 
   <td> <p>輸入新貯體的名稱。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL地區] </td> 
   <td> <p>選取您的地區端點。 如需詳細資訊，請參閱 <a href="https://docs.aws.amazon.com/general/latest/gr/rande.html">地區端點</a> 在AWS檔案中。</p> </td> 
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
   <td role="rowheader">[!UICONTROL連接] </td> 
   <td> <p>有關連接 [!DNL AWS] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-aws-to-workfront-fusion" class="MCXref xref">Connect [!DNL AWS] to [!DNL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL地區] </td> 
   <td> <p>選取您的地區端點。 如需詳細資訊，請參閱 <a href="https://docs.aws.amazon.com/general/latest/gr/rande.html">地區端點</a> 在 [!DNL AWS] 檔案。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL儲存貯體] </td> 
   <td> <p>選取您要從中下載檔案的貯體。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL路徑]</p> </td> 
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
    <td role="rowheader">[!UICONTROL連接] </td> 
   <td> <p>有關連接 [!DNL AWS] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-aws-to-workfront-fusion" class="MCXref xref">Connect [!DNL AWS] to [!DNL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL地區] </td> 
   <td> <p>選取您的地區端點。 如需詳細資訊，請參閱 <a href="https://docs.aws.amazon.com/general/latest/gr/rande.html">地區端點</a> 在 [!DNL AWS] 檔案。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL資料夾]（可選） </p> </td> 
   <td> <p>指定要將檔案上傳到的目標資料夾。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL源檔案]</td> 
   <td> <p>從上一個模組中選擇源檔案，或映射源檔案的名稱和資料。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL標題]（可選）</p> </td> 
   <td> <p> 插入請求標題。 可在 <a href="https://docs.aws.amazon.com/AmazonS3/latest/API/API_PutObject.html">[!DNL AWS S3] 文檔 — [!UICONTROLPUT]對象</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 進行API呼叫]

有關 [!DNL Amazon S3] API，請參閱 [[!DNL Amazon S3] [!UICONTROL REST] API簡介](https://docs.aws.amazon.com/AmazonS3/latest/API/Welcome.html).

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL連接] </td> 
   <td> <p>有關連接 [!DNL AWS] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-aws-to-workfront-fusion" class="MCXref xref">Connect [!DNL AWS] to [!DNL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL地區] </td> 
   <td> <p>選取您的地區端點。 如需詳細資訊，請參閱 <a href="https://docs.aws.amazon.com/general/latest/gr/rande.html">地區端點</a> 在 [!DNL AWS] 檔案。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL URL]</td> 
   <td> <p>URL輸入主機URL。 路徑必須相對於<code> https://s3.&lt;selected-region>.amazonaws.com/</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL方法]</td> 
   <td> <p>選取設定API呼叫所需的[!UICONTROL HTTP]要求方法。 如需詳細資訊，請參閱 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">中的[!UICONTROL HTTP]要求方法 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL標題]</td> 
   <td> <p>新增請求標題。 您可以使用下列通用請求標題。 如需更多請求標題，請參閱 <a href="https://docs.aws.amazon.com/AmazonS3/latest/API/RESTCommonRequestHeaders.html">[!DNL AWS S3] API檔案</a>.</p> <p>[!DNL Workfront Fusion] 自動添加授權標頭。</p> 
    <table style="table-layout:auto">
     <col> 
     <col> 
     <thead> 
      <tr> 
       <th>標題名稱</th> 
       <th> <p> 說明</p> </th> 
      </tr> 
     </thead> 
     <tbody> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL Content-Length]</p> </td> 
       <td> <p>根據RFC 2616的消息長度（不含標頭）。 [!UICONTROLPUT]和載入XML的操作（如日誌和ACL）需要此標頭。</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL Content-Type]</p> </td> 
       <td> <p>資源的內容類型（若要求內容位於內文中）。 範例: <code>text/plain</code>.</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL Content-MD5]</p> </td> 
       <td> <p>base64根據RFC 1864對消息的128位MD5摘要（沒有標頭）進行編碼。 此標題可用作消息完整性檢查，以驗證資料與最初發送的資料相同。 雖然這是選用的，但建議您使用[!UICONTROL Content-MD5]機製作為端對端完整性檢查。 如需[!UICONTROL REST]要求驗證的詳細資訊，請前往 <a href="https://docs.aws.amazon.com/AmazonS3/latest/dev/RESTAuthentication.html?r=1821">[!UICONTROL REST]驗證</a> 在 <i>[!DNL Amazon] 《簡單儲存服務開發人員指南》</i>.</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL日期]</p> </td> 
       <td> <p>根據請求者的當前日期和時間。 範例: <code>Wed, 01 Mar 2006 12:00:00 GMT</code>. 當您指定 <code>Authorization </code>標題，您必須指定 <code>x-amz-date</code> 或 <code>Date </code>頁首。</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL預期]</p> </td> 
       <td> <p>當您的應用程式使用[!UICONTROL 100-continue]時，在收到確認訊息之前，它不會傳送要求內文。 如果根據標題拒絕訊息，則不會傳送訊息的內文。 只有在傳送內文時，才能使用此標題。</p> <p>有效值：[!UICONTROL 100-continue]</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL主機]</p> </td> 
       <td> <p>若為路徑樣式請求，值為 <code>s3.amazonaws.com</code>. 對於虛擬樣式的請求，值為 <code>BucketName.s3.amazonaws.com</code>. 如需詳細資訊，請參閱 <a href="https://docs.aws.amazon.com/AmazonS3/latest/dev/VirtualHosting.html">虛擬托管</a> 在 <i>[!DNL Amazon] 《簡單儲存服務開發人員指南》</i>.</p> <p>HTTP 1.1需要此標題（大多數工具包都自動添加此標題）;選用於HTTP/1.0要求。</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL x-amz-content-sha256]</p> </td> 
       <td> <p>使用簽名版本4驗證請求時，此標題提供請求裝載的雜湊。 以區塊上傳物件時，請將值設為 <code>STREAMING-AWS4-HMAC-SHA256-PAYLOAD</code> 以指出簽名僅涵蓋標題且沒有裝載。 如需詳細資訊，請參閱 <a href="https://docs.aws.amazon.com/AmazonS3/latest/API/sigv4-streaming.html">授權標頭的簽名計算：以多個區塊傳輸裝載（區塊上傳）([!DNL AWS] 簽名版本4)</a>.</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL x-amz-date]</p> </td> 
       <td> <p>根據請求者的當前日期和時間。 範例: <code>Wed, 01 Mar 2006 12:00:00 GMT</code>. 當您指定 <code>Authorization </code>標題，您必須指定 <code>x-amz-date</code> 或 <code>Date </code>頁首。 若同時指定，則為 <code>x-amz-date</code> 標題優先。</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL x-amz-security-token]</p> </td> 
       <td> <p>此標題可用於下列案例：</p> 
        <ul> 
         <li>為提供安全令牌 [!DNL Amazon DevPay] 操作。 使用 [!DNL Amazon DevPay] 需要兩個 <code>x-amz-security-token</code> 標題：一個用於產品代號，另一個用於使用者代號。 當 [!DNL Amazon S3] 接收經驗證的請求，將計算的簽名與提供的簽名進行比較。 用於計算簽名的格式不正確的多值標題可能會導致身份驗證問題。</li> 
         <li>使用臨時安全憑證時提供安全權杖。 使用從IAM獲取的臨時安全憑據發出請求時，必須使用此標頭提供安全令牌。 若要進一步了解暫時安全性憑證，請前往Making Requests。</li> 
        </ul> <p>若要使用 [!DNL Amazon DevPay] 和使用臨時安全憑據簽名的請求。</p> </td> 
      </tr> 
     </tbody> 
    </table> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL查詢字串]</td> 
   <td> <p>新增所需的查詢字串，例如參數或表單欄位。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL正文]</td> 
   <td> <p>以標準JSON物件的形式新增API呼叫的內文內容。</p> <p>備註:   <p>使用條件陳述式時，例如 <code>if</code> 在JSON中，將引號放在條件陳述式之外。</p> 
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

從指定位置返回檔案清單。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL連接] </td> 
   <td> <p>有關連接 [!DNL AWS] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-aws-to-workfront-fusion" class="MCXref xref">Connect [!DNL AWS] to [!DNL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL地區] </td> 
   <td> <p>選取您的地區端點。 如需詳細資訊，請參閱 <a href="https://docs.aws.amazon.com/general/latest/gr/rande.html">地區端點</a> 在 [!DNL AWS] 檔案。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL儲存貯體] </td> 
   <td> <p>選取 [!DNL Amazon S3] 儲存器，您要搜尋檔案。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL前置詞]（可選）</p> </td> 
   <td> <p> 要在中查找檔案的資料夾路徑，例如 <code>workfrontfusion/work.</code></p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 清單資料夾]

從指定位置返回資料夾清單。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL連接] </td> 
   <td> <p>有關連接 [!DNL AWS] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-aws-to-workfront-fusion" class="MCXref xref">Connect [!DNL AWS] to [!DNL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL地區] </td> 
   <td> <p>選取您的地區端點。 如需詳細資訊，請參閱 <a href="https://docs.aws.amazon.com/general/latest/gr/rande.html">地區端點</a> 在AWS檔案中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL儲存貯體] </td> 
   <td> <p>選取 [!DNL Amazon S3] 儲存貯體，以搜尋資料夾。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL前置詞]（可選）</p> </td> 
   <td> <p> 要在中查找資料夾的資料夾路徑，例如 <code>workfrontfusion/work.</code></p> </td> 
  </tr> 
 </tbody> 
</table>
