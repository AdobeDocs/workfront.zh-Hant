---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 連接器
navigation-topic: apps-and-their-modules
title: Salesforce模組
description: 在Adobe Workfront Fusion案例中，您可以自動執行使用Salesforce的工作流程，並將其連接至多個協力廠商應用程式和服務。
author: Becky
feature: Workfront Fusion
exl-id: 3c8adcd9-fb5f-400d-9edd-6d9fc30cc728
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '2720'
ht-degree: 0%

---

# [!DNL Salesforce] 模組

在Adobe Workfront Fusion案例中，您可以自動執行使用 [!DNL Salesforce]，並將其連接至多個協力廠商應用程式和服務。

如果您需要建立案例的相關指示，請參閱 [在中建立案例 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

如需模組的相關資訊，請參閱 [中的模組 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

>[!NOTE]
>
>* 並非所有版本 [!DNL Salesforce] 擁有API存取權。 如需詳細資訊，請參閱 [!DNL Salesforce] 在 [!DNL Salesforce] 社群網站。
>* 如需從 [!DNL Salesforce] API，請參閱 [!DNL Salesforce] API檔案。 您也可以檢查 [!DNL Salesforce] API，用於任何可能的服務中斷。
>


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

使用 [!DNL Salesforce] 模組，您必須 [!DNL Salesforce] 帳戶。

## 關於搜尋 [!DNL Salesforce] 物件

在搜索對象時，您可以輸入單個搜索詞或使用通配符和運算子建立更複雜的查詢：

* 使用星號萬用字元(\*)取代零個或多個字元。 例如，搜索Ca\*會查找以Ca開頭的項目
* 使用問號萬用字元(?) 取代單一字元。 例如，搜尋Jo?n會找到詞語為John或Joan但不是Jon的項目
* 使用引號運算子(&quot; &quot;)來尋找完全相符的片語。 例如：&quot;星期一會議&quot;

如需搜尋可能性的詳細資訊，請參閱 [!DNL Salesforce] 有關SOQL和SOSL的開發人員文檔。

## [!DNL Salesforce] 模組及其欄位

* [觸發器](#triggers)
* [動作](#actions)
* [搜尋](#searches)

### 觸發器

* [[!UICONTROL 關注記錄]](#watch-for-records)
* [[!UICONTROL 觀看傳出訊息]](#watch-outbound-messages)
* [[!UICONTROL 觀看欄位]](#watch-a-field)

#### [!UICONTROL 關注記錄]

建立或更新物件中的記錄時，此觸發模組會執行案例。 模組會傳回與記錄或記錄相關聯的所有標準欄位，以及連線存取的任何自訂欄位和值。 您可以在案例的後續模組中對應此資訊。

設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL Salesforce] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL類型] </td> 
   <td> <p>選取 [!DNL Salesforce] 記錄您要讓模組觀看的項目。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL記錄欄位]</td> 
   <td>選取您要模組監看的欄位。 可用欄位取決於記錄類型。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL記錄的最大計數]</td> 
   <td> <p>輸入或映射您希望模組在每個方案執行週期中返回的最大記錄數。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Watch]</td> 
   <td> <p>確定是否希望方案只監視所選類型的新記錄，還是僅監視所選類型的新記錄以及對該類型記錄的所有其他更改。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 觀看傳出訊息]

此觸發器模組會在有人傳送訊息時執行案例。 模組會傳回與記錄或記錄相關聯的所有標準欄位，以及連線存取的任何自訂欄位和值。 您可以在案例的後續模組中對應此資訊。

此模組需要一些額外設定：

1. 前往 [!DNL Salesforce] 設定頁面。

   若要存取設定頁面，請找到並按一下標示為「 」的按鈕[!UICONTROL 設定]」 [!DNL Salesforce] 帳戶。 從 [!DNL Salesforce] 設定頁面，找到「[!UICONTROL 快速查找/搜索]欄。 搜索「[!UICONTROL 工作流程規則].&quot;

1. 按一下 **[!UICONTROL 工作流程規則]**.
1. 在 [!UICONTROL 工作流程規則] 頁面，按一下 **[!UICONTROL 新規則]** 並選取規則要套用的物件類型(例如「[!UICONTROL 機會]「如果您正在監視Opportunity記錄的更新)。
1. 按一下 **[!UICONTROL 下一個]**.
1. 設定規則名稱、評估標準和規則標準，然後按一下 **[!UICONTROL 儲存]** 和 **[!UICONTROL 下一個]**.

1. 按一下 **[!UICONTROL 完成]**.
1. 在新建立的工作流規則中，按一下 **[!UICONTROL 編輯]**...
1. 從 **[!UICONTROL 添加工作流操作]** 下拉清單，選擇 **[!UICONTROL 新的傳出訊息]**.

1. 指定名稱、說明、端點URL以及要包含在新傳出訊息中的欄位，然後按一下 **[!UICONTROL 儲存]**.

   此 **[!UICONTROL 端點URL]** 欄位包含 [!DNL Salesforce] [!UICONTROL 傳出訊息] in [!DNL Workfront Fusion].

1. 設定以開頭的案例 [!UICONTROL 傳出訊息] 事件。

1. 按一下 **&lt;/>** 圖示，並複製提供的URL。
1. 返回 **[!UICONTROL 工作流程規則]** 頁面，找到新建立的規則，然後按一下 **[!UICONTROL 啟動]**.

設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Webhook]</td> 
   <td> <p>選取您要用來監視傳出訊息的網頁連結。 若要新增網頁連結，請按一下 <strong>[!UICONTROL添加]</strong> 並輸入webhook的名稱和連接。</p> <p>有關連接 [!DNL Salesforce] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與[!UICONTROL Adobe Workfront Fusion]的連接 — 基本說明</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL記錄類型] </td> 
   <td> <p>選取 [!DNL Salesforce] 記錄您希望模組監視傳出郵件。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL欄位]</td> 
   <td> <p>選擇希望模組監視傳出郵件的欄位。 可用欄位取決於記錄類型。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### *[!UICONTROL 觀看欄位]*

