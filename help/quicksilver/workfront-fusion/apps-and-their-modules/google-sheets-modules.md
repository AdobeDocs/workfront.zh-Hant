---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: 連接器
navigation-topic: apps-and-their-modules
title: Google工作表模組
description: 為了使用 [!DNL Google Sheets] with [!DNL Adobe Workfront Fusion],you need the [!UICONTROL Workfront Fusion Google Sheets] 擴充功能（選用，但是立即觸發器需要）。
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 11d62222-df34-472d-93d7-f0d53eb95c9b
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '3894'
ht-degree: 0%

---

# [!DNL Google Sheets] 模組

在 [!DNL Adobe Workfront Fusion] 案例中，您可以自動執行使用 [!DNL Google Sheets]，並將其連接至多個協力廠商應用程式和服務。

有關連接 [!DNL Google Sheets] 帳戶 [!DNL Workfront Fusion]，請參閱 [建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示](../../workfront-fusion/connections/connect-to-fusion-general.md)

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

使用 [!UICONTROL Google工作表] 模組，您必須 [!UICONTROL Google] 帳戶。

## 觸發器

### [!UICONTROL 監視行]

從試算表中每新新增一列擷取值。

模組只會擷取以前未填入的新列。 觸發器不會處理被覆寫的列。

>[!IMPORTANT]
>
>如果工作表包含空白列，則不會處理空白列之後的任何列。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接] </td> 
   <td> <p>有關連接 [!DNL Google Sheets] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連接到 [!DNL Workfront Fusion]</a> 在文章中 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在中建立案例 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL電子錶格] </td> 
   <td> <p>選擇包含要監視的工作表的電子錶格。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL工作表] </td> 
   <td> <p>選擇要監視新行的工作表。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL表包含標題]</td> 
   <td> <p> 選取試算表是否包含標題列。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL是]</strong> </p> <p>模組不會擷取標題列作為輸出資料。 </p> <p>輸出中的變數名稱由標題呼叫。</p> </li> 
     <li> <p><strong>[!UICONTROL否]</strong> </p> <p>模組也會擷取第一個表格列</p> <p>輸出中的變數名稱為A、B、C、D等。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL帶標題的行] </td> 
   <td> <p>輸入標題行的範圍。 例如， <code>A1:F1</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL第一表行]</td> 
   <td> <p>輸入表格第一行的範圍。 例如， <code>A1:F1</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL值呈現選項]</p> </td> 
   <td> <p style="font-weight: bold;">[!UICONTROL格式化值]</p> <p>系統會根據儲存格的格式，在回覆中計算並格式化這些值。 格式設定是根據試算表的地區設定，而非要求使用者的地區設定。 例如，若 <code>A1</code> is <code>1.23</code> 和 <code>A2</code> is <code>=A1</code> 格式為貨幣，則 <code>A2</code> 會返回 <code>"$1.23"</code>.</p> <p style="font-weight: bold;">[!UICONTROL未格式化的值]</p> <p>系統將計算這些值，但不會在回覆中格式化。 例如，若 <code>A1</code> is <code>1.23</code> 和 <code>A2</code> is <code>=A1</code> 格式為貨幣，則 <code>A2</code> 會傳回 <code>"1.23"</code>.</p> <p style="font-weight: bold;">[!UICONTROL公式]</p> <p>將不會計算值。 回覆將包含公式。 例如，若 <code>A1</code> is <code>1.23</code> 和 <code>A2</code> is <code>=A1</code> 格式為貨幣，則 <code>A2</code> 會返回 <code>"=A1"</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL日期和時間呈現選項]</p> </td> 
   <td> <p style="font-weight: bold;">[!UICONTROL序列號]</p> <p>指示將日期、時間、日期時間和持續時間欄位以「序列號」格式雙倍輸出，如Lotus 1-2-3所推廣。 值的整數部分（小數點左側）會計算自1899年12月30日以來的天數。 小數部分（小數點的右側）會將時間計為當天的小數。 例如，1900年1月1日中午為2.5，因為是1899年12月30日後的2天，而0.5，因為中午是半天。 1900年2月1日下午3點將為33.625。這正確地將1900年視為不閏年。</p> <p style="font-weight: bold;">[!UICONTROL格式字串]</p> <p>指示日期、時間、日期時間和持續時間欄位以其指定數字格式（取決於電子錶格的地區設定）輸出為字串。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL限制] </td> 
   <td> <p>設定 [!DNL Workfront Fusion] 將在一個執行週期中運作。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 動作

