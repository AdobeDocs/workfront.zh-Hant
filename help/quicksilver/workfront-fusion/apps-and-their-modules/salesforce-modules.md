---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 聯結器
navigation-topic: apps-and-their-modules
title: Salesforce模組
description: Adobe Workfront Fusion檔案已移至新位置。 本文已棄用，但包含新文章的連結，內容涵蓋此功能。
author: Becky
feature: Workfront Fusion
exl-id: 3c8adcd9-fb5f-400d-9edd-6d9fc30cc728
source-git-commit: efbe888d370e20c895dc40f18f999f2d01ec6337
workflow-type: tm+mt
source-wordcount: '2806'
ht-degree: 0%

---

# [!DNL Salesforce]模組

>[!IMPORTANT]
>
>Adobe Workfront Fusion檔案已移至新位置。
>
>本文資訊可在以下文章中找到：
>
>* [Salesforce模組](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/salesforce-modules.html)
>
>請更新任何書籤。
>
>本文已不再更新，將於不久將來移除。

在Adobe Workfront Fusion案例中，您可以自動化使用[!DNL Salesforce]的工作流程，並將其連線至多個協力廠商應用程式和服務。

如需Salesforce聯結器的簡介影片，請參閱：

* [Salesforce](https://video.tv.adobe.com/v/3427027/){target=_blank}

如果您需要有關建立案例的指示，請參閱[在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md)中建立案例。

如需模組的相關資訊，請參閱 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md)中的[模組。

>[!NOTE]
>
>* 並非所有[!DNL Salesforce]版本都有API存取權。 如需詳細資訊，請參閱[!DNL Salesforce]社群網站上具有API存取許可權的[!DNL Salesforce]版本相關資訊。
>* 有關從[!DNL Salesforce] API傳回的特定錯誤的資訊，請參閱[!DNL Salesforce] API檔案。 您也可以檢查[!DNL Salesforce] API的狀態，瞭解是否有任何可能的服務中斷。
>

## 存取需求

您必須具有下列存取權才能使用本文中的功能：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計畫*</td>
  <td> <p>[！UICONTROL Pro]或更高版本</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權*</td>
   <td> <p>[！UICONTROL計畫]，[！UICONTROL工作]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] 授權**</td> 
   <td>
   <p>目前授權需求：無[!DNL Workfront Fusion]授權需求。</p>
   <p>或</p>
   <p>舊版授權需求：[！UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>
   <p>目前產品需求：如果您有[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Adobe Workfront]計畫，貴組織必須購買[!DNL Adobe Workfront Fusion]及[!DNL Adobe Workfront]，才能使用本文所述的功能。 [!DNL Workfront Fusion]包含在[！UICONTROL Ultimate] [!DNL Workfront]計畫中。</p>
   <p>或</p>
   <p>舊版產品需求：您的組織必須購買[!DNL Adobe Workfront Fusion]及[!DNL Adobe Workfront]，才能使用本文所述的功能。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的[!DNL Workfront]管理員。

如需[!DNL Adobe Workfront Fusion]授權的相關資訊，請參閱[[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md)。

## 先決條件

若要使用[!DNL Salesforce]模組，您必須有[!DNL Salesforce]帳戶。

## Salesforce API資訊

Salesforce聯結器會使用以下專案：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">基礎URL</td> 
   <td> {{connection.instanceUrl}}</td>
  </tr> 
  <tr> 
   <td role="rowheader">API版本</td> 
   <td> v46.0 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">API標籤</td> 
   <td>v1.15.14</td> 
  </tr>
 </tbody> 
 </table>

## 關於搜尋[!DNL Salesforce]物件

搜尋物件時，您可以輸入個別搜尋字詞，或使用萬用字元和運運算元建立更複雜的查詢：

* 使用星號萬用字元(\*)取代零或更多字元。 例如，搜尋Ca\*會尋找以Ca開頭的專案
* 使用問號萬用字元(？) 取代單一字元。 例如，搜尋Jo？n會尋找含有John或Joan字詞，但不包含Jon字詞的專案
* 使用引號運運算元(「 」)尋找完全相符的片語。 例如：「星期一會議」

如需有關搜尋可能性的詳細資訊，請參閱[!DNL Salesforce]有關SOQL和SOSL的開發人員檔案。

## [!DNL Salesforce]模組及其欄位

* [觸發器](#triggers)
* [動作](#actions)
* [搜尋](#searches)

### 觸發程序

* [[!UICONTROL 觀看記錄]](#watch-for-records)
* [[!UICONTROL 觀看傳出訊息]](#watch-outbound-messages)
* [[!UICONTROL 觀看欄位]](#watch-a-field)

#### [!UICONTROL 觀看記錄]

此觸發器模組會在物件中的記錄建立或更新時執行案例。 模組會傳回與一個或多個記錄相關聯的所有標準欄位，以及連線存取的任何自訂欄位和值。 您可以在情境中的後續模組中對應此資訊。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection]</td> 
   <td> <p>如需有關將您的[!DNL Salesforce]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與[!DNL Adobe Workfront Fusion]的連線 — 基本指示</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL型別] </td> 
   <td> <p>選取您希望模組觀看的[!DNL Salesforce]記錄型別。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL記錄欄位]</td> 
   <td>選取您希望模組觀看的欄位。 可用欄位取決於記錄型別。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL最大記錄數]</td> 
   <td> <p>輸入或對應您希望模組在每個案例執行週期中傳回的最大記錄數。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL手錶]</td> 
   <td> <p>決定您要案例只監視所選型別的新記錄，還是隻監視所選型別的新記錄以及該型別記錄的所有其他變更。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 觀看傳出訊息]

有人傳送訊息時，此觸發模組會執行案例。 模組會傳回與一個或多個記錄相關聯的所有標準欄位，以及連線存取的任何自訂欄位和值。 您可以在情境中的後續模組中對應此資訊。

此模組需要一些額外的設定：

1. 前往[!DNL Salesforce]設定頁面。

   若要存取設定頁面，請尋找並按一下[!DNL Salesforce]帳戶右上角標示為「[!UICONTROL 設定]」的按鈕。 從[!DNL Salesforce]設定頁面，找到左側的[!UICONTROL 快速尋找/搜尋]列。 搜尋「[!UICONTROL 工作流程規則]」。

1. 按一下&#x200B;**[!UICONTROL 工作流程規則]**。
1. 在顯示的[!UICONTROL 工作流程規則]頁面上，按一下&#x200B;**[!UICONTROL 新增規則]**，然後選取規則將套用到的物件型別(例如，[!UICONTROL Opportunity] （如果您正在監視機會記錄的更新）。
1. 按一下&#x200B;**[!UICONTROL 下一步]**。
1. 設定規則名稱、評估條件和規則條件，然後按一下[儲存] ]**和[下一步]****。**[!UICONTROL 

1. 按一下&#x200B;**[!UICONTROL 完成]**。
1. 從新建立的工作流程規則中，按一下&#x200B;**[!UICONTROL 編輯]**。
1. 從&#x200B;**[!UICONTROL 新增工作流程動作]**&#x200B;下拉式清單中，選取&#x200B;**[!UICONTROL 新增傳出訊息]**。

1. 指定名稱、說明、端點URL以及要納入新傳出訊息的欄位，然後按一下[儲存]。****

   **[!UICONTROL 端點URL]**&#x200B;欄位包含在[!DNL Workfront Fusion]中的[!DNL Salesforce] [!UICONTROL 傳出訊息]上提供的URL。

1. 設定以[!UICONTROL 傳出訊息]事件開頭的情境。

1. 按一下右下角的&#x200B;**&lt;/>**&#x200B;圖示，並複製提供的URL。
1. 返回&#x200B;**[!UICONTROL 工作流程規則]**&#x200B;頁面，找到新建立的規則，然後按一下&#x200B;**[!UICONTROL 啟動]**。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Webhook]</td> 
   <td> <p>選取您要用來觀看外寄郵件的webhook。 若要新增webhook，請按一下<strong>[！UICONTROL新增]</strong>並輸入webhook的名稱和連線。</p> <p>如需有關將您的[!DNL Salesforce]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與[！UICONTROL Adobe Workfront Fusion]的連線 — 基本說明</a></p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL記錄型別] </td> 
   <td> <p>選取您希望模組監視傳出訊息的[!DNL Salesforce]記錄型別。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL欄位]</td> 
   <td> <p>選取您希望模組監視傳出訊息的欄位。 可用欄位取決於記錄型別。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### *[!UICONTROL 觀看欄位]*

