---
content-type: overview
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: 計算自訂欄位與計算欄的比較
description: 若要彙總Adobe Workfront中的多個欄位並在新欄位中顯示彙總值，您可以在自訂表單中建立計算自訂欄位，或在檢視中建立計算欄。
author: Jenny
feature: Reports and Dashboards
exl-id: 17ac554d-0c90-4592-946e-a89f1784571d
source-git-commit: a1ead6d0c1c85bfbe6d7302506743db8d8b3e205
workflow-type: tm+mt
source-wordcount: '817'
ht-degree: 0%

---

# 計算自訂欄位與計算欄的比較

若要在Adobe Workfront中彙總數個欄位，並在新欄位中顯示該彙總值，您可以建立下列專案：

* 自訂表單中的計算自訂欄位\
  如需新增計算自訂欄位至自訂表單的詳細資訊，請參閱[新增計算欄位至表單](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md)。

* 檢視中的計算欄\
  如需有關在檢視中使用計算的詳細資訊，請參閱文章[文字模式常見用途概觀](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md#use-text-mode-in-views)中的[在檢視中使用文字模式](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md)一節。

雖然您使用文字模式來建立計算欄位和計算欄，但建立它們的語法不同。 請參閱上方列出的文章，以瞭解如何建立計算欄位和計算欄。 如需有關計算資料運算式（例如計算自訂欄位和欄）中所使用的不同語法的資訊，請參閱本文中的[計算自訂欄位與計算自訂欄位的語法](/help/quicksilver/reports-and-dashboards/reports/calc-cstm-data-reports/calculated-custom-fields-calculated-columns.md#syntax-of-calculated-custom-fields-vs-calculated-custom-columns)小節。

您可以在計算欄位和計算欄中使用相同的計算。 不過，視您用於這些計算的目的而定，您可能會想要考慮建立其中一個。

## 計算自訂欄位與計算自訂欄的語法

雖然您使用的函式相同，但在計算自訂欄位中建立運算式的語法可能與建立計算自訂欄的語法不同。

例如：

* 在自訂欄位中，在任務的自訂表單上，您可以使用以下專案產生附加自訂表單之任務的父專案名稱：

  `{project}.{name}`

* 在報表的自訂欄中，您會使用下列專案，在任務報表中新增「專案名稱」自訂欄：

  `valuefield=project:name`

  或

  `valueexpression={project}.{name}`

  >[!TIP]
  >
  >相同的語法會套用至使用計算運算式的所有文字模式報表元素：檢視、篩選器、群組和提示。

兩種語法之間的差異為：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>計算的自訂欄位</strong></td>
   <td><strong>已計算的自訂報表元素</strong></td> 
  </tr> 
  <tr> 
   <td> <p>使用在Workfront介面中顯示的欄位名稱。</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>範例： </b></span></span>計算自訂欄位中使用的欄位名稱範例： <code>Planned Completion Date</code>。</p> </td> 
   <td> <p>使用物件或欄位出現在Workfront資料庫中的名稱。 如果物件和欄位是複合名稱，則以小寫或駝峰式大小寫拼寫。 </p> <p>如需所有Workfront物件和欄位在資料庫中顯示的詳細目錄，請參閱<a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">API總管</a>。 </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>範例： </b></span></span>計算自訂報表元素中使用的欄位名稱範例： <code>plannedCompletionDate</code>。</p> </td> 
  </tr> 
  <tr> 
   <td>以括弧或大括弧括住欄位名稱</td> 
   <td> <p>在<code>valuefield </code>行中使用欄位名稱時，請勿將其括在方括弧或括弧中。</p> <p>在<code>valueexpression</code>行中使用欄位名稱時，請將欄位名稱括在大括弧中。</p> </td> 
  </tr> 
  <tr> 
   <td>依句點分隔欄位</td> 
   <td> <p>在<code>valuefield</code>行中使用欄位時，請以冒號分隔欄位。</p> <p>在<code>valueexpression</code>行中使用欄位時，請依句號分隔欄位。</p> </td> 
  </tr> 
 </tbody> 
</table>

如需有關計算自訂欄中必須使用的語法的詳細資訊，請參閱[文字模式概觀](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md)。

## 計算自訂欄位的使用時機

* 當您想要將報表中的彙總結果分組，或想要在圖表中顯示此資訊時
* 當您想要彙總資料超過欄位中計算的彙總時
* 若您不擔心資料的時效性，因為資料不會更新，而且可能會隨著時間變更

## 觸發計算自訂欄位更新的動作

* 在物件的首頁面上按一下「更多」圖示![「更多」圖示](assets/more-icon.png)，然後按一下&#x200B;**「重新計算運算式」**

* 啟用&#x200B;**重新計算自訂運算式**&#x200B;時大量編輯多個物件
* 為已計算的自訂欄位啟用&#x200B;**更新先前的計算**&#x200B;時編輯自訂表單

## 何時在檢視中使用計算欄

* 當您希望報表上有即時資料可用時。

  計算的檢視永遠是新的，因為計算是在執行報表或套用檢視時進行。

* 當您沒有計畫要依彙總結果分組或在圖表中使用此資訊時。
* 當您不打算彙總資料超過欄中所計算之彙總範圍時（資料只能彙總一次）。
* 當您希望計算使用$$TODAY或$$NOW萬用字元包含目前日期的參考時。

  >[!TIP]
  >
  >請勿在計算自訂欄位中使用此參考，因為它們只會在編輯附加物件時重新計算。 這些型別的計算會過時。

## 計算自訂欄位和欄的範例

如需計算自訂欄位的範例，請參閱[報表中的計算自訂資料](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-custom-data-reports.md)。

如需檢視中計算的自訂欄的範例，請參閱下列文章：

* [文字模式的常見使用概述](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md)
* [自訂檢視、篩選和分組範例：文章索引](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md)