此觸發模組會在 [!DNL Salesforce].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL Salesforce] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL記錄類型] </td> 
   <td> <p>選取包含您要模組監看之欄位的記錄類型。 必須選擇已開啟[!UICONTROL欄位歷史記錄]的記錄類型 [!DNL Salesforce] 設定。 如需詳細資訊，請參閱 <a href="https://help.salesforce.com/articleView?id=tracking_field_history.htm&amp;type=5">欄位歷史記錄追蹤</a> 在 [!DNL Salesforce] 檔案。 </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL欄位]</td> 
   <td> <p>選取您要讓模組監看變更的欄位。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL限制]</td> 
   <td> <p>輸入或映射您希望模組在每個方案執行週期期間返回的最大欄位數。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 動作

* [[!UICONTROL 建立記錄]](#create-a-record)
* [[!UICONTROL 閱讀記錄]](#read-a-record)
* [[!UICONTROL 刪除記錄]](#delete-a-record)
* [[!UICONTROL 自訂API呼叫]](#custom-api-call)
* [[!UICONTROL 上載附件/文檔]](#upload-attachmentdocument)
* [[!UICONTROL 下載附件/文檔]](#download-attachmentdocument)

#### [!UICONTROL 建立記錄]

此動作模組會在物件中建立新記錄。

模組可讓您選取模組中可用的物件欄位。 如此可減少設定模組時必須捲動的欄位數。

模組會傳回記錄和任何相關欄位的ID，以及連線存取的任何自訂欄位和值。 您可以在案例的後續模組中對應此資訊。

設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL Salesforce] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL記錄類型] </p> </td> 
   <td> <p>選取 [!DNL Salesforce] 記錄您要建立模組。 根據在[!UICONTROL記錄類型]欄位中選擇的記錄類型，欄位可供使用。 這些欄位是以 [!DNL Salesforce] API。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL選擇要映射的欄位]</td> 
   <td> <p>選擇建立新記錄時要模組配置的欄位。 必填欄位位於清單頂端。 </p> <p>您選取的欄位在此欄位下方開啟。 您現在可以在這些欄位中輸入值。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 閱讀記錄]

此動作模組會從中的單一物件讀取資料 [!DNL Salesforce].

您指定記錄的ID。

模組會傳回記錄和任何相關欄位的ID，以及連線存取的任何自訂欄位和值。 您可以在案例的後續模組中對應此資訊。

設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr>
    <td>[!UICONTROL連接]</td>
   <td> <p>有關連接 [!DNL Salesforce] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr>
    <td>[!UICONTROL記錄類型]</td>
    <td>選取 [!DNL Salesforce] 記錄您要讓模組執行[action].read。</td>
  </tr> 
  <tr>
    <td>[!UICONTROL記錄欄位]</td>
    <td>選取您要模組讀取的欄位。 您至少必須選取一個欄位。</td>
  </tr> 
  <tr>
    <td>[!UICONTROL ID]</td>
    <td> <p>輸入或對應唯一 [!DNL Salesforce] 您要模組讀取的記錄ID。</p> <p>若要取得ID，請開啟 [!DNL Salesforce] 物件，並複製URL結尾處最後一個斜線(/)的文字。 例如： <code>https://eu5.salesforce.com/&lt;object ID&gt;</code></p> </td>
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 刪除記錄]

此動作模組會刪除物件中的現有記錄。

您指定記錄的ID。

模組會傳回記錄和任何相關欄位的ID，以及連線存取的任何自訂欄位和值。 您可以在案例的後續模組中對應此資訊。

設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL Salesforce] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL記錄類型] </td> 
   <td> <p>選取 [!DNL Salesforce] 記錄您要刪除模組。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID]</td> 
   <td> <p>輸入或對應唯一 [!DNL Salesforce] 您要刪除模組的記錄ID。</p> <p>若要取得ID，請開啟 [!DNL Salesforce] 物件，並複製URL結尾處最後一個斜線(/)的文字。 例如： <code>https://eu5.salesforce.com/&lt;object ID&gt;</code></p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 自訂API呼叫]