* [[!UICONTROL 新增列]](#add-a-row)
* [[!UICONTROL 更新行]](#update-a-row)
* [[!UICONTROL 清除行]](#clear-a-row)
* [[!UICONTROL 刪除列]](#delete-a-row)
* [[!UICONTROL 獲取單元格]](#get-a-cell)
* [[!UICONTROL 更新儲存格]](#update-a-cell)
* [[!UICONTROL 清除儲存格]](#clear-a-cell)
* [[!UICONTROL 添加工作表]](#add-a-sheet)
* [[!UICONTROL 建立試算表]](#create-a-spreadsheet)
* [[!UICONTROL 刪除工作表]](#delete-a-sheet)
* [[!UICONTROL 進行API呼叫]](#make-an-api-call)

### [!UICONTROL 新增列]

此模組會附加一列至工作表。

設定時 [!DNL Google Sheets] 模組， [!DNL Workfront Fusion] 顯示下列欄位。 此外， [!DNL Google Sheets] 視您在應用程式或服務中的存取層級等因素而定，可能會顯示欄位。 模組中的粗體標題表示必填欄位。

如果您在欄位或函式上方看到對應按鈕，則可使用它來設定該欄位的變數和函式。 如需詳細資訊，請參閱 [將資訊從一個模組對應到 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL連接] </td> 
   <td> <p>有關連接 [!DNL Google Sheets] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連接到 [!DNL Workfront Fusion]</a> 在文章中 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在中建立案例 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL模式]</td> 
   <td> <p>選擇要手動選擇電子錶格和工作表還是通過映射選擇。</p> <p>注意：手動對應相當實用，例如當在 [!DNL Workfront Fusion] 情境中，而您想要直接在情境中新建立的試算表中新增資料。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL電子錶格] </td> 
   <td> <p>選取 [!DNL Google] 試算表。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL工作表] </td> 
   <td> <p>選擇要添加行的工作表。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL列範圍]</td> 
   <td>選取您要使用的欄範圍。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL表包含標題]</td> 
   <td> <p> 選取試算表是否包含標題列。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL是]</strong> </p> <p>模組不會擷取標題列作為輸出資料。 </p> <p>輸出中的變數名稱由標題呼叫。</p> </li> 
     <li> <p><strong>[!UICONTROL否]</strong> </p> <p>模組也會擷取第一個表格列</p> <p>輸出中的變數名稱為A、B、C、D等。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL值] </td> 
   <td> <p>輸入或映射您要新增的列的所需儲存格。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL值輸入選項]</td> 
   <td> 
    <ul> 
     <li> <p><strong>[!UICONTROL用戶輸入]</strong></p> <p>系統會將值剖析為使用者在UI中輸入值。 數字仍然是數字，但字串可以按照在透過 [!DNL Google Sheets] UI。</p> </li> 
     <li> <p><strong>[!UICONTROL Raw]</strong> </p> <p> 使用者輸入的值不會剖析，並依原樣儲存。 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL插入資料選項]</td> 
   <td> <p>指定輸入新資料時如何變更現有資料。 </p> 
    <ul> 
     <li> <p><strong>[!UICONTROL插入行]</strong></p> <p>會為新資料插入行。</p> </li> 
     <li> <p><strong>[!UICONTROL覆蓋]</strong> </p> <p>新資料會覆寫寫入區域中的現有資料。 將資料添加到工作表末尾將插入新行或列，以便寫入資料。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 更新行]

此模組可讓您變更所選列中的儲存格內容。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL連接] </td> 
   <td> <p>有關連接 [!DNL Google Sheets] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連接到 [!DNL Workfront Fusion]</a> 在文章中 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在中建立案例 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL模式]</td> 
   <td> <p>選擇要手動選擇電子錶格和工作表還是通過映射選擇。</p> <p>注意：例如，在[!UICONTROL Workfront Fusion]案例中建立新試算表，且您想直接在案例中將資料新增至新建立的試算表時，手動對應就十分實用。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL電子錶格] </td> 
   <td> <p>選取 [!DNL Google] 試算表。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL工作表] </td> 
   <td> <p>選擇要更新行的工作表。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL行號]</td> 
   <td> <p> 輸入要更新的行數。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL表包含標題]</td> 
   <td> <p> 選取試算表是否包含標題列。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL是]</strong> </p> <p>模組不會擷取標題列作為輸出資料。 </p> <p>輸出中的變數名稱由標題呼叫。</p> </li> 
     <li> <p><strong>[!UICONTROL否]</strong> </p> <p>模組也會擷取第一個表格列</p> <p>輸出中的變數名稱為A、B、C、D等。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL值] </td> 
   <td> <p>輸入值，或將值對應至您要變更（更新）的列所需儲存格。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL值輸入選項]</td> 
   <td> 
    <ul> 
     <li> <p><strong>[!UICONTROL用戶輸入]</strong></p> <p>系統會將值剖析為使用者在UI中輸入值。 數字仍然是數字，但字串可以按照在透過 [!DNL Google Sheets] UI。</p> </li> 
     <li> <p><strong>[!UICONTROL Raw]</strong> </p> <p> 使用者輸入的值不會剖析，並依原樣儲存。 </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 清除行]

