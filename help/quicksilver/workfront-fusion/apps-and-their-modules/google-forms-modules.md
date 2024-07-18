---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: 聯結器
navigation-topic: apps-and-their-modules
title: Google Forms模組
description: ' [!DNL Adobe Workfront Fusion Google Forms] 模組可讓您在您的Google Forms上監視、選擇、新增、更新或刪除回應。'
author: Becky
feature: Workfront Fusion
exl-id: 45c86879-bc4e-4134-b63c-02410b9de43b
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1420'
ht-degree: 0%

---

# [!DNL Google Forms]模組

[!DNL Adobe Workfront Fusion] [!DNL Google Forms]模組可讓您監視、選取、新增、更新或刪除您的[!DNL Google Forms]回應。

若要搭配[!DNL Adobe Workfront Fusion]使用[!DNL Google Docs]，必須有[!DNL Google]帳戶。 如果您還沒有[!DNL Google]帳戶，您可以在[!DNL Google]帳戶說明頁面建立一個帳戶。

如果您需要有關建立案例的指示，請參閱[在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md)中建立案例。

如需模組的相關資訊，請參閱 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md)中的[模組。

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
   <p>目前產品需求：如果您有[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Adobe Workfront]計畫，您的組織必須購買[!DNL Adobe Workfront Fusion]及[!DNL Adobe Workfront]，才能使用本文所述的功能。 [!DNL Workfront Fusion]包含在[！UICONTROL Ultimate] [!DNL Workfront]計畫中。</p>
   <p>或</p>
   <p>舊版產品需求：您的組織必須購買[!DNL Adobe Workfront Fusion]及[!DNL Adobe Workfront]，才能使用本文所述的功能。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的[!DNL Workfront]管理員。

如需[!DNL Adobe Workfront Fusion]授權的相關資訊，請參閱[[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md)。

## 先決條件

若要使用[!DNL Google Forms]模組，您必須有[!DNL Google]帳戶。

## 從表單建立試算表

若要使用您的表單回應，必須建立回應的試算表。

1. 開啟您的表單。
1. 移至&#x200B;**[!UICONTROL 回應]**&#x200B;標籤。
1. 按一下&#x200B;**[!UICONTROL 建立試算表]**&#x200B;圖示![](assets/spreadsheet-icon.png)。

1. 選取您要建立新的試算表或現有的試算表
1. 按一下「**[!UICONTROL 建立]**」。

## [!DNL Google Forms]模組及其欄位

當您設定[!DNL Google Forms]模組時，[!DNL Workfront Fusion]會顯示下列欄位。 除了這些欄位以外，可能還會顯示其他[!DNL Google Forms]欄位，視您在應用程式或服務中的存取層級等因素而定。 模組中的粗體標題表示必填欄位。

如果您在欄位或函式上方看到對應按鈕，則可以使用它來設定該欄位的變數和函式。 如需詳細資訊，請參閱[在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md)中將資訊從一個模組對應到另一個模組。

![](assets/map-toggle-350x74.png)

* [觸發器](#triggers)
* [動作](#actions)
* [搜尋](#searches)

### 觸發器

#### [!UICONTROL 觀看回應]

監視表單以取得新回應。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>如需有關將您的[!DNL Google]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中建立案例一文中的<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連線到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Spreadsheet]</td> 
   <td> <p>選取試算表，其中包含您要監視新回應的表單回應。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL工作表]</td> 
   <td> <p> 選取包含表單回應的工作表。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL含標題列]</td> 
   <td>指定表格的標頭列。 預設列為<code>A1:Z1</code>。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL值演算選項]</td> 
   <td> <p>指定要在輸出中呈現值的方式。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL格式化值]</strong> </p> <p>系統會根據儲存格的格式，在回覆中計算值並設定格式。 格式設定是以試算表的地區設定為基礎，而非請求使用者的地區設定。 例如，如果<code>A1</code>是<code>1. 23</code>，<code>A2 </code>是<code>=A1</code>且已格式化為貨幣，則<code>A2</code>會傳回<code>$1. 23</code>。</p> </li> 
     <li> <p><strong>[！UICONTROL未格式化的值]</strong> </p> <p>系統會計算值，但不會在回覆中設定格式。 例如，如果<code>A1</code>是<code>1. 23</code>，<code>A2 </code>是<code>=A1</code>且已格式化為貨幣，則<code>A2</code>會傳回數字<code>1. 23</code> 。</p> </li> 
     <li> <p><strong>[！UICONTROL公式]</strong> </p> <p>不會計算值。 回覆包含公式。 例如，如果<code>A1</code>是<code>1. 23</code>，<code>A2 </code>是<code>=A1</code>且已格式化為貨幣，則<code>A2</code>會傳回<code>=A1</code>。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL日期和時間轉譯選項]</td> 
   <td>選取要在輸出中呈現的日期、時間和持續時間。 如果[！UICONTROL Value Render Option]設定為[！UICONTROL格式值]，則會忽略此欄位。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制]</td> 
   <td> <p> 設定[!DNL Workfront Fusion]在一個週期內處理的最大回應數。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 動作

