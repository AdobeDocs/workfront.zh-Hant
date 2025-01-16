---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: 聯結器
navigation-topic: apps-and-their-modules
title: Google工作表模組
description: Adobe Workfront Fusion檔案已移至新位置。 本文已棄用，但包含新文章的連結，內容涵蓋此功能。
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 11d62222-df34-472d-93d7-f0d53eb95c9b
source-git-commit: efbe888d370e20c895dc40f18f999f2d01ec6337
workflow-type: tm+mt
source-wordcount: '4085'
ht-degree: 0%

---

# [!DNL Google Sheets]模組

>[!IMPORTANT]
>
>Adobe Workfront Fusion檔案已移至新位置。
>
>本文資訊可在以下文章中找到：
>
>* [Google工作表模組](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/google-sheets-modules.html)
>
>請更新任何書籤。
>
>本文已不再更新，將於不久將來移除。

在[!DNL Adobe Workfront Fusion]案例中，您可以自動化使用[!DNL Google Sheets]的工作流程，並將其連線至多個協力廠商應用程式和服務。

如需有關將您的[!DNL Google Sheets]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱[建立連線到 [!DNL Adobe Workfront Fusion]  — 基本指示](../../workfront-fusion/connections/connect-to-fusion-general.md)

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

若要使用[!UICONTROL Google工作表]模組，您必須有[!UICONTROL Google]帳戶。

## Google Sheets API資訊

Google Sheets聯結器使用下列專案：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">基礎URL</td> 
   <td> https://sheets.googleapis.com/v4</td> 
  </tr> 
  <tr> 
   <td role="rowheader">API版本</td> 
   <td> v4 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">API標籤</td> 
   <td>v2.5.7</td> 
  </tr>
 </tbody> 
 </table>

## 觸發程序

### [!UICONTROL 觀看列]

從試算表中每個新新增的列擷取值。

模組只會擷取之前未填入的新列。 觸發器不會處理覆寫的列。

>[!IMPORTANT]
>
>如果工作表包含空白列，則不會處理空白列之後的列。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection] </td> 
   <td> <p>如需有關將您的[!DNL Google Sheets]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中建立案例一文中的<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連線到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Spreadsheet] </td> 
   <td> <p>選取包含您要觀看之表格的試算表。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL工作表] </td> 
   <td> <p>選取要監視新列的工作表。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL表格包含標題]</td> 
   <td> <p> 選取試算表是否包含標題列。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL是]</strong> </p> <p>模組不會將標題列擷取為輸出資料。 </p> <p>輸出中的變數名稱由標題呼叫。</p> </li> 
     <li> <p><strong>[！UICONTROL號碼]</strong> </p> <p>模組也會擷取第一個表格列</p> <p>輸出中的變數名稱稱為A、B、C、D等等。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL含標題列] </td> 
   <td> <p>輸入頁首列的範圍。 例如，<code>A1:F1</code>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL第一個表格列]</td> 
   <td> <p>輸入表格第一列的範圍。 例如，<code>A1:F1</code>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL值演算選項]</p> </td> 
   <td> <p style="font-weight: bold;">[！UICONTROL格式值]</p> <p>將根據儲存格的格式在回覆中計算並格式化值。 格式設定是以試算表的地區設定為基礎，而非請求使用者的地區設定。 例如，如果<code>A1</code>是<code>1.23</code>，<code>A2</code>是<code>=A1</code>且已格式化為貨幣，則<code>A2</code>會傳回<code>"$1.23"</code>。</p> <p style="font-weight: bold;">[！UICONTROL未格式化的值]</p> <p>系統會計算值，但不會在回覆中設定格式。 例如，如果<code>A1</code>是<code>1.23</code>，<code>A2</code>是<code>=A1</code>且已格式化為貨幣，則<code>A2</code>會傳回數字<code>"1.23"</code>。</p> <p style="font-weight: bold;">[！UICONTROL公式]</p> <p>將不會計算值。 回覆將包含公式。 例如，如果<code>A1</code>是<code>1.23</code>，<code>A2</code>是<code>=A1</code>且已格式化為貨幣，則<code>A2</code>會傳回<code>"=A1"</code>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL日期和時間轉譯選項]</p> </td> 
   <td> <p style="font-weight: bold;">[！UICONTROL序號]</p> <p>指示date、time、datetime和duration欄位以「序號」格式輸出為兩倍，如Lotus 1-2-3所普及。 值的整數部分（小數點左側）計算自1899年12月30日以來的天數。 小數部分（小數點右側）會將時間計為一天中的小數。 例如，1900年1月1日中午是2.5、2，因為是在1899年12月30日之後的2天，而。5，因為中午是半天。 1900年2月1日下午3點會是33.625。這正確將1900年視為閏年。</p> <p style="font-weight: bold;">[！UICONTROL格式字串]</p> <p>指示日期、時間、日期時間和持續時間欄位，以指定的數字格式（視試算表的地區設定而定）輸出為字串。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制] </td> 
   <td> <p>設定[!DNL Workfront Fusion]在一個執行週期內可處理的最大結果數量。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 動作