刪除指定行中的值。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL連接] </td> 
   <td> <p>有關連接 [!DNL Google Sheets] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連接到 [!DNL Workfront Fusion]</a> 在文章中 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在中建立案例 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL電子錶格] </td> 
   <td> <p>選取 [!DNL Google] 包含要清除行的工作表的電子錶格。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL工作表] </td> 
   <td> <p> 選擇要清除資料的工作表。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL行號]</td> 
   <td> <p>輸入要清除資料的行數。 例如， <code> 23</code>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 刪除列]

刪除指定的行。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL連接] </td> 
   <td> <p>有關連接 [!DNL Google Sheets] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連接到 [!DNL Workfront Fusion]</a> 在文章中 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在中建立案例 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL電子錶格] </td> 
   <td> <p>選取包含您要從中刪除列的工作表的Google試算表。</p> </td> 
  </tr> 
  <tr> 
   <td>表 </td> 
   <td> <p>選擇要從中刪除行的工作表。</p> </td> 
  </tr> 
  <tr> 
   <td>行號</td> 
   <td> <p>輸入要刪除的行數。 範例: <code>23</code></p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 獲取單元格]

從選取的儲存格擷取值。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL連接] </td> 
   <td> <p>有關連接 [!DNL Google Sheets] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連接到 [!DNL Workfront Fusion]</a> 在文章中 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在中建立案例 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL電子錶格] </td> 
   <td> <p>選取 [!DNL Google] 試算表。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL工作表] </td> 
   <td> <p>選擇包含要從中檢索資料的單元格的工作表。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL單元格] </td> 
   <td> <p>輸入要從中擷取資料的儲存格ID。 範例: <code>A6</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL值呈現選項]</td> 
   <td> <p style="font-weight: bold;">[!UICONTROL格式化值]</p> <p>系統會根據儲存格的格式，在回覆中計算並格式化這些值。 格式設定是根據試算表的地區設定，而非要求使用者的地區設定。 例如，若 <code>A1</code> is <code>1.23</code> 和 <code>A2</code> is <code>=A1</code> 格式為貨幣，則 <code>A2</code> 會返回 <code>"$1.23"</code>.</p> <p style="font-weight: bold;">[!DNL Unformatted value]</p> <p>系統將計算這些值，但不會在回覆中格式化。 例如，若 <code>A1</code> is <code>1.23</code> 和 <code>A2</code> is <code>=A1</code> 格式為貨幣，則 <code>A2</code> 會傳回 <code>"1.23"</code>.</p> <p style="font-weight: bold;">[!DNL Formula]</p> <p>將不會計算值。 回覆將包含公式。 例如，若 <code>A1</code> is <code>1.23</code> 和 <code>A2</code> is <code>=A1</code> 格式為貨幣，則 <code>A2</code> 會返回 <code>"=A1"</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!DNL Date and time render option]</td> 
   <td> <p style="font-weight: bold;">[!DNL Serial number]</p> <p>指示將日期、時間、日期時間和持續時間欄位以「序列號」格式雙倍輸出，如Lotus 1-2-3所推廣。 值的整數部分（小數點左側）會計算自1899年12月30日以來的天數。 小數部分（小數點的右側）會將時間計為當天的小數。 例如，1900年1月1日中午為2.5，因為是1899年12月30日後的2天，而0.5，因為中午是半天。 1900年2月1日下午3點將為33.625。這正確地將1900年視為不閏年。</p> <p style="font-weight: bold;">[!DNL Formatted string]</p> <p>指示日期、時間、日期時間和持續時間欄位以其指定數字格式（取決於電子錶格的地區設定）輸出為字串。</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 更新儲存格]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL連接] </td> 
   <td> <p>有關連接 [!DNL Google Sheets] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連接到 [!DNL Workfront Fusion]</a> 在文章中 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在中建立案例 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL電子錶格] </td> 
   <td> <p>選取 [!DNL Google] 試算表。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL單元格] </td> 
   <td> <p>輸入要更新的儲存格ID。 範例: <code>A5</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL值]</td> 
   <td> <p>輸入儲存格的新值。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL值輸入選項]</td> 
   <td> 
    <ul> 
     <li> <p><strong>[!UICONTROL用戶輸入]</strong></p> <p>系統會將值剖析為使用者在UI中輸入值。 數字仍然是數字，但字串可以按照在透過 [!DNL Google Sheets] UI。</p> </li> 
     <li> <p><strong>[!UICONTROL Raw]</strong> </p> <p> 使用者輸入的值不會剖析，並依原樣儲存。 </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 清除儲存格]

