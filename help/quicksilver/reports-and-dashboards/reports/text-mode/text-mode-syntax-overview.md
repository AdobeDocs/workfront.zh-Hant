---
product-area: reporting
navigation-topic: text-mode-reporting
title: 文字模式語法概觀
description: 您可以使用文字模式介面，在清單和報表中建立更複雜的檢視、篩選、分組和自訂提示。 使用文本模式時，您可以訪問標準模式介面中不可用的欄位及其屬性。
author: Nolan
feature: Reports and Dashboards
exl-id: f24430e1-c5f7-4925-93df-0e956a03c863
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '1498'
ht-degree: 0%

---

# 文字模式語法概觀

您可以使用文字模式介面，在清單和報表中建立更複雜的檢視、篩選、分組和自訂提示。 使用文本模式時，您可以訪問標準模式介面中不可用的欄位及其屬性。

如需開始前文字模式的相關資訊和考量事項，請參閱 [文字模式概觀](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

如需所有可報告欄位及其屬性的完整清單，請參閱 [API Explorer](../../../wf-api/general/api-explorer.md).

## 文字模式語法的考量事項

* 您必須先了解Adobe Workfront語法，才能開始以文字模式建立報表元素。 文字模式的Workfront語法是此應用程式專屬的，且具有您必須熟悉的獨特特性。
* 在您開始在報表中使用文字模式之前，強烈建議您在進階報表中使用類別，以更深入了解我們的文字模式語言。 有關報告的培訓資料，請參閱 [Workfront報表和控制面板學習路徑](https://one.workfront.com/s/learningpath2/workfront-reporting-20Y0z000000blhLEAQ).
* 您可以使用標準模式介面來自訂檢視、篩選和群組。 但是，您只能使用文字模式來建立自訂提示。

## 在文字模式中建立報表元素的通用准則

以下是以文字模式建立任何報表或清單元素時的常見准則：

* 在Workfront資料庫中參考物件或屬性時，請一律使用駝峰式大小寫。
* 請記得Workfront中物件的階層。 檢視、篩選和群組之間有下列差異：

   * 可以顯示一個對象，該對象是離報表或清單對象遠的三個對象。
   * 在分組、篩選或自定義提示中，不能引用距主對象超過2個對象的對象。

   **範例：** 您可以在任務視圖中顯示Portfolio所有者的名稱或GUID:

   ```
   valuefield=project:portfolio:ownerID
   ```

   您不能在任務視圖中對Portfolio所有者進行分組、篩選或提示：

   ```
   project:portfolio:ownerID=5808f4bc00790b270a9629dd128e63fa
   ```

   在這些範例中，Portfolio擁有者ID是離清單物件三個物件。

   如需Workfront中物件階層的相關資訊，請參閱：

   * [了解Adobe Workfront中的物件](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md)
   * [API Explorer](../../../wf-api/general/api-explorer.md)


* 盡可能使用萬用字元(*)，讓您的報表和清單更具動態性，並避免針對不同使用者和類似的時間軸重複這些報表和清單。

## 駝峰案例概述

在文字模式中參考Workfront欄位或其屬性時，Workfront會要求您以駝峰式大小寫輸入其名稱。 在這種情況下，單名欄位會拼成小寫。 複合欄位的拼寫方式如下：

```
camelCaseSyntax
```

>[!IMPORTANT]
>
>所有報表元素都會遵循此大小寫模式。

駝峰案例的特點是：

* 第一個字一律以小寫字母開頭。
* 以下字詞的開頭一律為大寫字母。
* 字之間沒有空格。

**範例：** 要參考項目的實際完成日期，建立文本模式報告元素時要使用的欄位名稱為

```
actualCompletionDate
```

。

## 各種報表元素的文字模式語法

使用文字模式建立報表元素集時，下列報表元素集的語法之間有下列相似之處：

* 檢視和群組的程式碼行和語法類似。

   有關在文本模式中建立視圖和分組時代碼的關鍵行資訊，請參閱：

   * [使用文本模式編輯視圖](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-view.md)
   * [編輯分組中的文本模式](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-grouping.md)

* 程式碼行和語法對於篩選器和自訂提示類似。

   如需詳細資訊，請參閱：

   * [使用文字模式編輯篩選器](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md)
   * [新增提示至報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)

### 檢視和群組的語法

您可能會注意到建立檢視和群組時的程式碼行類似。

如需建立檢視和群組的相關資訊，請參閱下列文章：

* [Adobe Workfront中的檢視概觀](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)
* [Adobe Workfront中的群組概觀](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)

視圖或分組最重要的代碼行是標識視圖列或分組中引用的對象的行。 根據此欄位是Workfront資料庫欄位的直接參考，還是多個欄位之間的計算，程式碼行的開頭可能為

```
valuefield
```

或

```
valueexpression
```

。

* [檢視和群組的值欄位語法概觀](#valuefield-syntax-overview-for-views-and-groupings)
* [檢視和群組的值運算式語法概觀](#valueexpression-syntax-overview-for-views-and-groupings)

>[!TIP]
>
>* 雖然下列範例中的程式碼行在檢視和分組之間類似，但請一律記住，分組的每一行程式碼都以分組編號開頭。
>
>  要按項目清單或報表中的項目名稱分組，請對第一層分組使用以下行：
>
>  
```>
>  group.0.valuefield=name
>  ```>
>* If you edit multiple columns in a view in the same column (as it is the case of shared columns), remember that every line of code for each column starts with the column number. 
>
>  
Use the following format to identify the first column of a view: 
>
>  
```>
>  column.0.valuefield=name
>  ```>
>  For information about sharing columns, see [View: merge information from multiple columns in one shared column](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-merge-columns.md). 
>



```
Valuefield
```

檢視和群組的語法概觀 {#valuefield-syntax-overview-for-views-and-groupings}

```
Valuefield=
```

是檢視和群組中的關鍵程式碼行，可識別您直接參考的物件。

直接參考欄位的語法對於群組和檢視是相同的。

使用

```
valuefield
```

行：

* 使用駝峰大小寫直接參考欄位。

   **範例：** 要在任務視圖中參考任務實際完成日期，請使用以下行：

   ```
   valuefield=actualCompletionDate
   ```

* 使用駝峰式大小寫和冒號來分隔相同物件的彼此相關欄位。

   **範例：** 要在任務視圖中參考項目計畫完成日期，請使用以下行：

   ```
   valuefield=project:plannedCompletionDate
   ```

   有關在Workfront資料庫中如何互相引用對象的資訊，請參見 [API Explorer](../../../wf-api/general/api-explorer.md).

* 參考自訂欄位時，請使用與介面中顯示完全相同的欄位名稱。

   **範例：** 要在任務視圖中參考標籤為「附加詳細資訊」的項目自定義欄位，請使用以下行：

   ```
   valuefield=project:Additional Details
   ```

 

```
Valueexpression
```

檢視和群組的語法概觀 {#valueexpression-syntax-overview-for-views-and-groupings}

您可以取代

```
valuefield=
```

使用

```
valueexpression=
```

在文本模式中建立視圖和分組時，需要參考2個或多個欄位之間的計算。

>[!TIP]
>
>雖然您可以建立可在報表中顯示的計算欄位，但計算檢視和群組更具動態性。 每次執行報表或顯示清單時，計算的檢視和群組都會以新資訊重新整理。
>
>如需在檢視中建立計算欄的相關資訊，請參閱 [計算自訂欄位與計算欄](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-custom-fields-calculated-columns.md).

建立計算分組類似於在檢視中建立計算列。

使用

```
valueexpression
```

行：

* 使用駝峰大小寫直接參照欄位，並以大括弧括住每個欄位。

   **範例：** 要在任務列中顯示「任務名稱」欄位，請使用

   ```
   valueexpression
   ```

   ，請使用下列行：

   ```
   valueexpression={name}
   ```

* 使用駝峰式大小寫和句號來分隔彼此相關的欄位。

   **範例：** 要在任務報表中顯示與任務名稱串連的項目名稱，請使用以下行：

   * 在檢視中：

      ```
      valueexpression=CONCAT({project}.{name},' - ',{name})
      ```

   * 在分組中：

      ```
      group.0.valueexpression=CONCAT({project}.{name},' - ',{name})
      ```
   有關在Workfront資料庫中如何互相引用對象的資訊，請參見 [API Explorer](../../../wf-api/general/api-explorer.md).

* 參考自訂欄位時，請使用下列規則：

   * 使用介面中顯示的欄位名稱。
   * 在欄位名稱前面加上&quot;DE:&quot;。
   * 以大括弧括住欄位。
   * 依句號分隔與物件相關的欄位。

   **範例：** 要在值表達式行的任務視圖中顯示「附加詳細資訊」項目自定義欄位，請使用以下行：

   ```
   valueexpression={project}.{DE:Additional Details}
   ```

* 您可以在

   ```
   valueexpression
   ```

   但不在

   ```
   valuefield
   ```

   行。

   如需萬用字元的相關資訊，請參閱 [萬用字元篩選變數](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

```
Valueformat
```

概述

檢視或分組中第二最重要的程式碼行是

```
valueformat=
```

行。 這會以什麼格式傳回您在

```
valuefield
```

或值運算式行。 雖然您可以在

```
valueformat
```

行，建議您在使用

```
valueexpression
```

:

```
valueformat=HTML
```

### 篩選器和自訂提示的語法

建立篩選器的語法與建立自訂提示的語法類似。

>[!TIP]
>
>您可以先為要包含在提示中的陳述式建立篩選器，以建立自訂提示。 以&quot;&amp;&quot;連結篩選器中的所有代碼行，且行之間不含任何空格，這將成為您的自訂提示。

有關建立篩選器和自定義提示的資訊，請參閱：

* [Adobe Workfront中的篩選器概觀](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
* [新增提示至報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)

如需在文字模式中建立篩選器的相關資訊，請參閱 [使用文字模式編輯篩選器](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md).

您可以使用下列元素，以文字模式建立篩選器和自訂提示：

* 引用filter語句對象的代碼行。 篩選器物件請使用駝峰式大小寫。
* 引用篩選物件的程式碼行，以及篩選物件值的修飾元。 對此行中的篩選器對象使用駝峰大小寫。

   >[!TIP]
   >
   >參考範圍時，需要2個修改量行。

* 連接多個篩選器語句的語句連接器：

   * 與

      這是篩選器陳述式之間的預設連接器。

   * 或

      >[!TIP]
      >
      >語句連接器區分大小寫，且一律為大寫。 可在文字模式中省略&quot;AND&quot;。

* 萬用字元可讓篩選器更動態，並針對目前時間或登入的使用者加以自訂。 如需萬用字元的相關資訊，請參閱 [萬用字元篩選變數](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).