* [[!UICONTROL 新增列]](#add-a-row)
* [[!UICONTROL 更新列]](#update-a-row)
* [[!UICONTROL 清除列]](#clear-a-row)
* [[!UICONTROL 刪除列]](#delete-a-row)
* [[!UICONTROL 取得儲存格]](#get-a-cell)
* [[!UICONTROL 更新儲存格]](#update-a-cell)
* [[!UICONTROL 清除儲存格]](#clear-a-cell)
* [[!UICONTROL 新增工作表]](#add-a-sheet)
* [[!UICONTROL 建立試算表]](#create-a-spreadsheet)
* [[!UICONTROL 刪除工作表]](#delete-a-sheet)
* [[!UICONTROL 進行API呼叫]](#make-an-api-call)

### [!UICONTROL 新增列]

此模組會附加一列至工作表。

當您設定[!DNL Google Sheets]模組時，[!DNL Workfront Fusion]會顯示下列欄位。 除了這些欄位以外，可能還會顯示其他[!DNL Google Sheets]欄位，視您在應用程式或服務中的存取層級等因素而定。 模組中的粗體標題表示必填欄位。

如果您在欄位或函式上方看到對應按鈕，則可以使用它來設定該欄位的變數和函式。 如需詳細資訊，請參閱[在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md)中將資訊從一個模組對應到另一個模組。

![](assets/map-toggle-350x74.png)

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection] </td> 
   <td> <p>如需有關將您的[!DNL Google Sheets]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中建立案例一文中的<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連線到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL模式]</td> 
   <td> <p>選取您要手動選取試算表與工作表，還是透過對應。</p> <p>附註：例如在[!DNL Workfront Fusion]案例中建立新的試算表，而您想要直接在案例中新增資料到新建立的試算表時，手動對應就很實用。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL Spreadsheet] </td> 
   <td> <p>選取[!DNL Google]試算表。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL工作表] </td> 
   <td> <p>選取要新增列的頁面。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL欄範圍]</td> 
   <td>選取您要使用的欄範圍。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL表格包含標題]</td> 
   <td> <p> 選取試算表是否包含標題列。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL是]</strong> </p> <p>模組不會將標題列擷取為輸出資料。 </p> <p>輸出中的變數名稱由標題呼叫。</p> </li> 
     <li> <p><strong>[！UICONTROL號碼]</strong> </p> <p>模組也會擷取第一個表格列</p> <p>輸出中的變數名稱稱為A、B、C、D等等。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL值] </td> 
   <td> <p>在要新增的資料列中，輸入或對應所需的儲存格。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL值輸入選項]</td> 
   <td> 
    <ul> 
     <li> <p><strong>[！UICONTROL使用者已進入]</strong></p> <p>這些值會剖析為使用者在UI中輸入。 數字仍為數字，但字串可能會根據透過[!DNL Google Sheets] UI在儲存格中輸入文字時所套用的相同規則，轉換為數字、日期或其他格式。</p> </li> 
     <li> <p><strong>[！UICONTROL Raw]</strong> </p> <p> 使用者輸入的值不會剖析並依原樣儲存。 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL插入資料選項]</td> 
   <td> <p>指定輸入新資料時如何變更現有資料。 </p> 
    <ul> 
     <li> <p><strong>[！UICONTROL插入列]</strong></p> <p>會為新資料插入列。</p> </li> 
     <li> <p><strong>[！UICONTROL覆寫]</strong> </p> <p>新資料會覆寫其寫入區域中的現有資料。 將資料加入工作表結尾會插入新的列或欄，以便寫入資料。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 更新列]