從指定的儲存格刪除值。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL連接] </td> 
   <td> <p>有關連接 [!DNL Google Sheets] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連接到 [!DNL Workfront Fusion]</a> 在文章中 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在中建立案例 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL電子錶格] </td> 
   <td> <p>選取包含您要清除儲存格之工作表的Google試算表。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL工作表] </td> 
   <td> <p>選擇要清除單元格的工作表。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL單元格] </td> 
   <td> <p>輸入要清除的儲存格ID。 範例: <code>A5</code>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 添加工作表]

在選定電子錶格中建立新工作表。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL連接] </td> 
   <td> <p>有關連接 [!DNL Google Sheets] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連接到 [!DNL Workfront Fusion]</a> 在文章中 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在中建立案例 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL電子錶格] </td> 
   <td> <p>選取您要新增工作表的Google試算表。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL屬性]</td> 
   <td> 
    <ul> 
     <li> <p style="font-weight: bold;">[!UICONTROL標題]</p> <p>輸入新工作表的名稱。</p> </li> 
     <li> <p style="font-weight: bold;">[!UICONTROL索引]</p> <p>輸入工作表位置。 預設值為0（將工作表放在首位）</p> </li> 
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
   <td>[!UICONTROL連接] </td> 
   <td> <p>有關連接 [!DNL Google Sheets] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連接到 [!DNL Workfront Fusion]</a> 在文章中 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在中建立案例 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL標題] </td> 
   <td> <p>輸入新試算表的名稱。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL地區]</td> 
   <td> <p>以下列格式之一輸入試算表的地區設定：</p> 
    <ul> 
     <li>ISO 639-1語言代碼，例如 <code>en</code></li> 
     <li>ISO 639-2語言代碼，例如 <code>haw</code>，如果不存在639-1代碼</li> 
     <li>ISO語言代碼和國家/地區代碼的組合，例如 <code>en_US</code></li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL重新計算間隔]</td> 
   <td> <p>重新計算易失函式之前的等待時間：</p> <p style="font-weight: bold;">[！更改時UICONTROL]</p> <p>每次變更時都會更新易失性函式。</p> <p style="font-weight: bold;">[!UICONTROL更改時和每分鐘]</p> <p>易失性函式會隨著每次變更和每分鐘更新。</p> <p style="font-weight: bold;">[!UICONTROL更改時和每小時]</p> <p>每次變更和每小時都會更新易失性函式。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL時區]</td> 
   <td> <p> 選取試算表的時區。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL數字格式]</td> 
   <td> <p>選取試算表中所有儲存格的預設格式。</p> <p><strong>[!UICONTROL文本]</strong>:文本格式。 範例: <code>1000. 12</code></p> <p><strong>[!UICONTROL編號]</strong>:數字格式。 範例: <code>1,000.12</code></p> <p><strong>[!UICONTROL百分比]</strong>:百分比格式。 範例: <code>10. 12%</code></p> <p><strong>[!UICONTROL貨幣]</strong>:貨幣格式。 範例: <code>$1,000.12</code></p> <p><strong>[!UICONTROL日期]</strong>:日期格式。 範例: <code>9/26/2008</code></p> <p><strong>[!UICONTROL時間]</strong>:時間格式。 範例: <code>3:59:00 PM</code></p> <p><strong>[!UICONTROL日期時間]</strong>:日期和時間格式。 範例: <code>9/26/08 15:59:00</code> </p> <p><strong>[!UICONTROL Scientific]</strong>科學的數字格式。 範例: <code>1. 01E+03</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL工作表] </td> 
   <td> <p>按一下 <strong>[!UICONTROL添加]</strong> 將工作表新增至試算表。 對於每個工作表，輸入或映射工作表的標題和工作表的索引。 索引為0表示第一張表。</p> </td> 
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
   <td>[!UICONTROL連接] </td> 
   <td> <p>有關連接 [!DNL Google Sheets] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連接到 [!DNL Workfront Fusion]</a> 在文章中 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在中建立案例 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL電子錶格] </td> 
   <td> <p>選取 [!DNL Google] 試算表。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL工作表] </td> 
   <td> <p>選擇要刪除的工作表。</p> </td> 
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
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關將[Fusion App]帳戶連接到 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td>輸入相對於的路徑 <code>https://sheets.googleapis.com/v4/</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL方法]</p> </td> 
   <td> <p>選取設定API呼叫所需的HTTP要求方法。 如需詳細資訊，請參閱 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">中的HTTP要求方法 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL標題]</td> 
   <td> <p>以標準JSON物件的形式新增請求的標題。例如， <code>{"Content-type":"application/json"}</code>. [!DNL Workfront Fusion] 為您添加授權標頭。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL查詢字串]</td> 
   <td> <p> 以標準JSON物件的形式新增API呼叫的查詢。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL正文]</td> 
   <td> <p>以標準JSON物件的形式新增API呼叫的內文內容。</p> <p>備註:   <p>使用條件陳述式時，例如 <code>if</code> 在JSON中，將引號放在條件陳述式之外。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>">  
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

