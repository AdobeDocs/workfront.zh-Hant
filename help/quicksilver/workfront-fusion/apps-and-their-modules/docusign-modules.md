---
title: DocuSign模組
description: 此 [!DNL Adobe Workfront Fusion DocuSign] 模組可讓您監視和檢索信封狀態、搜索和檢索信封，或下載併發送文檔以登錄 [!DNL DocuSign] 帳戶。
author: Becky
draft: Probably
feature: Workfront Fusion, Digital Content and Documents
exl-id: a6ebfe6f-dc3f-41f7-8129-bbc5775cff33
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1911'
ht-degree: 0%

---

# DocuSign模組

此 [!DNL Adobe Workfront Fusion] [!DNL DocuSign] 模組可讓您監視和檢索信封狀態、搜索和檢索信封，或下載併發送文檔以登錄 [!DNL DocuSign] 帳戶。

如果您需要建立案例的相關指示，請參閱 [在中建立案例 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

如需模組的相關資訊，請參閱 [中的模組 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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

使用 [!DNL DocuSign] 模組，您必須 [!DNL DocuSign] 帳戶。

## Connect [!DNL DocuSign] to [!DNL Workfront Fusion] {#connect-docusign-to-workfront-fusion}

為 [!DNL DocuSign] 模組：

1. 按一下 **[!UICONTROL 新增]** 旁邊 [!UICONTROL 連線] 框 [!DNL DocuSign] 模組。
1. 輸入下列內容：

<table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL連接名]</p> </td> 
      <td>輸入新名稱 [!DNL DocuSign] 連接</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL帳戶類型]</td> 
      <td>選取您要連線的帳戶是生產帳戶還是示範帳戶。</td> 
     </tr> 
    </tbody> 
   </table>

1. 繼續，如 [建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示](../../workfront-fusion/connections/connect-to-fusion-general.md#connect).

## [!DNL DocuSign] 模組及其欄位

設定時 [!DNL DocuSign] 模組， [!DNL Workfront Fusion] 顯示下列欄位。 此外， [!DNL DocuSign] 視您在應用程式或服務中的存取層級等因素而定，可能會顯示欄位。 模組中的粗體標題表示必填欄位。

如果您在欄位或函式上方看到對應按鈕，則可使用它來設定該欄位的變數和函式。 如需詳細資訊，請參閱 [將資訊從一個模組對應到 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [觸發器](#triggers)
* [動作](#actions)

### 觸發器

#### [!UICONTROL 監視信封]

此觸發模組會在信封被發送、傳送、簽名、完成或拒絕時啟動案例。

<table style="table-layout:auto">
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接] </td> 
   <td> <p>有關連接 [!DNL DocuSign] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連接到 [!DNL Workfront Fusion]</a> 在文章中 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在中建立案例 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL帳戶] </td> 
   <td> <p>選擇包含要監視的記錄的帳戶。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL事件類型]</td> 
   <td> <p> 選取您要監看的事件類型。</p> 
    <ul> 
     <li>[!UICONTROL文檔已完成]</li> 
     <li>[!UICONTROL文檔已拒絕]</li> 
     <li>[!UICONTROL已發送文檔]</li> 
     <li>[!UICONTROL文檔已簽名]</li> 
     <li>[!UICONTROL收件箱中的新文檔]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL輸出欄位]</p> </td> 
   <td> <p>選取您要納入模組輸出的欄位。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL限制]</td> 
   <td>輸入或映射在每個方案執行週期中希望模組使用的最大記錄數。</td> 
  </tr> 
 </tbody> 
</table>

### 動作

