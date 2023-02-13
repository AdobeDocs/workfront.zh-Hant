---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: 連接器
navigation-topic: apps-and-their-modules
title: Microsoft Office 365 Excel模組
description: 在 [!DNL Adobe Workfront Fusion] 案例中，您可以自動執行使用Microsoft 365 Excel的工作流程，並將其連接至多個協力廠商應用程式和服務。
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 9aa3739d-6800-4eb1-a17f-32fdfd8ed0f2
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '2577'
ht-degree: 0%

---

# [!DNL Microsoft Office 365 Excel] 模組

在 [!DNL Adobe Workfront Fusion] 案例中，您可以自動執行使用 [!DNL Microsoft 365 Excel]，並將其連接至多個協力廠商應用程式和服務。

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] （工作自動化和整合） </p>  </td>  
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

使用 [!DNL Microsoft office 365 Excel]，您必須有Microsoft帳戶。

## [!DNL Microsoft Office 365 Excel] 模組及其欄位

設定時 [!DNL Microsoft 365 Excel] 模組， [!DNL Workfront Fusion] 顯示下列欄位。 此外， [!DNL Microsoft 365 Excel] 視您在應用程式或服務中的存取層級等因素而定，可能會顯示欄位。 模組中的粗體標題表示必填欄位。

如果您在欄位或函式上方看到對應按鈕，則可使用它來設定該欄位的變數和函式。 如需詳細資訊，請參閱 [將資訊從一個模組對應到 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [活頁簿](#workbook)
* [工作表](#worksheet)
* [表格](#table)
* [其他](#other)

### 活頁簿

* [監看活頁簿](#watch-workbooks)
* [搜尋活頁簿](#search-workbooks)
* [下載活頁簿](#download-a-workbook)

#### [!UICONTROL 監看活頁簿]

此觸發程式模組會在建立活頁簿時啟動案例。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL連接]</p> </td> 
   <td> <p>有關連接 [!DNL Office 365] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連接到 [!DNL Workfront Fusion]</a> 在文章中 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在中建立案例 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL資料夾]</td> 
   <td> <p>選取您要監看新活頁簿的資料夾。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL篩選器]</p> </td> 
   <td> <p>您可以設定篩選條件，只監看符合您選取之條件的活頁簿。</p> <p>對於每個篩選器，輸入您要篩選器評估的欄位、運算子，以及您希望篩選器允許的值。 您可以新增AND或OR規則，以使用多個篩選器。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL限制]</td> 
   <td> <p>輸入或對應您希望模組在每個案例執行週期期間傳回的活頁簿數目上限。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 搜尋活頁簿]

此動作模組會搜尋 [!DNL Excel] 活頁簿。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL連接]</p> </td> 
   <td> <p>有關連接 [!DNL Office 365] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連接到 [!DNL Workfront Fusion]</a> 在文章中 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在中建立案例 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL資料夾]</td> 
   <td> <p>選擇要搜索工作簿的資料夾。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL篩選器]</p> </td> 
   <td> <p>您可以設定篩選條件，以僅搜尋符合您選取條件的活頁簿。</p> <p>對於每個篩選器，輸入您要篩選器評估的欄位、運算子，以及您希望篩選器允許的值。 您可以新增AND或OR規則，以使用多個篩選器。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL限制]</td> 
   <td> <p>輸入或映射在每個方案執行週期期間希望模組返回的工作表數上限。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 下載活頁簿]

此動作模組會下載指定Excel活頁簿的內容。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL連接]</p> </td> 
   <td> <p>有關連接 [!DNL Office 365] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連接到 [!DNL Workfront Fusion]</a> 在文章中 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在中建立案例 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL下載活頁簿]</td> 
   <td> <p>選取您要如何識別要下載之模組的活頁簿。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL手動輸入ID]</strong> </p> <p>在「 [!UICONTROL活頁簿ID]」欄位中，輸入或對應您要讓模組下載的特定活頁簿ID。</p> </li> 
     <li> <p><strong>[!UICONTROL從路徑中選擇]</strong> </p> <p>在[!UICONTROL活頁簿]欄位中，選取您要模組下載的活頁簿。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 工作表

