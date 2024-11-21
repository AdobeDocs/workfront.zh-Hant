---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: 聯結器
navigation-topic: apps-and-their-modules
title: Microsoft Office 365 Excel模組
description: 在 [!DNL Adobe Workfront Fusion] 案例中，您可以自動執行使用Microsoft 365 Excel的工作流程，以及將其連線到多個協力廠商應用程式和服務。
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 9aa3739d-6800-4eb1-a17f-32fdfd8ed0f2
source-git-commit: 2e91e9a4c691430f3c98e3cbddb30706ea57f84a
workflow-type: tm+mt
source-wordcount: '2768'
ht-degree: 0%

---

# [!DNL Microsoft Office 365 Excel]模組

在[!DNL Adobe Workfront Fusion]案例中，您可以自動化使用[!DNL Microsoft 365 Excel]的工作流程，並將其連線至多個協力廠商應用程式和服務。

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

若要使用[!DNL Microsoft office 365 Excel]，您必須擁有Microsoft帳戶。

## Microsoft Office 365 Excel API資訊

Microsoft Office 365 Excel聯結器使用下列專案：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">基礎URL</td> 
   <td> https://graph.microsoft.com/v1.0</td> 
  </tr> 
  <tr> 
   <td role="rowheader">API版本</td> 
   <td> v1.0 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">API標籤</td> 
   <td>v2.0.16</td> 
  </tr>
 </tbody> 
 </table>



## 正在將[!DNL Office 365 Excel]服務連線到[!DNL Workfront Fusion]

如需有關將您的[!DNL Office 365 Excel]帳戶連線到[!UICONTROL Workfront Fusion]的指示，請參閱[建立與[!UICONTROL Adobe Workfront Fusion]的連線](../../workfront-fusion/connections/connect-to-fusion-general.md) — 基本指示

>[!NOTE]
>
>部分Microsoft應用程式使用相同的連線，而此連線會繫結至個別使用者許可權。 因此，在建立連線時，許可權同意畫面會顯示先前授與此使用者連線的所有許可權，以及目前應用程式所需的任何新許可權。
>
>例如，如果使用者擁有透過Excel聯結器授予的「讀取表格」許可權，然後在Outlook聯結器中建立連線以讀取電子郵件，則許可權同意畫面會顯示已授予的「讀取表格」許可權和新要求的「寫入電子郵件」許可權。

## [!DNL Microsoft Office 365 Excel]模組及其欄位

當您設定[!DNL Microsoft 365 Excel]模組時，[!DNL Workfront Fusion]會顯示下列欄位。 除了這些欄位以外，可能還會顯示其他[!DNL Microsoft 365 Excel]欄位，視您在應用程式或服務中的存取層級等因素而定。 模組中的粗體標題表示必填欄位。

如果您在欄位或函式上方看到對應按鈕，則可以使用它來設定該欄位的變數和函式。 如需詳細資訊，請參閱[在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md)中將資訊從一個模組對應到另一個模組。

![](assets/map-toggle-350x74.png)