此觸發模組會在[!DNL Salesforce]中更新欄位時啟動案例。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection]</td> 
   <td> <p>如需有關將您的[!DNL Salesforce]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與[!DNL Adobe Workfront Fusion]的連線 — 基本指示</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL記錄型別] </td> 
   <td> <p>選取記錄型別，其中包含您要模組觀看的欄位。 您必須選擇在[!DNL Salesforce]設定中開啟[！UICONTROL欄位歷程記錄]的記錄型別。 如需詳細資訊，請參閱[!DNL Salesforce]檔案中的<a href="https://help.salesforce.com/articleView?id=tracking_field_history.htm&amp;type=5">欄位歷程記錄追蹤</a>。 </p> </td> 
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

模組會傳回記錄ID及任何關聯欄位，連同連線存取的任何自訂欄位和值。 您可以在情境中的後續模組中對應此資訊。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection]</td> 
   <td> <p>如需有關將您的[!DNL Salesforce]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與[!DNL Adobe Workfront Fusion]的連線 — 基本指示</a>。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[！UICONTROL記錄型別] </p> </td> 
   <td> <p>選取您要模組建立的[!DNL Salesforce]記錄型別。 根據[！UICONTROL記錄型別]欄位中所選的記錄型別，欄位將變為可用。 這些欄位是以[!DNL Salesforce] API為基礎。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL選擇要對應的欄位]</td> 
   <td> <p>選取建立新記錄時您希望模組設定的欄位。 必填欄位位於清單頂端。 </p> <p>您選取的欄位會在此欄位下方開啟。 您現在可以在這些欄位中輸入值。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 讀取記錄]

