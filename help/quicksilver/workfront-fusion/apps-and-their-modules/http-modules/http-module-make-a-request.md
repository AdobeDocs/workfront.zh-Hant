---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 聯結器
navigation-topic: http-modules
title: HTTP &gt；建立請求模組
description: Adobe Workfront Fusion HTTP &gt；發出請求模組是一個通用模組，可讓您設定HTTP請求並將其提交至伺服器。 接收的HTTP回應隨後會包含在輸出套件組合中。
author: Becky
feature: Workfront Fusion
exl-id: 7857c395-ce84-480e-8fa2-065035ac5b95
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1006'
ht-degree: 0%

---

# [!UICONTROL HTTP] >[!UICONTROL 提出要求] 模組

>[!NOTE]
>
>Adobe Workfront Fusion需要 [!DNL Adobe Workfront Fusion] 除了授權外， [!DNL Adobe Workfront] 授權。

此 [!DNL Adobe Workfront Fusion] [!UICONTROL HTTP] > [!UICONTROL 建立請求模組] 是一個通用模組，可讓您設定HTTP請求並將其提交至伺服器。 接收的HTTP回應隨後會包含在輸出套件組合中。

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

有關以下專案的資訊： [!DNL Adobe Workfront Fusion] 授權，請參閱 [Adobe Workfront Fusion授權](../../../workfront-fusion/get-started/license-automation-vs-integration.md)

## [!UICONTROL HTTP] >[!UICONTROL 提出要求] 模組設定

當您設定 [!UICONTROL HTTP] >[!UICONTROL 提出要求] 模組， [!DNL Adobe Workfront Fusion] 顯示下列欄位。 模組中的粗體標題表示必填欄位。