* [[!UICONTROL 自訂API呼叫]](#custom-api-call)
* [[!UICONTROL 下載檔案]](#download-a-document)
* [[!UICONTROL 閱讀信封]](#read-an-envelope)
* [[!UICONTROL 將檔案上傳至信封]](#upload-a-file-to-an-envelope)
* [[!UICONTROL 建立新信封]](#create-a-new-envelope)
* [[!UICONTROL 將收件者添加到信封]](#add-recipient-to-envelope)
* [[!UICONTROL 新增自訂欄位]](#add-custom-field)
* [[!UICONTROL 修改自訂欄位]](#modify-custom-field)
* [[!UICONTROL 發送信封]](#send-envelope)

#### [!UICONTROL 自訂API呼叫]

此動作模組可讓您執行自訂API呼叫。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL DocuSign] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-docusign-to-workfront-fusion" class="MCXref xref">Connect [!DNL DocuSign] to [!DNL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL帳戶]</td> 
   <td>輸入或對應您要用來存取的帳戶 [!DNL DocuSign] API。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL URL]</td> 
   <td> <p>在Web伺服器上輸入您要模組與之互動的地址。</p> <p>您可以輸入相對URL，這表示您不需要包含通訊協定(例如 <code>http://</code>)。 這向Web伺服器建議，正在伺服器上進行互動。</p> <p>例如： <code>[!DNL /api/conversations].create</code></p> <p>提示：如需可用端點的清單，請參閱 <a href="https://developers.docusign.com/esign-rest-api/reference">[!DNL DocuSign] API參考</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL方法]</td> 
   td&gt; <p>選取設定API呼叫所需的HTTP要求方法。 如需詳細資訊，請參閱 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">中的HTTP要求方法 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL標題]</td> 
   <td> <p>以標準JSON物件的形式新增請求的標題。 這會決定請求的內容類型。</p> <p>例如，<code> {"Content-type":"application/json"}</code></p> <p>注意：如果您收到錯誤，且很難判斷其來源，請考慮根據 [!DNL Workfront] 檔案。 如果您的自訂API呼叫傳回422 HTTP要求錯誤，請嘗試使用「Content-Type」：「text/plain」標題。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL查詢字串]</td> 
   <td> <p>以標準JSON物件的形式新增API呼叫的查詢。</p> <p>例如： <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL正文]</td> 
   <td> <p>以標準JSON物件的形式新增API呼叫的內文內容。</p> <p>備註:  <p>使用條件陳述式時，例如 <code>if</code> 在JSON中，將引號放在條件陳述式之外。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL限制]</td> 
   <td>輸入或映射在一個執行週期中要處理的結果的最大數量。</td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**範例：** 清單信封
>
>下列API呼叫會從您 [!DNL DocuSign] 帳戶：
>
>**URL**: `/v2.1/accounts/{accountId}/envelopes/`
>
>**方法**: `GET`
>
>**查詢字串**:
>
>* **金鑰**: `from_date`
>
>* **值**: `YYYY-MM-DD`
>
>指定請求何時開始檢查帳戶中信封的狀態更改。
>
>![](assets/example-docusign-setup-350x770.png)
>
>結果可在模組的「輸出」(Output)下的「捆綁」(Bundle)>「主體」(Body)>「包絡」(envoputes)下找到。
>
>在我們的示例中，返回了6個信封：
>
>![](assets/docusign-example-output-350x677.png)

#### [!UICONTROL 下載檔案]

此動作模組會下載單一檔案。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL DocuSign] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-docusign-to-workfront-fusion" class="MCXref xref">Connect [!DNL DocuSign] to [!DNL Workfront Fusion]</a> 這篇文章。</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL帳戶] </td> 
   <td> <p>選擇包含要下載的文檔的帳戶。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL信封ID]</td> 
   <td> <p> 輸入或映射要下載的信封的ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL文檔ID]</p> </td> 
   <td> <p>輸入或映射要下載的文檔的ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL證書]</td> 
   <td>選擇 <strong>[!UICONTROL是]</strong> 如果要在下載中包含信封簽名證書。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL文檔（按用戶ID）]</td> 
   <td>選擇 <strong>[!UICONTROL是]</strong> 如果要允許收件者按用戶ID檢索文檔。 例如，如果用戶被包含在兩個具有不同可見性的不同工藝路線訂單中，則使用此選項將返回兩個工藝路線中的所有文檔。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Encrypt]</td> 
   <td>選擇 <strong>[!UICONTROL是]</strong> 如果希望對響應中返回的PDF位元組進行加密，以便對配置在您的 [!DNL DocuSign] 帳戶。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL語言]</td> 
   <td>選取語言。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL顯示更改]</td> 
   <td>設為時 <strong>[!UICONTROL是]</strong>，傳回PDF的任何已變更欄位都會以黃色強調顯示，而選用簽名或縮寫會以紅色列出。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL水印]</td> 
   <td> <p>選擇 <strong>[!UICONTROL否]</strong> 從PDF文檔中刪除水印。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 閱讀信封]