* [活頁簿](#workbook)
* [工作表](#worksheet)
* [表格](#table)
* [其他](#other)

### 活頁簿

* [監視活頁簿](#watch-workbooks)
* [搜尋活頁簿](#search-workbooks)
* [下載活頁簿](#download-a-workbook)

#### [!UICONTROL 觀看活頁簿]

此觸發模組會在建立活頁簿時啟動案例。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>如需有關將您的[!DNL Office 365]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中建立案例一文中的<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連線到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL資料夾]</td> 
   <td> <p>選取您要監視新活頁簿的資料夾。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL篩選器]</p> </td> 
   <td> <p>您可以設定篩選器，只監視符合您選取條件的活頁簿。</p> <p>針對每個篩選器，輸入您希望篩選器評估的欄位、運運算元，以及您希望篩選器允許的值。 您可以新增AND或OR規則，以使用一個以上的篩選器。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制]</td> 
   <td> <p>輸入或對應您希望模組在每個案例執行週期中傳回的最大活頁簿數量。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 搜尋活頁簿]

此動作模組搜尋[!DNL Excel]活頁簿。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>如需有關將您的[!DNL Office 365]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中建立案例一文中的<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連線到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL資料夾]</td> 
   <td> <p>選取您要搜尋活頁簿的資料夾。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL篩選器]</p> </td> 
   <td> <p>您可以設定篩選器，只搜尋符合您選取條件的活頁簿。</p> <p>針對每個篩選器，輸入您希望篩選器評估的欄位、運運算元，以及您希望篩選器允許的值。 您可以新增AND或OR規則，以使用一個以上的篩選器。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制]</td> 
   <td> <p>輸入或對應每個案例執行週期中您希望模組傳回的最大工作表數量。</p> </td> 
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
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>如需有關將您的[!DNL Office 365]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中建立案例一文中的<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連線到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL下載活頁簿]</td> 
   <td> <p>選取您要如何識別供模組下載的活頁簿。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL，手動輸入ID]</strong> </p> <p>在[！UICONTROL活頁簿ID]欄位中，輸入或對應您要模組下載之特定活頁簿的ID。</p> </li> 
     <li> <p>從路徑選取<strong>[！UICONTROL]</strong> </p> <p>在[！UICONTROL活頁簿]欄位中，選取您要模組下載的活頁簿。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 工作表

