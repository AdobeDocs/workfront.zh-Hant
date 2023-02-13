---
product-area: reporting
navigation-topic: text-mode-reporting
title: 在文字模式中使用條件式格式
description: 在文字模式中使用條件式格式
author: Nolan
feature: Reports and Dashboards
exl-id: 48fc8450-35c6-4d59-89d3-0feffe662b25
source-git-commit: 16d59c6e3d790f2804795f5a6fef05c8dca71b30
workflow-type: tm+mt
source-wordcount: '1758'
ht-degree: 2%

---

# 在文字模式中使用條件式格式

<!--
(NOTE: Alina: this article might need to be split in its sections. Tony asked that numbers and dates should be in separate articles (??))
-->

標準介面產生器在建立報表元素時，可提供極大的彈性，以符合組織的需求。

您可以使用標準介面，在檢視中套用條件式格式。\
如需將條件式格式套用至檢視的詳細資訊，請參閱 [在檢視中使用條件式格式](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md).

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>計劃 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>編輯對篩選器、檢視、群組的存取</p> <p>編輯對報表、控制面板、日曆的存取，以編輯報表中的檢視</p> <p>注意：如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>管理報表權限以編輯報表中的檢視</p> <p>管理檢視的權限以進行編輯</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 文本模式中的條件式格式

文本模式允許您使用標準介面中不可用的欄位，從而建立更複雜的視圖、篩選器、分組和提示。

如需所有可報告欄位的完整清單，請參閱  [API Explorer](../../../wf-api/general/api-explorer.md).

如需使用文字模式語法的詳細資訊，請參閱 [文字模式語法概觀](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md).

您也可以使用文字模式來設定報表和清單中的檢視格式。 您可以使用條件式格式，透過變更報表中結果的字型類型和背景，以及圖示和標幟，來變更報表的檢視。 建議您一律先使用標準介面建置檢視，並在絕對必要時切換至文字模式介面。

>[!NOTE]
>
> 不支援使用CSS樣式來自訂條件式格式。 您必須改用Adobe Workfront中提供的預先設計格式選項。

## 新增條件式格式至檢視

如需將條件式格式套用至標準產生器介面中檢視的詳細資訊，請參閱 [在檢視中使用條件式格式](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md).

要在文本模式介面中向視圖添加條件格式：

