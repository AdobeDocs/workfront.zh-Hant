---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 聯結器
navigation-topic: apps-and-their-modules
title: Salesforce模組
description: 在Adobe Workfront Fusion案例中，您可以自動化使用Salesforce的工作流程，並將其連線到多個第三方應用程式和服務。
author: Becky
feature: Workfront Fusion
exl-id: 3c8adcd9-fb5f-400d-9edd-6d9fc30cc728
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '2768'
ht-degree: 0%

---

# [!DNL Salesforce] 模組

在Adobe Workfront Fusion案例中，您可以自動化使用下列專案的工作流程： [!DNL Salesforce]，並將其連線到多個協力廠商應用程式和服務。

如果您需要建立案例的說明，請參閱 [在中建立情境 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

如需模組的相關資訊，請參閱 [中的模組 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

>[!NOTE]
>
>* 並非所有版本 [!DNL Salesforce] 擁有API存取權。 如需詳細資訊，請參閱以下資訊 [!DNL Salesforce] 具有API存取權的版本 [!DNL Salesforce] 社群網站。
>* 有關從傳回的特定錯誤的資訊 [!DNL Salesforce] API，請參閱 [!DNL Salesforce] API檔案 您也可以檢查 [!DNL Salesforce] API可用於任何可能的服務中斷。
>

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

使用 [!DNL Salesforce] 模組，您必須擁有 [!DNL Salesforce] 帳戶。

## 關於搜尋 [!DNL Salesforce] 物件

搜尋物件時，您可以輸入個別搜尋字詞，或使用萬用字元和運運算元建立更複雜的查詢：

* 使用星號萬用字元(\*)取代零或更多字元。 例如，搜尋Ca\*會尋找以Ca開頭的專案
* 使用問號萬用字元(？) 取代單一字元。 例如，搜尋Jo？n會尋找字詞為John或Joan但不為Jon的專案
* 使用引號運運算元(「 」)尋找完全相符的片語。 例如：「星期一會議」

如需搜尋可能性的詳細資訊，請參閱 [!DNL Salesforce] 有關SOQL和SOSL的開發人員檔案。

## [!DNL Salesforce] 模組及其欄位

* [觸發器](#triggers)
* [動作](#actions)
* [搜尋](#searches)

### 觸發器

* [[!UICONTROL 留意記錄]](#watch-for-records)
* [[!UICONTROL 觀看傳出訊息]](#watch-outbound-messages)
* [[!UICONTROL 觀看欄位]](#watch-a-field)

#### [!UICONTROL 留意記錄]

建立或更新物件中的記錄時，此觸發模組會執行案例。 模組會傳回與一個或多個記錄關聯的所有標準欄位，以及連線存取的任何自訂欄位和值。 您可以將此資訊對應到情境中的後續模組中。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL連線]</td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL Salesforce] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與的連線 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL型別] </td> 
   <td> <p>選取型別 [!DNL Salesforce] 錄製您希望模組觀看的影片。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL記錄欄位]</td> 
   <td>選取您希望模組觀看的欄位。 可用欄位取決於記錄型別。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL最大記錄數]</td> 
   <td> <p>輸入或對應您希望模組在每個案例執行週期內傳回的最大記錄數。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL監視]</td> 
   <td> <p>決定您希望案例只監視所選型別的新記錄，還是隻監視所選型別的新記錄以及該型別記錄的所有其他變更。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 觀看傳出訊息]

此觸發模組會在有人傳送訊息時執行案例。 模組會傳回與一個或多個記錄關聯的所有標準欄位，以及連線存取的任何自訂欄位和值。 您可以將此資訊對應到情境中的後續模組中。

此模組需要一些額外的設定：

1. 前往 [!DNL Salesforce] 設定頁面。

   若要存取設定頁面，請找到並按一下標示為「 」的按鈕[!UICONTROL 設定]&quot; （位於右上角） [!DNL Salesforce] 帳戶。 從 [!DNL Salesforce] 設定頁面，找出&quot;[!UICONTROL 快速尋找/搜尋]」列。 搜尋&quot;[!UICONTROL 工作流程規則].」

1. 按一下 **[!UICONTROL 工作流程規則]**.
1. 在 [!UICONTROL 工作流程規則] 頁面上，按一下 **[!UICONTROL 新規則]** 並選取將套用規則的物件型別(例如「[!UICONTROL 機會]&quot;如果您在監控機會記錄的更新)。
1. 按一下 **[!UICONTROL 下一個]**.
1. 設定規則名稱、評估條件和規則條件，然後按一下 **[!UICONTROL 儲存]** 和 **[!UICONTROL 下一個]**.

1. 按一下 **[!UICONTROL 完成]**.
1. 在新建立的工作流程規則中，按一下 **[!UICONTROL 編輯]**..
1. 從 **[!UICONTROL 新增工作流程動作]** 下拉式清單，選取 **[!UICONTROL 新傳出訊息]**.

1. 指定名稱、說明、端點URL，以及要納入新傳出訊息的欄位，然後按一下 **[!UICONTROL 儲存]**.

   此 **[!UICONTROL 端點URL]** 欄位包含 [!DNL Salesforce] [!UICONTROL 傳出訊息] 在 [!DNL Workfront Fusion].

1. 設定開頭為的情境 [!UICONTROL 傳出訊息] 事件。

1. 按一下 **&lt;/>** 圖示並複製提供的URL。
1. 返回 **[!UICONTROL 工作流程規則]** 頁面，找到新建立的規則，然後按一下 **[!UICONTROL 啟動]**.

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Webhook]</td> 
   <td> <p>選取您要用來觀看傳出訊息的webhook。 若要新增webhook，請按一下 <strong>[！UICONTROL新增]</strong> 並輸入webhook的名稱和連線。</p> <p>如需有關連線您的電腦的指示， [!DNL Salesforce] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與[！UICONTROL Adobe Workfront Fusion]的連線 — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL記錄型別] </td> 
   <td> <p>選取型別 [!DNL Salesforce] 錄製您希望模組監視傳出訊息的內容。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL欄位]</td> 
   <td> <p>選取您希望模組監視傳出訊息的欄位。 可用欄位取決於記錄型別。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### *[!UICONTROL 觀看欄位]*

