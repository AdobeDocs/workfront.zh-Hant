---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: 連接器
navigation-topic: apps-and-their-modules
title: Google Forms模組
description: 此 [!DNL Adobe Workfront Fusion Google Forms] 模組可讓您監視、選取、新增、更新或刪除Google Forms上的回應。
author: Becky
feature: Workfront Fusion
exl-id: 45c86879-bc4e-4134-b63c-02410b9de43b
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1382'
ht-degree: 0%

---

# [!DNL Google Forms] 模組

此 [!DNL Adobe Workfront Fusion] [!DNL Google Forms] 模組可讓您監視、選取、新增、更新或刪除您的回應 [!DNL Google Forms].

為了使用 [!DNL Google Docs] with [!DNL Adobe Workfront Fusion]，則必須有 [!DNL Google] 帳戶。 如果你沒有 [!DNL Google] 帳戶，您可以在 [!DNL Google] 帳戶說明頁面。

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

使用 [!DNL Google Forms] 模組，您必須 [!DNL Google] 帳戶。

## 從表單建立試算表

若要處理您的表單回應，必須建立回應的試算表。

1. 開啟表單。
1. 前往 **[!UICONTROL 回應]** 標籤。
1. 按一下 **[!UICONTROL 建立試算表]** 圖示 ![](assets/spreadsheet-icon.png).

1. 選擇您要建立新試算表還是現有試算表
1. 按一下 **[!UICONTROL 建立]**。

## [!DNL Google Forms] 模組及其欄位

設定時 [!DNL Google Forms] 模組， [!DNL Workfront Fusion] 顯示下列欄位。 此外， [!DNL Google Forms] 視您在應用程式或服務中的存取層級等因素而定，可能會顯示欄位。 模組中的粗體標題表示必填欄位。

如果您在欄位或函式上方看到對應按鈕，則可使用它來設定該欄位的變數和函式。 如需詳細資訊，請參閱 [將資訊從一個模組對應到 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [觸發器](#triggers)
* [動作](#actions)
* [搜尋](#searches)

### 觸發器

#### [!UICONTROL 監看回應]

監視表單以取得新回應。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL Google] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連接到 [!DNL Workfront Fusion]</a> 在文章中 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在中建立案例 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL電子錶格]</td> 
   <td> <p>從您要查看新回應的表單中，選取包含回應的試算表。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL工作表]</td> 
   <td> <p> 選擇包含表單響應的工作表。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL帶標題的行]</td> 
   <td>指定表格的標題列。 預設列為 <code>A1:Z1</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL值呈現選項]</td> 
   <td> <p>指定要如何在輸出中呈現值。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL格式化值]</strong> </p> <p>值會根據儲存格的格式在回覆中計算並格式化。 格式設定是根據試算表的地區設定，而非要求使用者的地區設定。 例如，若 <code>A1</code> is <code>1. 23</code> 和 <code>A2 </code>is <code>=A1</code> 格式為貨幣，則 <code>A2</code> 傳回 <code>$1. 23</code> .</p> </li> 
     <li> <p><strong>[!UICONTROL未格式化的值]</strong> </p> <p>值會經過計算，但不會在回覆中格式化。 例如，若 <code>A1</code> is <code>1. 23</code> 和 <code>A2 </code>is <code>=A1</code> 格式為貨幣，則 <code>A2</code> 返回數字 <code>1. 23</code> .</p> </li> 
     <li> <p><strong>[!UICONTROL公式]</strong> </p> <p>不會計算值。 回覆包含公式。 例如，若 <code>A1</code> is <code>1. 23</code> 和 <code>A2 </code>is <code>=A1</code> 格式為貨幣，則 <code>A2</code> 傳回 <code>=A1</code>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL日期和時間呈現選項]</td> 
   <td>選取要在輸出中顯示日期、時間和持續時間的方式。 如果將[!UICONTROL值呈現選項]設定為[!UICONTROL格式化值]，則忽略此欄位。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL限制]</td> 
   <td> <p> 設定 [!DNL Workfront Fusion] 可在單一週期中運作。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 動作

* [[!UICONTROL 新增回應]](#add-a-response)
* [[!UICONTROL 更新回應]](#update-a-response)
* [[!UICONTROL 刪除回應]](#delete-a-response)

#### [!UICONTROL 新增回應]

此模組會在表單試算表底部附加新回應。

設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL Google] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連接到 [!DNL Workfront Fusion]</a> 在文章中 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在中建立案例 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL電子錶格]</td> 
   <td> <p>選擇包含要添加響應的工作表的電子錶格。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL工作表]</td> 
   <td> <p> 選擇包含表單響應的工作表。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[!UICONTROL值]</p> </td> 
   <td> <p>在工作表列中輸入所需值。</p> <p>對於格式正確的[!UICONTROL時間戳]列，請使用以下值：</p><pre>formatDate(now;DD/MM/YYYY HH:mm;UTC)</pre> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL值輸入選項]</td> 
   <td> 
    <ul> 
     <li> <p><strong>[!UICONTROL Raw]</strong> </p> <p> 使用者輸入的值不會剖析，並依原樣儲存。 </p> </li> 
     <li> <p><strong>[!UICONTROL用戶輸入]</strong></p> <p>系統會將值剖析為使用者在UI中輸入值。 數字仍然是數字，但字串可以按照在透過 [!DNL Google Sheets] UI。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL插入資料選項]</td> 
   <td> <p>指定輸入新資料時如何變更現有資料。 </p> 
    <ul> 
     <li> <p><strong>[!UICONTROL覆蓋]</strong> </p> <p>新資料會覆寫寫入區域中的現有資料。 將資料添加到工作表末尾將插入新行或列，以便寫入資料。</p> </li> 
     <li> <p><strong>[!UICONTROL插入行]</strong></p> <p>會為新資料插入行。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 更新回應]

