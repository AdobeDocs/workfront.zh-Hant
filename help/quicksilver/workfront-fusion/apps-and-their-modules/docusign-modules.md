---
title: DocuSign模組
description: 此 [!DNL Adobe Workfront Fusion DocuSign] 模組可讓您監視和擷取信封狀態、搜尋和擷取信封，或下載和傳送檔案以登入 [!DNL DocuSign] 帳戶。
author: Becky
draft: Probably
feature: Workfront Fusion, Digital Content and Documents
exl-id: a6ebfe6f-dc3f-41f7-8129-bbc5775cff33
source-git-commit: 632952e91ebe2ae5caa370c310cfd5e7180232b7
workflow-type: tm+mt
source-wordcount: '1895'
ht-degree: 0%

---

# DocuSign模組

此 [!DNL Adobe Workfront Fusion] [!DNL DocuSign] 模組可讓您監視和擷取信封狀態、搜尋和擷取信封，或下載和傳送檔案以登入 [!DNL DocuSign] 帳戶。

如果您需要建立案例的說明，請參閱 [在中建立情境 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

如需模組的相關資訊，請參閱 [中的模組 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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
   <td> <p>[！UICONTROL [!DNL Workfront Fusion] 適用於工作自動化與整合] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>貴組織必須購買 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文所述功能。</td> 
  </tr> 
 </tbody> 
</table>

若要瞭解您擁有哪些計畫、授權型別或存取權，請聯絡您的 [!DNL Workfront] 管理員。

有關以下專案的資訊： [!DNL Adobe Workfront Fusion] 授權，請參閱 [[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 必要條件

使用 [!DNL DocuSign] 模組，您必須擁有 [!DNL DocuSign] 帳戶。

## Connect [!DNL DocuSign] 至 [!DNL Workfront Fusion] {#connect-docusign-to-workfront-fusion}

若要為建立連線，請執行下列步驟： [!DNL DocuSign] 模組：

1. 按一下 **[!UICONTROL 新增]** 旁邊 [!UICONTROL 連線] 方塊(當您開始設定第一個 [!DNL DocuSign] 模組。
1. 輸入下列內容：

<table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[！UICONTROL連線名稱]</p> </td> 
      <td>輸入新專案的名稱 [!DNL DocuSign] 連線</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL帳戶型別]</td> 
      <td>選取您要連線的帳戶是生產帳戶還是示範帳戶。</td> 
     </tr> 
    </tbody> 
   </table>

1. 繼續執行，如所述 [建立與的連線 [!DNL Adobe Workfront Fusion]  — 基本指示](../../workfront-fusion/connections/connect-to-fusion-general.md#connect).

## [!DNL DocuSign] 模組及其欄位

當您設定 [!DNL DocuSign] 模組， [!DNL Workfront Fusion] 顯示下列欄位。 除了這些以外， [!DNL DocuSign] 視您在應用程式或服務中的存取層級等因素而定，可能會顯示欄位。 模組中的粗體標題表示必填欄位。

如果您在欄位或函式上方看到對應按鈕，則可以使用它來設定該欄位的變數和函式。 如需詳細資訊，請參閱 [將資訊從一個模組對應至中的另一個模組 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [觸發器](#triggers)
* [動作](#actions)

### 觸發器

#### [!UICONTROL 觀看信封]

當信封已傳送、傳遞、簽署、完成或拒絕時，此觸發模組會啟動案例。

<table style="table-layout:auto">
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL連線] </td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL DocuSign] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連線至 [!DNL Workfront Fusion]</a> 在文章中 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在中建立情境 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL帳戶] </td> 
   <td> <p>選取包含您要監視之記錄的帳戶。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL事件型別]</td> 
   <td> <p> 選取您要觀看的事件型別。</p> 
    <ul> 
     <li>[！UICONTROL檔案已完成]</li> 
     <li>[！UICONTROL檔案已拒絕]</li> 
     <li>[！UICONTROL檔案已傳送]</li> 
     <li>[！UICONTROL檔案已簽署]</li> 
     <li>[！UICONTROL收件匣中的新檔案]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL輸出欄位]</p> </td> 
   <td> <p>選取您要納入模組輸出的欄位。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制]</td> 
   <td>輸入或對應您希望模組在每個案例執行週期使用的最大記錄數。</td> 
  </tr> 
 </tbody> 
</table>

### 動作

* [[!UICONTROL 自訂API呼叫]](#custom-api-call)
* [[!UICONTROL 下載檔案]](#download-a-document)
* [[!UICONTROL 讀取信封]](#read-an-envelope)
* [[!UICONTROL 將檔案上傳至信封]](#upload-a-file-to-an-envelope)
* [[!UICONTROL 建立新信封]](#create-a-new-envelope)
* [[!UICONTROL 將收件者新增至信封]](#add-recipient-to-envelope)
* [[!UICONTROL 新增自訂欄位]](#add-custom-field)
* [[!UICONTROL 修改自訂欄位]](#modify-custom-field)
* [[!UICONTROL 傳送信封]](#send-envelope)

#### [!UICONTROL 自訂API呼叫]

此動作模組可讓您執行自訂API呼叫。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL連線]</td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL DocuSign] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-docusign-to-workfront-fusion" class="MCXref xref">Connect [!DNL DocuSign] 至 [!DNL Workfront Fusion]</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL帳戶]</td> 
   <td>輸入或對應您要用來存取 [!DNL DocuSign] API。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL URL]</td> 
   <td> <p>輸入您希望模組與之互動的網頁伺服器位址。</p> <p>您可以輸入相對URL，這表示您不需要包含通訊協定(例如 <code>http://</code>)開頭的。 這會向網頁伺服器提示互動正在伺服器上發生。</p> <p>例如： <code>[!DNL /api/conversations].create</code></p>  </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL方法]</td> 
   <td> <p>選取設定API呼叫所需的HTTP要求方法。 如需詳細資訊，請參閱 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">中的HTTP要求方法 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL標頭]</td> 
   <td> <p>以標準JSON物件的形式新增請求的標頭。 這會決定請求的內容型別。</p> <p>例如，<code> {"Content-type":"application/json"}</code></p> <p>注意：如果您收到錯誤且難以判斷其來源，請考慮根據 [!DNL Workfront] 說明檔案。 如果您的自訂API呼叫傳回422 HTTP請求錯誤，請嘗試使用"Content-Type"："text/plain"標頭。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL查詢字串]</td> 
   <td> <p>以標準JSON物件的形式新增API呼叫的查詢。</p> <p>例如： <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL內文]</td> 
   <td> <p>以標準JSON物件的形式新增API呼叫的正文內容。</p> <p>備註:  <p>使用條件陳述式時，例如 <code>if</code> 在JSON中，將引號放在條件陳述式之外。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL限制]</td> 
   <td>輸入或對應在一個執行週期內使用的最大結果數量。</td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**範例：** 清單信封
>
>以下API呼叫會傳回中指定日期的信封 [!DNL DocuSign] 帳戶：
>
>**URL**： `/v2.1/accounts/{accountId}/envelopes/`
>
>**方法**： `GET`
>
>**查詢字串**：
>
>* **金鑰**： `from_date`
>
>* **值**： `YYYY-MM-DD`
>
>指定請求何時開始檢查帳戶信封的狀態變更。
>
>![](assets/example-docusign-setup-350x770.png)
>
>結果可在模組的輸出中找到，位於「束>內文>信封」下。
>
>在我們的範例中，傳回6個信封：
>
>![](assets/docusign-example-output-350x677.png)

#### [!UICONTROL 下載檔案]

此動作模組會下載單一檔案。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL連線]</td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL DocuSign] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-docusign-to-workfront-fusion" class="MCXref xref">Connect [!DNL DocuSign] 至 [!DNL Workfront Fusion]</a> 本文章內容。</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL帳戶] </td> 
   <td> <p>選取包含您要下載之檔案的帳戶。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL信封ID]</td> 
   <td> <p> 輸入或對應您要下載的信封ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL檔案ID]</p> </td> 
   <td> <p>輸入或對映您要下載的檔案ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL憑證]</td> 
   <td>選取 <strong>[！UICONTROL是]</strong> 如果要在下載中包含信封簽署憑證。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">依據使用者ID的[！UICONTROL檔案]</td> 
   <td>選取 <strong>[！UICONTROL是]</strong> 是否允許收件者依使用者ID擷取檔案。 例如，如果使用者包含在具有不同可見度的兩個不同製程訂單中，則使用此選項會傳回兩個製程中的所有檔案。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL加密]</td> 
   <td>選取 <strong>[！UICONTROL是]</strong> 如果您想要將回應中傳回的PDF位元組加密，供您設定的所有金鑰管理員使用， [!DNL DocuSign] 帳戶。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL語言]</td> 
   <td>選取語言。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL顯示變更]</td> 
   <td>當設定為 <strong>[！UICONTROL是]</strong>，傳回PDF的任何變更欄位都會以黃色醒目提示，而選填簽名或縮寫則會以紅色醒目提示。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL浮水印]</td> 
   <td> <p>選取 <strong>[！UICONTROL否]</strong> 以從PDF檔案中移除浮水印。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 讀取信封]