此動作模組會從[!DNL Salesforce]中的單一物件讀取資料。

您指定記錄的ID。

模組會傳回記錄ID及任何關聯欄位，連同連線存取的任何自訂欄位和值。 您可以在情境中的後續模組中對應此資訊。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr>
    <td>[！UICONTROL Connection]</td>
   <td> <p>如需有關將您的[!DNL Salesforce]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與[!DNL Adobe Workfront Fusion]的連線 — 基本指示</a>。</p> </td> 
  </tr> 
  <tr>
    <td>[！UICONTROL記錄型別]</td>
    <td>選取您希望模組[action].read的[!DNL Salesforce]記錄型別。</td>
  </tr> 
  <tr>
    <td>[！UICONTROL記錄欄位]</td>
    <td>選取您希望模組讀取的欄位。 您必須至少選取一個欄位。</td>
  </tr> 
  <tr>
    <td>[！UICONTROL ID]</td>
    <td> <p>輸入或對應您要模組讀取之記錄的唯一[!DNL Salesforce]識別碼。</p> <p>若要取得ID，請在瀏覽器中開啟[!DNL Salesforce]物件，並複製URL結尾處最後一個正斜線(/)之後的文字。 例如： <code>https://eu5.salesforce.com/&lt;object ID&gt;</code></p> </td>
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 刪除記錄]

此動作模組會刪除物件中的現有記錄。

您指定記錄的ID。

模組會傳回記錄ID及任何關聯欄位，連同連線存取的任何自訂欄位和值。 您可以在情境中的後續模組中對應此資訊。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection]</td> 
   <td> <p>如需有關將您的[!DNL Salesforce]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與[!DNL Adobe Workfront Fusion]的連線 — 基本指示</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL記錄型別] </td> 
   <td> <p>選取您要模組刪除的[!DNL Salesforce]記錄型別。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL ID]</td> 
   <td> <p>輸入或對應您要模組刪除之記錄的唯一[!DNL Salesforce]識別碼。</p> <p>若要取得ID，請在瀏覽器中開啟[!DNL Salesforce]物件，並複製URL結尾處最後一個正斜線(/)之後的文字。 例如： <code>https://eu5.salesforce.com/&lt;object ID&gt;</code></p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 自訂API呼叫]

此動作模組可讓您對[!DNL Salesforce] API進行自訂的已驗證呼叫。 如此一來，您就可以建立其他[!DNL Salesforce]模組無法完成的資料流程自動化。

模組傳回以下內容：