此動作模組可讓您對 [!DNL Salesforce] API。 這樣，您就可以建立資料流自動化，而另一個無法完成 [!DNL Salesforce] 模組。

模組會傳回下列內容：

* **[!UICONTROL 狀態代碼]** （數字）:這表示HTTP要求是否成功。 這些是標準代碼，你可以在網際網路上查找。
* **[!UICONTROL 標題]** （對象）:與輸出內文無關之回應/狀態代碼的更詳細內容。 並非所有顯示在回應標題中的標題都是回應標題，因此有些標題可能對您沒有用。

   回應標題取決於您在設定模組時選擇的HTTP要求。

* **[!UICONTROL 主體]** （對象）:根據您在設定模組時選擇的HTTP要求，您可能會收到一些資料。 該資料，例如來自 [!UICONTROL GET] 請求。

設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL Salesforce] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td> <p>輸入相對於的路徑<code> &lt;Instance URL&gt;/services/data/v46.0/</code>.</p> <p>如需可用端點的清單，請參閱 <a href="https://developer.salesforce.com/docs/atlas.en-us.api_rest.meta/api_rest/intro_what_is_rest_api.htm">Salesforce REST API開發人員指南</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL方法]</p> </td> 
   td&gt; <p>選取設定API呼叫所需的HTTP要求方法。 如需詳細資訊，請參閱 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">中的HTTP要求方法 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL標題]</td> 
   <td> <p>以標準JSON物件的形式新增請求的標題。例如， <code>{"Content-type":"application/json"}</code>. Workfront Fusion會為您新增授權標頭。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL查詢字串]</td> 
   <td> <p>以標準JSON物件的形式新增API呼叫的查詢。例如： <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL正文]</td> 
   <td> <p>以標準JSON物件的形式新增API呼叫的內文內容。</p> <p>備註:  <p>使用條件陳述式時，例如 <code>if</code> 在JSON中，將引號放在條件陳述式之外。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**範例：** 下列API呼叫會傳回 [!DNL Salesforce] 帳戶：
>
>* **URL**: `query`
>
>* **方法**: [!UICONTROL GET]
>
>* **查詢字串**:
>
>* **金鑰**: `q`
>
>* **值**: `SELECT Id, Name, CreatedDate, LastModifiedDate FROM User LIMIT 10`
>
>如需搜尋的相符項目，請在模組的「輸出」下方找到 **[!UICONTROL 捆綁] > [!UICONTROL 主體] > [!UICONTROL 記錄]**.
>
>在我們的範例中，傳回6個使用者：
>
>![](assets/matches-of-the-search-350x573.png)


#### [!UICONTROL 上載附件/文檔]

此動作模組會上傳檔案並將其附加至您指定的記錄，或上傳檔案。

模組會傳回附件或檔案的ID以及任何相關欄位，以及連線存取的任何自訂欄位和值。 您可以在案例的後續模組中對應此資訊。

設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL Salesforce] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL上載類型]</td> 
   <td>選擇要模組上載附件還是文檔。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID]</td> 
   <td>輸入或映射要上載附件的對象的ID。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL資料夾]</td> 
   <td>選取包含您要模組上傳之檔案的資料夾。 </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL源檔案]</td> 
   <td>從上一個模組中選擇源檔案，或映射源檔案的名稱和資料。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 下載附件/文檔]

此操作模組從記錄下載文檔或附件。

您可指定記錄的ID以及所需的下載類型。

模組會傳回附件或檔案的ID以及任何相關欄位，以及連線存取的任何自訂欄位和值。 您可以在案例的後續模組中對應此資訊。