## 搜尋

* [[!UICONTROL 搜尋列]](#search-rows)
* [[!UICONTROL 搜尋列（進階）]](#search-rows-advanced)
* [[!UICONTROL 獲取範圍值]](#get-range-values)
* [[!UICONTROL 清單工作表]](#list-sheets)

### [!UICONTROL 搜尋列]

使用篩選選項搜尋列。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL連接] </td> 
   <td> <p>有關將[Fusion App]帳戶連接到 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL電子錶格] </td> 
   <td> <p>選取 [!DNL Google] 試算表。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL工作表] </td> 
   <td> <p>選擇要搜索中行的工作表。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL表包含標題]</td> 
   <td> <p> 選取試算表是否包含標題列。 如果選取[!UICONTROL是]選項，則模組不會擷取標題列，因為輸出資料和輸出中的變數名稱隨後由標題呼叫。 如果選取了[!UICONTROL No]選項，則模組也會擷取第一個表格列，然後輸出中的變數名稱只會呼叫A、B、C、D等。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL列範圍]</td> 
   <td>選取要使用的欄範圍。 範例: <code>A-F</code></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL篩選器]</td> 
   <td> <p>設定要搜索的行的篩選器。</p> <p>如需篩選器的詳細資訊，請參閱 <a href="../../workfront-fusion/scenarios/add-a-filter-to-a-scenario.md" class="MCXref xref">為[!UICONTROL Adobe Workfront Fusion]中的案例新增篩選器</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL排序順序]</td> 
   <td>選取您要遞增排序或遞減排序。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL順序依]</td> 
   <td>選擇要排序的列。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL值呈現選項]</td> 
   <td> <p style="font-weight: bold;">[!UICONTROL格式化值]</p> <p>系統會根據儲存格的格式，在回覆中計算並格式化這些值。 格式設定是根據試算表的地區設定，而非要求使用者的地區設定。 例如，若 <code>A1</code> is <code>1.23</code> 和 <code>A2</code> is <code>=A1</code> 格式為貨幣，則 <code>A2</code> 會返回 <code>"$1.23"</code>.</p> <p style="font-weight: bold;">[!UICONTROL未格式化的值]</p> <p>系統將計算這些值，但不會在回覆中格式化。 例如，若 <code>A1</code> is <code>1.23</code> 和 <code>A2</code> is <code>=A1</code> 格式為貨幣，則 <code>A2</code> 會傳回 <code>"1.23"</code>.</p> <p style="font-weight: bold;">[!UICONTROL公式]</p> <p>將不會計算值。 回覆將包含公式。 例如，若 <code>A1</code> is <code>1.23</code> 和 <code>A2</code> is <code>=A1</code> 格式為貨幣，則 <code>A2</code> 會返回 <code>"=A1"</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL日期和時間呈現選項]</td> 
   <td> <p style="font-weight: bold;">[!UICONTROL序列號]</p> <p>指示日期、時間、日期時間和持續時間欄位以「序列號」格式雙倍輸出，如Lotus 1-2-3所推廣。 值的整數部分（小數點左側）會計算自1899年12月30日以來的天數。 小數部分（小數點的右側）會將時間計為當天的小數。 例如，1900年1月1日中午為2.5，因為是1899年12月30日後的2天，而0.5，因為中午是半天。 1900年2月1日下午3點將為33.625。這正確地將1900年視為不閏年。</p> <p style="font-weight: bold;">[!UICONTROL格式字串]</p> <p>指示日期、時間、日期時間和持續時間欄位以其指定數字格式（取決於電子錶格的地區設定）輸出為字串。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL返回行數上限]</td> 
   <td>設定 [!DNL Workfront Fusion] 會在一個執行週期期間傳回。</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 搜尋列（進階）]

