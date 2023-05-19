---
product-area: reporting
navigation-topic: text-mode-reporting
title: 文本模式語法概述
description: 可以使用文本模式介面在清單和報告中建立更複雜的視圖、篩選器、分組和自定義提示。 通過使用文本模式，可以訪問在標準模式介面中不可用的欄位及其屬性。
author: Nolan
feature: Reports and Dashboards
exl-id: f24430e1-c5f7-4925-93df-0e956a03c863
source-git-commit: 888c938e5d649557df69374a55d4e4ecc2da6f55
workflow-type: tm+mt
source-wordcount: '1478'
ht-degree: 0%

---

# 文本模式語法概述

可以使用文本模式介面在清單和報告中建立更複雜的視圖、篩選器、分組和自定義提示。 通過使用文本模式，可以訪問在標準模式介面中不可用的欄位及其屬性。

有關開始前文本模式的資訊和注意事項，請參見 [文本模式概述](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md)。

有關所有可報告欄位及其屬性的完整清單，請參閱 [API資源管理器](../../../wf-api/general/api-explorer.md)。

## 關於文本模式語法的注意事項

* 您必須先瞭解Adobe Workfront語法，然後才能開始在文本模式下生成報告元素。 文本模式的Workfront語法是此應用程式獨有的，它具有您必須熟悉的獨特特性。
* 在您開始在報告中使用文本模式之前，我們強烈建議您學習我們有關高級報告的課程，以便更深入地瞭解我們的文本模式語言。 <!--outdated link: For training materials on reporting see [Workfront Reports and Dashboards Learning Paths](https://one.workfront.com/s/learningpath2/workfront-reporting-20Y0z000000blhLEAQ).-->
* 可以使用標準模式介面定制視圖、過濾器和分組。 但是，您只能使用文本模式生成自定義提示。

## 在文本模式下生成報告元素的通用准則

在文本模式下構建任何報告或清單元素時，以下是常用准則：

* 在Workfront資料庫中引用對象或屬性時，始終使用駝峰大小寫。
* 記住Workfront的物體層次。 視圖、篩選器和分組之間存在以下差異：

   * 可以在視圖中顯示一個對象，該對象是三個與報表或清單對象不同的對象。
   * 在分組、篩選或自定義提示中，不能引用與主對象相距超過2個對象的對象。

   **示例：** 可以在任務視圖中顯示Portfolio所有者的名稱或GUID:

   ```
   valuefield=project:portfolio:ownerID
   ```

   不能在任務視圖中對Portfolio所有者進行分組、篩選或提示：

   ```
   project:portfolio:ownerID=5808f4bc00790b270a9629dd128e63fa
   ```

   在這些示例中，Portfolio所有者ID是遠離清單對象的三個對象。

   有關Workfront對象層次結構的資訊，請參閱：

   * [瞭解Adobe Workfront的對象](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md)
   * [API資源管理器](../../../wf-api/general/api-explorer.md)


* 盡可能使用通配符使報告和清單更加動態，並避免為不同用戶和類似時間表複製它們。

## 駱駝案例概述

在文本模式下引用Workfront欄位或其屬性時，Workfront要求您在駝峰大小寫中鍵入它們的名稱。 在這種情況下，單名字欄位的拼寫為小寫。 複合欄位按以下模式拼寫：

```
camelCaseSyntax
```

>[!IMPORTANT]
>
>所有報告元素都遵循此外殼模式。

駝峰的特點是：

* 第一個單詞總是以小寫字母開頭。
* 以下單詞始終以大寫字母開頭。
* 單詞之間沒有空格。

**示例：** 要引用項目的實際完成日期，在生成文本模式報告元素時要使用的欄位的名稱為

```
actualCompletionDate
```

。

## 各種報表元素的文本模式語法

使用文本模式建立報表元素集時，以下報表元素集的語法之間存在以下相似性：

* 對於視圖和分組，代碼行和語法行類似。

   有關在文本模式下構建視圖和分組時的關鍵代碼行的資訊，請參閱：

   * [使用文本模式編輯視圖](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-view.md)
   * [編輯分組中的文本模式](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-grouping.md)

* 對於篩選器和自定義提示，代碼行和語法行類似。

   有關詳細資訊，請參閱：

   * [使用文本模式編輯篩選器](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md)
   * [向報表添加提示](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)

### 視圖和分組的語法

您可能會注意到，在構建視圖和分組時，代碼行相似。

有關建立視圖和分組的資訊，請參閱以下文章：

* [Adobe Workfront視圖概述](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)
* [Adobe Workfront分組概覽](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)

視圖或分組最重要的代碼行是標識在視圖列或分組中引用的對象的行。 根據此欄位是對Workfront資料庫欄位的直接引用還是多個欄位之間的計算，代碼行可以從

```
valuefield
```

或

```
valueexpression
```

。

* [視圖和分組的值欄位語法概述](#valuefield-syntax-overview-for-views-and-groupings)
* [視圖和分組的值表達式語法概述](#valueexpression-syntax-overview-for-views-and-groupings)

>[!TIP]
>
>* 雖然下面示例中的代碼行在視圖和分組之間類似，但請始終記住，分組的每個代碼行都以分組編號開頭。
>
>  要在項目清單或報表中按項目名稱分組，請對第一層分組使用以下行：
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

視圖和組的語法概述 {#valuefield-syntax-overview-for-views-and-groupings}

```
Valuefield=
```

是視圖和分組中標識您直接引用的對象的關鍵代碼行。

直接引用欄位的語法對於分組和視圖是相同的。

使用Java引用Workfront對象時適用以下規則

```
valuefield
```

行：

* 使用駱駝案例直接引用欄位。

   **示例：** 要在任務視圖中參考任務實際完成日期，請使用以下行：

   ```
   valuefield=actualCompletionDate
   ```

* 使用駱駝大小寫和冒號來分隔同一對象中彼此相關的欄位。

   **示例：** 要在任務視圖中參考項目計畫完成日期，請使用以下行：

   ```
   valuefield=project:plannedCompletionDate
   ```

   有關對象在Workfront資料庫中如何相互引用的資訊，請參見 [API資源管理器](../../../wf-api/general/api-explorer.md)。

* 引用自定義欄位時，請完全按該欄位在介面中的顯示方式使用該欄位的名稱。

   **示例：** 要引用任務視圖中標籤為「附加詳細資訊」的項目自定義欄位，請使用以下行：

   ```
   valuefield=project:Additional Details
   ```

 

```
Valueexpression
```

視圖和組的語法概述 {#valueexpression-syntax-overview-for-views-and-groupings}

可以替換

```
valuefield=
```

代碼行

```
valueexpression=
```

在文本模式下構建視圖和分組時，要在2個或多個欄位之間引用計算。

>[!TIP]
>
>雖然可以構建可在報表中顯示的計算欄位，但計算視圖和分組更具動態性。 每次運行報表或顯示清單時，計算的視圖和分組都會使用新資訊刷新。
>
>有關在視圖中建立計算列的資訊，請參見 [計算的自定義欄位與計算的列](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-custom-fields-calculated-columns.md)。

構建計算分組類似於在視圖中構建計算列。

使用Java引用Workfront對象時適用以下規則

```
valueexpression
```

行：

* 使用駱駝大小寫直接引用欄位，並將每個欄位括在花括弧中。

   **示例：** 要在任務列中顯示「任務名稱」欄位，請使用

   ```
   valueexpression
   ```

   ，使用以下行：

   ```
   valueexpression={name}
   ```

* 使用駱駝大小寫和句點分隔彼此相關的欄位。

   **示例：** 要顯示與任務報表中任務名稱連接的項目名稱，請使用以下行：

   * 在視圖中：

      ```
      valueexpression=CONCAT({project}.{name},' - ',{name})
      ```

   * 在分組中：

      ```
      group.0.valueexpression=CONCAT({project}.{name},' - ',{name})
      ```
   有關對象在Workfront資料庫中如何相互引用的資訊，請參見 [API資源管理器](../../../wf-api/general/api-explorer.md)。

* 引用自定義欄位時，請使用以下規則：

   * 使用欄位的名稱，與在介面中顯示的欄位完全相同。
   * 在欄位名稱前加「DE：」。
   * 將欄位括在花括弧中。
   * 按句點分隔與對象相關的欄位。

   **示例：** 要在值表達式行的任務視圖中顯示「附加詳細資訊」項目自定義欄位，請使用以下行：

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

   。

   有關通配符的資訊，請參見 [通配符篩選器變數](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md)。

```
Valueformat
```

概述

視圖或分組中第二重要的代碼行是

```
valueformat=
```

。 這將告訴Workfront以何種格式返回您在

```
valuefield
```

或value表達式行。 雖然您可以使用各種格式

```
valueformat
```

行時，建議您在使用

```
valueexpression
```

:

```
valueformat=HTML
```

### 篩選器和自定義提示的語法

建立篩選器的語法與建立自定義提示的語法類似。

>[!TIP]
>
>您可以先為要包括在提示中的語句構建篩選器，從而建立自定義提示。 通過「&amp;」將篩選器中的所有代碼行連接，這些行之間沒有空格，並且該行將成為您的自定義提示。

有關生成篩選器和自定義提示的資訊，請參閱：

* [篩選器概述Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
* [向報表添加提示](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)

有關在文本模式下建立篩選器的資訊，請參見 [使用文本模式編輯篩選器](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md)。

可以使用以下元素在文本模式下生成篩選器和自定義提示：

* 引用filter語句對象的代碼行。 將駝峰案例用於篩選器對象。
* 引用篩選器對象的代碼行和篩選器對象值的修飾符。 對此行中的篩選器對象使用駝峰案例。

   >[!TIP]
   >
   >引用範圍時，這需要2個修改量行。

* 連接多個篩選器語句的語句連接器：

   * 且

      這是篩選器語句之間的預設連接器。

   * 或

      >[!TIP]
      >
      >語句連接器區分大小寫，並且始終為大寫。 「AND」可在文本模式下省略。

* 通配符，使篩選器更加動態，並為當前時間或登錄的用戶自定義它們。 有關通配符的資訊，請參見 [通配符篩選器變數](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md)。