此模組可讓您變更所選列中的儲存格內容。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection] </td> 
   <td> <p>如需有關將您的[!DNL Google Sheets]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中建立案例一文中的<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連線到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL模式]</td> 
   <td> <p>選取您要手動選取試算表與工作表，還是透過對應。</p> <p>注意：例如在[！UICONTROL Workfront Fusion]情境中建立新試算表時，而您想要直接在情境中新增資料至新建立的試算表時，手動對應就相當實用。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL Spreadsheet] </td> 
   <td> <p>選取[!DNL Google]試算表。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL工作表] </td> 
   <td> <p>選取要更新資料列的工作表。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL列號]</td> 
   <td> <p> 輸入您要更新的資料列編號。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL表格包含標題]</td> 
   <td> <p> 選取試算表是否包含標題列。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL是]</strong> </p> <p>模組不會將標題列擷取為輸出資料。 </p> <p>輸出中的變數名稱由標題呼叫。</p> </li> 
     <li> <p><strong>[！UICONTROL號碼]</strong> </p> <p>模組也會擷取第一個表格列</p> <p>輸出中的變數名稱稱為A、B、C、D等等。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL值] </td> 
   <td> <p>輸入值或將值對應至要變更（更新）之列的所需儲存格。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL值輸入選項]</td> 
   <td> 
    <ul> 
     <li> <p><strong>[！UICONTROL使用者已進入]</strong></p> <p>這些值會剖析為使用者在UI中輸入。 數字仍為數字，但字串可能會根據透過[!DNL Google Sheets] UI在儲存格中輸入文字時所套用的相同規則，轉換為數字、日期或其他格式。</p> </li> 
     <li> <p><strong>[！UICONTROL Raw]</strong> </p> <p> 使用者輸入的值不會剖析並依原樣儲存。 </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 清除列]

從指定的列刪除值。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection] </td> 
   <td> <p>如需有關將您的[!DNL Google Sheets]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中建立案例一文中的<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連線到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL Spreadsheet] </td> 
   <td> <p>選取包含您要清除資料列之工作表的[!DNL Google]試算表。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL工作表] </td> 
   <td> <p> 選取您要清除其資料的工作表。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL列號]</td> 
   <td> <p>輸入您要清除資料的資料列編號。 例如，<code> 23</code>。</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 刪除列]

刪除指定的列。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection] </td> 
   <td> <p>如需有關將您的[!DNL Google Sheets]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中建立案例一文中的<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連線到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL Spreadsheet] </td> 
   <td> <p>選取包含您要刪除列之工作表的Google試算表。</p> </td> 
  </tr> 
  <tr> 
   <td>表 </td> 
   <td> <p>選取您要從中刪除資料列的頁面。</p> </td> 
  </tr> 
  <tr> 
   <td>列號</td> 
   <td> <p>輸入要刪除的列數。 範例： <code>23</code></p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 取得儲存格]

