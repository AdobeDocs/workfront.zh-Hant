---
content-type: reference
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: 計算資料運算式
description: 您可以使用資料運算式來定義Adobe Workfront中的計算自訂資料欄位。 它們會連結陳述式中現有的Workfront欄位，以產生新欄位。
author: Nolan
feature: Reports and Dashboards
exl-id: cfb3ace9-76c3-4006-878f-e2ad25ffa03b
source-git-commit: 1e91514f86a307ffa71cde650b35a2e3b8f0fa88
workflow-type: tm+mt
source-wordcount: '2302'
ht-degree: 7%

---

# 計算資料運算式

您可以使用資料運算式來定義Adobe Workfront中的計算自訂資料欄位。 它們會連結陳述式中現有的Workfront欄位，以產生新欄位。

您可以在下列位置使用計算資料運算式：

* 自訂表單

   如需在Workfront中自訂表單上建立計算自訂資料欄位的詳細資訊，請參閱 [將計算資料新增至自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

* 使用文字模式時，報表或清單中的計算自訂欄

   如需在報表和檢視中使用文字模式的詳細資訊，請參閱 [文字模式概觀](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

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
   <td><strong>計算自訂欄位</strong></td> 
   <td><strong>計算自訂報表元素</strong></td> 
  </tr> 
   <td>以大括弧括住欄位名稱。</td> 
   <td>在 <code>valuefield </code>行。 <p>在 <code>valueexpression</code> 行。</p> </td> 
  </tr> 
  <tr> 
   <td>依句號分隔欄位。</td> 
   <td> <p>在 <code>valuefield </code>線</p> <p>在 <code>valueexpression </code>行。 </p> </td> 
  </tr> 
 </tbody> 
</table>

如需您必須在計算自訂欄中使用語法的詳細資訊，請參閱 [文字模式概觀](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

## 您可以使用的資料運算式

下列清單定義您在Workfront中建立3種不同類型計算自訂欄位之一時，可使用的可用運算式：

* [日期和時間計算的自訂欄位](#date-time-calculated-custom-fields)
* [數學計算的自訂欄位](#mathematical-calculated-custom-fields)
* [文字計算自訂欄位](#text-calculated-custom-fields)

### 日期和時間計算的自訂欄位 {#date-time-calculated-custom-fields}

>[!NOTE]
>
>如果您建立的日期和時間計算不含時間部分，或使用日期通配符$$TODAY或$$NOW，則系統會根據協調通用時間(UTC)區域使用日期，而不是根據您的本地時區。 這可能會造成非預期的日期結果。

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
   <td> <p>此運算式會新增日期的天數。 數字值可能包含部分天數（例如1.5會新增一個半天至日期）。</p> <p>表達式的格式如下：</p><pre>ADDDAYS(date, number)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>每週新增日</strong> </td> 
   <td> <p>此運算式會將工作日數新增至日期。 此運算式只會將整數值加到日期，並往下捨入。 </p> <p>表達式的格式如下：</p><pre>每週新增日（日期、數目）</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>ADDMONTHS</strong> </td> 
   <td> <p>此運算式會將月數新增至日期，格式如下：</p><pre>ADDMONTHS(date, number)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>ADDYEARS</strong> </td> 
   <td> <p>此運算式會將年數新增至日期，格式如下：</p><pre>ADDYEARS(date, number)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>CLEARTIME</strong> </td> 
   <td> <p>此運算式會清除日期的時間部分，格式如下。 在此示例中，日期是工作對象的輸入日期。</p><pre>CLEARTIME({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>日期</strong> </td> 
   <td> <p>此運算式會將字串轉換為日期，格式如下：</p><pre>DATE(string)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DATEDIFF</strong> </td> 
   <td> <p>此運算式會傳回兩個日期之間的天數，並考慮所選期間的開始和結束天數，以及這些日期的時間戳記。 例如，如果開始日期的開始時間是下午3點，則開始日不會計為一整天。</p> <p>表達式的格式如下：</p><pre>DATEDIFF(date1, date2)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYOFMONTH</strong> </td> 
   <td> <p>此運算式會以數字形式傳回日期的月份日期，介於1到31之間。</p> <p>表達式的格式如下。 在此示例中，日期是工作對象的輸入日期。</p><pre>DAYOFMONTH({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYOFWEEK</strong> </td> 
   <td> <p>此運算式會以數字形式傳回日期的星期幾，介於1（星期日）和7（星期六）之間。</p> <p>表達式的格式如下。 在此示例中，日期是工作對象的輸入日期。</p><pre>DAYOFWEEK({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYSINMONTH</strong> </td> 
   <td> <p>此運算式會以數字傳回日期月份中的總天數，格式如下。 在此示例中，日期是工作對象的輸入日期。</p><pre>DAYSINMONTH({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYSINSPLITWEEK</strong> </td> 
   <td> <p>此運算式會傳回日期與週末（或月末）之間的總工作日（以先發生者為準）。 在此示例中，日期是工作對象的輸入日期。</p> <p>表達式的格式如下：</p><pre>DAYSINSPLITWEEK({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYSINYEAR</strong> </td> 
   <td> <p>此運算式會以數字形式傳回日期年份中的總天數，格式如下。 在此示例中，日期是工作對象的輸入日期。</p><pre>DAYSINYEAR({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DMAX</strong> </td> 
   <td> <p>此運算式會傳回清單中的最新日期，格式如下：</p><pre>DMAX(date1, date2, ...)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DMIN</strong> </td> 
   <td> <p>此表達式返回清單中的最早日期，格式如下：</p><pre>DMIN(date1, date2, ...)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>HOUR</strong> </td> 
   <td> <p>此運算式會傳回日期的小時，做為介於0到23之間的數字。</p> <p>表達式的格式如下。 在此示例中，日期是工作對象的輸入日期。</p><pre>HOUR({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>MINUTE</strong> </td> 
   <td> <p>此運算式會以介於0和60之間的數字傳回日期的分鐘，格式如下。 在此示例中，日期是工作對象的輸入日期。</p><pre>MINUTE({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>月</strong> </td> 
   <td> <p>此運算式會以介於1和12之間的數字傳回日期的月份，格式如下。 在此示例中，日期是工作對象的輸入日期。</p><pre>MONTH({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>SECOND</strong> </td> 
   <td> <p>此運算式會以介於0和60之間的數字傳回日期的秒數，格式如下。 在此示例中，日期是工作對象的輸入日期。</p><pre>SECOND({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>WEEKDAYDIFF</strong> </td> 
   <td> <p>此運算式會傳回兩個日期之間的工作日數，並考慮所選時段的開始和結束日以及這些日的時間戳記。 例如，如果開始日期的開始時間是下午3點，則開始日不會計為一整天。</p> <p>表達式的格式如下：</p><pre>WEEKDAYDIFF(date2, date1)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>WORKMINUTESDIFF</strong> </td> 
   <td> <p>此運算式會根據預設排程，傳回日期之間的排程分鐘數。</p> <p>表達式的格式如下：</p><pre>WORKMINUTESDIFF(date1, date2)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>年</strong> </td> 
   <td> <p>此運算式會以4位數字傳回日期的年份，格式如下。 在此示例中，日期是工作對象的輸入日期。</p><pre>YEAR({entryDate})</pre> </td> 
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
   <td>此表達式返回數字的絕對值，格式如下。 此示例使用附加自定義表單的對象下的對象數。<pre>ABS({numberOfChildren})</pre></td> 
  </tr> 
  <tr> 
   <td><strong>AVERAGE</strong> </td> 
   <td>此運算式會傳回數字平均值，格式如下：<pre>AVERAGE(number1, number2, ...)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>CEIL</strong> </td> 
   <td>此運算式會將數字四捨五入到最接近的整數，格式如下。 此示例使用附加自定義表單的對象下的對象數。<pre>CEIL({numberOfChildren})</pre></td> 
  </tr> 
  <tr> 
   <td><strong>DIV</strong> </td> 
   <td>此運算式會依提供的順序分隔所有數字，格式如下：<pre>DIV(number1, number2, ...)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>FLOOR</strong> </td> 
   <td>此表達式將數字向下捨入到最接近的整數，格式如下。 此示例使用附加自定義表單的對象下的對象數。<pre>FLOOR({numberOfChildren})</pre></td> 
  </tr> 
  <tr> 
   <td><strong>LN</strong> </td> 
   <td>此表達式返回數字的自然對數值，格式如下：<pre>LN({numberOfChildren})</pre></td> 
  </tr> 
  <tr> 
   <td><strong>LOG</strong> </td> 
   <td>此表達式將數字2的對數值返回到底數1，格式如下：<pre>LOG(number1、number2)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>最大值</strong> </td> 
   <td>此表達式返回清單中最大的項，格式如下：<pre>MAX(item1, item2, ...)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>最小值</strong> </td> 
   <td>此表達式返回清單中最小的項，格式如下：<pre>MIN(item1, item2, ...)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>數量</strong> </td> 
   <td>此表達式將字串轉換為數字，格式如下：<pre>NUMBER(string)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>POWER</strong> </td> 
   <td>此表達式返回一個引發為冪的數字，格式如下：<pre>POWER(number, power)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>PROD</strong> </td> 
   <td>此表達式將所有數字相乘，格式如下：<pre>PROD(number1, number2, ....)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>ROUND</strong> </td> 
   <td>此表達式將數字四捨五入到指定的精確小數，格式如下：<p>ROUND（數字、精度）</p></td> 
  </tr> 
  <tr> 
   <td><strong>SORTASCNUM</strong> </td> 
   <td> <p> 此表達式按升序排列數字，格式如下：</p><pre>SORTASCNUM(number1, number2, ...)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>SORTDESCNUM</strong> </td> 
   <td>此運算式會以降序排序數字，格式如下：<pre>SORTDESCNUM(number1, number2, ...)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>SQRT</strong> </td> 
   <td> <p>此表達式返回數字的平方根，格式如下。 此示例使用附加自定義表單的對象下的對象數。</p><pre>SQRT({numberOfChildren})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>SUB</strong> </td> 
   <td>此運算式會依提供的順序減去所有數字，格式如下：<pre>SUB(number1, number2, ...)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>總和</strong> </td> 
   <td>此表達式將添加所有數字，格式如下：<pre>SUM(number1, number2, ...)</pre></td> 
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
   <td> <p>此表達式與其他表達式一起使用，以便根據索引號從清單中選擇值。 索引數是可傳回數值（通常在已知範圍內）的欄位或函式。</p> <p>表達式的格式如下：</p><pre>CASE(indexNumber, value1, value2, ...)</pre> <p>例如，下列運算式會在計算欄中傳回一週中某天的名稱，其中1=Sunday、2=Monday等：</p><pre>CASE(DAYOFWEEK({entryDate}),"Sunday","Monday","Tudeday","Wendday","週四","Friday","Saturday")</pre> <p>此運算式最適合傳回數字的其他運算式，例如DAYOFWEEK、DAYOFMONTH和MONTH。</p> </td> 
  </tr> 
  <tr> 
   <td><strong>CONCAT</strong> </td> 
   <td> <p>此運算式會串連字串，格式如下：</p><pre>CONCAT(string1,"separator", string2)</pre> <p>以下是您可以包含的分隔符號範例：</p> 
    <ul> 
     <li>空間："</li> 
     <li>短划線："-"</li> 
     <li>斜線："/"</li> 
     <li>逗號：","</li> 
     <li>一個詞："or"、"and"</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td><strong>包含</strong> </td> 
   <td>如果在withinText字串內找到findText字串，則此表達式返回true，格式如下：<pre>CONTAINS(findText, withinText)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>ENCODEURL</strong> </td> 
   <td>此運算式會逸出字串中的任何特殊字元，以便納入URL引數中。<p>表達式的格式如下：</p><pre>ENCODEURL(string)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>IF</strong> </td> 
   <td> <p>此表達式會評估您指定的條件，如果為true，則返回trueExpression的值；如果為false，則返回falseExpression的值。</p> <p>表達式的格式如下：</p><pre>IF(condition, trueExpression, falseExpression)</pre> <p>例如，您可以比較兩個不同的日期欄位，後接True/False結果作為資料字串：</p><pre>IF({projectedCompletionDate}&gt;{plannededCompletionDate},"Off Track","On Track")</pre> <p>在日常言論中，這句話的意思是：「如果我對象的預計完成日期是同一對象的計畫完成日期的「大於」，則在此欄位中顯示「偏離軌道」字詞；否則，顯示「在追蹤上」這幾個字。</p> <p>如果您不想為true或false運算式加上標籤，必須在陳述式中插入空白標籤，例如：</p><pre>IF({projectedCompletionDate}&gt;{plannededCompletionDate},"","On Track")</pre> <p>或</p><pre>IF({projectedCompletionDate}&gt;{plannededCompletionDate},"Off Track","")</pre> <p>如需有關建立「IF」陳述式的詳細資訊，請參閱 <a href="../../../reports-and-dashboards/reports/calc-cstm-data-reports/if-statements-overview.md" class="MCXref xref">"IF"陳述式概述</a>.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>IFIN</strong> </td> 
   <td> <p>此運算式可讓您在可能的值字串中尋找特定值。 如果您要尋找的值等於其中一個提供的值，則運算式會傳回trueExpression;否則，它會傳回falseExpression。</p> <p>表達式的格式如下：</p><pre>IFIN(value, value1, value2,..., trueExpression, falseExpression)</pre> <p>例如，您可以找到特定的專案擁有者，並在專案檢視中以指定的標籤標籤這些專案： <br><code>IFIN({owner}.{name},"Jennifer Campbell","Rick Kuvec","Marketing Team","Other Teams")</code></p> <p> 在日常言論中，這句話的意思是：「如果專案擁有者是Jennifer Campbell或Rick Kuvec，請使用『行銷團隊』標示此專案；否則，使用「其他團隊」標籤。」</p> <p> 如果您不想為true或false運算式加上標籤，必須在陳述式中插入空白標籤，例如： </p> <p><code>IFIN({owner}.{name},"Jennifer Campbell","Rick Kuvec","","Other Teams")</code></p> <p>或 </p> <p><code>IFIN({owner}.{name},"Jennifer Campbell","Rick Kuvec","Marketing Team",""</code> </p> </td> 
  </tr> 
  <tr> 
   <td><strong>在</strong> </td> 
   <td> <p>如果值等於所提供的值之一，則此運算式會傳回true;否則，運算式會傳回false。</p> <p>表達式的格式如下：</p><pre>IN(value, value1[, value2...])</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>ISBLANK</strong> </td> 
   <td> <p>如果值為null或empty，則此表達式返回true;否則，運算式會傳回false。</p> <p>表達式的格式如下：</p><pre>ISBLANK(value)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>LEFT</strong> </td> 
   <td> <p>此表達式從字串的左側返回指定數量的字元，格式如下：</p><pre>LEFT(string, length)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>LEN</strong> </td> 
   <td> <p>此運算式會傳回字串的長度，格式如下：</p><pre>LEN(string)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>LOWER</strong> </td> 
   <td>此運算式會以小寫傳回字串，格式如下：<pre>LOWER(string)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>REPLACE</strong> </td> 
   <td> <p>此運算式會以string1中的string3取代string2的所有例項。</p> <p>表達式的格式如下：</p><pre>REPLACE(string1, string2, string3)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>RIGHT</strong> </td> 
   <td> <p>此運算式會從字串的右側傳回指定的字元數，格式如下：</p><pre>RIGHT(string, length)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>SEARCH</strong> </td> 
   <td> <p>此表達式返回在Text內的字串中首次出現findText的索引（從給定的開始位置開始）；如果找不到文本，則返回–1。</p> <p>表達式的格式如下：</p><pre>SEARCH(findText, withinText, start)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>字串</strong> </td> 
   <td> <p>此表達式將數字轉換為字串，格式如下：</p><pre>STRING(number)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>SORTASCSTRING</strong> </td> 
   <td> <p>此表達式按升序對字串清單進行排序，格式如下：</p><pre>SORTASCSTRING(string1, string2, ...)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>SORTDESCSTRING</strong> </td> 
   <td> <p> 此表達式按降序對字串清單進行排序，格式如下：</p><pre>SORTDESCSTRING(string1, string2, ...)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>SUBSTR</strong> </td> 
   <td> <p>此表達式根據指定的起始和終止索引返回字串的字元，格式如下：</p><pre>SUBSTR（{string}，開始位置數，結束位置數）</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>TRIM</strong> </td> 
   <td> <p>此運算式會從字串的開頭和結尾移除空白字元，格式如下：</p><pre>TRIM(string)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>UPPER</strong> </td> 
   <td> <p>此運算式會傳回大寫字串，格式如下：</p><pre>UPPER(string)</pre> </td> 
  </tr> 
 </tbody> 
</table>
