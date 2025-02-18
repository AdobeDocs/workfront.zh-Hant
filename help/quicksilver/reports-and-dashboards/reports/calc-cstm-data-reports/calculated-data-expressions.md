---
content-type: reference
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: 計算資料運算式的概觀
description: 您可以使用資料運算式，在Adobe Workfront中定義計算的自訂資料欄位。 計算運算式會連線產生新欄位的陳述式中的現有Workfront欄位。
author: Nolan
feature: Reports and Dashboards
exl-id: cfb3ace9-76c3-4006-878f-e2ad25ffa03b
source-git-commit: 6a46486b62974f1cc7033b4497d32ab787b05bf2
workflow-type: tm+mt
source-wordcount: '2433'
ht-degree: 2%

---

# 計算資料運算式的概觀

<!--Audited: 12/2023-->

您可以使用資料運算式，在Adobe Workfront中定義計算的自訂欄位。 計算運算式會連線產生新欄位的陳述式中的現有Workfront欄位。

您可以在下列位置使用計算資料運算式：

* 自訂表單上的計算自訂欄位

  如需在Workfront中的自訂表單上建立計算自訂欄位的詳細資訊，請參閱[將計算欄位新增至表單](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md)。

* 使用文字模式時，報表或清單中的計算自訂欄

  如需有關在報表和檢視中使用文字模式的詳細資訊，請參閱[文字模式概觀](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md)。

## 計算自訂欄位與計算自訂欄的語法

雖然您使用的函式相同，但在計算自訂欄位中建立運算式的語法可能與建立計算自訂欄的語法不同。

兩種語法之間的差異為：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>計算的自訂欄位</strong></td> 
   <td><strong>已計算的自訂報表元素</strong></td> 
  </tr> 
   <td>以大括弧括住欄位名稱</td> 
   <td>在中使用欄位名稱時，請勿以方括弧或括弧括住欄位名稱 <p><code>valuefield </code></p>行。 <p>在欄位中使用欄位名稱時，請以大括弧括住欄位名稱 <p><code>valueexpression</code></p> 行。</p> </td> 
  </tr> 
  <tr> 
   <td>依句點分隔欄位</td> 
   <td> <p>在中使用欄位時，請以冒號分隔欄位 <p><code>valuefield </code></p>折線圖</p> <p>在中使用欄位時，請依句號區隔欄位 <p><code>valueexpression </code></p>行。 </p> </td> 
  </tr> 
 </tbody> 
</table>

例如：

* 在自訂欄位中，在任務的自訂表單上，您可以使用以下專案產生附加自訂表單之任務的父專案名稱：


  ` {project}.{name}`


* 在報表的自訂欄中，您會使用下列專案，在任務報表中新增「專案名稱」自訂欄：


  `valuefield=project:name`


  或

  `valueexpression={project}.{name}`


  >[!TIP]
  >
  >相同的語法適用於所有使用計算運算式的文字模式報表元素：檢視、篩選器、群組、提示。

如需有關計算自訂欄中必須使用的語法的詳細資訊，請參閱[文字模式概觀](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md)。

## 您可以使用的資料運算式

下列清單定義當您在Workfront中建置3種不同型別的計算自訂欄位之一時，可用的運算式：