從選取的儲存格擷取值。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection] </td> 
   <td> <p>如需有關將您的[!DNL Google Sheets]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中建立案例一文中的<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連線到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL Spreadsheet] </td> 
   <td> <p>選取[!DNL Google]試算表。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL工作表] </td> 
   <td> <p>選取包含您要擷取資料之儲存格的工作表。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL儲存格] </td> 
   <td> <p>輸入您要擷取資料的儲存格識別碼。 範例： <code>A6</code></p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL值演算選項]</td> 
   <td> <p style="font-weight: bold;">[！UICONTROL格式值]</p> <p>將根據儲存格的格式在回覆中計算並格式化值。 格式設定是以試算表的地區設定為基礎，而非請求使用者的地區設定。 例如，如果<code>A1</code>是<code>1.23</code>，<code>A2</code>是<code>=A1</code>且已格式化為貨幣，則<code>A2</code>會傳回<code>"$1.23"</code>。</p> <p style="font-weight: bold;">[!DNL Unformatted value]</p> <p>系統會計算值，但不會在回覆中設定格式。 例如，如果<code>A1</code>是<code>1.23</code>，<code>A2</code>是<code>=A1</code>且已格式化為貨幣，則<code>A2</code>會傳回數字<code>"1.23"</code>。</p> <p style="font-weight: bold;">[!DNL Formula]</p> <p>將不會計算值。 回覆將包含公式。 例如，如果<code>A1</code>是<code>1.23</code>，<code>A2</code>是<code>=A1</code>且已格式化為貨幣，則<code>A2</code>會傳回<code>"=A1"</code>。</p> </td> 
  </tr> 
  <tr> 
   <td>[!DNL Date and time render option]</td> 
   <td> <p style="font-weight: bold;">[!DNL Serial number]</p> <p>指示date、time、datetime和duration欄位以「序號」格式輸出為兩倍，如Lotus 1-2-3所普及。 值的整數部分（小數點左側）計算自1899年12月30日以來的天數。 小數部分（小數點右側）會將時間計為一天中的小數。 例如，1900年1月1日中午是2.5、2，因為是在1899年12月30日之後的2天，而。5，因為中午是半天。 1900年2月1日下午3點會是33.625。這正確將1900年視為閏年。</p> <p style="font-weight: bold;">[!DNL Formatted string]</p> <p>指示日期、時間、日期時間和持續時間欄位，以指定的數字格式（視試算表的地區設定而定）輸出為字串。</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 更新儲存格]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection] </td> 
   <td> <p>如需有關將您的[!DNL Google Sheets]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中建立案例一文中的<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連線到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL Spreadsheet] </td> 
   <td> <p>選取[!DNL Google]試算表。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL儲存格] </td> 
   <td> <p>輸入要更新的儲存格識別碼。 範例： <code>A5</code></p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL值]</td> 
   <td> <p>輸入儲存格的新值。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL值輸入選項]</td> 
   <td> 
    <ul> 
     <li> <p><strong>[！UICONTROL使用者已進入]</strong></p> <p>這些值會剖析為使用者在UI中輸入。 數字仍為數字，但字串可能會根據透過[!DNL Google Sheets] UI在儲存格中輸入文字時所套用的相同規則，轉換為數字、日期或其他格式。</p> </li> 
     <li> <p><strong>[！UICONTROL Raw]</strong> </p> <p> 使用者輸入的值不會剖析並依原樣儲存。 </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 清除儲存格]

刪除指定儲存格的值。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection] </td> 
   <td> <p>如需有關將您的[!DNL Google Sheets]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中建立案例一文中的<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連線到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL Spreadsheet] </td> 
   <td> <p>選取包含您要清除儲存格之工作表的Google試算表。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL工作表] </td> 
   <td> <p>選取您要清除儲存格的頁面。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL儲存格] </td> 
   <td> <p>輸入您要清除的儲存格識別碼。 範例： <code>A5</code>。</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 新增工作表]