此模組會更新所選回應。

設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL Google] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連接到 [!DNL Workfront Fusion]</a> 在文章中 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在中建立案例 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL電子錶格]</td> 
   <td> <p>選擇包含要更新響應的工作表的電子錶格。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL工作表]</td> 
   <td> <p> 選擇包含表單響應的工作表。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL行號]</p> </td> 
   <td> <p>輸入或映射要更新的行數。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL值]</p> </td> 
   <td> <p>輸入所需欄的新值。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL值輸入選項]</td> 
   <td> 
    <ul> 
     <li> <p><strong>[!UICONTROL Raw]</strong> </p> <p> 使用者輸入的值不會剖析，並依原樣儲存。 </p> </li> 
     <li> <p><strong>[!UICONTROL用戶輸入]</strong></p> <p>系統會將值剖析為使用者在UI中輸入值。 數字仍然是數字，但字串可以按照在透過 [!DNL Google Sheets] UI。</p> </li> 
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
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL Google] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連接到 [!DNL Workfront Fusion]</a> 在文章中 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在中建立案例 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL電子錶格]</td> 
   <td> <p>選擇包含要刪除響應的工作表的電子錶格。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL工作表]</td> 
   <td> <p> 選擇包含表單響應的工作表。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL行號]</p> </td> 
   <td> <p>輸入或映射要刪除的行數。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 搜尋

* [[!UICONTROL 搜尋回應]](#search-responses)
* [[!UICONTROL 搜尋回應（進階）])](#search-responses-advanced)

#### [!UICONTROL 搜尋回應]

此模組會傳回符合指定條件的回應。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
    <td>連接</td>
   <td> <p>有關連接 [!DNL Google] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連接到 [!DNL Workfront Fusion]</a> 在文章中 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在中建立案例 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
    <td>[!UICONTROL電子錶格]</td>
   <td> <p>選擇要搜索的表單。</p> </td> 
  </tr> 
  <tr data-mc-conditions="">
    <td>[!UICONTROL工作表] </td>
   <td> <p>選擇包含表單響應的工作表。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
    <td>[!UICONTROL列範圍]</td>
   <td> <p> 選擇要搜索的列範圍。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL篩選器]</td> 
   <td> <p>定義要依搜尋回應的篩選器。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
    <td>[!UICONTROL排序順序] </td>
   <td> <p>選擇按升序還是降序排序返回的響應。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
    <td>[!UICONTROL順序依據]</td>
   <td> <p> 選擇要按返迴響應排序的列。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL值呈現選項]</td> 
   <td> <p>指定要如何在輸出中呈現值。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL格式化值]</strong></p> <p>值會根據儲存格的格式在回覆中計算並格式化。 格式設定是根據試算表的地區設定，而非要求使用者的地區設定。 例如，若 <code>A1</code> is <code>1. 23</code> 和 <code>A2 </code>is <code>=A1</code> 格式為貨幣，則 <code>A2</code> 傳回 <code>$1. 23</code> .</p> </li> 
     <li> <p><strong>[!UICONTROL未格式化的值]</strong> </p> <p>值會經過計算，但不會在回覆中格式化。 例如，若 <code>A1</code> is <code>1. 23</code> 和 <code>A2 </code>is <code>=A1</code> 格式為貨幣，則 <code>A2</code> 返回數字 <code>1. 23</code> .</p> </li> 
     <li> <p><strong>[!UICONTROL公式]</strong> </p> <p>不會計算值。 回覆包含公式。 例如，若 <code>A1</code> is <code>1. 23</code> 和 <code>A2 </code>is <code>=A1</code> 格式為貨幣，則 <code>A2</code> 傳回 <code>=A1</code>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions="">
    <td>[!UICONTROL日期和時間呈現選項]</td>
    <td>選取要在輸出中顯示日期、時間和持續時間的方式。 如果[!UICONTROL值呈現]選項設定為格式化值，則忽略此欄位。 </td>
  </tr> 
  <tr>
    <td role="rowheader" data-mc-conditions="QuicksilverOrClassic.Draft mode">[!UICONTROL返迴響應的最大數]</td>
   <td> <p> 設定 [!DNL Workfront Fusion] 在一個週期中傳回。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 搜尋回應（進階）]

此模組使用 [[!DNL Google Charts Query Language]](https://developers.google.com/chart/interactive/docs/querylanguage). 此模組不會傳回列號。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
    <td>[!UICONTROL連接]</td>
   <td> <p>有關連接 [!DNL Google] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連接到 [!DNL Workfront Fusion]</a> 在文章中 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在中建立案例 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr>
    <td>[!UICONTROL電子錶格]</td>
   <td> <p>選擇包含要搜索工作表的電子錶格。</p> </td> 
  </tr> 
  <tr>
    <td>[!UICONTROL工作表]</td>
   <td> <p> 選擇包含表單響應的工作表。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL篩選器]</td> 
   <td> <p>使用 <a href="https://developers.google.com/chart/interactive/docs/querylanguage">[!DNL Google Charts Query Language]</a>.</p> <p>範例： <code>select * where C = "John"</code> 擷取C欄為「John」的列的所有值。</p> </td> 
  </tr> 
  <tr>
    <td>[!UICONTROL返回行數上限]</td>
   <td> <p> 設定 [!DNL Workfront Fusion] 在一個週期中傳回。</p> </td> 
  </tr> 
 </tbody> 
</table>