* [日期與時間計算的自訂欄位](#date-time-calculated-custom-fields)
* [數學計算的自訂欄位](#mathematical-calculated-custom-fields)
* [文字計算自訂欄位](#text-calculated-custom-fields)

您可以使用下面列出的運算式來建置計算出的自訂欄。 不過，您必須使用計算自訂欄的正確語法，如本文中[計算自訂欄位與計算自訂欄位語法](#syntax-of-calculated-custom-fields-vs-calculated-custom-columns)一節所述。

### 日期和時間計算自訂欄位 {#date-time-calculated-custom-fields}

>[!NOTE]
>
>如果您建立的日期和時間計算不包含時間部分，或使用日期萬用字元$$TODAY或$$NOW，則系統會根據世界協調時間(UTC)區域使用日期，而不是根據您的當地時區。 這可能會造成非預期的日期結果。

您可以使用以下運算式建立日期或時間計算自訂欄位：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>運算式</th> 
   <th>說明和範例</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><strong>ADDDAYS</strong> </td> 
   <td> <p>新增日期的天數。 數值可包含部分天數。 例如，1.5會新增一個半天至日期。</p> <p>運算式的格式如下：</p>

<p><code>ADDDAYS(date, number)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>ADDWEEKDAYS</strong> </td> 
   <td> <p>將工作日數新增至日期。 此運算式只會將整數值加到日期，往下舍入。 </p> <p>運算式的格式如下：</p>

<p><code>ADDWEEKDAYS(date, number)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>ADDMONTHS</strong> </td> 
   <td> <p>將月數新增至日期，格式如下：

</p><p><code>ADDMONTHS(date, number)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>年</strong> </td> 
   <td> <p>將年份新增至日期，格式如下：</p>

<p><code>ADDYEARS(date, number)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>ADDHOURS</strong> </td> 
   <td> <p>將時數新增至日期，格式如下：</p>

<p><code>ADDHOUR(date, number)</code></p>
   <p>注意：Workfront Planning不支援此運算式。</p></td> 
  </tr>
  <tr> 
   <td><strong>CLEARTIME</strong> </td> 
   <td> <p>清除日期的時間部分，格式如下。 在此範例中，日期是工作物件的「輸入日期」。</p>

<p><code>CLEARTIME({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>日期</strong> </td> 
   <td> <p>將字串轉換為日期，格式如下：</p>

<p><code>DATE(string)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DATEDIFF</strong> </td> 
   <td> <p>傳回兩個日期之間的天數，考量所選期間的開始和結束天數以及這些天的時間戳記。 例如，如果開始日期的開始時間是下午3點，則開始日期不會計算為全天。</p> <p>運算式的格式如下：</p>

<p><code>DATEDIFF(date1, date2)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYOFMONTH</strong> </td> 
   <td> <p>以數字傳回日期的月份，數字介於1到31之間。</p> <p>運算式的格式如下。 在此範例中，日期是工作物件的「輸入日期」。</p>

<p><code>DAYOFMONTH({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYOFWEEK</strong> </td> 
   <td> <p>以數字傳回日期是一週中的第幾天，數字介於1 （星期日）和7 （星期六）之間。</p> <p>運算式的格式如下。 在此範例中，日期是工作物件的「輸入日期」。</p>

<p><code>DAYOFWEEK({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYSINMONTH</strong> </td> 
   <td> <p>以數字傳回日期所在月份的總天數，格式如下。 在此範例中，日期是工作物件的「輸入日期」。</p>

<p><code>DAYSINMONTH({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYSINSPLITWEEK</strong> </td> 
   <td> <p>傳回該日期和一星期結束之間、或一個月結束之間（視其中哪個日期先到）的工作日總數。 在此範例中，日期是工作物件的「輸入日期」。</p> <p>運算式的格式如下：</p>

<p><code>DAYSINSPLITWEEK({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYSINYEAR</strong> </td> 
   <td> <p>以數字傳回日期所在年份的總天數，格式如下。 在此範例中，日期是工作物件的「輸入日期」。</p>

<p><code>DAYSINYEAR({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DMAX</strong> </td> 
   <td> <p>傳回清單中的最新日期，格式如下：</p>

<p><code>DMAX(date1, date2, ...)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>分鐘</strong> </td> 
   <td> <p>傳回清單中最早的日期，格式如下：</p>

<p><code>DMIN(date1, date2, ...)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>小時</strong> </td> 
   <td> <p>以0到23之間的數字傳回日期的小時數。</p> <p>運算式的格式如下。 在此範例中，日期是工作物件的「輸入日期」。</p>

<p><code>HOUR({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>分鐘</strong> </td> 
   <td> <p>以0到60之間的數字傳回日期的分鐘數，格式如下。 在此範例中，日期是工作物件的「輸入日期」。</p>

<p><code>MINUTE({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>個月</strong> </td> 
   <td> <p>以1到12之間的數字傳回日期的月份，格式如下。 在此範例中，日期是工作物件的「輸入日期」。</p>

<p><code>MONTH({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>秒</strong> </td> 
   <td> <p>以0到60之間的數字傳回日期的秒數，格式如下。 在此範例中，日期是工作物件的「輸入日期」。</p>

<p><code>SECOND({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>WEEKDAYDIFF</strong> </td> 
   <td> <p>傳回兩個日期之間的工作日數，考量所選期間的開始和結束天數以及這些天的時間戳記。 例如，如果開始日期的開始時間是下午3點，則開始日期不會計算為全天。</p> <p>運算式的格式如下：</p>

<p><code>WEEKDAYDIFF(date2, date1)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>WORKMINUTESDIFF</strong> </td> 
   <td> <p>根據預設排程，傳回日期之間排程的分鐘數。</p> <p>運算式的格式如下：</p>

<p><code>WORKMINUTESDIFF(date1, date2)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>年</strong> </td> 
   <td> <p>以4位數字傳回日期的年份，格式如下。 在此範例中，日期是工作物件的「輸入日期」。</p>

<p><code>YEAR({entryDate})</code></p> </td> 
  </tr> 
 </tbody> 
</table>

### 數學計算的自訂欄位 {#mathematical-calculated-custom-fields}

您可以建立使用下列部分數學運算式的計算自訂欄位：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>運算式</th> 
   <th>解釋</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><strong>ABS</strong> </td> 
   <td>傳回數字的絕對值，格式如下。 此範例使用物件下附加自訂表單的物件數目。

<p><code>ABS({numberOfChildren})</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>平均</strong> </td> 
   <td>傳回數字的平均值，格式如下：

<p><code>AVERAGE(number1, number2, ...)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>CEIL</strong> </td> 
   <td>將數字四捨五入到最接近的整數，格式如下。 此範例使用物件下附加自訂表單的物件數目。

<p><code>CEIL({numberOfChildren})</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>DIV</strong> </td> 
   <td>按照提供的順序除以所有數字，格式如下：

<p><code>DIV(number1, number2, ...)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>樓層</strong> </td> 
   <td>將數字下調至最接近的整數，格式如下。 此範例使用物件下附加自訂表單的物件數目。

<p><code>FLOOR({numberOfChildren})</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>LN</strong> </td> 
   <td>傳回該數字的自然對數值，格式如下：

<p><code>LN({numberOfChildren})</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>記錄檔</strong> </td> 
   <td>傳回number2對數值至基礎number1，格式如下：

<p><code>LOG(number1, number2)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>MAX</strong> </td> 
   <td>傳回清單中最大的專案，格式如下：

<p><code>MAX(item1, item2, ...)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>分鐘</strong> </td> 
   <td>傳回清單中的最小專案，格式如下：

<p><code>MIN(item1, item2, ...)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>數字</strong> </td> 
   <td>將字串轉換為數字，格式如下：<p><code>NUMBER(string)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>電源</strong> </td> 
   <td>傳回提升為次方的數字，格式如下：

<p><code>POWER(number, power)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>PROD</strong> </td> 
   <td>將所有數字相乘，格式如下：

<p><code>PROD(number1, number2, ....)</code></p>
   <p><b>附註</b></p>

<p>將包含時數的欄位相乘時，請確定您瞭解資料庫是否要將所選欄位中的時數儲存為分鐘、小時或秒。 如果時數儲存為分鐘或秒，但在Workfront介面中以時數顯示，使用此計算撰寫運算式時，您可能需要考慮從分鐘或秒到時數的轉換。 </p>
   </td> 
  </tr> 
  <tr> 
   <td><strong>回合</strong> </td> 
   <td>將數字四捨五入到指定的精確位數，格式如下：

<p><code>ROUND(number, precision)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>SORTASCNUM</strong> </td> 
   <td> <p> 以遞增順序排序數字，格式如下：</p>

<p><code>SORTASCNUM(number1,number2, ...)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>SORTDESCNUM</strong> </td> 
   <td>以遞減順序排序數字，格式如下：

<p><code>SORTDESCNUM(number1, number2, ...)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>SQRT</strong> </td> 
   <td> <p>傳回數字的平方根，格式如下。 此範例使用物件下附加自訂表單的物件數目。</p>

<p><code>SQRT({numberOfChildren})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>SUB</strong> </td> 
   <td>依照提供的順序減去所有數字，格式如下：

<p><code>SUB(number1, number2, ...)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>總和</strong> </td> 
   <td>將所有數字相加，格式如下：

<p><code>SUM(number1, number2, ...)</code></p></td> 
  </tr> 
 </tbody> 
</table>

### 文字計算自訂欄位 {#text-calculated-custom-fields}

您可以使用下列運算式建立計算自訂欄位，以顯示文字格式的值：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>運算式</th> 
   <th>解釋</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><strong>陣列</strong> </td> 
   <td> <p>將字串轉換為陣列。delimiter 可以是任何字串。</p> 
   <p>運算式的格式如下：</p>
   <p><code>ARRAY(string1, "delimiter")</code></p> 
   </td> 
  </tr>
  <tr> 
   <td><strong>ARRAYLENGTH</strong> </td> 
   <td> <p>傳回陣列中的元素數，格式如下：</p>
   <p><code>ARRAYLENGTH(array)</code></p> 
   </td> 
  </tr>
  <tr> 
   <td><strong>ARRAYELEMENT</strong> </td> 
   <td> <p>傳回陣列中位於指定編號的元素。如果索引超出範圍，則傳回空白。</p> 
   <p>運算式的格式如下：</p>
   <p><code>ARRAYELEMENT(array, number)</code></p> 
   </td> 
  </tr>
  <tr> 
   <td><strong>SORTASCARRAY</strong> </td> 
   <td> <p>以遞增順序排序陣列元素，並將其轉換為第一個元素的型別。</p>
   <p>運算式的格式如下：</p>
   <p><code>SORTASCARRAY(array)</code></p>
   <p>例如，["-12.6"， -13.0]會變成["-12.6"， "-13"]。</p>
   <p>注意：Workfront Planning不支援此運算式。</p></td> 
  </tr>
  <tr> 
   <td><strong>SORTDESCARRAY</strong> </td> 
   <td> <p>以遞減順序排序陣列元素，並將其轉換為第一個元素的型別。</p>
   <p>運算式的格式如下：</p>
   <p><code>SORTDESCARRAY(array)</code></p>
   <p>例如，["-12.6"， -13.0]會變成["-13"， "-12.6"]。</p>
   <p>注意：Workfront Planning不支援此運算式。</p></td> 
  </tr>
  <tr>   
   <td><strong>個案例</strong> </td> 
   <td> <p>與其他運算式搭配使用，根據索引編號從清單中選擇值。 </p>
   <p>索引數字是傳回數值（通常在已知範圍內）的欄位或函式。</p> 
   <p>運算式的格式如下：</p>
   <p><code>CASE(indexNumber, value1, value2, ...)</code></p>

<p>例如，下列運算式會在計算欄中傳回一週中某天的名稱，其中1=星期日、2=星期一，以此類推：</p>

<p><code>CASE(DAYOFWEEK({entryDate}),"Sunday","Monday","Tuesday","Wednesday","Thursday","Friday","Saturday")</code></p>

<p>最適合搭配其他傳回數字的運算式，例如DAYOFWEEK、DAYOFMONTH和MONTH。</p> </td> 
  </tr> 
  <tr> 
   <td><strong>CONCAT</strong> </td> 
   <td> <p>串連字串，格式如下：</p><p><code>CONCAT(string1,"separator", string2)</code></p> <p>以下是您可以包括的分隔符號範例：</p> 
    <ul> 
     <li>空格：「 」</li> 
     <li>破折號：「 — 」</li> 
     <li>斜線： "/"</li> 
     <li>逗號： "，"</li> 
     <li>單字：「or」、「and」</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td><strong>包含</strong> </td> 
   <td>如果在withinText字串中找到findText字串且其格式如下，則傳回true：

<p><code>CONTAINS(findText, withinText)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>ENCODEURL</strong> </td> 
   <td>逸出字串中的任何特殊字元，以便包含在URL引數中。<p>運算式的格式如下：</p>

<p><code>ENCODEURL(string)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>格式</strong> </td> 
   <td><p>傳回格式化文字。 FORMAT只允許此處列出的引數選項。</p>
   <p>顏色選項有$$正面、$$資訊、$$負面、$$注意，其他格式選項有$$粗體、$$斜體、$$底線。 只允許一個顏色選項，以及最多三個其他格式選項。 如果未指定顏色選項，則會套用系統的預設顏色。</p>
   <p>運算式的格式如下：</p>
   <p><code>FORMAT($$POSITIVE, $$BOLD, $$ITALIC)</code></p>
   <p>注意：Workfront Planning不支援此運算式。</p></td> 
  </tr>   
  <tr> 
   <td><strong>IF</strong> </td> 
   <td> <p>評估您指定的條件，如果為true，則傳回trueExpression的值；如果為false，則傳回falseExpression的值。</p>

<p>運算式的格式如下：</p>

<p><code>IF(condition, trueExpression, falseExpression)</code></p>

<p>例如，您可以比較兩個不同的日期欄位，然後以True/False結果作為資料字串：</p>

<p><code>IF({projectedCompletionDate}&gt;{plannedCompletionDate},"Off Track","On Track")</code></p>

<p>在日常演講中，此陳述表示：「如果物件的預計完成日期大於'相同物件的計畫完成日期，則在此欄位中顯示'Off Track'字詞；否則，顯示'On Track'字詞。」</p>

<p>如果您不想要標示true或false運算式，則必須在陳述式中插入空白標籤，例如：</p>

<p><code>IF({projectedCompletionDate}&gt;{plannedCompletionDate},"","On Track")</code></p> 
   <p>或</p>

<p><code>IF({projectedCompletionDate}&gt;{plannedCompletionDate},"Off Track","")</code></p>

<p>如需有關建立「IF」陳述式的詳細資訊，請參閱<a href="../../../reports-and-dashboards/reports/calc-cstm-data-reports/if-statements-overview.md" class="MCXref xref">「IF」陳述式概述</a>。</p> </td> 
  </tr> 
  <tr> 
   <td><strong>IFIN</strong> </td> 
   <td> <p>可讓您在可能值的字串中尋找特定值。 如果您要尋找的值等於其中一個提供的值，則運算式會傳回trueExpression；否則，會傳回falseExpression。</p> 
   <p>運算式的格式如下：</p>

<p><code>IFIN(value, value1, value2,..., trueExpression, falseExpression)</code></p>

<p>例如，您可以尋找特定的專案所有者，並在專案檢視中以指定的標籤標籤標籤這些專案： <br><p><code>IFIN({owner}.{name},"Jennifer Campbell","Rick Kuvec","Marketing Team","Other Teams")
   </code></p>
    <p> 在日常演講中，此陳述表示：「如果專案所有者是Jennifer Campbell或Rick Kuvec，請使用「行銷團隊」標籤此專案；否則，請使用「其他團隊」標籤此專案。」</p> 
    <p> 如果您不想要標示true或false運算式，則必須在陳述式中插入空白標籤，例如： </p> 
    <p><code>IFIN({owner}.{name},"Jennifer Campbell","Rick Kuvec","","Other Teams")</code></p> 
    <p>或 </p> 
    <p><code>IFIN({owner}.{name},"Jennifer Campbell","Rick Kuvec","Marketing Team","")</code></p> </p> </td> 
  </tr> 
  <tr> 
   <td><strong>IN</strong> </td> 
   <td> <p>如果值等於提供的值之一，則傳回true；否則，運算式會傳回false。</p> <p>運算式的格式如下：

</p><p><code>IN(value, value1[, value2...])</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>ISBLANK</strong> </td> 
   <td> <p>如果值為空值或空白，則傳回true；否則，運算式會傳回false。</p> <p>運算式的格式如下：

</p><p><code>ISBLANK(value)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>左</strong> </td> 
   <td> <p>傳回字串左側的指定字元數，格式如下：</p>

<p><code>LEFT(string, length)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>長度</strong> </td> 
   <td> <p>傳回字串長度，格式如下：</p>

<p><code>LEN(string)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>下層</strong> </td> 
   <td>傳回小寫的字串，格式如下：

<p><code>LOWER(string)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>取代</strong> </td> 
   <td> <p>在string1中，以string3取代所有出現的string2。</p> <p>運算式的格式如下：</p>

<p><code>REPLACE(string1, string2, string3)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>右</strong> </td> 
   <td> <p>從字串右側傳回指定的字元數，格式如下：</p>

<p><code>RIGHT(string, length)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>搜尋</strong> </td> 
   <td> <p>傳回withinText字串中第一個findText事件的索引（從給定的起始位置開始），或如果找不到文字，則傳回–1。</p> <p>運算式的格式如下：</p>

<p><code>SEARCH(findText, withinText, start)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>字串</strong> </td> 
   <td> <p>將數字轉換為字串，格式如下：</p>

<p><code>STRING(number)</code></p> </td> 
  </tr>
  <tr> 
   <td><strong>SORTASCSTRING</strong> </td> 
   <td> <p>以遞增順序來排列字串清單，格式如下：</p>
   <p><code>SORTASCSTRING(string1, string2, ...)</code></p> </td> 
  </tr>
  <tr> 
   <td><strong>SORTDESCSTRING</strong> </td> 
   <td> <p> 以遞減順序來排列字串清單，格式如下：</p>
   <p><code>SORTDESCSTRING(string1, string2, ...)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>SUBSTR</strong> </td> 
   <td> <p>根據指定的開始和結束索引，傳回字串的字元，格式如下：</p>

<p><code>SUBSTR({string}, number of start position, number of end position)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>開關</strong> </td> 
   <td> <p>根據值清單來評估運算式，並傳回與第一個相符值對應的結果。</p>
   <p>運算式的格式如下：</p>
   <p><code>SWITCH(expression, value1, result1, [value2, result2], ...)</code></p>
   <p>Workfront Planning不支援此運算式。</p></td> 
  </tr>   
  <tr> 
   <td><strong>TRIM</strong> </td> 
   <td> <p>移除字串開頭和結尾的空格，格式如下：</p>

<p><code>TRIM(string)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>UPPER</strong> </td> 
   <td> <p>傳回大寫的字串，格式如下：</p>

<p><code>UPPER(string)</code></p> </td> 
  </tr> 
 </tbody> 
</table>
