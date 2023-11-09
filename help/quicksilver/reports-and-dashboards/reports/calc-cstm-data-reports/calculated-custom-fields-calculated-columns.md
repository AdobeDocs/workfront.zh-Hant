---
content-type: overview
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: 計算自訂欄位與計算欄的比較
description: 瞭解報告和儀表板中的自訂資料
author: Nolan
feature: Reports and Dashboards
exl-id: 17ac554d-0c90-4592-946e-a89f1784571d
source-git-commit: bcafa607da733b89747f6b448dd295d9b906d060
workflow-type: tm+mt
source-wordcount: '800'
ht-degree: 0%

---

# 計算自訂欄位與計算欄的比較

若要在Adobe Workfront中彙總數個欄位，並在新欄位中顯示該彙總值，您可以執行以下操作：

* 自訂表單中的計算自訂欄位\
  如需將計算自訂欄位新增至自訂表單的詳細資訊，請參閱區段 [新增計算欄位至自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md#creating-calculated-custom-fields) 在文章中 [新增計算資料至自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

* 檢視中的計算欄\
  如需在檢視中使用計算的詳細資訊，請參閱區段 [在檢視中使用文字模式](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md#using-text-mode-in-views) 在文章中 [文字模式的常見用途概觀](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md).

雖然您使用文字模式來建立計算欄位和計算欄，但建立它們的語法不同。 請參閱上方列出的文章，以瞭解如何建立計算欄位和計算欄。 如需有關計算資料運算式（例如計算自訂欄位和欄）中所使用不同語法的資訊，請參閱區段 [計算自訂欄位與計算自訂欄的語法](#syntax-of-calculated-custom-fields-vs-calculated-custom-columns-syntax) 本文章內容。

您可以在計算欄位和計算欄中使用相同的計算。 不過，視您用於這些計算的目的而定，您可能會想要考慮建立一種而非另一種模型。

## 計算自訂欄位與計算自訂欄的語法

雖然您使用的函式相同，但在計算自訂欄位中建立運算式的語法可能與建立計算自訂欄的語法不同。

例如：

* 在自訂欄位中，在任務的自訂表單上，您可以使用以下專案產生附加自訂表單之任務的父專案名稱：

  ```
  {project}.{name}
  ```

* 在報表的自訂欄中，您會使用下列專案，在任務報表中新增「專案名稱」自訂欄：

  ```
  valuefield=project:name
  ```

  或

  ```
  valueexpression={project}.{name}
  ```

  >[!TIP]
  >
  >相同的語法適用於所有使用計算運算式的文字模式報表元素：檢視、篩選器、群組、提示。

兩種語法之間的差異為：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>計算的自訂欄位</td> 
   <td>已計算的自訂報表元素</td> 
  </tr> 
  <tr> 
   <td> <p>使用在Workfront介面中顯示的欄位名稱。</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>範例： </b></span></span>計算自訂欄位中使用的欄位名稱範例： <code>Planned Completion Date</code>.</p> </td> 
   <td> <p>使用物件或欄位出現在Workfront資料庫中的名稱。 如果物件和欄位是複合名稱，則以小寫或駝峰式大小寫拼寫。 </p> <p>如需所有Workfront物件和欄位在資料庫中顯示的詳細目錄，請參閱 <a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">API總管</a>. </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>範例： </b></span></span>用於計算自訂報表元素中的欄位名稱範例： <code>plannedCompletionDate</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>以括弧或大括弧括住欄位名稱</td> 
   <td> <p>在中使用欄位名稱時，請勿以方括弧或括弧括住欄位名稱 <code>valuefield </code>行。</p> <p>在欄位中使用欄位名稱時，請以大括弧括住欄位名稱 <code>valueexpression</code> 行。</p> </td> 
  </tr> 
  <tr> 
   <td>依句點分隔欄位</td> 
   <td> <p>在中使用欄位時，請以冒號分隔欄位 <code>valuefield </code>折線圖</p> <p>在中使用欄位時，請依句號區隔欄位 <code>valueexpression </code>行。 </p> </td> 
  </tr> 
 </tbody> 
</table>

如需有關計算自訂欄中必須使用的語法的詳細資訊，請參閱 [文字模式概觀](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

## 計算自訂欄位的使用時機

* 當您想要將報表中的彙總結果分組，或想要在圖表中顯示此資訊時
* 當您想要彙總資料超過欄位中計算的彙總時
* 若您不擔心資料的時效性，因為資料不會更新，而且可能會隨著時間變更

## 觸發計算自訂欄位更新的動作

* 在物件的首頁面上，按一下「更多」圖示 ![](assets/more-icon.png)，然後按一下 **重新計算運算式**

* 大量編輯多個物件，當 **重新計算自訂運算式** 已啟用
* 編輯自訂表單時機 **更新先前的計算** 已針對計算自訂欄位啟用

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

如需計算自訂欄位的範例，請參閱 [報表中計算的自訂資料](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-custom-data-reports.md).

如需檢視中計算自訂欄的範例，請參閱下列文章：

* [文字模式的常見用途概觀](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md)
* [自訂檢視、篩選和分組範例](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md)