* [[!UICONTROL 新增回應]](#add-a-response)
* [[!UICONTROL 更新回應]](#update-a-response)
* [[!UICONTROL 刪除回應]](#delete-a-response)

#### [!UICONTROL 新增回應]

此模組會將新回應附加至表單試算表底部。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>如需有關將您的[!DNL Google]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中建立案例一文中的<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連線到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Spreadsheet]</td> 
   <td> <p>選取包含您要新增回應之工作表的工作表。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL工作表]</td> 
   <td> <p> 選取包含表單回應的工作表。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[！UICONTROL值]</p> </td> 
   <td> <p>在工作表欄中輸入所需的值。</p> <p>若為正確格式的[！UICONTROL Timestamp]欄，請使用下列值：</p><pre>formatDate（現在；DD/MM/YYYY HH：mm；UTC）</pre> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[！UICONTROL值輸入選項]</td> 
   <td> 
    <ul> 
     <li> <p><strong>[！UICONTROL Raw]</strong> </p> <p> 使用者輸入的值不會剖析並依原樣儲存。 </p> </li> 
     <li> <p><strong>[！UICONTROL使用者已進入]</strong></p> <p>這些值會剖析為使用者在UI中輸入。 數字仍為數字，但字串可能會根據透過[!DNL Google Sheets] UI在儲存格中輸入文字時所套用的相同規則，轉換為數字、日期或其他格式。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[！UICONTROL插入資料選項]</td> 
   <td> <p>指定輸入新資料時如何變更現有資料。 </p> 
    <ul> 
     <li> <p><strong>[！UICONTROL覆寫]</strong> </p> <p>新資料會覆寫其寫入區域中的現有資料。 將資料加入工作表結尾會插入新的列或欄，以便寫入資料。</p> </li> 
     <li> <p><strong>[！UICONTROL插入列]</strong></p> <p>會為新資料插入列。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 更新回應]

此模組會更新選取的回應。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>如需有關將您的[!DNL Google]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中建立案例一文中的<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連線到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Spreadsheet]</td> 
   <td> <p>選取包含您要更新回應的工作表試算表。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL工作表]</td> 
   <td> <p> 選取包含表單回應的工作表。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL列號]</p> </td> 
   <td> <p>輸入或對應您要更新的資料列編號。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL值]</p> </td> 
   <td> <p>在所需欄中輸入新值。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[！UICONTROL值輸入選項]</td> 
   <td> 
    <ul> 
     <li> <p><strong>[！UICONTROL Raw]</strong> </p> <p> 使用者輸入的值不會剖析並依原樣儲存。 </p> </li> 
     <li> <p><strong>[！UICONTROL使用者已進入]</strong></p> <p>這些值會剖析為使用者在UI中輸入。 數字仍為數字，但字串可能會根據透過[!DNL Google Sheets] UI在儲存格中輸入文字時所套用的相同規則，轉換為數字、日期或其他格式。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 刪除回應]

此模組會刪除選取的回應。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>如需有關將您的[!DNL Google]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中建立案例一文中的<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連線到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Spreadsheet]</td> 
   <td> <p>選取包含您要刪除回應之工作表的工作表。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL工作表]</td> 
   <td> <p> 選取包含表單回應的工作表。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL列號]</p> </td> 
   <td> <p>輸入或對應您要刪除的列編號。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 搜尋