此觸發模組會在欄位更新時啟動案例 [!DNL Salesforce].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL連線]</td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL Salesforce] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與的連線 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL記錄型別] </td> 
   <td> <p>選取記錄型別，其中包含您要模組觀看的欄位。 您必須選擇已開啟[！UICONTROL欄位歷程記錄]的記錄型別 [!DNL Salesforce] 設定。 如需詳細資訊，請參閱 <a href="https://help.salesforce.com/articleView?id=tracking_field_history.htm&amp;type=5">欄位歷史記錄追蹤</a> 在 [!DNL Salesforce] 說明檔案。 </p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL欄位]</td> 
   <td> <p>選取您希望模組監視變更的欄位。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL限制]</td> 
   <td> <p>輸入或對應您希望模組在每個案例執行週期中傳回的最大欄位數。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 動作

* [[!UICONTROL 建立記錄]](#create-a-record)
* [[!UICONTROL 讀取記錄]](#read-a-record)
* [[!UICONTROL 刪除記錄]](#delete-a-record)
* [[!UICONTROL 自訂API呼叫]](#custom-api-call)
* [[!UICONTROL 上傳附件/檔案]](#upload-attachmentdocument)
* [[!UICONTROL 下載附件/檔案]](#download-attachmentdocument)

#### [!UICONTROL 建立記錄]

此動作模組會在物件中建立新記錄。

模組可讓您選取可在模組中取得哪些物件欄位。 這可減少設定模組時必須捲動瀏覽的欄位數。

模組會傳回記錄ID和任何關聯欄位，以及連線存取的任何自訂欄位和值。 您可以將此資訊對應到情境中的後續模組中。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL連線]</td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL Salesforce] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與的連線 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td> <p>[！UICONTROL記錄型別] </p> </td> 
   <td> <p>選取型別 [!DNL Salesforce] 您要模組建立的記錄。 根據[！UICONTROL記錄型別]欄位中選取的記錄型別，欄位會變為可用。 這些欄位是根據 [!DNL Salesforce] API。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL選取要對應的欄位]</td> 
   <td> <p>選取建立新記錄時您希望模組設定的欄位。 必要欄位位於清單頂端。 </p> <p>您選取的欄位會在此欄位下方開啟。 您現在可以在這些欄位中輸入值。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 讀取記錄]

此動作模組會從中的單一物件讀取資料 [!DNL Salesforce].

您指定記錄的ID。

模組會傳回記錄ID和任何關聯欄位，以及連線存取的任何自訂欄位和值。 您可以將此資訊對應到情境中的後續模組中。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr>
    <td>[！UICONTROL連線]</td>
   <td> <p>如需有關連線您的電腦的指示， [!DNL Salesforce] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與的連線 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr>
    <td>[！UICONTROL記錄型別]</td>
    <td>選取型別 [!DNL Salesforce] 記錄您希望模組執行[action].read。</td>
  </tr> 
  <tr>
    <td>[！UICONTROL記錄欄位]</td>
    <td>選取您希望模組讀取的欄位。 您必須至少選取一個欄位。</td>
  </tr> 
  <tr>
    <td>[！UICONTROL ID]</td>
    <td> <p>輸入或對映唯一的 [!DNL Salesforce] 您希望模組讀取的記錄ID。</p> <p>若要取得ID，請開啟 [!DNL Salesforce] 物件，並複製URL結尾處的最後一個正斜線(/)之後的文字。 例如： <code>https://eu5.salesforce.com/&lt;object ID&gt;</code></p> </td>
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 刪除記錄]

此動作模組會刪除物件中的現有記錄。

您指定記錄的ID。

模組會傳回記錄ID和任何關聯欄位，以及連線存取的任何自訂欄位和值。 您可以將此資訊對應到情境中的後續模組中。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL連線]</td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL Salesforce] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與的連線 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL記錄型別] </td> 
   <td> <p>選取型別 [!DNL Salesforce] 您要模組刪除的記錄。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL ID]</td> 
   <td> <p>輸入或對映唯一的 [!DNL Salesforce] 您要模組刪除的記錄ID。</p> <p>若要取得ID，請開啟 [!DNL Salesforce] 物件，並複製URL結尾處的最後一個正斜線(/)之後的文字。 例如： <code>https://eu5.salesforce.com/&lt;object ID&gt;</code></p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 自訂API呼叫]