* [[!UICONTROL 監視工作表行]](#watch-worksheet-rows)
* [[!UICONTROL 列出工作表]](#list-worksheets)
* [[!UICONTROL 列出工作表行]](#list-worksheet-rows)
* [[!UICONTROL 新增工作表]](#add-a-worksheet)
* [[!UICONTROL 新增工作表列]](#add-a-worksheet-row)
* [[!UICONTROL 更新工作表行]](#update-a-worksheet-row)
* [[!UICONTROL 刪除工作表行]](#delete-a-worksheet-row)

#### [!UICONTROL 監視工作表行]

此觸發模組會在工作表中新增新列時啟動案例。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL連接]</p> </td> 
   <td> <p>有關連接 [!DNL Office 365] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連接到 [!DNL Workfront Fusion]</a> 在文章中 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在中建立案例 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL工作簿] </td>
   <td> <p>選擇包含要查看新行的工作表的工作簿。</p> </td> 
  </tr> 
  <tr>
    <td role="rowheader" >[!UICONTROL工作表] </td>
   <td> <p>選擇要監視新行的Excel工作表。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL限制]</td>
   <td> <p>輸入或映射您希望模組在每個方案執行週期期間返回的最大工作表行數。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 列出工作表]

此動作模組會擷取指定活頁簿中的工作表清單。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL連接]</p> </td> 
   <td> <p>有關連接 [!DNL Office 365] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連接到 [!DNL Workfront Fusion]</a> 在文章中 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在中建立案例 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL工作簿] </td>
   <td> <p>選擇包含要列出模組的工作表的工作簿。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL限制]</td>
   <td> <p>輸入或映射在每個方案執行週期期間希望模組返回的工作表數上限。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 列出工作表行]

此動作模組會擷取指定工作表中的列清單。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL連接]</p> </td> 
   <td> <p>有關連接 [!DNL Office 365] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連接到 [!DNL Workfront Fusion]</a> 在文章中 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在中建立案例 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr>
    <td role="rowheader" >[!UICONTROL工作簿] </td>
   <td> <p>選擇包含工作表的活頁簿，工作表中包含您要列出的行。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL工作表] </td>
   <td> <p>選擇包含要列出行的工作表。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL限制]</td>
   <td> <p>輸入或映射您希望模組在每個方案執行週期期間返回的最大工作表行數。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 新增工作表]

此動作模組會在選取的活頁簿內建立新的工作表。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL連接]</p> </td> 
   <td> <p>有關連接 [!DNL Office 365] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連接到 [!DNL Workfront Fusion]</a> 在文章中 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在中建立案例 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr>
    <td role="rowheader" >[!UICONTROL工作簿] </td>
   <td> <p>選擇要添加工作表的工作簿。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL名稱] </td>
   <td> <p>輸入或映射新工作表的名稱。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 新增工作表列]

此動作模組會將新列新增至所選工作表。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL連接]</p> </td> 
   <td> <p>有關連接 [!DNL Office 365] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連接到 [!DNL Workfront Fusion]</a> 在文章中 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在中建立案例 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL工作簿] </td>
   <td> <p>選擇包含要添加行的工作表的工作簿。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL工作表] </td>
   <td> <p>選擇要添加行的工作表。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL要輸入的值類型]</p> </td> 
   <td> <p>選擇要輸入到工作表中的值類型。 </p> 
    <ul> 
     <li> <p><strong>[!UICONTROL公式]</strong> </p> <p> Excel嘗試評估指定的運算式。 公式中的函式名稱是英文。 範例: <code>[!DNL =SUM(A1:A10)]</code></p> </li> 
     <li> <p><strong>[!UICONTROL公式本地]</strong> </p> <p>Excel嘗試評估指定的運算式。 函式名稱使用Excel應用程式的語言。 範例： <code>=SUM(A1, 1.5)</code> vs <code>=SUMME(A1; 1,5)</code></p> </li> 
     <li> <p><strong>[!UICONTROL值]</strong> </p> <p>Excel不會評估值。 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL行]</td>
    <td>對於每一列，輸入您希望該列在新行中的值。</td>
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 更新工作表行]

此動作模組會更新現有的工作表列。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL連接]</p> </td> 
   <td> <p>有關連接 [!DNL Office 365] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連接到 [!DNL Workfront Fusion]</a> 在文章中 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在中建立案例 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL工作簿] </td>
   <td> <p>選擇包含工作表的活頁簿，工作表中包含您要更新的行。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL工作表] </td>
   <td> <p>選擇包含要更新行的工作表。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL要輸入的值類型]</p> </td> 
   <td> <p>選擇要輸入到工作表中的值類型。 </p> 
    <ul> 
     <li> <p><strong>[!UICONTROL公式]</strong> </p> <p> Excel嘗試評估指定的運算式。 公式中的函式名稱是英文。 範例: <code>[!DNL =SUM(A1:A10)]</code></p> </li> 
     <li> <p><strong>[!UICONTROL公式本地]</strong> </p> <p>Excel嘗試評估指定的運算式。 函式名稱使用Excel應用程式的語言。 範例： <code>=SUM(A1, 1.5)</code> vs <code>=SUMME(A1; 1,5)</code></p> </li> 
     <li> <p><strong>[!UICONTROL值]</strong> </p> <p>Excel不會評估值。 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL行ID]</td> 
   <td>選取要更新的列數。</td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL行]</td>
    <td>對於每一列，輸入您希望該列在新行中的值。</td>
   —&gt; 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 刪除工作表行]