* [[!UICONTROL 監視工作表列]](#watch-worksheet-rows)
* [[!UICONTROL 列出工作表]](#list-worksheets)
* [[!UICONTROL 列出工作表列]](#list-worksheet-rows)
* [[!UICONTROL 新增工作表]](#add-a-worksheet)
* [[!UICONTROL 新增工作表列]](#add-a-worksheet-row)
* [[!UICONTROL 更新工作表列]](#update-a-worksheet-row)
* [[!UICONTROL 刪除工作表列]](#delete-a-worksheet-row)

#### [!UICONTROL 監視工作表列]

此觸發模組會在工作表新增新列時啟動案例。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>如需有關將您的[!DNL Office 365]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中建立案例一文中的<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連線到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[！UICONTROL活頁簿] </td>
   <td> <p>選取包含您要監視新資料列的工作表的活頁簿。</p> </td> 
  </tr> 
  <tr>
    <td role="rowheader" >[！UICONTROL工作表] </td>
   <td> <p>選取要監視新列的Excel工作表。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[！UICONTROL限制]</td>
   <td> <p>輸入或對應您希望模組在每個案例執行週期中傳回的最大工作表列數。</p> </td> 
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
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>如需有關將您的[!DNL Office 365]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中建立案例一文中的<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連線到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[！UICONTROL活頁簿] </td>
   <td> <p>選取包含您要模組列出之工作表的工作簿。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[！UICONTROL限制]</td>
   <td> <p>輸入或對應每個案例執行週期中您希望模組傳回的最大工作表數量。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 列出工作表列]

此動作模組會擷取指定工作表中的列清單。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>如需有關將您的[!DNL Office 365]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中建立案例一文中的<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連線到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr>
    <td role="rowheader" >[！UICONTROL活頁簿] </td>
   <td> <p>選取包含您要列出之資料列的工作表的活頁簿。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[！UICONTROL工作表] </td>
   <td> <p>選取包含您要列示之資料列的工作表。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[！UICONTROL限制]</td>
   <td> <p>輸入或對應您希望模組在每個案例執行週期中傳回的最大工作表列數。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 新增工作表]

此動作模組會在選取的活頁簿中建立新的工作表。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>如需有關將您的[!DNL Office 365]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中建立案例一文中的<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連線到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr>
    <td role="rowheader" >[！UICONTROL活頁簿] </td>
   <td> <p>選取您要新增工作表的活頁簿。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[！UICONTROL名稱] </td>
   <td> <p>輸入或對應新工作表的名稱。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 新增工作表列]

此動作模組會新增一列至選取的工作表。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>如需有關將您的[!DNL Office 365]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中建立案例一文中的<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連線到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[！UICONTROL活頁簿] </td>
   <td> <p>選取包含您要新增列的工作表的活頁簿。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[！UICONTROL工作表] </td>
   <td> <p>選取您要新增資料列的工作表。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL輸入的值型別]</p> </td> 
   <td> <p>選取要輸入工作表中的值型態。 </p> 
    <ul> 
     <li> <p><strong>[！UICONTROL公式]</strong> </p> <p> Excel會嘗試評估指定的運算式。 公式中的函式名稱為英文。 範例： <code>[!DNL =SUM(A1:A10)]</code></p> </li> 
     <li> <p><strong>[！UICONTROL公式本機]</strong> </p> <p>Excel會嘗試評估指定的運算式。 函式名稱使用Excel應用程式的語言。 範例： <code>=SUM(A1, 1.5)</code> vs <code>=SUMME(A1; 1,5)</code></p> </li> 
     <li> <p><strong>[！UICONTROL值]</strong> </p> <p>Excel不會評估值。 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[！UICONTROL Row]</td>
    <td>針對每一欄，輸入您希望欄在新列中的值。</td>
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 更新工作表列]

此動作模組會更新現有的工作表列。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>如需有關將您的[!DNL Office 365]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中建立案例一文中的<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連線到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[！UICONTROL活頁簿] </td>
   <td> <p>選取包含您要更新之資料列的工作表的活頁簿。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[！UICONTROL工作表] </td>
   <td> <p>選取包含您要更新之資料列的工作表。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL輸入的值型別]</p> </td> 
   <td> <p>選取要輸入工作表中的值型態。 </p> 
    <ul> 
     <li> <p><strong>[！UICONTROL公式]</strong> </p> <p> Excel會嘗試評估指定的運算式。 公式中的函式名稱為英文。 範例： <code>[!DNL =SUM(A1:A10)]</code></p> </li> 
     <li> <p><strong>[！UICONTROL公式本機]</strong> </p> <p>Excel會嘗試評估指定的運算式。 函式名稱使用Excel應用程式的語言。 範例： <code>=SUM(A1, 1.5)</code> vs <code>=SUMME(A1; 1,5)</code></p> </li> 
     <li> <p><strong>[！UICONTROL值]</strong> </p> <p>Excel不會評估值。 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL列ID]</td> 
   <td>選取要更新的列編號。</td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[！UICONTROL Row]</td>
    <td>針對每一欄，輸入您希望欄在新列中的值。</td>
   —&gt; 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 刪除工作表列]

此動作模組會從工作表刪除列。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>如需有關將您的[!DNL Office 365]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中建立案例一文中的<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連線到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[！UICONTROL活頁簿] </td>
   <td> <p>選取包含您要刪除之資料列的工作表的活頁簿。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[！UICONTROL工作表]</td>
   <td> <p> 選取包含您要刪除之資料列的工作表。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[！UICONTROL列ID]</td>
   <td>輸入或對應您要刪除之列的ID。</td> 
  </tr> 
 </tbody> 
</table>

### 表格