1. 轉到對象清單。
1. 展開您要新增條件式格式的檢視的下拉式功能表。
1. 按一下 **自訂檢視**.
1. 在要套用條件式格式的檢視中，按一下欄。
1. 按一下 **切換到文本模式**.
1. 在 **顯示於此欄中：** 按一下 **按一下「 」以編輯文字**.
1. 新增中提供的程式碼範例 [使用文字模式設定檢視格式](#format-views-using-text-mode) 在所選列中的文本底部。
1. 按一下 **儲存**，然後按一下 **保存視圖**.

## 使用文字模式設定檢視格式 {#format-views-using-text-mode}

您可以將下列元件新增至檢視中的欄，以有條件地以文字模式格式化：

* [欄設定](#column-settings)
* [欄規則](#column-rules)
* [有條件地格式化值表達式](#conditionally-format-a-valueexpression)

### 欄設定 {#column-settings}

您必須先熟悉文字模式介面，才能將條件式格式新增至檢視。

在檢視中使用條件式格式時，您可以自訂欄的下列元素：

* [欄標題](#column-headers)
* [日期格式](#format-dates)
* [格式編號](#format-numbers)

#### 欄標題 {#column-headers}

若要變更顯示的欄標題，請新增下列程式碼至您的欄： `displayname= [Name of column]`. 例如，若要將欄命名為「專案擁有者」，文字代碼會如下所示：

```
displayname=Project Owner
```

#### 日期格式 {#format-dates}

日期可設定為以多種格式顯示。

如需詳細資訊，請參閱 [以文字模式報表格式化日期](../../../reports-and-dashboards/reports/text-mode/format-dates-in-text-mode-reports.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this is drafted and replaced by the article linked above)</p>
<p>To establish a date format, you must modify the <code>valueformat</code> line of the text mode code in the column.</p>
<pre>valueformat= [new date format]</pre>
<p>For example, if you wanted the Projected Completion Date to be displayed as MM/DD/YY the code would look like:</p>
<pre>valueformat=atDate<br>valuefield=projectedCompletionDate </pre>
<p>If you wanted to show the Planned Completion Date as <em>Mth, DD, Year</em>, the code would look like:</p>
<pre>valueformat=mediumAtdate<br>valuefield=plannedCompletionDate</pre>
<p>You can format dates using the following <code>valueformat</code> text mode values:</p>
<table style="table-layout:auto">
<col>
<col>
<col>
<thead>
<tr>
<th scope="col"><strong>Format</strong> </th>
<th scope="col">Example </th>
<th scope="col"><em><strong>valueformat=</strong></em> </th>
</tr>
</thead>
<tbody>
<tr>
<td>MM/DD/YY</td>
<td>10/11/18</td>
<td><pre>atDate</pre> </td>
</tr>
<tr>
<td>MM/DD/YY Time</td>
<td>10/11/18 12:00pm</td>
<td><pre>longAtDate</pre> </td>
</tr>
<tr>
<td>MM/DD/YY</td>
<td>10/11/18</td>
<td><pre>shortAtDate</pre> </td>
</tr>
<tr>
<td>Mth, DD, YR</td>
<td>Oct, 11, 2018</td>
<td><pre>mediumAtDate</pre> </td>
</tr>
<tr>
<td>DW, Mth, Day, YR</td>
<td>Mon, Oct, 11, 2018</td>
<td><pre>partialAtDate</pre> </td>
</tr>
<tr>
<td>DW, Mth, Day, YR Time</td>
<td>Mon, Oct, 11, 2018 12:00 pm</td>
<td><pre>fullAtDate</pre> </td>
</tr>
</tbody>
</table>
</div>
-->

#### 格式編號 {#format-numbers}

您可以設定數值格式，以顯示最符合您報表需求的資訊。

如需詳細資訊，請參閱 [文本模式報告中的數字、貨幣和百分比值的格式](../../../reports-and-dashboards/reports/text-mode/format-numbers-in-text-mode-reports.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>To modify the format of a numeric value, you must edit the <strong>valueformat</strong> line of your column.</p> 
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this is drafted and replaced by the article linked above) </p>
<p>For example, if you wanted to display the Budget column as $1000, the value format line would look like:</p>
<pre>valueformat=currencyStringCurrencyRounded<br>valuefield=budget</pre>
<p>You can format numbers using the following values for the <code>valueformat</code> line of your column:</p>
<table border="2" cellspacing="15" cellpadding="1">
<col>
<col>
<thead>
<tr>
<th scope="col"><strong>Example</strong> </th>
<th scope="col"><em><code>valueformat=</code></em> </th>
</tr>
</thead>
<tbody>
<tr>
<td>1234</td>
<td><pre>doubleAsString</pre> or <pre>int</pre></td>
</tr>
<tr>
<td>1,234</td>
<td><pre>doubleAsInt</pre> </td>
</tr>
<tr>
<td>$1,234</td>
<td><pre>currencyStringCurrencyRounded</pre> </td>
</tr>
<tr>
<td>1234.56</td>
<td><pre>doubleAsDouble</pre> </td>
</tr>
<tr>
<td>$1,234.56</td>
<td><pre>currencyStringCurrency</pre> </td>
</tr>
<tr>
<td>12%</td>
<td><pre>doubleAsPercentRounded</pre> </td>
</tr>
<tr>
<td>12.34%</td>
<td><pre>doubleAsPercent</pre> </td>
</tr>
<tr>
<td>(1,234.56)</td>
<td><pre>doubleAsFinancial</pre> </td>
</tr>
<tr>
<td>(1,234)</td>
<td><pre>doubleAsFiancialRounded</pre> </td>
</tr>
</tbody>
</table>
</div>
-->

### 欄規則 {#column-rules}

欄規則允許在檢視中新增影像、顏色、格式和文字覆寫。 欄規則可以獨立建立，也可以包含欄的多個條件。

* [條件式格式設定](#conditional-formatting)
* [多種條件式格式](#multiple-conditional-formats)
* [套用文字](#apply-text)
* [應用行格式](#apply-row-formats)
* [套用影像](#apply-images)

#### 條件式格式設定 {#conditional-formatting}

合併顏色或格式化文本時，必須應用特定文本模式語句。

>[!NOTE]
>
>合併的列中可能不支援條件式格式。\
>有關使用文本模式合併列的詳細資訊，請參見 [查看：從一個共用列中合併多列中的資訊](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-merge-columns.md).

在您要新增條件式格式的任何欄中插入下列程式碼：

```
styledef.case.0.comparison.leftmethod= [field name]
styledef.case.0.comparison.lefttext= [field name]
styledef.case.0.comparison.righttext= [field value]
styledef.case.0.comparison.operator= [qualifier]
styledef.case.0.comparison.operatortype= [data type]
styledef.case.0.comparison.icon=false
styledef.case.0.comparison.truetext= 
styledef.case.0.comparison.trueproperty.0.name= [format option]
styledef.case.0.comparison.trueproperty.0.value= [format style]
```

>[!NOTE]
>
>此 *styledef.case.0.comparison.icon* 除非使用圖示，否則行一律為false。
>
>此 *styledef.case.0.comparison.truetext* 直到處理覆寫文字為止，折線始終留空。
>
>此 *styledef.case.0.comparision.righttext* 當限定符不為空時，行為空。

例如，如果我們想在專案報表上以綠色文字顯示公司名稱，您可以使用下列程式碼：

```
styledef.case.0.comparison.leftmethod=company:name
styledef.case.0.comparison.lefttext=company:name ;
styledef.case.0.comparison.righttext= 
styledef.case.0.comparison.operator=notblank
styledef.case.0.comparison.operatortype=string
styledef.case.0.comparison.icon=false
styledef.case.0.comparison.truetext=
styledef.case.0.comparison.trueproperty.0.name=textcolor
styledef.case.0.comparison.trueproperty.0.value=03a219
```

>[!NOTE]
>
>* 此陳述式可套用至「公司名稱」欄，也可套用至報表上的任何其他欄。 只有在專案有關聯的公司時，才會顯示綠色文字。 記住 `[field name]`, `[value]`，和 `[qualifier]` 驅動是否最終在列上顯示條件。
>* 使用限定詞時，我們建議使用 `cicontains` 而非 `equal`. 依預設， `equal` 尋找ID號碼。 使用 `cicontains` 限定符，您可以按項目名稱訪問項目。


![](assets/screen-shot-2013-08-15-at-2.53.51-pm-350x199.png)

![](assets/screen-shot-2013-08-15-at-2.54.08-pm-350x185.png)

無論文本顏色、對齊方式、字型樣式還是背景顏色都應用於文本模式，都使用相同的語句（如上所示）。

必須修改下列行以反映列所需的相應格式：

```
styledef.case.0.comparison.trueproperty.0.name= [format option]
styledef.case.0.comparison.trueproperty.0.value= [format style]
```

使用下表來標識需要修改的行以及應指定哪些值來定義列的格式樣式：

| **文字顏色** | **行：textcolor=** |
|---|---|
| 黑色 | `000000` |
| 深藍色 | `0c6aca` |
| 蒂爾 | `1b878c` |
| 綠色 | `03a219` |
| 紫色 | `6408c4` |
| 灰色 | `767676` |
| 紅色 | `d30519` |
| 黃色 | `e19503` |

{style=&quot;table-layout:auto&quot;}

| **校準** | **行：align=** |
|---|---|
| 左對齊 | `left` |
| 右對齊 | `right` |
| 居中對齊 | `center` |

{style=&quot;table-layout:auto&quot;}

| 字型 | 行： ***fontstyle=*** |
|---|---|
| 粗體 | `bold` |
| 斜體 | `italic` |

{style=&quot;table-layout:auto&quot;}

| **背景顏色** | **行：bgcolor=** |
|---|---|
| 蒂爾 | `dcf6f7` |
| 綠色 | `def6e2` |
| 灰色 | `e8e8e8` |
| 藍色 | `e8f1ff` |
| 紫色 | `e9def4` |
| 紅色 | `eac6c9` |
| 黃色 | `feecc8` |
| 白色 | `ffffff` |

{style=&quot;table-layout:auto&quot;}

#### 多種條件式格式 {#multiple-conditional-formats}

可以將多個格式樣式應用到語句。 核心語句保持不變，任何附加格式表達式將添加到該語句中。

例如，使用先前的陳述式，在綠色粗體文字中加入公司名稱。 該語句將使用以下代碼編寫：

```
styledef.case.0.comparison.leftmethod=company:name
styledef.case.0.comparison.lefttext=company:name
styledef.case.0.comparison.righttext=
styledef.case.0.comparison.operator=notblank
styledef.case.0.comparison.operatortype=string
styledef.case.0.comparison.icon=false
styledef.case.0.comparison.truetext= 
styledef.case.0.comparison.trueproperty.0.name=textcolor
styledef.case.0.comparison.trueproperty.0.value=03a219
styledef.case.0.comparison.trueproperty.1.name=fontstyle
styledef.case.0.comparison.trueproperty.1.value=bold
```

>[!NOTE]
>
>當包含多個條件式格式表達式時，必須用數字標識語句中的每個表達式。 請注意，已識別運算式0和運算式1。

![](assets/screen-shot-2013-08-15-at-3.18.45-pm-350x198.png)

#### 套用文字 {#apply-text}

如果要用您選擇的值替換列中填充的預設值，則在將文本應用於列時可能。

例如，在項目報表上，將「計畫起始日期」列值設定為不顯示項目的計畫起始日期，而是顯示「非今天」文本。 對「計劃開始日期」列使用以下代碼：

```
case.0.comparison.leftmethod=plannedStartDate
case.0.comparison.lefttext=plannedStartDate
case.0.comparison.righttext=2013-04-10T10:45:00:000
case.0.comparison.operator=ne
case.0.comparison.operatortype=date
case.0.comparison.icon=false
case.0.comparison.truetext=not today
styledef.case.0.comparison.leftmethod=plannedStartDate
styledef.case.0.comparison.lefttext=plannedStartDate
styledef.case.0.comparison.righttext=2013-04-10T10:45:00:000 
styledef.case.0.comparison.operator=ne
styledef.case.0.comparison.operatortype=date&
styledef.case.0.comparison.icon=false
styledef.case.0.comparison.truetext=not today
```

>[!NOTE]
>
>開頭為 `case.0.` 使用案例比較來識別文字的使用。 開頭為 **styledef.case.0。** 是早期的條件式格式陳述式，可讓我們透過 `truetext` 運算式。 請務必設定 `truetext` 值，而非保留為空白。

![](assets/screen-shot-2013-08-15-at-3.22.02-pm-350x196.png)

![](assets/screen-shot-2013-08-15-at-3.22.16-pm-350x151.png)

#### 應用行格式 {#apply-row-formats}

如果您想要將條件套用至整列，請搭配您的欄程式碼使用下列程式碼：

```
styledef.case.0.comparison.icon=false
```

```
styledef.case.0.comparison.isrowcase=true
```

```
styledef.case.0.comparison.leftmethod= [field name]
```

```
styledef.case.0.comparison.lefttext= [field name]
```

```
styledef.case.0.comparison.operator= [qualifier]
```

```
styledef.case.0.comparison.operatortype= [data type]
```

```
styledef.case.0.comparison.righttext= [field value]
```

```
styledef.case.0.comparison.trueproperty.0.name= [format option]
```

```
styledef.case.0.comparison.trueproperty.0.value= [format style]
```

```
styledef.case.0.comparison.truetext=
```

```
row.0.styledef.applyallcases=true
```

```
row.0.styledef.case.0.comparison.icon=false
```

```
row.0.styledef.case.0.comparison.isrowcase=true
```

```
row.0.styledef.case.0.comparison.leftmethod= [field name]
```

```
row.0.styledef.case.0.comparison.lefttext= [field name]
```

```
row.0.styledef.case.0.comparison.operator= [qualifier]
```

```
row.0.styledef.case.0.comparison.operatortype= [data type]
```

```
row.0.styledef.case.0.comparison.righttext= [field value]
```

```
row.0.styledef.case.0.comparison.trueproperty.0.name= [format option]
```

```
row.0.styledef.case.0.comparison.trueproperty.0.value= [format style]
```

```
row.0.styledef.case.0.comparison.truetext=
```


#### 套用影像 {#apply-images}

與使用文字進行格式設定類似，影像也可用來在報表中顯示資訊。 Workfront有許多內建影像，可傳達報表設定中的視覺資訊。 若要在條件式格式設定中使用影像，需要下列陳述式：

```
image.case.0.comparison.leftmethod= [field name]
image.case.0.comparison.lefttext= [field name]
image.case.0.comparison.righttext= [field value]
image.case.0.comparison.operator= [qualifier]
image.case.0.comparison.operatortype= [data type]
image.case.0.comparison.icon=true
image.case.0.comparison.truetext=
```

例如，在項目報表上，您想要建立一個欄，其中顯示每個計畫完成日期（不等於今天的日期）的皺眉。 使用下列文字模式代碼將圖示新增至欄：

```
image.case.0.comparison.leftmethod=plannedCompletionDate
image.case.0.comparison.lefttext=plannedCompletionDate
image.case.0.comparison.righttext=2013-04-10T13:00:00:000 
image.case.0.comparison.operator=ne 
image.case.0.comparison.operatortype=date
image.case.0.comparison.icon=true
image.case.0.comparison.truetext=/interface/images/v4_redux/icons/casebuilder/emoticon_frown.gif
```

>[!NOTE]
>
>請注意，陳述式使用 `icon=true` 運算式。 此語句也與其他條件式格式語句不同，因為它不使用 `style.def` 格式，而非唯一的影像格式。

![](assets/screen-shot-2013-08-15-at-3.35.08-pm-350x199.png)

![](assets/screen-shot-2013-08-15-at-3.35.22-pm-1-350x167.png)

若要使用可用的影像，請套用下列程式碼和值：

| **圖示** | **行：image.case.0.comparison.truetext=** |
|---|---|
| 皺眉臉 ![](assets/face-sad.png) | =`/interface/images/v4_redux/icons/casebuilder/emoticon_frown.gif` |
| 快樂臉 ![](assets/face-happy.png) | =`/interface/images/v4_redux/icons/casebuilder/emoticon_smile.gif` |
| 藍旗  ![](assets/flag-blue-large.png) | =`/interface/images/v4_redux/icons/casebuilder/flag_blue.gif` |
| 綠旗  ![](assets/flag-green-large.png) | =`/interface/images/v4_redux/icons/casebuilder/flag_green.gif` |
| 紅旗  ![](assets/flag-red-style2.png) | =`/interface/images/v4_redux/icons/casebuilder/flag_red.gif` |
| 黃旗  ![](assets/flag-yellow-style2.png) | =`/interface/images/v4_redux/icons/casebuilder/flag_yellow.gif` |
| 黑色圓圈  ![](assets/dot-black.png) | =`/interface/images/v4_redux/icons/casebuilder/light_black.gif` |
| 藍色圓圈 ![](assets/dot-blue.png) | =`/interface/images/v4_redux/icons/casebuilder/light_blue.gif` |
| 灰圓 ![](assets/dot-gray.png) | =`/interface/images/v4_redux/icons/casebuilder/light_grey.gif` |
| 綠色圓圈 ![](assets/dot-green.png) | =`/interface/images/v4_redux/icons/casebuilder/light_green.gif` |
| 橙色圓圈 ![](assets/dot-orange.png) | =`/interface/images/v4_redux/icons/casebuilder/light_orange.gif` |
| 粉紅色圓圈 ![](assets/dot-pink.png) | =`/interface/images/v4_redux/icons/casebuilder/light_pink.gif` |
| 紫色圓圈 ![](assets/dot-purple.png) | =`/interface/images/v4_redux/icons/casebuilder/light_purple.gif` |
| 紅圓圈 ![](assets/dot-red.png) | =`/interface/images/v4_redux/icons/casebuilder/light_red.gif` |
| 白圈 ![](assets/dot-white.png) | =`/interface/images/v4_redux/icons/casebuilder/light_white.gif` |
| 黃色圓 ![](assets/dot-yellow.png) | =`/interface/images/v4_redux/icons/casebuilder/light_yellow.gif` |

{style=&quot;table-layout:auto&quot;}

### 有條件式格式 `valueexpression` {#conditionally-format-a-valueexpression}

若要在欄中顯示計算值，您可以取代 `valuefield` 行代碼(含 `valueexpression`. 計算值允許您根據同一對象上兩個現有欄位之間的計算來顯示對象的新值。

如需格式化的詳細資訊 `valueexpression line`，請參閱 [文字模式語法概觀](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md).

您無法有條件地格式化包含 `valueexpression` 代碼行。 反之，您可以將「計算自訂欄位」新增至「自訂表單」，並將其與報表中顯示的物件建立關聯。 然後，您可以有條件地設定顯示此欄位的欄格式。

如需計算自訂欄位的詳細資訊，請參閱 [將計算資料新增至自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

## 在「文字模式」欄中新增匯總值

建議您先在產生器介面中建置欄、在此新增匯總值，然後在文字模式中編輯欄。

在文本模式中將聚合器添加到列時，請考慮以下事項：

* 欄中的值必須有可匯總的格式。 例如，它們必須有下列其中一種格式：

   * 數量
   * 日期
   * 貨幣

* 您可以將匯總器新增至顯示計算的欄。 匯總值會顯示在檢視或報表的分組中。 如需詳細資訊，請參閱 [分組：顯示在分組中聚合多個計算值的結果](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/grouping-calculation-between-two-fields-aggregated-in-grouping.md).
* 列定義的代碼行必須與引入聚合器的代碼行相同，前面加上「聚合器」。 例如，如果您有一個列，其中在項目上顯示了計畫小時數，則列的主行的文本模式為：

   ```
   valuefield=workRequired
   valueformat=compound
   ```

   如果要匯總視圖分組中所有行的值，可以添加以下代碼以添加聚合器值： `aggregator.valuefield=workRequired` ( `aggregator.valuefield` 行必須與 `valuefield` 說明欄) `aggregator.valueformat=compound` ( `aggregator.valueformat` 行的值必須與 `valueformat` 說明欄) `aggregator.function=SUM` （這是表示要如何匯總列的強制行，在此情況下，您要將所有單個計畫小時數添加到分組行中的一個數字中） `aggregator.displayformat=minutesAsHoursString` (因為小時數以分鐘為單位儲存在Workfront中，我們想指出 `displayformat` （以分鐘為單位）