此動作模組會從工作表中刪除一列。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL連接]</p> </td> 
   <td> <p>有關連接 [!DNL Office 365] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連接到 [!DNL Workfront Fusion]</a> 在文章中 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在中建立案例 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL工作簿] </td>
   <td> <p>選擇包含工作表的活頁簿，工作表中包含您要刪除的列。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL工作表]</td>
   <td> <p> 選擇包含要刪除的行的工作表。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL行ID]</td>
   <td>輸入或映射要刪除的行的ID。</td> 
  </tr> 
 </tbody> 
</table>

### 表格

* [[!UICONTROL 監看表行]](#watch-table-rows)
* [[!UICONTROL 清單表]](#list-tables)
* [[!UICONTROL 清單表行]](#list-table-rows)
* [[!UICONTROL 取得表格]](#get-a-table)
* [[!UICONTROL 新增表格]](#add-a-table)
* [[!UICONTROL 添加表行]](#add-a-table-row)
* [[!UICONTROL 更新表]](#update-a-table)
* [[!UICONTROL 刪除表]](#delete-a-table)

#### [!UICONTROL 監看表行]

此觸發器會在新增新列至表格時啟動案例。

>[!NOTE]
>
>此處的表格是指活頁簿中的內嵌表格元素。 不是整個表格（活頁簿/工作表）。

![](assets/embedded-table-350x420.png)

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL連接]</p> </td> 
   <td> <p>有關連接 [!DNL Office 365] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連接到 [!DNL Workfront Fusion]</a> 在文章中 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在中建立案例 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL工作簿]</p> </td> 
   <td> <p>選取包含您要監看之表格的活頁簿。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL工作表] </td>
   <td> <p> 選擇包含要監視的表的工作表。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL表]</p> </td> 
   <td> <p>選擇要監視的表。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL限制]</td>
   <td> <p>輸入或映射您希望模組在每個方案執行週期中返回的最大行數。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 清單表]

此搜索模組檢索所有表對象的清單。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL連接]</p> </td> 
   <td> <p>有關連接 [!DNL Office 365] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連接到 [!DNL Workfront Fusion]</a> 在文章中 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在中建立案例 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr>
    <td role="rowheader" >[!UICONTROL工作簿] </td>
   <td> <p>選擇包含要列出的表的工作簿。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL工作表] </td>
   <td> <p>選擇包含要列出的表的工作表</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL限制]</td>
   <td> <p>輸入或映射您希望模組在每個方案執行週期中返回的最大表數。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 清單表行]

此搜尋模組會擷取活頁簿中所有表格列的清單。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL連接]</p> </td> 
   <td> <p>有關連接 [!DNL Office 365] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連接到 [!DNL Workfront Fusion]</a> 在文章中 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在中建立案例 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL工作簿] </td>
   <td> <p>選擇包含要列出行的表的工作簿。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL工作表] </td>
   <td> <p>選擇包含要列出行的表的工作表</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL表] </td>
   <td> <p>選擇包含要列出行的表。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL限制]</td>
   <td> <p>輸入或映射您希望模組在每個方案執行週期期間返回的最大表行數。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 取得表格]

此動作模組會擷取指定表格的中繼資料。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> 
     <p >[!UICONTROL連接]</p>
   </td> 
   <td> 
     <p>有關將Office 365帳戶連接到 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連接到 [!DNL Workfront Fusion]</a> 在文章中 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在中建立案例 [!DNL Adobe Workfront Fusion]</a>.</p>
    --&gt; </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL獲取表]</td> 
   <td> <p>選擇要如何標識要檢索的表。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL手動輸入]</strong> </p> <p>在[!UICONTROL活頁簿ID]欄位中，輸入或映射包含您要檢索的表的工作簿的ID。</p> <p>在[!UICONTROL表名]欄位中，輸入或映射要檢索的表的名稱。</p> </li> 
     <li> <p><strong>[!UICONTROL從清單中選擇]</strong> </p> <p>選擇包含要檢索的表的工作簿和工作表，然後選擇表。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 新增表格]

此動作模組會在Excel工作表中建立表格元素。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL連接]</p> </td> 
   <td> <p>有關連接 [!DNL Office 365] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連接到 [!DNL Workfront Fusion]</a> 在文章中 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在中建立案例 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL工作簿] </td> 
   <td> <p>選擇包含要添加表的工作表的工作簿。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL工作表] </td> 
   <td> <p>選擇要添加表的工作表。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL有標題]</td> 
   <td> <p>啟用此選項可將第一列定義為表格標題。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL地址]</p> </td> 
   <td> <p>指示左上角和右下角的儲存格，以設定表格的大小。 範例： <code>A1:C10</code> 建立一個表，其中包含3列和10列。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 添加表行]