在選取的試算表中建立新工作表。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection] </td> 
   <td> <p>如需有關將您的[!DNL Google Sheets]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中建立案例一文中的<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連線到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL Spreadsheet] </td> 
   <td> <p>選取您要新增工作表的Google試算表。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL屬性]</td> 
   <td> 
    <ul> 
     <li> <p style="font-weight: bold;">[！UICONTROL標題]</p> <p>輸入新頁面的名稱。</p> </li> 
     <li> <p style="font-weight: bold;">[！UICONTROL Index]</p> <p>輸入頁面位置。 預設值為0 （將頁面放在第一位）</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 建立試算表]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection] </td> 
   <td> <p>如需有關將您的[!DNL Google Sheets]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中建立案例一文中的<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連線到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL標題] </td> 
   <td> <p>輸入新試算表的名稱。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL Locale]</td> 
   <td> <p>以下列格式之一輸入試算表的地區設定：</p> 
    <ul> 
     <li>ISO 639-1語言代碼，例如 <code>en</code></li> 
     <li>ISO 639-2語言代碼，例如<code>haw</code> （如果沒有639-1代碼）</li> 
     <li>ISO語言代碼和國家/地區代碼的組合，例如 <code>en_US</code></li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL重新計算間隔]</td> 
   <td> <p>重新計算易失性函式之前要等待的時間量：</p> <p style="font-weight: bold;">[！UICONTROL變更時]</p> <p>每次變更時，都會更新易失性函式。</p> <p style="font-weight: bold;">[！UICONTROL開啟變更且每分鐘]</p> <p>易失性函式會在每一次變更和每分鐘更新一次。</p> <p style="font-weight: bold;">[！UICONTROL變更時每小時]</p> <p>揮發性函式會在每次變更時每小時更新。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL時區]</td> 
   <td> <p> 選取試算表的時區。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL數字格式]</td> 
   <td> <p>選取試算表中所有儲存格的預設格式。</p> <p><strong>[！UICONTROL文字]</strong>：文字格式設定。 範例： <code>1000. 12</code></p> <p><strong>[！UICONTROL Number]</strong>：數字格式。 範例： <code>1,000.12</code></p> <p><strong>[！UICONTROL Percent]</strong>：百分比格式。 範例： <code>10. 12%</code></p> <p><strong>[！UICONTROL貨幣]</strong>：貨幣格式。 範例： <code>$1,000.12</code></p> <p><strong>[！UICONTROL日期]</strong>：日期格式。 範例： <code>9/26/2008</code></p> <p><strong>[！UICONTROL時間]</strong>：時間格式。 範例： <code>3:59:00 PM</code></p> <p><strong>[！UICONTROL日期時間]</strong>：日期與時間格式。 範例： <code>9/26/08 15:59:00</code> </p> <p><strong>[！UICONTROL Scientific]</strong>科學數字格式。 範例： <code>1. 01E+03</code></p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL工作表] </td> 
   <td> <p>按一下<strong>[！UICONTROL新增]</strong>，將工作表新增至試算表。 對於每個頁面，輸入或對應頁面的標題和頁面的索引。 0的索引代表第一個工作表。</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 刪除工作表]

刪除特定工作表。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection] </td> 
   <td> <p>如需有關將您的[!DNL Google Sheets]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中建立案例一文中的<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連線到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL Spreadsheet] </td> 
   <td> <p>選取[!DNL Google]試算表。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL工作表] </td> 
   <td> <p>選取您要刪除的頁面。</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 進行API呼叫]

此動作模組可讓您執行自訂API呼叫。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>如需有關將您的[Fusion App]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">建立與[!DNL Adobe Workfront Fusion]的連線 — 基本指示</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL URL]</p> </td> 
   <td>輸入相對於<code>https://sheets.googleapis.com/v4/</code>的路徑。</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL方法]</p> </td> 
   <td> <p>選取設定API呼叫所需的HTTP要求方法。 如需詳細資訊，請參閱[!DNL Adobe Workfront Fusion]</a>中的<a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">HTTP要求方法。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Headers]</td> 
   <td> <p>以標準JSON物件的形式新增要求的標頭。例如，<code>{"Content-type":"application/json"}</code>。 [!DNL Workfront Fusion]為您新增授權標頭。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL查詢字串]</td> 
   <td> <p> 以標準JSON物件的形式新增API呼叫的查詢。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Body]</td> 
   <td> <p>以標準JSON物件的形式新增API呼叫的內文內容。</p> <p>注意：   <p>在JSON中使用條件陳述式（例如<code>if</code>）時，請將引號放在條件陳述式之外。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>">  
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

## 搜尋