此動作模組會讀取 [!DNL DocuSign] 使用信封ID。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL DocuSign] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-docusign-to-workfront-fusion" class="MCXref xref">Connect [!DNL DocuSign] to [!DNL Workfront Fusion]</a> 這篇文章。</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL帳戶] </td> 
   <td> <p>選擇包含要從中讀取資訊的文檔的帳戶。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL信封ID]</td> 
   <td> <p> 輸入或映射ID，該ID包含要從中讀取資訊的文檔。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL輸出]</td> 
   <td>選取您要在模組輸出中顯示的屬性。 </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 將檔案上傳至信封]

此模組將指定的檔案上載到DocuSign中的現有信封。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL DocuSign] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-docusign-to-workfront-fusion" class="MCXref xref">Connect [!DNL DocuSign] to [!DNL Workfront Fusion]</a> 這篇文章。</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL帳戶] </td> 
   <td> <p>選擇包含要上載檔案的信封的帳戶。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL信封ID]</td> 
   <td> <p> 輸入或映射要上載檔案的信封的ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL源檔案]</td> 
   <td>從上一個模組中選擇源檔案，或輸入源檔案的名稱和資料。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 建立新信封]

此操作模組從模板建立新信封。 它返回新信封的ID以及新信封的狀態。

<table style="table-layout:auto">
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL連接] </td>

<td> <p>如需將DocuSign帳戶連接至Workfront Fusion的指示，請參閱 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連接到Workfront Fusion</a> 在文章中 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在Adobe Workfront Fusion中建立案例</a>.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader">[!UICONTROL帳戶] </td>
   <td> <p>選擇包含要上載檔案的信封的帳戶。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL模板]</td>
   <td> <p> 選取要從中建立新包絡的模板。 範本是根據您選取的[!UICONTROL帳戶]而提供。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">
     [!UICONTROL建立後]
   </td> 
   <td> <p>選擇要將信封另存為草稿還是發送以進行簽名。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL模板收件人]</td>
    <td>選擇此信封的收件人</td>
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 將收件者添加到信封]

此動作模組會將一或多個收件者新增至現有信封。 如果信封已發送，則收件人會收到電子郵件。 此模組對已完成的信封無效。