設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr>
    <td>[!UICONTROL連接]</td>
   <td> <p>有關連接 [!DNL Salesforce] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr>
    <td>[!UICONTROL下載類型]</td>
    <td> <p>指定要從Salesforce下載的檔案類型。</p> 
     <ul> 
      <li>[!UICONTROL附件]</li> 
      <li>[!UICONTROL文檔]</li> 
      <li>[!UICONTROL ContentDocument](此文檔已上載到中的庫 [!DNL Saleforce CRM Content] 或 [!DNL Salesforce Files].)</li> 
     </ul> </td>
  </tr> 
  <tr>
    <td> <p>[!UICONTROL ID] / </p> <p>[!UICONTROL附件ID] / </p> <p>[!UICONTROL ContentDocument ID]</p> </td>
    <td> <p>輸入或對應唯一 [!DNL Salesforce] 您要下載模組的記錄ID。</p> <p>若要取得ID，請開啟 [!DNL Salesforce] 物件，並複製URL結尾處最後一個斜線(/)的文字。 例如： <code>https://eu5.salesforce.com/&lt;object ID&gt;</code></p> </td>
  </tr> 
 </tbody> 
</table>


#### [!UICONTROL 更新記錄]

此動作模組會編輯物件中的記錄。

模組可讓您選取模組中可用的物件欄位。 如此可減少設定模組時必須捲動的欄位數。

模組會傳回記錄和任何相關欄位的ID，以及連線存取的任何自訂欄位和值。 您可以在案例的後續模組中對應此資訊。

設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL Salesforce] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID]</td> 
   <td>輸入或映射要更新的記錄ID。</td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL記錄類型] </p> </td> 
   <td> <p>選取 [!DNL Salesforce] 記錄您要更新模組。 根據在「記錄類型」欄位中選擇的記錄類型，欄位可供使用。 這些欄位是以 [!DNL Salesforce] API。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL選擇要映射的欄位]</td> 
   <td> <p>選擇建立新記錄時要模組配置的欄位。 必填欄位位於清單頂端。 </p> <p>您選取的欄位在此欄位下方開啟。 您現在可以在這些欄位中輸入值。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 搜尋

#### [!UICONTROL 使用查詢搜索]

此搜尋模組會在 [!DNL Salesforce] 符合您指定的搜尋查詢。 您可以在案例的後續模組中對應此資訊。

設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL Salesforce] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL搜索類型]</td> 
   <td> <p>選擇要模組執行的搜索類型：</p> 
    <ul> 
     <li> <p>[!UICONTROL簡單]</p> </li> 
     <li> <p>[!UICONTROL使用SOSL（Salesforce對象搜索語言）]</p> </li> 
     <li> <p>[!UICONTROL使用SOQL（Salesforce對象查詢語言）]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL類型] </p> </td> 
   <td> <p>如果選擇了簡單搜索類型，請選擇 [!DNL Salesforce] 記錄您要模組搜尋的。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Query] / [!UICONTROL SOSL Query] / [!UICONTROL SOQL Query]</td> 
   <td> <p>輸入要搜索的查詢。</p> <p>有關SOSL的詳細資訊，請參閱 <a href="https://developer.salesforce.com/docs/atlas.en-us.soql_sosl.meta/soql_sosl/sforce_api_calls_sosl.htm">Salesforce物件搜尋語言(SOSL)</a> 在 [!DNL Salesforce] 檔案。</p> <p>有關SOQL的詳細資訊，請參見 <a href="https://developer.salesforce.com/docs/atlas.en-us.soql_sosl.meta/soql_sosl/sforce_api_calls_soql.htm">Salesforce對象查詢語言(SOQL)</a> 在 [!DNL Salesforce] 檔案。</p> <p>注意：請注意，參數的值 <code>RETURNING </code>會影響模組的輸出。 如果您使用 <code>LIMIT</code>, [!DNL Fusion] 將忽略[!UICONTROL記錄的最大計數]欄位中的設定。 如果未設定任何限制，則Fusion將插入值[!UICONTROL LIMIT =記錄的最大計數]。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL記錄的最大計數]</td> 
   <td> <p>輸入或映射您希望模組在每個方案執行週期中返回的最大記錄數。</p> </td> 
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
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td>有關連接 [!DNL Salesforce] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至[!DNL  Adobe Workfront Fusion]  — 基本指示</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL類型]</td> 
   <td> <p>選擇要搜索的對象類型。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL搜索條件]</td> 
   <td>選擇要搜索的欄位、要在查詢中使用的運算子，以及要在欄位中搜索的值。 您可以使用AND或OR連接查詢。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL輸出]</td> 
   <td>選取您要納入模組輸出的欄位。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL結果集]</td> 
   <td>選擇是否希望模組返回「所有匹配記錄」，還是僅返回「第一個匹配記錄」。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL最大]</td> 
   <td>輸入或映射您希望模組在每個方案執行週期中檢索的最大記錄數。</td> 
  </tr> 
 </tbody> 
</table>