此動作模組會讀取中信封的相關資訊 [!DNL DocuSign] 使用信封ID。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL連線]</td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL DocuSign] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-docusign-to-workfront-fusion" class="MCXref xref">Connect [!DNL DocuSign] 至 [!DNL Workfront Fusion]</a> 本文章內容。</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL帳戶] </td> 
   <td> <p>選取包含您要讀取資訊之檔案的帳戶。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL信封ID]</td> 
   <td> <p> 輸入或對應包含您要讀取資訊之檔案的ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL輸出]</td> 
   <td>選取您要顯示在模組輸出中的屬性。 </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 將檔案上傳至信封]

此模組會將指定的檔案上傳到DocuSign中的現有信封。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL連線]</td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL DocuSign] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-docusign-to-workfront-fusion" class="MCXref xref">Connect [!DNL DocuSign] 至 [!DNL Workfront Fusion]</a> 本文章內容。</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL帳戶] </td> 
   <td> <p>選取包含要上傳檔案之信封的帳戶。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL信封ID]</td> 
   <td> <p> 輸入或對應您要上傳檔案之信封的識別碼。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL來源檔案]</td> 
   <td>從先前的模組中選取來源檔案，或輸入來源檔案的名稱和資料。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 建立新信封]

此動作模組會從範本建立新的信封。 它會傳回新信封的ID以及新信封的狀態。