* **[!UICONTROL 狀態碼]** （數字）：這表示您的HTTP要求成功或失敗。 這些是您可在網際網路上查閱的標準程式碼。
* **[!UICONTROL Headers]** （物件）：與輸出本文無關之回應/狀態代碼的更詳細內容。 並非顯示在回應標題中的所有標題都是回應標題，因此某些標題可能對您並不實用。

  回應標題取決於您在設定模組時選擇的HTTP請求。

* **[!UICONTROL 內文]** （物件）：根據您在設定模組時所選擇的HTTP要求，您可能會收到一些傳回的資料。 該資料(例如[!UICONTROL GET]請求的資料)包含在此物件中。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>如需有關將您的[!DNL Salesforce]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與[!DNL Adobe Workfront Fusion]的連線 — 基本指示</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL URL]</p> </td> 
   <td> <p>輸入相對於<code> &lt;Instance URL&gt;/services/data/v46.0/</code>的路徑。</p> <p>如需可用端點的清單，請參閱<a href="https://developer.salesforce.com/docs/atlas.en-us.api_rest.meta/api_rest/intro_what_is_rest_api.htm">Salesforce REST API開發人員指南</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL方法]</p> </td> 
   td&gt; <p>選取設定API呼叫所需的HTTP要求方法。 如需詳細資訊，請參閱[!DNL Adobe Workfront Fusion]</a>中的<a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP要求方法。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Headers]</td> 
   <td> <p>以標準JSON物件的形式新增要求的標頭。例如，<code>{"Content-type":"application/json"}</code>。 Workfront Fusion會為您新增授權標頭。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL查詢字串]</td> 
   <td> <p>以標準JSON物件的形式新增API呼叫的查詢。例如： <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Body]</td> 
   <td> <p>以標準JSON物件的形式新增API呼叫的內文內容。</p> <p>注意：  <p>在JSON中使用條件陳述式（例如<code>if</code>）時，請將引號放在條件陳述式之外。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**範例：**&#x200B;下列API呼叫傳回您[!DNL Salesforce]帳戶中的所有使用者清單：
>
>* **URL**： `query`
>
>* **方法**： [!UICONTROL GET]
>
>* **查詢字串**：
>
>* **索引鍵**： `q`
>
>* **值**： `SELECT Id, Name, CreatedDate, LastModifiedDate FROM User LIMIT 10`
>
>在&#x200B;**[!UICONTROL 組合] > [!UICONTROL 內文] > [!UICONTROL 記錄]**&#x200B;下的模組輸出中，可找到搜尋的相符專案。
>
>在我們的範例中，傳回6個使用者：
>
>![](assets/matches-of-the-search-350x573.png)


#### [!UICONTROL 上傳附件/檔案]

此動作模組會上傳檔案並將其附加至您指定的記錄，或上傳檔案。

模組會傳回附件或檔案的ID以及任何關聯欄位，連同連線存取的任何自訂欄位和值。 您可以在情境中的後續模組中對應此資訊。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection]</td> 
   <td> <p>如需有關將您的[!DNL Salesforce]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與[!DNL Adobe Workfront Fusion]的連線 — 基本指示</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL上傳型別]</td> 
   <td>選取您要模組上傳附件還是檔案。</td> 
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
   <td>[！UICONTROL Source檔案]</td> 
   <td>從先前的模組中選取來源檔案，或對應來源檔案的名稱和資料。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 下載附件/檔案]

此動作模組會從記錄下載檔案或附件。

您可以指定記錄的ID以及您想要的下載型別。

模組會傳回附件或檔案的ID以及任何關聯欄位，連同連線存取的任何自訂欄位和值。 您可以在情境中的後續模組中對應此資訊。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr>
    <td>[！UICONTROL Connection]</td>
   <td> <p>如需有關將您的[!DNL Salesforce]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與[!DNL Adobe Workfront Fusion]的連線 — 基本指示</a>。</p> </td> 
  </tr> 
  <tr>
    <td>[！UICONTROL下載型別]</td>
    <td> <p>指定您要從Salesforce下載的檔案型別。</p> 
     <ul> 
      <li>[！UICONTROL附件]</li> 
      <li>[！UICONTROL檔案]</li> 
      <li>[！UICONTROL ContentDocument] （這是已在[!DNL Saleforce CRM Content]或[!DNL Salesforce Files]中上傳至檔案庫的檔案）。</li> 
     </ul> </td>
  </tr> 
  <tr>
    <td> <p>[！UICONTROL ID] / </p> <p>[！UICONTROL附件ID] / </p> <p>[！UICONTROL ContentDocument ID]</p> </td>
    <td> <p>輸入或對應您要模組下載之記錄的唯一[!DNL Salesforce]識別碼。</p> <p>若要取得ID，請在瀏覽器中開啟[!DNL Salesforce]物件，並複製URL結尾處最後一個正斜線(/)之後的文字。 例如： <code>https://eu5.salesforce.com/&lt;object ID&gt;</code></p> </td>
  </tr> 
 </tbody> 