傳回符合指定條件的結果。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL連接] </td> 
   <td> <p>有關連接 [!DNL Google Sheets] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連接到 [!DNL Workfront Fusion]</a> 在文章中 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在中建立案例 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL電子錶格] </td> 
   <td> <p>選擇包含要搜索工作表的Google電子錶格。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL工作表] </td> 
   <td> <p>選擇包含要搜索行的工作表。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL查詢]</td> 
   <td> <p>使用 [!DNL Google Charts Query Language]. 範例: <code>select * where B = "John"</code></p> <p>如需 [!DNL Google Charts Query Language]，請參閱 <a href="https://developers.google.com/chart/interactive/docs/querylanguage">查詢語言參考</a> 在 [!DNL Google] 檔案。</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 獲取範圍值]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL連接] </td> 
   <td> <p>有關連接 [!DNL Google Sheets] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連接到 [!DNL Workfront Fusion]</a> 在文章中 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在中建立案例 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL電子錶格] </td> 
   <td> <p>選取 [!DNL Google] 試算表。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL工作表] </td> 
   <td> <p>選擇要從中獲取範圍內容的工作表。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL範圍] </td> 
   <td> <p>輸入您要取得的範圍。 範例: <code>A1:D25</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL表包含標題]</td> 
   <td> <p>如果工作表具有標題行，請選中此框</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL帶標題的行]</td> 
   <td>輸入表標題的範圍。 範例 <code>A1:F1</code>. 如果欄位空白， [!DNL Workfront Fusion] 會假設標題位於指定範圍的第一列。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL值呈現選項]</td> 
   <td> <p style="font-weight: bold;">[!UICONTROL格式化值]</p> <p>系統會根據儲存格的格式，在回覆中計算並格式化這些值。 格式設定是根據試算表的地區設定，而非要求使用者的地區設定。 例如，若 <code>A1</code> is <code>1.23</code> 和 <code>A2</code> is <code>=A1</code> 格式為貨幣，則 <code>A2</code> 會返回 <code>"$1.23"</code>.</p> <p style="font-weight: bold;">[!UICONTROL未格式化的值]</p> <p>系統將計算這些值，但不會在回覆中格式化。 例如，若 <code>A1</code> is <code>1.23</code> 和 <code>A2</code> is <code>=A1</code> 格式為貨幣，則 <code>A2</code> 會傳回 <code>"1.23"</code>.</p> <p style="font-weight: bold;">[!UICONTROL公式]</p> <p>將不會計算值。 回覆將包含公式。 例如，若 <code>A1</code> is <code>1.23</code> 和 <code>A2</code> is <code>=A1</code> 格式為貨幣，則 <code>A2</code> 會返回 <code>"=A1"</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL日期和時間呈現選項]</td> 
   <td> <p style="font-weight: bold;">[!UICONTROL序列號]</p> <p>指示日期、時間、日期時間和持續時間欄位以「序列號」格式雙倍輸出，如Lotus 1-2-3所推廣。 值的整數部分（小數點左側）會計算自1899年12月30日以來的天數。 小數部分（小數點的右側）會將時間計為當天的小數。 例如，1900年1月1日中午為2.5，因為是1899年12月30日後的2天，而0.5，因為中午是半天。 1900年2月1日下午3點將為33.625。這正確地將1900年視為不閏年。</p> <p style="font-weight: bold;">[!UICONTROL格式字串]</p> <p>指示日期、時間、日期時間和持續時間欄位以其指定數字格式（取決於電子錶格的地區設定）輸出為字串。</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 清單工作表]