* [[!UICONTROL 搜尋列]](#search-rows)
* [[!UICONTROL 搜尋列（進階）]](#search-rows-advanced)
* [[!UICONTROL 取得範圍值]](#get-range-values)
* [[!UICONTROL 清單工作表]](#list-sheets)

### [!UICONTROL 搜尋列]

使用篩選選項來搜尋列。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection] </td> 
   <td> <p>如需有關將您的[Fusion App]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">建立與[!DNL Adobe Workfront Fusion]的連線 — 基本指示</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL Spreadsheet] </td> 
   <td> <p>選取[!DNL Google]試算表。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL工作表] </td> 
   <td> <p>選取要搜尋資料列的工作表。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL表格包含標題]</td> 
   <td> <p> 選取試算表是否包含標題列。 如果選取[！UICONTROL是]選項，模組不會擷取標題列做為輸出資料，而輸出中的變數名稱隨後由標題呼叫。 如果選取了[！UICONTROL否]選項，模組也會擷取第一個表格列，然後輸出中的變數名稱就只稱為A、B、C、D等。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL欄範圍]</td> 
   <td>選取要使用的欄範圍。 範例： <code>A-F</code></td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL篩選器]</td> 
   <td> <p>設定要搜尋之列的篩選器。</p> <p>如需有關篩選器的詳細資訊，請參閱<a href="../../workfront-fusion/scenarios/add-a-filter-to-a-scenario.md" class="MCXref xref">在[！UICONTROL Adobe Workfront Fusion]</a>中將篩選器新增到情境。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL排序順序]</td> 
   <td>選取您要遞增排序還是遞減排序。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL Order by]</td> 
   <td>選擇您要作為排序依據的欄。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL值演算選項]</td> 
   <td> <p style="font-weight: bold;">[！UICONTROL格式值]</p> <p>將根據儲存格的格式在回覆中計算並格式化值。 格式設定是以試算表的地區設定為基礎，而非請求使用者的地區設定。 例如，如果<code>A1</code>是<code>1.23</code>，<code>A2</code>是<code>=A1</code>且已格式化為貨幣，則<code>A2</code>會傳回<code>"$1.23"</code>。</p> <p style="font-weight: bold;">[！UICONTROL未格式化的值]</p> <p>系統會計算值，但不會在回覆中設定格式。 例如，如果<code>A1</code>是<code>1.23</code>，<code>A2</code>是<code>=A1</code>且已格式化為貨幣，則<code>A2</code>會傳回數字<code>"1.23"</code>。</p> <p style="font-weight: bold;">[！UICONTROL公式]</p> <p>將不會計算值。 回覆將包含公式。 例如，如果<code>A1</code>是<code>1.23</code>，<code>A2</code>是<code>=A1</code>且已格式化為貨幣，則<code>A2</code>會傳回<code>"=A1"</code>。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL日期和時間轉譯選項]</td> 
   <td> <p style="font-weight: bold;">[！UICONTROL序號]</p> <p>指示date、time、datetime和duration欄位輸出為Lotus 1-2-3所推廣的「序號」格式的雙面。 值的整數部分（小數點左側）計算自1899年12月30日以來的天數。 小數部分（小數點右側）會將時間計為一天中的小數。 例如，1900年1月1日中午是2.5、2，因為是在1899年12月30日之後的2天，而。5，因為中午是半天。 1900年2月1日下午3點會是33.625。這正確將1900年視為閏年。</p> <p style="font-weight: bold;">[！UICONTROL格式字串]</p> <p>指示日期、時間、日期時間和持續時間欄位，以指定的數字格式（視試算表的地區設定而定）輸出為字串。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL傳回資料列數目上限]</td> 
   <td>設定[!DNL Workfront Fusion]在一個執行週期內傳回的最大列數。</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 搜尋列（進階）]

