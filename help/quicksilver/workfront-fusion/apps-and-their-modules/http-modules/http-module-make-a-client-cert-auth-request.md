---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 連接器
navigation-topic: http-modules
title: HTTP &gt;建立客戶端證書授權請求模組
description: 此 [!DNL Adobe Workfront Fusion] 模組可讓您使用HTTP用戶端憑證授權來設定HTTP要求，並將其提交至伺服器。 接著，接收的HTTP回應便包含在輸出套件中。
author: Becky
feature: Workfront Fusion
exl-id: c0b0057f-3db0-4c10-a274-ebaec1a5b87b
source-git-commit: 58db2129dd764d24b0a681735c2405be402d8b43
workflow-type: tm+mt
source-wordcount: '878'
ht-degree: 0%

---

# HTTP >[!UICONTROL 提出客戶端證書授權請求] 模組

>[!NOTE]
>
>Adobe Workfront Fusion需要 [!DNL Adobe Workfront Fusion] 授權，以及Adobe Workfront授權。

此 [!DNL Adobe Workfront Fusion] 模組可讓您使用HTTP用戶端憑證授權來設定HTTP要求，並將其提交至伺服器。 接著，接收的HTTP回應便包含在輸出套件中。

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

## [!UICONTROL HTTP] >[!UICONTROL 提出客戶端證書授權請求] 模組配置

當您設定 [!UICONTROL HTTP] >[!UICONTROL 提出客戶端證書授權請求] 模組， [!DNL Adobe Workfront Fusion] 顯示下列欄位。 模組中的粗體標題表示必填欄位。

如果您在欄位或函式上方看到對應按鈕，則可使用它來設定該欄位的變數和函式。 如需詳細資訊，請參閱 [將資訊從一個模組對應到 [!DNL Adobe Workfront Fusion]](../../../workfront-fusion/mapping/map-information-between-modules.md).

<img src="assets/map-toggle-350x74.png" style="width: 350;height: 74;" data-mc-conditions="QuicksilverOrClassic.Draft mode">

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL憑據]</td> 
   <td> <p>選擇包含客戶端證書身份驗證憑據的密鑰，或按一下 <strong>[!UICONTROL添加]</strong> 將憑據添加到新密鑰中。 </p> <p>注意：您可以新增更多憑證，以便輕鬆在每個連線之間切換。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL將所有狀態評估為錯誤（2xx和3xx除外）] </td> 
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
     <li> <p><strong>[!UICONTROL Raw]</strong> </p> <p>原始內文類型通常適用於大部分HTTP內文要求，即使在開發人員檔案未指定要傳送的資料的情況下亦然。</p> <p>在[!UICONTROL內容類型]欄位中指定解析資料的形式。</p> <p>儘管選取了內容類型，模組仍會以開發人員檔案所規定或要求的任何格式輸入資料。</p> </li> 
     <li> <p><strong>[!UICONTROL Application/x-www-form-urlencoded]</strong> </p> <p>此內文類型是用於[!UICONTROLPOST]資料，使用 <code>application/x-www-form-urlencoded</code>.</p> <p>針對 <code>[!UICONTROL application/x-www-form-urlencoded]</code>，則傳送至伺服器的HTTP訊息內文基本上是一個查詢字串。 索引鍵和值會以由 <code>&amp;</code> 和 <code>=</code> 在索引鍵和值之間。 </p> <p>對於二進位資料，請使用 <code>[!UICONTROL multipart/form-data]</code> 。</p> 
      <div class="example" data-mc-autonum="<b>Example: </b>">
       <span class="autonumber"><span><b>範例: </b></span></span> 
       <p>產生的HTTP要求格式範例：</p> 
       <p><code>field1=value1&amp;field2=value2</code> </p> 
      </div> </li> 
     <li> <p><strong>[!UICONTROL多部分/表單資料]</strong> </p> <p>[!UICONTROL Multipart/form-data]是用於傳送檔案和資料的HTTP多部分請求。 它通常用於將檔案上傳至伺服器。</p> <p>新增要在請求中傳送的欄位。 每個欄位都必須包含索引鍵值組。</p> 
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
   <td> <p>以秒為單位指定請求逾時(1-300)。 預設為40秒。</p> </td> 
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
   <td> <p> 啟用此選項可要求壓縮版本的網站。</p> <p>新增 <code>[!UICONTROL Accept-Encoding]</code> 要求壓縮內容的標題。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL使用相互TLS]</td> 
   <td> <p>啟用此選項，可在HTTP要求中使用相互TLS。</p> <p>如需相互TLS的詳細資訊，請參閱 <a href="../../../workfront-fusion/apps-and-their-modules/http-modules/use-mtls-in-http-modules.md" class="MCXref xref">在的HTTP模組中使用相互TLS [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