<table style="table-layout:auto">
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
    <td role="rowheader">[！UICONTROL連線] </td>

<td> <p>如需將DocuSign帳戶連線至Workfront Fusion的說明，請參閱 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連線至Workfront Fusion</a> 在文章中 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在Adobe Workfront Fusion中建立情境</a>.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader">[！UICONTROL帳戶] </td>
   <td> <p>選取包含要上傳檔案之信封的帳戶。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[！UICONTROL範本]</td>
   <td> <p> 選取要從中建立新信封的範本。 根據您選取的[！UICONTROL帳戶]可使用範本。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">
     [！UICONTROL建立後]
   </td> 
   <td> <p>選取您要將信封另存為草稿或傳送以進行簽署。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[！UICONTROL範本收件者]</td>
    <td>選取此信封的收件者</td>
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 將收件者新增至信封]

此動作模組會將一或多個收件者新增至現有信封。 如果信封已傳送，則會傳送電子郵件給收件者。 此模組對已完成的信封無效。

<table style="table-layout:auto">
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr data-mc-conditions=""> 
    <td>[！UICONTROL連線] </td>
   <td> <p>如需將DocuSign帳戶連線至Workfront Fusion的說明，請參閱 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連線至Workfront Fusion</a> 在文章中 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在Adobe Workfront Fusion中建立情境</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="">
    <td>[！UICONTROL帳戶] </td>
   <td> <p>選取包含要新增收件者之信封的帳戶。</p> </td> 
  </tr> 
  <tr> 
    <td>[！UICONTROL信封ID]</td>
    <td>選取或對應您要新增收件者之信封的ID。</td>
  </tr> 
  <tr data-mc-conditions="">
    <td role="rowheader">[！UICONTROL收件者型別]</td>
   <td> <p> 選取您要新增至信封的收件者型別。</p> 
    <ul> 
     <li> <p>[！UICONTROL Agent]</p> </li> 
     <li> <p>[！UICONTROL副本]</p> </li> 
     <li> <p>[！UICONTROL Certified delivery]</p> </li> 
     <li> <p>[！UICONTROL個人簽名者]</p> </li> 
     <li> <p>[！UICONTROL Intermediate]</p> </li> 
     <li> <p>[！UICONTROL簽署者]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
    <td>[！UICONTROL電子郵件]</td>
   <td> <p>輸入或對應您要新增至信封的收件者電子郵件地址。</p> </td> 
  </tr> 
  <tr> 
    <td>[！UICONTROL名稱]</td>
   <td>輸入或對應您要新增至信封的收件者名稱。</td> 
  </tr> 
  <tr>
    <td>[！UICONTROL路由順序]</td>
   <td> <p>輸入或對應收件者的路由編號。 路由號碼決定收件者接收和簽署檔案的順序。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader">[！UICONTROL電子郵件內文]</td>
   <td>輸入或對應傳送給收件者的電子郵件內文（內容）。</td> 
  </tr> 
  <tr>
    <td role="rowheader">[！UICONTROL電子郵件主旨]</td>
   <td>輸入或對應傳送給收件者的電子郵件主旨。</td> 
  </tr> 
    <td role="rowheader">[！UICONTROL私人訊息]</td>
   <td> <li> <p>只有選取的收件者會看到私人訊息以及一般訊息。 私人訊息限製為1000個字元。</p> </li> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Authentication]</td> 
   <td> <p>選取您要用來確認收件者身分的驗證方法。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL無]</strong> </p> </li> 
     <li> <p><strong>[！UICONTROL存取碼]</strong> </p> <p>輸入或對映存取代碼。</p> </li> 
     <li> <p><strong>[！UICONTROL Phone]</strong> </p> <p>輸入或對應電話號碼</p> </li> 
     <li> <p><strong>[！UICONTROL SMS]</strong> </p> <p>輸入或對應電話號碼</p> </li> 
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
   <td role="rowheader">[！UICONTROL連線]</td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL DocuSign] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-docusign-to-workfront-fusion" class="MCXref xref">Connect [!DNL DocuSign] 至 [!DNL Workfront Fusion]</a> 本文章內容。</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL帳戶] </td> 
   <td> <p>選取包含您要新增自訂欄位之檔案的帳戶。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL信封ID]</td> 
   <td> <p> 輸入或對應信封的ID，該信封包含您要新增自訂欄位的檔案。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL欄位名稱]</td> 
   <td>輸入或對應您要新增之新欄位的名稱。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL必填]</td> 
   <td>如果您希望新增的欄位是必填欄位，請啟用此選項。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL顯示欄位]</td> 
   <td>如果您希望顯示欄位，請啟用此選項。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL值]</td> 
   <td>輸入或對映新增欄位的值（內容）。 </td> 
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
   <td role="rowheader">[！UICONTROL連線]</td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL DocuSign] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-docusign-to-workfront-fusion" class="MCXref xref">Connect [!DNL DocuSign] 至 [!DNL Workfront Fusion]</a> 本文章內容。</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL帳戶] </td> 
   <td> <p>選取包含您要修改自訂欄位之檔案的帳戶。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL信封ID]</td> 
   <td> <p> 輸入或對映包含要修改自訂欄位之檔案的信封的ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL欄位ID]</td> 
   <td>輸入或對應您要修改之欄位的ID。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL欄位名稱]</td> 
   <td>輸入或對應您要修改的欄位名稱。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL必填]</td> 
   <td>如果您希望修改的欄位成為必填欄位，請啟用此選項。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL顯示欄位]</td> 
   <td>如果您希望顯示欄位，請啟用此選項。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL值]</td> 
   <td>輸入或對映修改欄位的值（內容）。 </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 傳送信封]

此動作模組會傳送草稿信封給其收件者。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL連線]</td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL DocuSign] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-docusign-to-workfront-fusion" class="MCXref xref">Connect [!DNL DocuSign] 至 [!DNL Workfront Fusion]</a> 本文章內容。</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL帳戶] </td> 
   <td> <p>選取包含您要傳送給其收件者之草稿信封的帳戶。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL信封ID]</td> 
   <td> <p> 輸入或對應您要傳送給收件者的草稿信封的ID。</p> </td> 
  </tr> 
 </tbody> 
</table>