傳回符合指定准則的結果。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection] </td> 
   <td> <p>如需有關將您的[!DNL Google Sheets]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中建立案例一文中的<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連線到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL Spreadsheet] </td> 
   <td> <p>選取包含您要搜尋之工作表的Google試算表。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL工作表] </td> 
   <td> <p>選取包含要搜尋之資料列的工作表。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL Query]</td> 
   <td> <p>使用[!DNL Google Charts Query Language]。 範例： <code>select * where B = "John"</code></p> <p>如需[!DNL Google Charts Query Language]的詳細資訊，請參閱[!DNL Google]檔案中的<a href="https://developers.google.com/chart/interactive/docs/querylanguage">查詢語言參考</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 取得範圍值]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection] </td> 
   <td> <p>如需有關將您的[!DNL Google Sheets]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中建立案例一文中的<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連線到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL Spreadsheet] </td> 
   <td> <p>選取[!DNL Google]試算表。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL工作表] </td> 
   <td> <p>選取您要取得範圍內容的工作表。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL範圍] </td> 
   <td> <p>輸入您要取得的範圍。 範例： <code>A1:D25</code>。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL表格包含標題]</td> 
   <td> <p>如果工作表有標題列，請核取此方塊</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL含標題列]</td> 
   <td>輸入表格標題的範圍。 範例<code>A1:F1</code>。 如果您將欄位留空，[!DNL Workfront Fusion]會假設標題在指定範圍的第一列。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL值演算選項]</td> 
   <td> <p style="font-weight: bold;">[！UICONTROL格式值]</p> <p>將根據儲存格的格式在回覆中計算並格式化值。 格式設定是以試算表的地區設定為基礎，而非請求使用者的地區設定。 例如，如果<code>A1</code>是<code>1.23</code>，<code>A2</code>是<code>=A1</code>且已格式化為貨幣，則<code>A2</code>會傳回<code>"$1.23"</code>。</p> <p style="font-weight: bold;">[！UICONTROL未格式化的值]</p> <p>系統會計算值，但不會在回覆中設定格式。 例如，如果<code>A1</code>是<code>1.23</code>，<code>A2</code>是<code>=A1</code>且已格式化為貨幣，則<code>A2</code>會傳回數字<code>"1.23"</code>。</p> <p style="font-weight: bold;">[！UICONTROL公式]</p> <p>將不會計算值。 回覆將包含公式。 例如，如果<code>A1</code>是<code>1.23</code>，<code>A2</code>是<code>=A1</code>且已格式化為貨幣，則<code>A2</code>會傳回<code>"=A1"</code>。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL日期和時間轉譯選項]</td> 
   <td> <p style="font-weight: bold;">[！UICONTROL序號]</p> <p>指示date、time、datetime和duration欄位輸出為Lotus 1-2-3所推廣的「序號」格式的雙面。 值的整數部分（小數點左側）計算自1899年12月30日以來的天數。 小數部分（小數點右側）會將時間計為一天中的小數。 例如，1900年1月1日中午是2.5、2，因為是在1899年12月30日之後的2天，而。5，因為中午是半天。 1900年2月1日下午3點會是33.625。這正確將1900年視為閏年。</p> <p style="font-weight: bold;">[！UICONTROL格式字串]</p> <p>指示日期、時間、日期時間和持續時間欄位，以指定的數字格式（視試算表的地區設定而定）輸出為字串。</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 清單工作表]

此模組會傳回試算表中所有工作表的清單。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection] </td> 
   <td> <p>如需有關將您的[!DNL Google Sheets]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中建立案例一文中的<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連線到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL Spreadsheet] </td> 
   <td> <p>選取包含您要列出工作表的[!DNL Google]試算表。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 使用量限制

如果發生錯誤`429: RESOURCE_EXHAUSTED`，表示您已超過API速率限制。

[!DNL Google Sheets] API限制每個專案每100秒500個要求，每個使用者每100秒100個要求。 讀取和寫入限制會個別追蹤。 沒有每日使用量限制。

