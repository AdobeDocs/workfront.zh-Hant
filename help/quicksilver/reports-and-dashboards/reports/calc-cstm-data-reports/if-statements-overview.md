---
content-type: overview
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: IF陳述式概述
description: 您可以在一般程式語言中使用「IF」陳述式。 在Adobe Workfront中，「IF」陳述式可讓您比較資料的欄位、將其格式化，以及將其字串在一起，以用於報表和自訂資料用途。 此外，以數學方式思考「IF」陳述式可導致更佳的概念性理解，因為通常會使用運算式的變數。
author: Jenny
feature: Reports and Dashboards
exl-id: 090a85fd-fdbe-4507-8bad-ce8c29bf8fc9
source-git-commit: a1ead6d0c1c85bfbe6d7302506743db8d8b3e205
workflow-type: tm+mt
source-wordcount: '925'
ht-degree: 0%

---

# 「IF」陳述式概述

<!-- Audited: 1/2024 -->

您可以在一般程式語言中使用「IF」陳述式。 在Adobe Workfront中，「IF」陳述式可讓您比較資料的欄位、將其格式化，以及將其字串在一起，以用於報表和自訂資料用途。 此外，以數學方式思考「IF」陳述式可導致更佳的概念性理解，因為通常會使用運算式的變數。

## 針對「IF」陳述式的建議

建立「IF」陳述式之前，請先考慮下列事項：

* 我們建議您先瞭解一般程式設計語言的基本知識，但在本指南中，我們並不需要此知識。
* 您需要進一步瞭解Workfront文字模式語法。 這有助於掌握Workfront API的術語，並有助於瞭解這些特定格式中的自訂資料語法。

  如需Workfront API的相關資訊，請參閱[API基本知識](../../../wf-api/general/api-basics.md)。

  如需有關使用文字模式的資訊，請參閱[文字模式概觀](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md)。

* 您可以為下列Workfront元素建立「IF」陳述式：

   * 檢視
   * 群組
   * 已計算的自訂欄位

* 您無法建立篩選器的「IF」陳述式。 這會導致Workfront發生「糟糕」錯誤。
* 支援團隊不協助建立自訂資料。 建立自訂欄位或欄位後，如果看不到想要的結果，可以聯絡支援團隊。 如需建立運算式的協助，請聯絡您的客戶經理，查詢我們的諮詢選項。
* 我們建議您先在文字編輯器中撰寫這些運算式，例如Sublime或Visual Studio Code，因為這樣可協助您更清楚檢視資料，而不是顯示在Workfront中。

## 「IF」陳述式的元件

您可以使用以下格式在Workfront中建置「IF」陳述式：
<pre>IF(Condition，True Expression，False Expression)</pre>「IF」陳述式的元件包括：

* **IF** =這是「函式」的Workfront計算資料運算式。 與SUM和PROD運算式類似，這首先會告訴系統要將函式理解為「IF」陳述式。 在此陳述式中，一律使用大寫字母表示「IF」。\
  如需所有計算資料運算式的清單，請參閱[計算資料運算式概觀](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md)。

* **條件** =這是Workfront變數必須符合的條件，也是這個方程式的基礎。 之後可在方程式中指定的所有內容都取決於條件。 您可以使用許多參照、比較或數學運算式來啟動方程式。 條件的一些範例包括：

   * 指定物件上的日期晚於另一個日期。
   * 狀態等於指定物件上可用的狀態之一。
   * 任務的完成百分比小於或大於特定百分比。

* **條件運運算元** =這是協助您建置「IF」陳述式條件的運運算元。 例如，「等於」或「大於」是條件運運算元。 如需可在陳述式中使用的條件運運算元清單，請參閱計算自訂運算式中的[條件運運算元](../../../reports-and-dashboards/reports/calc-cstm-data-reports/condition-operators-calculated-custom-expressions.md)。

* **True****Expression** =這是「True」變數，它告訴方程式當滿足條件的條件時，要顯示哪個指標（true指標）。

* **False運算式** =這是「False」變數，它告訴方程式當條件條件條件不符時要顯示哪個指標（false指標）。

在下列範例中，原始陳述式格式是用來為「IF」陳述式寫入簡單資料運算式。 運算式會比較Workfront中的兩個不同日期欄位，然後以True/False結果作為資料字串：

```
IF({projectedCompletionDate}>{plannedCompletionDate},"Off Track","On Track")
```

在日常演講中，此陳述表示：如果物件的預計完成日期大於相同物件的計畫完成日期，則在此欄位中顯示「偏離軌道」字樣。 如果沒有，則顯示「On Track」字樣。

## 使用「IF」陳述式在自訂表單或自訂欄中建置計算欄位

您可以在自訂表單的計算欄位或自訂欄中建立「IF」陳述式。

您在計算自訂表單中使用的語法與計算自訂欄中的語法不同。 請參閱下列範例：

* [單一「IF」陳述式](#single-if-statements)
* [多個「IF」陳述式](#multiple-if-statements)

### 單一「IF」陳述式 {#single-if-statements}

以下是使用「IF」陳述式計算自訂欄位及其對應欄的範例：

* 計算自訂欄位：

建立自訂欄位時，請針對「IF」陳述式使用以下語法：

```
IF({Projected Completion Date}>{Planned Completion Date},"Off Track","On Track")
```

* 計算自訂欄：

建立自訂欄時，您應該針對值運算式行中的「IF」陳述式使用以下語法：

```
valueexpression=IF({projectedCompletionDate}>{plannedCompletionDate},"Off Track","On Track")
```

### 多個「IF」陳述式 {#multiple-if-statements}

您可以將多個「IF」陳述式與下列陳述式放在一起，以建置更複雜且更動態的運算式：

<pre>IF(Condition1，True運算式，IF（Condition2，True運算式，False運算式）)</pre>請注意，第一個「IF」現在沒有錯誤陳述式。 我們改為以第二個「IF」開頭來取代。

以下是使用多個「IF」陳述式的計算自訂欄位及其對應自訂欄的範例：

* 計算自訂欄位：

  ```
  IF({projectedCompletionDate}>{plannedCompletionDate},"Off Track",IF({plannedCompletionDate}>{projectedCompletionDate},"Off Track","On Track"))
  ```

* 計算自訂欄：

```
valueexpression=IF({"projectedCompletionDate"}>{"plannedCompletionDate"},"Off Track",IF({plannedCompletionDate}>{projectedCompletionDate},"Off Track","On Track"))
```

在此範例中，將兩個不同的條件變數放在一起，可達成相同的目標。\
您可以在自己的環境中重建這些範例，以進一步探索這些選項。

要瞭解這一點，最好的方式是嘗試各種欄位和情境。 此外，熟悉API Explorer，這會顯示可以使用的欄位名稱。 如需API Explorer的相關資訊，請參閱[API Explorer](../../../wf-api/general/api-explorer.md)。

如需有關計算資料運算式的Workfront語法的詳細資訊，請參閱[計算資料運算式概觀](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md)。