* [[!UICONTROL 觀看資料表列]](#watch-table-rows)
* [[!UICONTROL 列出資料表]](#list-tables)
* [[!UICONTROL 列出資料表列]](#list-table-rows)
* [[!UICONTROL 取得資料表]](#get-a-table)
* [[!UICONTROL 新增資料表]](#add-a-table)
* [[!UICONTROL 新增資料表列]](#add-a-table-row)
* [[!UICONTROL 更新資料表]](#update-a-table)
* [[!UICONTROL 刪除資料表]](#delete-a-table)

#### [!UICONTROL 觀看資料表列]

此觸發器會在表格中新增新列時啟動案例。

>[!NOTE]
>
>此處的表格參考活頁簿中的內嵌表格元素。 不是整個表格（活頁簿/工作表）。

![](assets/embedded-table-350x420.png)

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>如需有關將您的[!DNL Office 365]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中建立案例一文中的<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連線到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL活頁簿]</p> </td> 
   <td> <p>選取包含您要觀看之表格的活頁簿。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[！UICONTROL工作表] </td>
   <td> <p> 選取包含您要監視之表格的工作表。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL表格]</p> </td> 
   <td> <p>選取您要觀看的表格。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[！UICONTROL限制]</td>
   <td> <p>輸入或對應您希望模組在每個案例執行週期中傳回的最大列數。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 列出資料表]

此搜尋模組會擷取所有表格物件的清單。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>如需有關將您的[!DNL Office 365]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中建立案例一文中的<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連線到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr>
    <td role="rowheader" >[！UICONTROL活頁簿] </td>
   <td> <p>選取包含您要列出之表格的活頁簿。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[！UICONTROL工作表] </td>
   <td> <p>選取包含您要列出之表格的工作表</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[！UICONTROL限制]</td>
   <td> <p>輸入或對應您希望模組在每個案例執行週期中傳回的最大表格數量。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 列出資料表列]

此搜尋模組會擷取活頁簿中所有表格列的清單。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>如需有關將您的[!DNL Office 365]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中建立案例一文中的<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連線到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[！UICONTROL活頁簿] </td>
   <td> <p>選取包含您要列出之資料列的表格活頁簿。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[！UICONTROL工作表] </td>
   <td> <p>選取包含您要列示之資料列的表格的工作表</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[！UICONTROL表格] </td>
   <td> <p>選取包含要列出之列的表格。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[！UICONTROL限制]</td>
   <td> <p>輸入或對應您希望模組在每個案例執行週期中傳回的最大表格列數。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 取得資料表]

此動作模組會擷取指定表格的中繼資料。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> 
     <p >[！UICONTROL Connection]</p>
   </td> 
   <td> 
     <p>如需有關將Office 365帳戶連線到[!DNL Workfront Fusion]的說明，請參閱<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中建立情境<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連線到[!DNL Workfront Fusion]</a>。</p>
    --&gt; </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL取得表格]</td> 
   <td> <p>選取您要如何識別要擷取的表格。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL手動輸入]</strong> </p> <p>在[！UICONTROL活頁簿ID]欄位中，輸入或對應包含您要擷取之表格之活頁簿的ID。</p> <p>在[！UICONTROL表格名稱]欄位中，輸入或對應您要擷取的表格名稱。</p> </li> 
     <li> <p><strong>[！UICONTROL從清單中選取]</strong> </p> <p>選取包含您要擷取之表格的活頁簿和工作表，然後選取表格。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 新增資料表]

此動作模組會在Excel工作表中建立表格元素。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>如需有關將您的[!DNL Office 365]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中建立案例一文中的<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連線到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL活頁簿] </td> 
   <td> <p>選取包含您要新增表格之工作表的活頁簿。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL工作表] </td> 
   <td> <p>選取您要新增表格的工作表。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL有標題]</td> 
   <td> <p>啟用此選項可將第一列定義為表格標題。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL位址]</p> </td> 
   <td> <p>指示左上角與右下角的儲存格，以設定表格的大小。 範例： <code>A1:C10</code>會建立包含3欄和10列的表格。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 新增資料表列]