<table style="table-layout:auto">
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr data-mc-conditions=""> 
    <td>[!UICONTROL連接] </td>
   <td> <p>如需將DocuSign帳戶連接至Workfront Fusion的指示，請參閱 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連接到Workfront Fusion</a> 在文章中 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在Adobe Workfront Fusion中建立案例</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="">
    <td>[!UICONTROL帳戶] </td>
   <td> <p>選擇包含要添加收件者的信封的帳戶。</p> </td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL信封ID]</td>
    <td>選擇或映射要添加收件人的信封的ID。</td>
  </tr> 
  <tr data-mc-conditions="">
    <td role="rowheader">[!UICONTROL收件人類型]</td>
   <td> <p> 選擇要添加到信封的收件人類型。</p> 
    <ul> 
     <li> <p>[!UICONTROL代理]</p> </li> 
     <li> <p>[!UICONTROL碳副本]</p> </li> 
     <li> <p>[!UICONTROL認證的交付]</p> </li> 
     <li> <p>[!UICONTROL面向簽署者]</p> </li> 
     <li> <p>[!UICONTROL中介]</p> </li> 
     <li> <p>[!UICONTROL簽名者]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL電子郵件]</td>
   <td> <p>輸入或映射要添加到信封的收件人的電子郵件地址。</p> </td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL名稱]</td>
   <td>輸入或映射要添加到信封的收件人的名稱。</td> 
  </tr> 
  <tr>
    <td>[!UICONTROL路由順序]</td>
   <td> <p>輸入或映射收件人的工藝路線編號。 路由編號決定收件者接收和簽署您的檔案的順序。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader">[!UICONTROL電子郵件正文]</td>
   <td>輸入或對應會傳送至收件者的電子郵件內文（內容）。</td> 
  </tr> 
  <tr>
    <td role="rowheader">[!UICONTROL電子郵件主題]</td>
   <td>輸入或對應傳送給收件者的電子郵件主旨。</td> 
  </tr> 
    <td role="rowheader">[!UICONTROL專用消息]</td>
   <td> <li> <p>只有選取的收件者會看見私人訊息以及一般訊息。 私人訊息的長度限制為1000個字元。</p> </li> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL驗證]</td> 
   <td> <p>選取您要用來確認收件者身分的驗證方法。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL無]</strong> </p> </li> 
     <li> <p><strong>[!UICONTROL訪問代碼]</strong> </p> <p>輸入或對應存取代碼。</p> </li> 
     <li> <p><strong>[!UICONTROL電話]</strong> </p> <p>輸入或映射電話號碼</p> </li> 
     <li> <p><strong>[!UICONTROL SMS]</strong> </p> <p>輸入或映射電話號碼</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 新增自訂欄位]

此動作模組會將自訂欄位新增至檔案

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL DocuSign] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-docusign-to-workfront-fusion" class="MCXref xref">Connect [!DNL DocuSign] to [!DNL Workfront Fusion]</a> 這篇文章。</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL帳戶] </td> 
   <td> <p>選擇包含要添加自定義欄位的文檔的帳戶。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL信封ID]</td> 
   <td> <p> 輸入或映射包含要添加自定義欄位的文檔的信封的ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL欄位名稱]</td> 
   <td>輸入或映射要添加的新欄位的名稱。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL必要]</td> 
   <td>如果要將新增的欄位設為必要欄位，請啟用此選項。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL顯示欄位]</td> 
   <td>如果要顯示欄位，請啟用此選項。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL值]</td> 
   <td>輸入或映射新增欄位的值（內容）。 </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 修改自訂欄位]

此動作模組會使用欄位名稱修改自訂欄位。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL DocuSign] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-docusign-to-workfront-fusion" class="MCXref xref">Connect [!DNL DocuSign] to [!DNL Workfront Fusion]</a> 這篇文章。</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL帳戶] </td> 
   <td> <p>選擇包含要修改自定義欄位的文檔的帳戶。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL信封ID]</td> 
   <td> <p> 輸入或映射包含要修改自定義欄位的文檔的信封的ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL欄位ID]</td> 
   <td>輸入或映射要修改的欄位ID。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL欄位名稱]</td> 
   <td>輸入或映射要修改的欄位名稱。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL必要]</td> 
   <td>如果希望修改的欄位是必填欄位，請啟用此選項。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL顯示欄位]</td> 
   <td>如果要顯示欄位，請啟用此選項。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL值]</td> 
   <td>輸入或映射修改欄位的值（內容）。 </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 發送信封]

此動作模組會傳送草稿信封給收件者。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL DocuSign] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-docusign-to-workfront-fusion" class="MCXref xref">Connect [!DNL DocuSign] to [!DNL Workfront Fusion]</a> 這篇文章。</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL帳戶] </td> 
   <td> <p>選取包含要傳送給其收件者之草稿信封的帳戶。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL信封ID]</td> 
   <td> <p> 輸入或映射要發送給其收件人的草稿信封的ID。</p> </td> 
  </tr> 
 </tbody> 
</table>