此動作模組可讓您對 [!DNL Salesforce] API。 如此一來，您就可以建立其他人無法完成的資料流程自動化 [!DNL Salesforce] 模組。

模組傳回以下內容：

* **[!UICONTROL 狀態代碼]** （數字）：這表示HTTP要求成功或失敗。 這些是您可在網際網路上查閱的標準程式碼。
* **[!UICONTROL 標頭]** （物件）：與輸出內文無關之回應/狀態代碼的更詳細內容。 並非所有顯示在回應標頭中的標頭都是回應標頭，因此某些標頭可能對您並無用處。

  回應標頭取決於您在設定模組時選擇的HTTP請求。

* **[!UICONTROL 內文]** （物件）：根據您在設定模組時選擇的HTTP請求，您可能會收到傳回的一些資料。 該資料，例如來自 [!UICONTROL GET] 要求，包含在此物件中。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL連線]</td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL Salesforce] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與的連線 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL URL]</p> </td> 
   <td> <p>輸入相對於<code> &lt;Instance URL&gt;/services/data/v46.0/</code>.</p> <p>如需可用端點的清單，請參閱 <a href="https://developer.salesforce.com/docs/atlas.en-us.api_rest.meta/api_rest/intro_what_is_rest_api.htm">Salesforce REST API開發人員指南</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL方法]</p> </td> 
   td&gt; <p>選取設定API呼叫所需的HTTP要求方法。 如需詳細資訊，請參閱 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">中的HTTP要求方法 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL標頭]</td> 
   <td> <p>以標準JSON物件的形式新增請求的標頭。例如， <code>{"Content-type":"application/json"}</code>. Workfront Fusion會為您新增授權標頭。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL查詢字串]</td> 
   <td> <p>以標準JSON物件的形式新增API呼叫的查詢。例如： <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL內文]</td> 
   <td> <p>以標準JSON物件的形式新增API呼叫的正文內容。</p> <p>備註:  <p>使用條件陳述式時，例如 <code>if</code> 在JSON中，將引號放在條件陳述式之外。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**範例：** 以下API呼叫會傳回 [!DNL Salesforce] 帳戶：