此模組會傳回試算表中的所有工作表清單。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL連接] </td> 
   <td> <p>有關連接 [!DNL Google Sheets] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連接到 [!DNL Workfront Fusion]</a> 在文章中 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在中建立案例 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL電子錶格] </td> 
   <td> <p>選取 [!DNL Google] 包含您要列出的工作表的試算表。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 使用量限制

如果錯誤 `429: RESOURCE_EXHAUSTED` 發生時，您已超過API比率限制。

此 [!DNL Google Sheets] API的限制是每個專案每100秒最多500個請求，而每個使用者每100秒最多100個請求。 讀取和寫入的限制將單獨跟蹤。 沒有每日使用量限制。

如需詳細資訊，請參閱 [developers.google.com/sheets/api/limits](https://developers.google.com/sheets/api/limits).

## 提示與秘訣

* [如何從 [!DNL Google] 工作表](#how-to-get-empty-cells-from-a-google-sheet)
* [在工作表中新增按鈕以執行情境](#add-a-button-in-a-sheet-to-run-a-scenario)

### 如何從 [!DNL Google Sheet]

使用 [!UICONTROL 搜尋列（進階）] 模組和使用此公式來取得空白的欄。
<pre>選擇* [!UICONTROL，其中E為空​]</pre>此處「E」為欄，「is null」為條件。 您可以使用[Google查詢函式]建立更高級的查詢。](https://developers.google.com/chart/interactive/docs/querylanguage)

### 在工作表中新增按鈕以執行情境

1. 在 [!DNL Workfront Fusion]，插入 **[!UICONTROL Webhook]** > **[!UICONTROL 自訂Webhook]** 案例中的模組/觸發程式並加以設定(請參閱 [Webhook](../../workfront-fusion/apps-and-their-modules/webhooks-updated.md))。

1. 複製網頁連結的URL。
1. 執行情境。
1. 在「Google工作表」中，選擇 **[!UICONTROL 插入]** > **[!UICONTROL 繪圖]**...從主菜單欄。

1. 在 [!UICONTROL 繪圖] ，按一下 **[!UICONTROL 文字方塊]** 圖示 ![](assets/text-box.png) 靠近窗頂。
1. 設計按鈕，然後按一下 **[!UICONTROL 儲存並關閉]** 按鈕（位於右上角）:
1. 按鈕將放在您的工作表中。 按一下按鈕右上角的三個垂直點：
1. 選擇 **[!UICONTROL 指派指令碼……].** 的上界。
1. 輸入指令碼（函式）的名稱，例如 `runScenario` 按一下 **[!UICONTROL 確定]**:
1. 選擇 **[!UICONTROL 工具]** > **[!UICONTROL 指令碼編輯器]** 的上界。

1. 插入下列程式碼：

   * 函式的名稱必須與在步驟9中指定的名稱相對應。
   * 將URL取代為您在步驟2中複製的網頁連結URL。

      <pre>函式runScenario(){</pre><pre>UrlFetchApp.fetch("<webhook you copied>「);</pre><pre>}</pre>

1. Press **[!UICONTROL Ctrl+S]** 要保存指令碼檔案，請輸入項目名稱，然後按一下 **[!UICONTROL 確定]**.

1. 切換回 [!DNL Google Sheets] 並按一下新按鈕。
1. 將所需的授權授予指令碼：
1. 在 [!DNL Workfront Fusion]，確認藍本已成功執行。

## 將日期儲存在試算表中

如果將「日期」值儲存在試算表中，且沒有任何格式設定，則該值在試算表中會以ISO 8601格式的文字顯示。 不過， [!DNL Google Sheets] 與不了解此文本的日期一起使用的公式或函式(示例：公式 `=A1+10`)會顯示下列錯誤：

![](assets/mceclip6-350x87.png)

若要允許 [!DNL Google Sheets] 若要了解日期，請以 [[!UICONTROL formatDate] （日期）格式；[時區])](../../workfront-fusion/functions/date-and-time-functions.md#formatda) 函式。 作為第二個引數傳遞至函式的正確格式取決於試算表的地區設定。

要確定正確格式，請執行以下操作：

1. 選擇 **[!UICONTROL 檔案]** > **[!UICONTROL 試算表]** 從主菜單中進行設定以驗證/設定區域設定。

1. 驗證/設定正確的地區設定後，通過選擇 **[!UICONTROL 格式]** > **[!UICONTROL 數字]** 的上界。 格式會顯示在「日期時間」功能表項目旁：

1. 若要撰寫應傳遞至的正確格式 [!UICONTROL formatDate()] 函式，請參閱 [日期和時間格式的代號，位於 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/tokens-for-date-and-time-formatting.md).

**範例：** 使用 `MM/DD/YYYY HH:mm:ss` 美國地區設定格式：

![](assets/locale-time-350x83.png)

## 開發 [!DNL Google Sheets] 函式

如果您遺漏了內建函式，但此功能有 [!DNL Google Sheets]，您可加以利用。 如需詳細資訊，請參閱 [使用 [!DNL Google Sheets] 函式](../../workfront-fusion/functions/map-using-functions.md#exploiti) in [在中使用函式映射項目 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/map-using-functions.md) .

## 保留 [!DNL Google Sheets] 從數字到日期

您可能會發現，您使用作為文字的數字字串，會解讀為 [!DNL Google] 工作表。 例如，您輸入1-2019，並打算輸入文字，但Google會將其解譯為日期。 您可以將數字預先格式化為純文字，以避免此情況。

1. 在 [!DNL Google Sheets]，突出顯示包含數字或數字的列或單元格。
1. 按一下 **[!UICONTROL 格式]** > **[!UICONTROL 數字]** > **[!UICONTROL 純文字]**.

中的其他解決方法 [!DNL Workfront Fusion] 是在數字前面輸入撇號(&#39;)，例如&#39;1-2019或&#39;1/47。 從傳送資料後，單引號不會顯示在儲存格中 [!DNL Workfront Fusion].