如果您在欄位或函式上方看到對應按鈕，則可以使用它來設定該欄位的變數和函式。 如需詳細資訊，請參閱 [將資訊從一個模組對應至中的另一個模組 [!DNL Adobe Workfront Fusion]](../../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL將所有狀態評估為錯誤（2xx和3xx除外）] </td> 
   <td> <p>使用此選項可設定錯誤處理。</p> <p>如需詳細資訊，請參閱 <a href="../../../workfront-fusion/errors/error-handling.md" class="MCXref xref">中的錯誤處理 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL URL] </td> 
   <td> <p>輸入您要傳送請求的URL，例如API端點、網站等。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL方法]</p> </td> 
   <td> <p>選取設定API呼叫所需的HTTP要求方法。 如需詳細資訊，請參閱 <a href="../../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">中的HTTP要求方法 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL標頭] </td> 
   <td> <p>以標準JSON物件的形式新增請求的標頭。例如， <code>{"Content-type":"application/json"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL查詢字串]</td> 
   <td> <p> 輸入所需的查詢索引鍵值配對。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL主體型別]</p> </td> 
   <td> <p>HTTP內文是HTTP交易訊息中傳輸的資料位元組，緊接在標題之後（如果有任何要使用的話）。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL Raw]</strong> </p> <p>Raw內文型別通常適用於大多數HTTP內文要求，即使開發人員檔案未指定要傳送的資料亦然。</p> <p>在[！UICONTROL內容型別]欄位中指定剖析資料的表單。</p> <p>儘管選取了內容型別，但資料仍會以開發人員檔案規定或要求的任何格式輸入。</p> </li> 
     <li> <p><strong>[！UICONTROL Application/x-www-form-urlencoded]</strong> </p> <p>此內文型別會使用以下專案來POST[！UICONTROL]資料： <code>[!UICONTROL application/x-www-form-urlencoded]</code>.</p> <p>對象 <code>application/x-www-form-urlencoded</code>，傳送至伺服器的HTTP訊息內文基本上是一個查詢字串。 索引鍵和值會以索引鍵/值組編碼，並以以下方式分隔 <code>&amp;</code> 和 <code>=</code> 介於鍵和值之間。 </p> <p>若為二進位資料，請使用 <code>[!UICONTROL multipart/form-data]</code> 而非。</p> 
      <div class="example" data-mc-autonum="<b>Example: </b>">
       <span class="autonumber"><span><b>範例: </b></span></span> 
       <p>產生的HTTP要求格式範例：</p> 
       <p><code>field1=value1&amp;field2=value2</code> </p> 
      </div> </li> 
     <li> <p><strong>[！UICONTROL Multipart/form-data]</strong> </p> <p>[！UICONTROL Multipart/form-data]是用於傳送檔案和資料的HTTP多部分要求。 它通常用於將檔案上傳到伺服器。</p> <p>新增要在請求中傳送的欄位。 每個欄位都必須包含索引鍵/值組。</p> 
      <ul> 
       <li> <p><strong>[！UICONTROL文字]</strong> </p> <p>輸入要在要求內文中傳送的索引鍵和值。</p> </li> 
       <li> <p><strong>[！UICONTROL檔案]</strong> </p> <p>輸入金鑰，並指定您要在要求內文中傳送的來源檔案。</p> <p>對應您要從上一個模組上傳的檔案(例如[！UICONTROL HTTP] &gt;[！UICONTROL Get a File]或[！UICONTROL Google Drive] &gt;[！UICONTROL Download a File)]，或手動輸入檔案名稱和檔案資料。</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL剖析回應]</p> </td> 
   <td> <p>啟用此選項可自動剖析回應並轉換JSON和XML回應，因此您不需要使用[！UICONTROL JSON] &gt; [！UICONTROL Parse JSON]或[！UICONTROL XML] &gt; [！UICONTROL Parse XML]模組。</p> <p>在使用剖析的JSON或XML內容之前，請先手動執行一次模組，讓模組可以識別回應內容，並允許您將其對應到後續模組中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL使用者名稱]</p> </td> 
   <td> <p> 如果您要使用基本授權傳送請求，請輸入使用者名稱。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL密碼] </td> 
   <td> <p>如果要使用基本授權傳送請求，請輸入密碼。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL逾時] </td> 
   <td> <p>以秒為單位指定請求逾時(1-300)。 預設值為40秒。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL與其他HTTP模組共用Cookie]</td> 
   <td> <p> 啟用此選項即可將伺服器的Cookie與您情境中的所有HTTP模組共用。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL自我簽署憑證]</td> 
   <td> <p> 如果您想要使用自我簽署憑證的TLS，請上傳憑證。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL拒絕使用未驗證（自我簽署）憑證的連線] </td> 
   <td> <p>啟用此選項可拒絕使用未驗證TLS憑證的連線。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL遵循重新導向]</td> 
   <td> <p> 啟用此選項可在URL重新導向之後附帶3xx回應。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL遵循所有重新導向] </td> 
   <td> <p>啟用此選項後，URL會重新導向並帶有所有回應代碼。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL停用將多個相同的查詢字串索引鍵序列化為陣列]</p> </td> 
   <td> <p>依預設， [!DNL Workfront Fusion] 處理作為陣列的同一URL查詢字串引數索引鍵的多個值。 例如， <code>www.test.com?foo=bar&amp;foo=baz</code> 將轉換為 <code>www.test.com?foo[0]=bar&amp;foo[1]=baz</code>. 啟動此選項以停用此功能。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL要求壓縮內容]</td> 
   <td> <p> 啟用此選項可請求網站的壓縮版本。</p> <p>新增 <code>[!UICONTROL Accept-Encoding]</code> 標頭以請求壓縮內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL使用雙向TLS]</td> 
   <td> <p>啟用此選項可在HTTP請求中使用雙向TLS。</p> <p>如需雙向TLS的詳細資訊，請參閱 <a href="../../../workfront-fusion/apps-and-their-modules/http-modules/use-mtls-in-http-modules.md" class="MCXref xref">在HTTP模組中使用雙向TLS [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**範例：** 此範例說明如何設定模組以提交 [!UICONTROL POST] 具有JSON裝載的要求：
>
>![](assets/make-a-request-example-350x522.png)

>[!NOTE]
>
>若要確認您的 [!UICONTROL JSON] 有效，您可以使用下列任一可用的線上服務： [https://jsonlint.com/](https://jsonlint.com/). 您也可以使用 [!UICONTROL JSON] >[!UICONTROL 建立JSON模組] 以動態方式建立JSON並處理所有必要的逸出。
>
>將JSON片段與運算式及專案直接混合在 [!UICONTROL 要求內容] 不建議使用欄位，因為它可能會導致無效的JSON。