>
>* **URL**： `query`
>
>* **方法**： [!UICONTROL GET]
>
>* **查詢字串**：
>
>* **金鑰**： `q`
>
>* **值**： `SELECT Id, Name, CreatedDate, LastModifiedDate FROM User LIMIT 10`
>
>您可以在模組的輸出中找到搜尋的相符專案，位於 **[!UICONTROL 組合] > [!UICONTROL 內文] > [!UICONTROL 記錄]**.
>
>在我們的範例中，傳回6位使用者：
>
>![](assets/matches-of-the-search-350x573.png)


#### [!UICONTROL 上傳附件/檔案]

此動作模組會上傳檔案並將其附加至您指定的記錄，或上傳檔案。

模組會傳回附件或檔案的ID以及任何關聯欄位，以及連線存取的任何自訂欄位和值。 您可以將此資訊對應到情境中的後續模組中。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL連線]</td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL Salesforce] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與的連線 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL上傳型別]</td> 
   <td>選取您希望模組上傳附件還是檔案。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL ID]</td> 
   <td>輸入或對應您要上傳附件的物件ID。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL資料夾]</td> 
   <td>選取包含您要模組上傳之檔案的資料夾。 </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL來源檔案]</td> 
   <td>從先前的模組中選取來源檔案，或對應來源檔案的名稱和資料。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 下載附件/檔案]

此動作模組會從記錄下載檔案或附件。

您可以指定記錄的ID以及您想要的下載型別。

模組會傳回附件或檔案的ID以及任何關聯欄位，以及連線存取的任何自訂欄位和值。 您可以將此資訊對應到情境中的後續模組中。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr>
    <td>[！UICONTROL連線]</td>
   <td> <p>如需有關連線您的電腦的指示， [!DNL Salesforce] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與的連線 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr>
    <td>[！UICONTROL下載型別]</td>
    <td> <p>指定您要從Salesforce下載的檔案型別。</p> 
     <ul> 
      <li>[！UICONTROL附件]</li> 
      <li>[！UICONTROL檔案]</li> 
      <li>[！UICONTROL ContentDocument] (這是已上傳至程式庫的檔案，位於 [!DNL Saleforce CRM Content] 或 [!DNL Salesforce Files].)</li> 
     </ul> </td>
  </tr> 
  <tr>
    <td> <p>[！UICONTROL ID] / </p> <p>[！UICONTROL附件ID] / </p> <p>[！UICONTROL ContentDocument ID]</p> </td>
    <td> <p>輸入或對映唯一的 [!DNL Salesforce] 您要模組下載的記錄ID。</p> <p>若要取得ID，請開啟 [!DNL Salesforce] 物件，並複製URL結尾處的最後一個正斜線(/)之後的文字。 例如： <code>https://eu5.salesforce.com/&lt;object ID&gt;</code></p> </td>
  </tr> 
 </tbody> 
</table>


#### [!UICONTROL 更新記錄]

此動作模組會編輯物件中的記錄。

模組可讓您選取可在模組中取得哪些物件欄位。 這可減少設定模組時必須捲動瀏覽的欄位數。