此動作模組會修改現有表格。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL連接]</p> </td> 
   <td> <p>有關連接 [!DNL Office 365] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連接到 [!DNL Workfront Fusion]</a> 在文章中 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在中建立案例 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL工作簿] </td>
   <td> <p>選取包含您要新增列之表格的活頁簿。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL工作表] </td>
   <td> <p>選擇包含要添加行的表的工作表。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL表]</td>
   <td>選擇要添加行的表。</td> 
  </tr> 
  <tr>
    <td role="rowheader" >[!UICONTROL行]</td>
    <td>對於每一列，輸入您希望該列在新行中的值。</td>
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL行ID]</p> </td> 
   <td> <p>要在表的特定位置中添加行，請輸入或映射行號。 模組會在此列後面插入新行。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 更新表]

此動作模組會更新現有表格。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL連接]</p> </td> 
   <td> <p>有關連接 [!DNL Office 365] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連接到 [!DNL Workfront Fusion]</a> 在文章中 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在中建立案例 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL更新表]</td> 
   <td> <p>選擇要如何標識要更新的表。</p> 
    <ul> 
     <li> <p><strong>手動輸入</strong> </p> <p>在「 [!UICONTROL活頁簿ID]」欄位中，輸入或映射包含您要更新之表格的活頁簿ID。</p> <p>在[!UICONTROL表名]欄位中，輸入或映射要更新的表的名稱。</p> </li> 
     <li> <p><strong>[!UICONTROL從清單中選擇]</strong> </p> <p>選擇包含要更新的表的工作簿和工作表，然後選擇表。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL表] </td> 
   <td> <p>選擇要更新的表。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL名稱]</td> 
   <td> <p>如果要更名表，請輸入或映射表的新名稱。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL顯示標題]</td> 
   <td> <p>啟用此選項可顯示更新表格的標題。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL顯示總計]</td> 
   <td>啟用此選項可顯示表的總值。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL樣式]</td> 
   <td>為新表選擇樣式。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 刪除表]

此動作模組會從 [!DNL Excel] 工作表。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL連接]</p> </td> 
   <td> <p>有關連接 [!DNL Office 365] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連接到 [!DNL Workfront Fusion]</a> 在文章中 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在中建立案例 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL獲取表]</td> 
   <td> <p>選擇要如何標識要刪除的表。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL手動輸入]</strong> </p> <p>在[!UICONTROL活頁簿ID]欄位中，輸入或映射包含您要刪除之表格的活頁簿ID。</p> <p>在[!UICONTROL表名]欄位中，輸入或映射要刪除的表的名稱。</p> </li> 
     <li> <p><strong>[!UICONTROL從清單中選擇]</strong> </p> <p>選擇包含要刪除的表的工作簿和工作表，然後選擇表。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 其他

* [[!UICONTROL 擷取資料]](#retrieve-data)
* [[!UICONTROL 進行API呼叫]](#make-an-api-call)

#### [!UICONTROL 擷取資料]

此動作會從定義的工作表範圍中擷取資料，並針對每列傳回套件。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL連接]</p> </td> 
   <td> <p>有關連接 [!DNL Office 365] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連接到 [!DNL Workfront Fusion]</a> 在文章中 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在中建立案例 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL工作簿] </td> 
   <td> <p>選取包含您要擷取之資料的活頁簿。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL工作表] </td> 
   <td> <p>選擇包含要檢索的資料的工作表。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL範圍] </td> 
   <td> <p>通過指示左上角和右下角的單元格，指定要從中檢索資料的工作表的區域。 範例: <code>A1:D10</code></p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 進行API呼叫]

此動作模組可讓您進行自訂API呼叫。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL連接]</p> </td> 
   <td> <p>有關連接 [!DNL Office 365] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連接到 [!DNL Workfront Fusion]</a> 在文章中 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在中建立案例 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>輸入相對於的路徑 <code>https://graph.microsoft.com</code>. 範例:<code> /v1.0/me/drive/root/children</code></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL方法]</td> 
   td&gt; <p>選取設定API呼叫所需的HTTP要求方法。 如需詳細資訊，請參閱 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">中的HTTP要求方法 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL標題]</td> 
   <td> <p>以標準JSON物件的形式新增請求的標題。</p> <p>例如， <code>{"Content-type":"application/json"}</code></p> <p>Workfront Fusion會為您新增授權標頭。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL查詢字串]</td> 
   <td> <p>以標準JSON物件的形式新增API呼叫的查詢。</p> <p>例如： <code>{"name":"something-urgent"}</code></p> </td> 
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
