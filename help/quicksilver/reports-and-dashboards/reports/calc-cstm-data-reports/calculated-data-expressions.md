---
content-type: reference
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: 計算資料運算式
description: 您可以在Adobe Workfront中使用資料運算式來定義計算後的自訂資料欄位。 它們可連線產生新欄位的陳述式中的現有Workfront欄位。
author: Nolan
feature: Reports and Dashboards
exl-id: cfb3ace9-76c3-4006-878f-e2ad25ffa03b
source-git-commit: 18f26f976a47af003817f2f82f8550bdfbc0ab90
workflow-type: tm+mt
source-wordcount: '2368'
ht-degree: 7%

---

# 計算資料運算式

您可以在Adobe Workfront中使用資料運算式來定義計算後的自訂資料欄位。 它們可連線產生新欄位的陳述式中的現有Workfront欄位。

您可以在下列位置使用計算資料運算式：

* 自訂表格

   如需在Workfront中的自訂表單中建立計算自訂資料欄位的詳細資訊，請參閱 [將計算資料新增至自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

* 使用文字模式時，報表或清單中的計算自訂欄

   如需有關在報表和檢視中使用文字模式的詳細資訊，請參閱 [文字模式概觀](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

## 計算自訂欄位與計算自訂欄位的語法

雖然您使用的函式相同，但在計算自訂欄位中建立運算式的語法可能與建立計算自訂欄的語法不同。

例如：

* 在自訂欄位中，在任務的自訂表單上，您可以使用以下專案產生附加自訂表單之任務的父專案名稱：

   ```
   {project}.{name}
   ```

* 在報表的自訂欄中，您會使用下列專案在任務報表中新增「專案名稱」自訂欄：

   ```
   valuefield=project:name
   ```

   或

   ```
   valueexpression={project}.{name}
   ```

   >[!TIP]
   >
   >相同的語法適用於使用計算運算式的所有文字模式報表元素：檢視、篩選器、群組、提示。

兩種語法之間的差異如下：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>計算的自訂欄位</strong></td> 
   <td><strong>計算出的自訂報表元素</strong></td> 
  </tr> 
   <td>將欄位名稱括在大括弧中。</td> 
   <td>在中使用欄位名稱時，請勿將其括在方括弧或括弧中 <code>valuefield </code>行。 <p>在中使用欄位名稱時，請以大括弧括住欄位名稱 <code>valueexpression</code> 行。</p> </td> 
  </tr> 
  <tr> 
   <td>依句點分隔欄位。</td> 
   <td> <p>在中使用欄位時，請以冒號分隔欄位 <code>valuefield </code>折線</p> <p>在中使用欄位時，請依句號來區隔欄位 <code>valueexpression </code>行。 </p> </td> 
  </tr> 
 </tbody> 
</table>

如需計算自訂欄中必須使用的語法的詳細資訊，請參閱 [文字模式概觀](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

## 您可以使用的資料運算式

下列清單定義當您在Workfront中建置3種不同型別的計算自訂欄位之一時，可以使用的運算式：

* [日期與時間計算自訂欄位](#date-time-calculated-custom-fields)
* [數學計算的自訂欄位](#mathematical-calculated-custom-fields)
* [文字計算自訂欄位](#text-calculated-custom-fields)

### 日期與時間計算自訂欄位 {#date-time-calculated-custom-fields}

>[!NOTE]
>
>如果您建立的日期和時間計算不包含時間部分，或使用日期萬用字元$$TODAY或$$NOW，則系統會根據世界協調時間(UTC)區域使用日期，而不是根據您的當地時區。 這可能會造成非預期的日期結果。

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
   <td> <p>此運算式會新增日期的天數。 數字值可包含部分天數（例如1.5會為日期新增一天半）。</p> <p>運算式的格式如下：</p><pre>ADDDAYS(date, number)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>每週新增日</strong> </td> 
   <td> <p>此運算式會將工作日數新增至日期。 此運算式只會將整數值加到日期，往下舍入。 </p> <p>運算式的格式如下：</p><pre>每週新增日（日期、數目）</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>ADDMONTHS</strong> </td> 
   <td> <p>此運算式會將月份數加到日期，格式如下：</p><pre>ADDMONTHS(date, number)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>ADDYEARS</strong> </td> 
   <td> <p>此運算式會將年數加到日期，格式如下：</p><pre>ADDYEARS(date, number)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>CLEARTIME</strong> </td> 
   <td> <p>此運算式會清除日期的時間部分，格式如下。 在此範例中，日期是工作物件的輸入日期。</p><pre>CLEARTIME({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>日期</strong> </td> 
   <td> <p>此運算式會將字串轉換為日期，格式如下：</p><pre>DATE(string)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DATEDIFF</strong> </td> 
   <td> <p>此運算式會傳回兩個日期之間的天數，並考量所選期間的開始和結束天數以及這些天的時間戳記。 例如，如果開始日期的開始時間是下午3點，則開始日期不會計算為全天。</p> <p>運算式的格式如下：</p><pre>DATEDIFF(date1, date2)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYOFMONTH</strong> </td> 
   <td> <p>此運算式會以數字傳回日期所在的月份，數字介於1到31之間。</p> <p>運算式的格式如下。 在此範例中，日期是工作物件的輸入日期。</p><pre>DAYOFMONTH({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYOFWEEK</strong> </td> 
   <td> <p>此運算式會以數字傳回日期的周中日，介於1 （星期日）和7 （星期六）之間。</p> <p>運算式的格式如下。 在此範例中，日期是工作物件的輸入日期。</p><pre>DAYOFWEEK({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYSINMONTH</strong> </td> 
   <td> <p>此運算式會以數字傳回日期所在月份的總天數，格式如下。 在此範例中，日期是工作物件的輸入日期。</p><pre>DAYSINMONTH({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYSINSPLITWEEK</strong> </td> 
   <td> <p>此運算式會傳回日期和一星期結束之間、或一個月結束之間（以先到者為準）的工作日總數。 在此範例中，日期是工作物件的輸入日期。</p> <p>運算式的格式如下：</p><pre>DAYSINSPLITWEEK({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYSINYEAR</strong> </td> 
   <td> <p>此運算式會以數字傳回日期所在年份的總天數，格式如下。 在此範例中，日期是工作物件的輸入日期。</p><pre>DAYSINYEAR({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DMAX</strong> </td> 
   <td> <p>此運算式會傳回清單中的最新日期，格式如下：</p><pre>DMAX(date1, date2, ...)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DMIN</strong> </td> 
   <td> <p>此運算式會傳回清單中最早的日期，格式如下：</p><pre>DMIN(date1, date2, ...)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>HOUR</strong> </td> 
   <td> <p>此運算式會以0到23之間的數字傳回日期的時數。</p> <p>運算式的格式如下。 在此範例中，日期是工作物件的輸入日期。</p><pre>HOUR({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>MINUTE</strong> </td> 
   <td> <p>此運算式會以0到60之間的數字傳回日期的分鐘數，格式如下。 在此範例中，日期是工作物件的輸入日期。</p><pre>MINUTE({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>月</strong> </td> 
   <td> <p>此運算式會以1到12之間的數字傳回日期的月份，格式如下。 在此範例中，日期是工作物件的輸入日期。</p><pre>MONTH({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>SECOND</strong> </td> 
   <td> <p>此運算式會以0到60之間的數字傳回日期的秒數，格式如下。 在此範例中，日期是工作物件的輸入日期。</p><pre>SECOND({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>WEEKDAYDIFF</strong> </td> 
   <td> <p>此運算式會傳回兩個日期之間的工作日數，並考量所選期間的開始和結束天數以及這些天的時間戳記。 例如，如果開始日期的開始時間是下午3點，則開始日期不會計算為全天。</p> <p>運算式的格式如下：</p><pre>WEEKDAYDIFF(date2, date1)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>WORKMINUTESDIFF</strong> </td> 
   <td> <p>此運算式會根據預設排程，傳回日期之間排程的分鐘數。</p> <p>運算式的格式如下：</p><pre>WORKMINUTESDIFF(date1, date2)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>年</strong> </td> 
   <td> <p>此運算式會以4位數的數字傳回日期年份，格式如下。 在此範例中，日期是工作物件的輸入日期。</p><pre>YEAR({entryDate})</pre> </td> 
  </tr> 
 </tbody> 
</table>

### 數學計算的自訂欄位 {#mathematical-calculated-custom-fields}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>運算式</th> 
   <th>說明</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><strong>ABS</strong> </td> 
   <td>此運算式會傳回數字的絕對值，格式如下。 此範例使用物件下附加自訂表單的物件數目。<pre>ABS({numberOfChildren})</pre></td> 
  </tr> 
  <tr> 
   <td><strong>AVERAGE</strong> </td> 
   <td>此運算式會傳回數字的平均值，格式如下：<pre>AVERAGE(number1, number2, ...)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>CEIL</strong> </td> 
   <td>此運算式會將數字四捨五入到最接近的整數，格式如下。 此範例使用物件下附加自訂表單的物件數目。<pre>CEIL({numberOfChildren})</pre></td> 
  </tr> 
  <tr> 
   <td><strong>DIV</strong> </td> 
   <td>此運算式會依照提供的順序除以所有數字，格式如下：<pre>DIV(number1, number2, ...)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>FLOOR</strong> </td> 
   <td>此運算式將數字向下舍入至最接近的整數，格式如下。 此範例使用物件下附加自訂表單的物件數目。<pre>FLOOR({numberOfChildren})</pre></td> 
  </tr> 
  <tr> 
   <td><strong>LN</strong> </td> 
   <td>此運算式會傳回數字的自然對數值，格式如下：<pre>LN({numberOfChildren})</pre></td> 
  </tr> 
  <tr> 
   <td><strong>LOG</strong> </td> 
   <td>此運算式會將number2的對數值傳回至基礎number1，格式如下：<pre>LOG(number1、number2)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>最大值</strong> </td> 
   <td>此運算式會傳回清單中最大的專案，其格式如下：<pre>MAX(item1, item2, ...)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>最小值</strong> </td> 
   <td>此運算式會傳回清單中最小的專案，格式如下：<pre>MIN(item1, item2, ...)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>數量</strong> </td> 
   <td>此運算式會將字串轉換為數字，格式如下：<pre>NUMBER(string)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>POWER</strong> </td> 
   <td>此運算式會傳回引力至次方的數字，格式如下：<pre>POWER(number, power)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>PROD</strong> </td> 
   <td>此運算式會乘以所有數字，格式如下：<pre>PROD(number1, number2, ....)</pre>
   <b>附註</b>

將包含時數的欄位相乘時，請確定您瞭解所選欄位中的時數是儲存在資料庫中的分鐘、小時還是秒。 如果時數儲存為分鐘或秒，但在Workfront介面中以時數顯示，使用此計算撰寫運算式時，您可能需要考慮從分鐘或秒到小時的轉換。
</td> 
  </tr> 
  <tr> 
   <td><strong>ROUND</strong> </td> 
   <td>此運算式會將數字四捨五入到指定的小數位數位數，格式如下：<p>ROUND(number， precision)</p></td> 
  </tr> 
  <tr> 
   <td><strong>SORTASCNUM</strong> </td> 
   <td> <p> 此運算式會依遞增順序排序數字，格式如下：</p><pre>SORTASCNUM(number1, number2, ...)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>SORTDESCNUM</strong> </td> 
   <td>此運算式會以遞減順序排序數字，格式如下：<pre>SORTDESCNUM(number1, number2, ...)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>SQRT</strong> </td> 
   <td> <p>此運算式會傳回數字的平方根，格式如下。 此範例使用物件下附加自訂表單的物件數目。</p><pre>SQRT({numberOfChildren})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>SUB</strong> </td> 
   <td>此運算式會依照提供的順序減去所有數字，格式如下：<pre>SUB(number1, number2, ...)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>總和</strong> </td> 
   <td>此運算式會加總所有數字，格式如下：<pre>SUM(number1, number2, ...)</pre></td> 
  </tr> 
 </tbody> 
</table>

### 文字計算自訂欄位 {#text-calculated-custom-fields}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>運算式</th> 
   <th>說明</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><strong>CASE</strong> </td> 
   <td> <p>此運算式與其他運算式搭配使用，可根據索引編號從清單中選擇值。 索引編號是傳回數值（通常在已知範圍內）的欄位或函式。</p> <p>運算式的格式如下：</p><pre>CASE(indexNumber， value1， value2， ...)</pre> <p>例如，下列運算式會在計算欄中傳回一週中某天的名稱，其中1=星期日、2=星期一，依此類推：</p><pre>CASE(DAYOFWEEK({entryDate})，"Sunday"，"Monday"，"Tuesday"，"Threday"，"Tethday"，"Friday"，"Saturday")</pre> <p>此運算式最適合用於傳回數字的其他運算式，例如DAYOFWEEK、DAYOFMONTH和MONTH。</p> </td> 
  </tr> 
  <tr> 
   <td><strong>CONCAT</strong> </td> 
   <td> <p>此運算式串連字串，格式如下：</p><pre>CONCAT(string1，"separator"， string2)</pre> <p>以下是您可以包含的分隔符號範例：</p> 
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
   <td>如果在withinText字串中找到findText字串，且格式如下，則此運算式會傳回true：<pre>CONTAINS(findText, withinText)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>ENCODEURL</strong> </td> 
   <td>此運算式會逸出字串中的任何特殊字元，以便包含在URL引數中。<p>運算式的格式如下：</p><pre>ENCODEURL(string)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>IF</strong> </td> 
   <td> <p>此運算式會評估您指定的條件，如果為true，則傳回trueExpression的值；如果為false，則傳回falseExpression的值。</p> <p>運算式的格式如下：</p><pre>IF(condition, trueExpression, falseExpression)</pre> <p>例如，您可以比較兩個不同的日期欄位，然後以True/False結果作為資料字串：</p><pre>IF({projectedCompletionDate}&gt;{plannedCompletionDate}，"Off Track"，"On Track")</pre> <p>在日常演講中，此陳述式表示：「如果物件的預計完成日期大於」相同物件的計畫完成日期，則在此欄位中顯示'Off Track'字樣；否則顯示'On Track'字樣。」</p> <p>如果您不想要標示true或false運算式，則必須在陳述式中插入空白標籤，例如：</p><pre>IF({projectedCompletionDate}&gt;{plannedCompletionDate}，"，"On Track")</pre> <p>或</p><pre>IF({projectedCompletionDate}&gt;{plannedCompletionDate}，"Off Track"，")</pre> <p>如需有關建立「IF」陳述式的詳細資訊，請參閱 <a href="../../../reports-and-dashboards/reports/calc-cstm-data-reports/if-statements-overview.md" class="MCXref xref">「IF」陳述式概觀</a>.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>IFIN</strong> </td> 
   <td> <p>此運算式可讓您在可能值的字串中尋找特定值。 如果您要尋找的值等於所提供的其中一個值，則運算式會傳回trueExpression；否則會傳回falseExpression。</p> <p>運算式的格式如下：</p><pre>IFIN(value， value1， value2，...， trueExpression， falseExpression)</pre> <p>例如，您可以尋找特定的專案所有者，並在專案檢視中以指定的標籤標籤標籤這些專案： <br><code>IFIN({owner}.{name},"Jennifer Campbell","Rick Kuvec","Marketing Team","Other Teams")</code></p> <p> 在日常演講中，此陳述表示：「如果專案所有者是Jennifer Campbell或Rick Kuvec，請用「行銷團隊」標籤此專案；否則請用「其他團隊」標籤。」</p> <p> 如果您不想要標示true或false運算式，則必須在陳述式中插入空白標籤，例如： </p> <p><code>IFIN({owner}.{name},"Jennifer Campbell","Rick Kuvec","","Other Teams")</code></p> <p>或 </p> <p><code>IFIN({owner}.{name},"Jennifer Campbell","Rick Kuvec","Marketing Team",""</code> </p> </td> 
  </tr> 
  <tr> 
   <td><strong>在</strong> </td> 
   <td> <p>如果值等於所提供的值之一，此運算式會傳回true；否則，運算式會傳回false。</p> <p>運算式的格式如下：</p><pre>IN(value, value1[, value2...])</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>ISBLANK</strong> </td> 
   <td> <p>如果值為null或空白，此運算式會傳回true，否則會傳回false。</p> <p>運算式的格式如下：</p><pre>ISBLANK(value)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>LEFT</strong> </td> 
   <td> <p>此運算式會從字串左側傳回指定數目的字元，格式如下：</p><pre>LEFT(string, length)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>LEN</strong> </td> 
   <td> <p>此運算式會傳回字串長度，格式如下：</p><pre>LEN(string)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>LOWER</strong> </td> 
   <td>此運算式會傳回小寫的字串，格式如下：<pre>LOWER(string)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>REPLACE</strong> </td> 
   <td> <p>此運算式會以string1中的string3取代所有出現的string2。</p> <p>運算式的格式如下：</p><pre>REPLACE(string1, string2, string3)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>RIGHT</strong> </td> 
   <td> <p>此運算式會從字串右側傳回指定數目的字元，格式如下：</p><pre>RIGHT(string, length)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>SEARCH</strong> </td> 
   <td> <p>此運算式會傳回withinText字串中findText第一次出現的索引，從指定的開始位置開始，或如果找不到文字，則傳回–1。</p> <p>運算式的格式如下：</p><pre>SEARCH(findText， withinText， start)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>字串</strong> </td> 
   <td> <p>此運算式將數字轉換為字串，格式如下：</p><pre>STRING(number)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>SORTASCSTRING</strong> </td> 
   <td> <p>此運算式會以遞增順序來排序字串清單，格式如下：</p><pre>SORTASCSTRING(string1, string2, ...)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>SORTDESCSTRING</strong> </td> 
   <td> <p> 此運算式會以遞減順序來排序字串清單，格式如下：</p><pre>SORTDESCSTRING(string1, string2, ...)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>SUBSTR</strong> </td> 
   <td> <p>此運算式會根據指定的開始和結束索引，傳回字串的字元，格式如下：</p><pre>SUBSTR（{string}，開始位置數目、結束位置數目）</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>TRIM</strong> </td> 
   <td> <p>此運算式會移除字串開頭和結尾的空格，格式如下：</p><pre>TRIM(string)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>UPPER</strong> </td> 
   <td> <p>此運算式會傳回大寫的字串，格式如下：</p><pre>UPPER(string)</pre> </td> 
  </tr> 
 </tbody> 
</table>