如需詳細資訊，請參閱[developers.google.com/sheets/api/limits](https://developers.google.com/sheets/api/limits)。

## 提示與秘訣

* [如何從 [!DNL Google] 工作表取得空白儲存格](#how-to-get-empty-cells-from-a-google-sheet)
* [在工作表中新增按鈕以執行案例](#add-a-button-in-a-sheet-to-run-a-scenario)

### 如何從[!DNL Google Sheet]取得空白儲存格

使用[!UICONTROL 搜尋列（進階）]模組並使用此公式來取得空白欄。
<pre>選取*，其中E為Null</pre>其中，「E」為欄，「為null」為條件。 您可以使用[Google Query Lang](https://developers.google.com/chart/interactive/docs/querylanguage)建立更進階的查詢。

### 在工作表中新增按鈕以執行案例

1. 在[!DNL Workfront Fusion]中，在情境中插入&#x200B;**[!UICONTROL Webhook]** > **[!UICONTROL 自訂Webhook]**&#x200B;模組/觸發器，並加以設定（請參閱[Webhooks](../../workfront-fusion/apps-and-their-modules/webhooks-updated.md)）。

1. 複製webhook的URL。
1. 執行情境。
1. 在Google工作表中，從主功能表列選擇&#x200B;**[!UICONTROL 插入]** > **[!UICONTROL 繪圖]**...。

1. 在[!UICONTROL 繪圖]視窗中，按一下視窗頂端附近的&#x200B;**[!UICONTROL 文字方塊]**&#x200B;圖示![](assets/text-box.png)。
1. 設計按鈕並按一下右上角的&#x200B;**[!UICONTROL 儲存並關閉]**&#x200B;按鈕：
1. 此按鈕將會放置在您的工作表中。 按一下按鈕右上角的三個垂直點：
1. 選擇&#x200B;**[!UICONTROL 指派指令碼……]。功能表中的**。
1. 輸入指令碼（函式）的名稱，例如`runScenario`，然後按一下&#x200B;**[!UICONTROL 確定]**：
1. 從主功能表列選擇&#x200B;**[!UICONTROL 工具]** > **[!UICONTROL 指令碼編輯器]**。

1. 插入下列程式碼：

   * 函式的名稱必須對應到您在步驟9中指定的名稱。
   * 將URL取代為您在步驟2中複製的webhook URL。

     <pre>函式runScenario() {</pre><pre>UrlFetchApp.fetch("&lt;webhook you copied&gt;")；</pre><pre>}</pre>

1. 按&#x200B;**[!UICONTROL Ctrl+S]**&#x200B;儲存指令碼檔案，輸入專案名稱並按一下&#x200B;**[!UICONTROL 確定]**。

1. 切換回[!DNL Google Sheets]並按一下您的新按鈕。
1. 將所需的授權授與指令碼：
1. 在[!DNL Workfront Fusion]中，確認案例已成功執行。

## 將日期儲存在試算表中

如果您將「日期」值儲存在沒有任何格式的試算表中，該值會在試算表中以ISO 8601格式顯示為文字。 但是，使用日期的[!DNL Google Sheets]公式或函式若不瞭解此文字（範例：公式`=A1+10`），將會顯示下列錯誤：

![](assets/mceclip6-350x87.png)

為協助讓[!DNL Google Sheets]瞭解日期，請使用[[!UICONTROL formatDate] (date； format； [timezone])](../../workfront-fusion/functions/date-and-time-functions.md#formatda)函式將其格式化。 傳遞給函式做為第二個引數的正確格式，取決於試算表的地區設定。

若要判斷正確的格式：

1. 從主功能表選擇&#x200B;**[!UICONTROL 檔案]** > **[!UICONTROL 試算表]**&#x200B;設定以驗證/設定地區設定。

1. 驗證/設定適當的地區設定後，請從主功能表中選擇&#x200B;**[!UICONTROL 格式]** > **[!UICONTROL 數字]**&#x200B;來決定對應的日期和時間格式。 格式會顯示在日期時間功能表專案旁：

1. 若要撰寫應傳遞至[!UICONTROL formatDate()]函式的正確格式，請參閱[Token清單，以瞭解 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/tokens-for-date-and-time-formatting.md)中的日期和時間格式。

**範例：**&#x200B;美國地區設定使用`MM/DD/YYYY HH:mm:ss`格式：

![](assets/locale-time-350x83.png)

## 正在利用[!DNL Google Sheets]功能

如果您遺漏內建功能，但此功能是由[!DNL Google Sheets]所提供，則您可以加以利用。 如需詳細資訊，請參閱[使用 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/map-using-functions.md)中的函式對映專案中的[使用 [!DNL Google Sheets] 函式](../../workfront-fusion/functions/map-using-functions.md#exploiti)。

## 保留[!DNL Google Sheets]不要將數字變更為日期

您可能會發現您當作文字使用的數字字串正在解譯為[!DNL Google]工作表中的日期。 例如，您輸入1-2019，打算將它當作文字，但Google將其解譯為日期。 您可以預先將數字格式設定為純文字以防止此情況發生。

1. 在[!DNL Google Sheets]中，反白顯示包含數字的欄或儲存格。
1. 按一下&#x200B;**[!UICONTROL 格式]** > **[!UICONTROL 數字]** > **[!UICONTROL 純文字]**。

[!DNL Workfront Fusion]中的另一個因應措施是在數字前輸入撇號(&#39;)，例如，&#39;1-2019或&#39;1/47。 從[!DNL Workfront Fusion]傳送資料後，儲存格中不會顯示單引號。
