---
content-type: overview
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: 計算自訂欄位與計算欄
description: 若要匯總Adobe Workfront中的數個欄位，並在新欄位中顯示該匯總值，您可以執行下列操作 — EDIT ME。
author: Nolan
feature: Reports and Dashboards
exl-id: 17ac554d-0c90-4592-946e-a89f1784571d
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '815'
ht-degree: 0%

---

# 計算自訂欄位與計算欄

若要匯總Adobe Workfront中的數個欄位，並在新欄位中顯示該匯總值，您可以執行下列操作：

* 自訂表單中的計算自訂欄位\
   如需將計算的自訂欄位新增至自訂表單的詳細資訊，請參閱區段 [新增計算欄位至自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md#creating-calculated-custom-fields) 在文章中 [將計算資料新增至自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

* 檢視中的計算欄\
   有關在視圖中使用計算的詳細資訊，請參閱 [在檢視中使用文字模式](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md#using-text-mode-in-views) 在文章中 [文字模式常見用途概觀](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md).

雖然您使用文字模式來建立計算欄位和計算欄，但建立計算欄位和計算欄的語法有所不同。 請參閱上述文章，了解如何建立計算欄位和計算欄。 如需計算資料運算式（例如計算自訂欄位和欄）中所使用不同語法的相關資訊，請參閱區段 [計算自訂欄位與計算自訂欄的語法](#syntax-of-calculated-custom-fields-vs-calculated-custom-columns-syntax) 這篇文章。

您可以在計算欄位和計算欄中使用相同的計算。 不過，根據您用於這些計算的目的，您可能會想要考慮建置兩者。

## 計算自訂欄位與計算自訂欄的語法

雖然您使用的函式相同，但在計算自訂欄位中建立運算式的語法可能與建立計算自訂欄時的語法不同。

例如：

* 在自定義欄位中，在任務的自定義表單上，您將使用以下內容生成附加自定義表單的任務的父項目名稱：

   ```
   {project}.{name}
   ```

* 在報表的自訂欄中，您可使用下列項目名稱自訂欄，在任務報表中新增專案名稱自訂欄：

   ```
   valuefield=project:name
   ```

   或

   ```
   valueexpression={project}.{name}
   ```

   >[!TIP]
   >
   >所有使用計算運算式的文字模式報表元素也使用相同語法：視圖、篩選器、分組、提示。

這兩種語法之間的差異為：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>計算自訂欄位</td> 
   <td>計算自訂報表元素</td> 
  </tr> 
  <tr> 
   <td> <p>使用欄位在Workfront介面中顯示的名稱。</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>範例： </b></span></span>計算自訂欄位中使用的欄位名稱範例： <code>Planned Completion Date</code>.</p> </td> 
   <td> <p>使用對象或欄位的名稱，如Workfront資料庫中所示。 對象和欄位的名稱是小寫或駝峰式大寫，如果它們是複合名稱。 </p> <p>有關資料庫中顯示的所有Workfront對象和欄位的清單，請參見 <a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">API Explorer</a>. </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>範例： </b></span></span>計算量度自訂報表元素中使用的欄位名稱範例： <code>plannedCompletionDate</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>以括弧或大括弧括住欄位名稱</td> 
   <td> <p>在 <code>valuefield </code>行。</p> <p>在 <code>valueexpression</code> 行。</p> </td> 
  </tr> 
  <tr> 
   <td>依句號分隔欄位</td> 
   <td> <p>在 <code>valuefield </code>線</p> <p>在 <code>valueexpression </code>行。 </p> </td> 
  </tr> 
 </tbody> 
</table>

如需您必須在計算自訂欄中使用語法的詳細資訊，請參閱 [文字模式概觀](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

## 計算自訂欄位的使用時機

* 要將匯總的結果分組到報表中，或要在圖表中顯示此資訊時
* 想要匯總欄位中計算之匯總以外的資料時
* 若您不擔心資料的時效性，因為資料不會更新，且可能會隨著時間而變更

## 觸發計算自訂欄位更新的動作

* 在物件的首頁上，按一下「更多」圖示 ![](assets/more-icon.png)，然後按一下 **重新計算表達式**

* 在 **重新計算自定義運算式** 已啟用
* 編輯自訂表單時 **更新先前的計算** 已為計算的自訂欄位啟用

## 檢視中的計算欄使用時機

* 想要在報表上提供即時資料時。

   計算的視圖始終為新視圖，因為計算是在運行報表或應用視圖時進行的。

* 如果您沒有按匯總結果分組的計畫，或在圖表中使用此資訊。
* 當您不打算將資料匯總到列中計算的匯總之外時（資料只能匯總一次）。
* 當您想要計算包含對使用$$TODAY或$$NOW通配符的當前日期的引用時。

   >[!TIP]
   >
   >請勿在計算的自訂欄位中使用此參考，因為這些參考只會在編輯附加的物件時重新計算。 這些類型的計算已過時。

## 計算自訂欄位和欄的範例

如需計算自訂欄位的範例，請參閱 [報表中的計算自訂資料](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-custom-data-reports.md).

如需檢視中計算自訂欄的範例，請參閱下列文章：

* [文字模式常見用途概觀](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md)
* [自訂檢視、篩選和分組範例](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md)
