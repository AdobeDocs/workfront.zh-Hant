---
content-type: overview
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: IF陳述式概述
description: 您可以在一般程式設計語言中使用「IF」陳述式。 在Adobe Workfront中，「IF」陳述式可讓您比較、格式化資料欄位，以及將資料欄位串結在一起，以用於報表和自訂資料用途。 此外，以數學方式思考「IF」陳述式可讓您更了解概念，因為運算式的變數通常使用。
author: Nolan
feature: Reports and Dashboards
exl-id: 090a85fd-fdbe-4507-8bad-ce8c29bf8fc9
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '928'
ht-degree: 0%

---

# &quot;IF&quot;陳述式概述

您可以在一般程式設計語言中使用「IF」陳述式。 在Adobe Workfront中，「IF」陳述式可讓您比較、格式化資料欄位，以及將資料欄位串結在一起，以用於報表和自訂資料用途。 此外，以數學方式思考「IF」陳述式可讓您更了解概念，因為運算式的變數通常使用。

## Recommendations for 「IF」陳述式

在建立「IF」語句之前，請考慮以下事項：

* 對於本指南，我們建議您基本了解任何一般程式設計語言，但我們不需要它。
* 我們需要進階了解Workfront文字模式語法。 這有助於掌握Workfront API的術語，並了解這些特定格式的自訂資料語法。

   如需Workfront API的相關資訊，請參閱 [API基本介紹](../../../wf-api/general/api-basics.md).

   如需使用文字模式的相關資訊，請參閱 [文字模式概觀](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

* 您可以為下列Workfront元素建立「IF」陳述式：

   * 檢視
   * 群組
   * 計算自訂欄位

* 無法為篩選器建立「IF」陳述式。 這會在Workfront中導致「Whoops」錯誤。
* 支援團隊不協助建立自訂資料。 建立自訂欄位或欄後，您就可以聯絡支援團隊，而您看不到想要的結果。 如需建立運算式的協助，請連絡您的帳戶主管以查詢我們的諮詢選項。
* 建議您先在文字編輯器中撰寫這些運算式，例如「崇高」或「Visual Studio Code」，因為這可協助您比在Workfront中更清楚地查看資料。

## &quot;IF&quot;語句的元件

您可以使用下列格式在Workfront中建立「IF」陳述式：
<pre>IF（條件，True運算式，False運算式）</pre>「IF」語句的元件包括：

* **若**=這是「函式」的Workfront計算資料運算式。 與SUM和PROD表達式類似，它首先指示系統將函式理解為「IF」語句。 在此語句中，請始終為&quot;IF&quot;使用大寫字母。\
   如需所有計算資料運算式的清單，請參閱 [計算資料運算式](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

* **條件**=這是Workfront變數必須符合的條件，也是此方程式的基礎。 之後可在方程式中指定的所有項目，都取決於條件。 您可以使用許多參照、比較或數學表達式來啟動方程式。 條件的一些範例為：

   * 日期大於指定對象上的其他日期。
   * 狀態等於指定物件上的可用狀態之一。
   * 任務完成百分比小於或大於某個百分比。

* **條件運算子** =這是可協助您建立「IF」陳述式條件的運算子。 例如，「等於」或「大於」是條件運算子。 如需可在陳述式中使用的條件運算子清單，請參閱 [計算的自訂運算式中的條件運算子](../../../reports-and-dashboards/reports/calc-cstm-data-reports/condition-operators-calculated-custom-expressions.md).

* **True****Expression**=這是「True」變數，會告訴方程式，當符合條件的條件時，要顯示哪個指標（true指標）。

* **False運算式**=這是&quot;False&quot;變數，會告訴方程式在不符合條件條件時要顯示哪個指標（false指標）。

在以下示例中，原始語句格式用於為&quot;IF&quot;語句編寫簡單資料表達式。 運算式會比較Workfront中的兩個不同日期欄位，後接True/False結果為資料字串：

```
IF({projectedCompletionDate}>{plannedCompletionDate},"Off Track","On Track")
```

在日常言論中，這一聲明意味著：如果我對象的預計完成日期大於同一對象的計畫完成日期，則在此欄位中顯示&quot;Off Track&quot;。 否則顯示「在追蹤上」字詞。

## 使用&quot;IF&quot;陳述式在自訂表單或自訂欄中建立計算欄位

您可以在自訂表單或自訂欄中的計算欄位中建立「IF」陳述式。

您在計算自訂表單中使用的語法，與在計算自訂欄中使用的語法有所差異。 請參閱下列範例：

* [單個「IF」語句](#single-if-statements)
* [多個&quot;IF&quot;語句](#multiple-if-statements)

### 單個「IF」語句 {#single-if-statements}

以下是使用&quot;IF&quot;陳述式的計算自訂欄位及其對應欄的範例：

* 計算自訂欄位：

建立自訂欄位時，請對&quot;IF&quot;陳述式使用下列語法：

```
IF({Projected Completion Date}>{Planned Completion Date},"Off Track","On Track")
```

* 計算自訂欄：

建立自訂欄時，應對值運算式行中的&quot;IF&quot;陳述式使用下列語法：

```
valueexpression=IF({projectedCompletionDate}>{plannedCompletionDate},"Off Track","On Track")
```

### 多個&quot;IF&quot;語句 {#multiple-if-statements}

您可以使用下列陳述式集合多個&quot;IF&quot;陳述式，以建立更複雜且動態的運算式：

<pre>IF(Condition1,True Expression,IF(Condition2,True Expression,False Expression))</pre>請注意，第一個"IF"現在沒有錯誤陳述式。 相反，我們用第二個「IF」開頭來替換它。

以下是使用多個&quot;IF&quot;陳述式之計算自訂欄位及其對應自訂欄的範例：

* 計算自訂欄位：

   ```
   IF({projectedCompletionDate}>{plannedCompletionDate},"Off Track",IF({plannedCompletionDate}>{projectedCompletionDate},"Off Track","On Track"))
   ```

* 計算自訂欄：

```
valueexpression=IF({"projectedCompletionDate"}>{"plannedCompletionDate"},"Off Track",IF({plannedCompletionDate}>{projectedCompletionDate},"Off Track","On Track"))
```

在此範例中，將兩個不同的條件變數放在一起，就能達成相同的目標。\
您可以在自己的環境中重建這些範例，以進一步探索這些選項。

要了解這一點，最好的方法就是嘗試各種領域和場景。 此外，請熟悉API總管，如此可顯示可使用的欄位名稱。 如需API總管的相關資訊，請參閱 [API Explorer](../../../wf-api/general/api-explorer.md).

如需計算資料運算式的Workfront語法的詳細資訊，請參閱 [計算資料運算式](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).