模組會傳回記錄ID和任何關聯欄位，以及連線存取的任何自訂欄位和值。 您可以將此資訊對應到情境中的後續模組中。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL連線]</td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL Salesforce] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與的連線 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL ID]</td> 
   <td>輸入或對應您要更新的記錄ID。</td> 
  </tr> 
  <tr> 
   <td> <p>[！UICONTROL記錄型別] </p> </td> 
   <td> <p>選取型別 [!DNL Salesforce] 記錄您希望模組更新的內容。 根據「記錄型別」欄位中選取的記錄型別，欄位變為可用。 這些欄位是根據 [!DNL Salesforce] API。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL選取要對應的欄位]</td> 
   <td> <p>選取建立新記錄時您希望模組設定的欄位。 必要欄位位於清單頂端。 </p> <p>您選取的欄位會在此欄位下方開啟。 您現在可以在這些欄位中輸入值。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 搜尋

#### [!UICONTROL 使用查詢搜尋]

此搜尋模組會在中尋找物件中的記錄 [!DNL Salesforce] 符合您指定的搜尋查詢。 您可以將此資訊對應到情境中的後續模組中。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL連線]</td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL Salesforce] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與的連線 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL搜尋型別]</td> 
   <td> <p>選取您希望模組執行的搜尋型別：</p> 
    <ul> 
     <li> <p>[！UICONTROL簡單]</p> </li> 
     <li> <p>使用SOSL （Salesforce物件搜尋語言）的[！UICONTROL]</p> </li> 
     <li> <p>使用SOQL （Salesforce物件查詢語言）的[！UICONTROL]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td> <p>[！UICONTROL型別] </p> </td> 
   <td> <p>如果您選取了「簡單」搜尋型別，請選擇 [!DNL Salesforce] 您要模組搜尋的記錄。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL查詢] / [！UICONTROL SOSL查詢] / [！UICONTROL SOQL查詢]</td> 
   <td> <p>輸入您要搜尋的查詢。</p> <p>如需有關SOSL的詳細資訊，請參閱 <a href="https://developer.salesforce.com/docs/atlas.en-us.soql_sosl.meta/soql_sosl/sforce_api_calls_sosl.htm">Salesforce物件搜尋語言(SOSL)</a> 在 [!DNL Salesforce] 說明檔案。</p> <p>如需有關SOQL的詳細資訊，請參閱 <a href="https://developer.salesforce.com/docs/atlas.en-us.soql_sosl.meta/soql_sosl/sforce_api_calls_soql.htm">Salesforce物件查詢語言(SOQL)</a> 在 [!DNL Salesforce] 說明檔案。</p> <p>注意：請注意，引數的值 <code>RETURNING </code>會影響模組的輸出。 如果您使用 <code>LIMIT</code>， [!DNL Fusion] 將忽略[！UICONTROL最大記錄數]欄位中的設定。 如果您未設定任何限制，Fusion會插入值[！UICONTROL LIMIT =最大記錄數]。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL最大記錄數]</td> 
   <td> <p>輸入或對應您希望模組在每個案例執行週期內傳回的最大記錄數。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 搜尋]

此動作模組會擷取符合指定條件的所有記錄。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL連線]</td> 
   <td>如需有關連線您的電腦的指示， [!DNL Salesforce] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與的連線[!DNL  Adobe Workfront Fusion]  — 基本指示</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL型別]</td> 
   <td> <p>選取您要搜尋的物件型別。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL搜尋條件]</td> 
   <td>選取您要搜尋的欄位、要在查詢中使用的運運算元，以及要在欄位中搜尋的值。 您可以使用AND或OR來連線查詢。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL輸出]</td> 
   <td>選取您要納入模組輸出的欄位。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL結果集]</td> 
   <td>選取您希望模組傳回「所有比對記錄」，還是隻傳回「第一個比對記錄」。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Maximal]</td> 
   <td>輸入或對應您希望模組在每個案例執行週期中擷取的記錄數上限。</td> 
  </tr> 
 </tbody> 
</table>