* [[!UICONTROL 搜尋回應]](#search-responses)
* [[!UICONTROL 搜尋回應（進階]）](#search-responses-advanced)

#### [!UICONTROL 搜尋回應]

此模組會傳回符合指定條件的回應。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
    <td>連接</td>
   <td> <p>如需有關將您的[!DNL Google]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中建立案例一文中的<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連線到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
    <td>[！UICONTROL Spreadsheet]</td>
   <td> <p>選取您要搜尋的表單。</p> </td> 
  </tr> 
  <tr data-mc-conditions="">
    <td>[！UICONTROL工作表] </td>
   <td> <p>選取包含表單回應的工作表。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
    <td>[！UICONTROL欄範圍]</td>
   <td> <p> 選取您要搜尋的欄範圍。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[！UICONTROL篩選器]</td> 
   <td> <p>定義您要搜尋回應依據的篩選器。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
    <td>[！UICONTROL排序順序] </td>
   <td> <p>選取要以遞增或遞減順序來排序傳回的回應。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
    <td>[！UICONTROL Order By]</td>
   <td> <p> 選取要排序傳回回回回應的資料行。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[！UICONTROL值演算選項]</td> 
   <td> <p>指定要在輸出中呈現值的方式。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL格式值]</strong></p> <p>系統會根據儲存格的格式，在回覆中計算值並設定格式。 格式設定是以試算表的地區設定為基礎，而非請求使用者的地區設定。 例如，如果<code>A1</code>是<code>1. 23</code>，<code>A2 </code>是<code>=A1</code>且已格式化為貨幣，則<code>A2</code>會傳回<code>$1. 23</code>。</p> </li> 
     <li> <p><strong>[！UICONTROL未格式化的值]</strong> </p> <p>系統會計算值，但不會在回覆中設定格式。 例如，如果<code>A1</code>是<code>1. 23</code>，<code>A2 </code>是<code>=A1</code>且已格式化為貨幣，則<code>A2</code>會傳回數字<code>1. 23</code> 。</p> </li> 
     <li> <p><strong>[！UICONTROL公式]</strong> </p> <p>不會計算值。 回覆包含公式。 例如，如果<code>A1</code>是<code>1. 23</code>，<code>A2 </code>是<code>=A1</code>且已格式化為貨幣，則<code>A2</code>會傳回<code>=A1</code>。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions="">
    <td>[！UICONTROL日期和時間轉譯選項]</td>
    <td>選取要在輸出中呈現的日期、時間和持續時間。 如果[！UICONTROL Value Render]選項設為「格式化值」，則會忽略此欄位。 </td>
  </tr> 
  <tr>
    <td role="rowheader" data-mc-conditions="QuicksilverOrClassic.Draft mode">[！UICONTROL傳回回回回應的最大數目]</td>
   <td> <p> 設定[!DNL Workfront Fusion]在一個週期內傳回的回應數上限。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 搜尋回應（進階）]

此模組使用[[!DNL Google Charts Query Language]](https://developers.google.com/chart/interactive/docs/querylanguage)執行搜尋。 此模組未傳回列號。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
    <td>[！UICONTROL Connection]</td>
   <td> <p>如需有關將您的[!DNL Google]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中建立案例一文中的<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連線到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr>
    <td>[！UICONTROL Spreadsheet]</td>
   <td> <p>選取包含您要搜尋之工作表的試算表。</p> </td> 
  </tr> 
  <tr>
    <td>[！UICONTROL工作表]</td>
   <td> <p> 選取包含表單回應的工作表。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL篩選器]</td> 
   <td> <p>使用<a href="https://developers.google.com/chart/interactive/docs/querylanguage">[!DNL Google Charts Query Language]</a>定義搜尋查詢。</p> <p>範例： <code>select * where C = "John"</code>會擷取C欄為"John"的資料列的所有值。</p> </td> 
  </tr> 
  <tr>
    <td>[！UICONTROL傳回資料列數目上限]</td>
   <td> <p> 設定[!DNL Workfront Fusion]在一個週期內傳回的回應數上限。</p> </td> 
  </tr> 
 </tbody> 
</table>