</table>


#### [!UICONTROL 更新記錄]

此動作模組會編輯物件中的記錄。

模組可讓您選取可在模組中取得哪些物件欄位。 這可減少設定模組時必須捲動瀏覽的欄位數。

模組會傳回記錄ID及任何關聯欄位，連同連線存取的任何自訂欄位和值。 您可以在情境中的後續模組中對應此資訊。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection]</td> 
   <td> <p>如需有關將您的[!DNL Salesforce]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與[!DNL Adobe Workfront Fusion]的連線 — 基本指示</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL ID]</td> 
   <td>輸入或對應您要更新的記錄ID。</td> 
  </tr> 
  <tr> 
   <td> <p>[！UICONTROL記錄型別] </p> </td> 
   <td> <p>選取您希望模組更新的[!DNL Salesforce]記錄型別。 根據在「記錄型別」欄位中選取的記錄型別，欄位將變為可用。 這些欄位是以[!DNL Salesforce] API為基礎。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL選擇要對應的欄位]</td> 
   <td> <p>選取建立新記錄時您希望模組設定的欄位。 必填欄位位於清單頂端。 </p> <p>您選取的欄位會在此欄位下方開啟。 您現在可以在這些欄位中輸入值。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 搜尋

#### [!UICONTROL 使用查詢搜尋]

此搜尋模組會在[!DNL Salesforce]中尋找符合您指定之搜尋查詢的物件記錄。 您可以在情境中的後續模組中對應此資訊。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection]</td> 
   <td> <p>如需有關將您的[!DNL Salesforce]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與[!DNL Adobe Workfront Fusion]的連線 — 基本指示</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL搜尋型別]</td> 
   <td> <p>選取您要模組執行的搜尋型別：</p> 
    <ul> 
     <li> <p>[！UICONTROL Simple]</p> </li> 
     <li> <p>使用SOSL (Salesforce物件搜尋語言)的[！UICONTROL]</p> </li> 
     <li> <p>使用SOQL (Salesforce物件查詢語言)的[！UICONTROL]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td> <p>[！UICONTROL型別] </p> </td> 
   <td> <p>如果您選取簡單搜尋型別，請選擇您要模組搜尋的[!DNL Salesforce]記錄型別。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL Query] / [！UICONTROL SOSL Query] / [！UICONTROL SOQL Query]</td> 
   <td> <p>輸入搜尋依據的查詢。</p> <p>如需有關SOSL的詳細資訊，請參閱[!DNL Salesforce]檔案中的<a href="https://developer.salesforce.com/docs/atlas.en-us.soql_sosl.meta/soql_sosl/sforce_api_calls_sosl.htm">Salesforce物件搜尋語言(SOSL)</a>。</p> <p>如需有關SOQL的詳細資訊，請參閱[!DNL Salesforce]檔案中的<a href="https://developer.salesforce.com/docs/atlas.en-us.soql_sosl.meta/soql_sosl/sforce_api_calls_soql.htm">Salesforce物件查詢語言(SOQL)</a>。</p> <p>注意：請注意，引數<code>RETURNING </code>的值會影響模組的輸出。 如果您使用<code>LIMIT</code>，[!DNL Fusion]將會忽略[！UICONTROL最大記錄計數]欄位中的設定。 如果您未設定任何限制，Fusion將會插入值[！UICONTROL LIMIT =最大記錄計數]。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL最大記錄數]</td> 
   <td> <p>輸入或對應您希望模組在每個案例執行週期中傳回的最大記錄數。</p> </td> 
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
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td>如需有關將您的[!DNL Salesforce]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與[!DNL  Adobe Workfront Fusion]的連線 — 基本指示</a></td> 
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