此動作模組會修改現有表格。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>如需有關將您的[!DNL Office 365]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中建立案例一文中的<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連線到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[！UICONTROL活頁簿] </td>
   <td> <p>選取包含您要新增列之表格的活頁簿。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[！UICONTROL工作表] </td>
   <td> <p>選取包含您要新增資料列之表格的工作表。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[！UICONTROL表格]</td>
   <td>選取您要新增列的表格。</td> 
  </tr> 
  <tr>
    <td role="rowheader" >[！UICONTROL Row]</td>
    <td>針對每一欄，輸入您希望欄在新列中的值。</td>
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL列ID]</p> </td> 
   <td> <p>若要在表格的特定位置中新增列，請輸入或對映列號。 模組會在此列之後插入新的一列。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 更新資料表]

此動作模組會更新現有的表格。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>如需有關將您的[!DNL Office 365]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中建立案例一文中的<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連線到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL更新表格]</td> 
   <td> <p>選取要如何識別要更新的表格。</p> 
    <ul> 
     <li> <p><strong>手動輸入</strong> </p> <p>在[！UICONTROL活頁簿ID]欄位中，輸入或對應包含您要更新之資料表的活頁簿ID。</p> <p>在[！UICONTROL表格名稱]欄位中，輸入或對應您要更新的表格名稱。</p> </li> 
     <li> <p><strong>[！UICONTROL從清單中選取]</strong> </p> <p>選取包含您要更新之表格的活頁簿和工作表，然後選取表格。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL表格] </td> 
   <td> <p>選取要更新的表格。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL名稱]</td> 
   <td> <p>如果要重新命名表格，請輸入或對應表格的新名稱。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Show Headers]</td> 
   <td> <p>啟用此選項以顯示更新表格的標題。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL顯示總計]</td> 
   <td>啟用此選項以顯示表格的總值。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL樣式]</td> 
   <td>選擇新表格的樣式。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 刪除資料表]

此動作模組會從[!DNL Excel]工作表刪除指定的資料表。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>如需有關將您的[!DNL Office 365]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中建立案例一文中的<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連線到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL取得表格]</td> 
   <td> <p>選取您要如何識別要刪除的表格。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL手動輸入]</strong> </p> <p>在[！UICONTROL活頁簿ID]欄位中，輸入或對應包含您要刪除之表格之活頁簿的ID。</p> <p>在[！UICONTROL表格名稱]欄位中，輸入或對應您要刪除的表格名稱。</p> </li> 
     <li> <p><strong>[！UICONTROL從清單中選取]</strong> </p> <p>選取包含您要刪除之表格的活頁簿和工作表，然後選取表格。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 其他

* [[!UICONTROL 擷取資料]](#retrieve-data)
* [[!UICONTROL 進行API呼叫]](#make-an-api-call)

#### [!UICONTROL 擷取資料]

此動作會從定義的工作表範圍擷取資料，並傳回每一列的組合。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>如需有關將您的[!DNL Office 365]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中建立案例一文中的<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連線到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL活頁簿] </td> 
   <td> <p>選取包含您要擷取之資料的活頁簿。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL工作表] </td> 
   <td> <p>選取包含您要擷取之資料的工作表。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL範圍] </td> 
   <td> <p>指定您要擷取資料的工作表區域，方法為指定左上方與右下方的儲存格。 範例： <code>A1:D10</code></p> </td> 
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
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>如需有關將您的[!DNL Office 365]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中建立案例一文中的<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連線到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL URL]</td> 
   <td>輸入相對於<code>https://graph.microsoft.com</code>的路徑。 範例：<code> /v1.0/me/drive/root/children</code></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL方法]</td> 
   td&gt; <p>選取設定API呼叫所需的HTTP要求方法。 如需詳細資訊，請參閱[!DNL Adobe Workfront Fusion]</a>中的<a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP要求方法。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Headers]</td> 
   <td> <p>以標準JSON物件的形式新增請求的標頭。</p> <p>例如， <code>{"Content-type":"application/json"}</code></p> <p>Workfront Fusion會為您新增授權標頭。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL查詢字串]</td> 
   <td> <p>以標準JSON物件的形式新增API呼叫的查詢。</p> <p>例如： <code>{"name":"something-urgent"}</code></p> </td> 
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
