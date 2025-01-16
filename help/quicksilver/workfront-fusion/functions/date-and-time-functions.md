---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: Adobe Workfront Fusion中的日期和時間函式
description: Adobe Workfront Fusion檔案已移至新位置。 本文已棄用，但包含新文章的連結，內容涵蓋此功能。
author: Becky
feature: Workfront Fusion
exl-id: 76c63afc-4bb6-4895-9bba-6b3913ecbcf6
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '2018'
ht-degree: 1%

---

# [!DNL Adobe Workfront Fusion]中的日期和時間函式

>[!IMPORTANT]
>
>Adobe Workfront Fusion檔案已移至新位置。
>
>本文資訊可在以下文章中找到：
>
>* [日期與時間函式](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/mapping-panel/functions/date-and-time-functions.html)
>
>請更新任何書籤。
>
>本文已不再更新，將於不久將來移除。

## 存取需求



您必須具有下列存取權才能使用本文中的功能：



<table style="table-layout:auto"> 
 <col>  
 <col>  
 <tbody>  
  <tr>  
   <td role="rowheader">[!DNL Adobe Workfront] 計劃</td>  
   <td> <p>任何</p> </td>  
  </tr>  
  <tr data-mc-conditions="">  
   <td role="rowheader">[!DNL Adobe Workfront] 授權</td>  
   <td> <p>新增：[！UICONTROL Standard]</p><p>或</p><p>目前： [！UICONTROL Work]或更高版本</p> </td>  
  </tr>  
  <tr>  
   <td role="rowheader">[!DNL Adobe Workfront Fusion] 授權**</td>  
   <td> 
   <p>目前：無[!DNL Workfront Fusion]授權需求。</p> 
   <p>或</p> 
   <p>舊版：任何 </p> 
   </td>  
  </tr>  
  <tr>  
   <td role="rowheader">產品</td>  
   <td> 
   <p>新增：</p> <ul><li>[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Workfront]計畫：您的組織必須購買[!DNL Adobe Workfront Fusion]。</li><li>已包含[！UICONTROL Ultimate] [!DNL Workfront]計畫： [!DNL Workfront Fusion]。</li></ul> 
   <p>或</p> 
   <p>目前：您的組織必須購買[!DNL Adobe Workfront Fusion]。</p> 
   </td>  
  </tr> 
 </tbody>  
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

如需[!DNL Adobe Workfront Fusion]授權的相關資訊，請參閱[[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md)。

## 變數

### now

### timestamp

## 函數

### [!UICONTROL addSeconds （日期；數字）]

將指定秒數新增至日期後，傳回新日期。 若要減去秒數，請輸入負數。

>[!INFO]
>
>**範例：**
>
>* `addSeconds(2016-12-08T15:55:57.536Z;2)`
>
>   傳回2016-12-08T15:55:59.536Z
>
>* `addSeconds(2016-12-08T15:55:57.536Z;-2)`
>
>   傳回2016-12-08T15:55:55.536Z

### [!UICONTROL addMinutes （日期；數字）] {#addminutes-date-number}

將指定分鐘數新增至日期後，傳回新日期。 若要減去分鐘，請輸入負數。

>[!INFO]
>
>**範例：**
>
>* `addMinutes(2016-12-08T15:55:57.536Z;2)`
>
>    傳回2016-12-08T15:57:57.536Z
>
>* `addMinutes(2016-12-08T15:55:57.536Z;-2)`
>
>    傳回2016-12-08T15:53:57.536Z

### [!UICONTROL addHours （日期；數字）] {#addhours-date-number}

將指定小時數新增至日期後，傳回新日期。 若要減去時數，請輸入負數。

>[!INFO]
>
>**範例：**
>
>* `addHours(2016-12-08T15:55:57.536Z; 2)`
>
>    傳回2016-12-08T17:55:57.536Z
>
>* `addHours(2016-12-08T15:55:57.536Z;-2)`
>
>    傳回2016-12-08T13:55:57.536Z

### [!UICONTROL addDays （日期；數字）] {#adddays-date-number}

將指定天數新增至日期後，傳回新日期。 若要減去天數，請輸入負數。

>[!INFO]
>
>**範例：**
>
>* `addDays(2016-12-08T15:55:57.536Z;2)`
>
>    傳回2016-12-10T15:55:57.536Z
>
>* `addDays(2016-12-08T15:55:57.536Z;-2)`
>
>    傳回2016-12-6T15:55:57.536Z

### [!UICONTROL addMonths （日期；數字）]

將指定月份數新增至日期後，傳回新日期。 若要減去月份，請輸入負數。

>[!INFO]
>
>**範例：**
>
>* `addMonths(2016-08-08T15:55:57.536Z;2)`
>
>    傳回2016-10-08T15:55:57.536Z
>
>* `addMonths(2016-08-08T15:55:57.536Z;-2)`
>
>    傳回2016-06-08T15:55:57.536Z

### [!UICONTROL addYears （日期；數字）]

將指定年份新增至日期後，傳回新日期。 若要減去年數，請輸入負數。

>[!INFO]
>
>**範例：**
>
>* `addYears(2016-08-08T15:55:57.536Z;2)`
>
>    傳回2018-08-08T15:55:57.536Z
>
>* `addYears(2016-12-08T15:55:57.536Z; -2)`
>
>    傳回2014-08-08T15:55:57.536Z

### [!UICONTROL setSecond （日期；數字）]

此函式使用引數中指定的秒數傳回新日期。

指定從0到59的數字。 如果數字超出該範圍，此函式會傳回前一分鐘的第二秒（代表負數）或後續的分鐘（代表正數）。

如果您需要指定超出範圍的數字，建議您使用[!UICONTROL  addSeconds]，如上節[addSeconds (date； number)](#addseconds-date-number)所述。

>[!INFO]
>
>**範例：**
>
>* `setSecond(2015-10-07T11:36:39.138Z;10)`
>
>    傳回2015-10-07T11:36:10.138Z
>
>* `setSecond(2015-10-07T11:36:39.138Z; 6)`
>
>    傳回2015-10-07T11:37:01.138Z

### [!UICONTROL setMinute （日期；數字）]

此函式使用引數中指定的分鐘數傳回新日期。

指定從0到59的數字。 如果數字超出該範圍，此函式會傳回前一小時（負數）或後續小時（正數）的分鐘數。

如果您需要指定超出範圍的數字，建議您使用addMinutes，如上方[addMinutes (date； number)](#addminutes-date-number)所述。

>[!INFO]
>
>**範例：**
>
>* `setMinute(2015-10-07T11:36:39.138Z;10)`
>
>    傳回2015-10-07T11:10:39.138Z
>
>* `setMinute(2015-10-07T11:36:39.138Z;61)`
>
>    傳回2015-10-07T12:01:39.138Z

### [!UICONTROL setHour （日期；數字）]

此函式使用引數中指定的小時數傳回新日期。

指定從0到23的數字。 如果數字超出此範圍，此函式會傳回前一天的一小時（若為負數）或後續的天數（若為正數）。

如果您需要指定超出範圍的數字，建議您使用addHours，如上方[addHours (date； number)](#addhours-date-number)所述。

>[!INFO]
>
>**範例：**
>
>* `setHour(2015-08-07T11:36:39.138Z;6)`
>
>   傳回2015-08-07T06:36:39.138Z
>
>* `setHour(2015-08-07T11:36:39.138;-6)`
>
>    傳回2015-08-06T18:36:39.138Z

### [!UICONTROL setDay （日期；英文的當日編號/名稱）]

此函式傳回具有引數中所指定日期的新日期。

您可以使用此函式將星期日設為1，將星期六設為7。 如果您指定從1到7的數字，則產生的日期會在目前（星期日至星期六）的周內。 如果數字超出該範圍，此函式會傳回前一週（負數）或後續周（正數）的某天。

如果您需要指定超出範圍的數字，建議您使用addDays，如上方[addDays (date； number)](#adddays-date-number)所述。

>[!INFO]
>
>**範例：**
>
>* `setDay(2018-06-27T11:36:39.138Z;Monday)`
>
>   傳回2018-06-25T11:36:39.138Z
>
>* `setDay(2018-06-27T11:36:39.138Z;1)`
>
>   傳回2018-06-24T11:36:39.138Z
>
>* `setDay(2018-06-27T11:36:39.138Z;7)`
>
>   傳回2018-06-30T11:36:39.138Z

### [!UICONTROL setDate （日期；數字）]

此函式傳回新的日期，其中包含引數中指定的月份日期。

指定從1到31的數字。 如果數字超出此範圍，此函式會傳回前一個月中的一天（如果是負數）或後續的月份（如果是正數）。

>[!INFO]
>
>**範例：**
>
>* `setDate(2015-08-07T11:36:39.138Z;5)`
>
>   傳回2015-08-05T11:36:39.138Z
>
>* `setDate(2015-08-07T11:36:39.138Z;32)`
>
>   傳回2015-09-01T11:36:39.138Z

### [!UICONTROL setMonth （日期；英文的月份編號/名稱）]

此函式使用引數中指定的月份傳回新日期。

指定從1到12的數字。 如果數字超出此範圍，此函式會傳回前一年（負數）或後續年度（正數）中的月份。

>[!INFO]
>
>**範例：**
>
>* `setMonth(2015-08-07T11:36:39.138Z;5)`
>
>   傳回2015-05-07T11:36:39.138Z
>
>* `setMonth(2015-08-07T11:36:39.138Z;17)`
>
>   傳回2016-05-07T11:36:39.138Z
>
>* `setMonth(2015-08-07T11:36:39.138Z;january)`
>
>   傳回2015-01-07T12:36:39.138Z

### [!UICONTROL setYear （日期；數字）]

以引數中指定的年份傳回新日期。

>[!INFO]
>
>**範例：**
>
>* `setYear(2015-08-07T11:36:39.138Z;2017)`
>
>   傳回2017-08-07T11:36:39.138Z

### [!UICONTROL formatDate （日期；格式；[時區]）]

當您有Date值（例如`12-10-2021 20:30`）且想要格式化為Text值（例如`Dec 10, 2021 8:30 PM`）時，請使用此函式。

例如，當您需要將某個應用程式或Web服務的日期格式變更為相同案例中連線應用程式或Web服務的日期格式時，這個選項會很有用。

如需詳細資訊，請參閱文章[Adobe Workfront Fusion中的專案資料型別](../../workfront-fusion/mapping/item-data-types.md)中的[日期](../../workfront-fusion/mapping/item-data-types.md#date)和[文字](../../workfront-fusion/mapping/item-data-types.md#text)。

#### 參數

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>參數</th> 
   <th>預期的資料型別* </th> 
   <th>作用</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL日期] </td> 
   <td>日期 </td> 
   <td> <p>將日期值轉換為文字值。 </p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL格式] </td> 
   <td>文字 </td> 
   <td> <p>可讓您使用日期/時間格式代號來指定格式。 如需詳細資訊，請參閱[!DNL Adobe Workfront Fusion]</a>中日期和時間格式的<a href="../../workfront-fusion/functions/tokens-for-date-and-time-formatting.md" class="MCXref xref">代號。</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>範例： </b></span></span><code>DD.MM.YYYY HH:mm</code> </p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL時區] </td> 
   <td>文字 </td> 
   <td> <p>（選用）可讓您指定用於轉換的時區。 </p> <p>如需可辨識時區的清單，請參閱Wikipedia <a href="https://en.wikipedia.org/wiki/List_of_tz_database_time_zones"> tz資料庫時區清單</a>中的「TZ資料庫名稱」欄。 函式只會將此欄中列出的值辨識為有效時區。 系統會忽略任何其他值，而改用設定檔中指定的案例時區。 如需詳細資訊，請參閱文章<a href="../../workfront-fusion/workfront-fusion-basics/change-profile-settings.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中變更設定檔設定。</p> <p>如果您忽略此引數，則會套用設定檔設定中指定的情境時區。 </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>範例： </b></span></span><code>Europe/Prague</code>， <code>UTC</code></p> </td> 
  </tr> 
 </tbody> 
</table>

如果提供不同的型別，則會套用型別強制執行。 如需詳細資訊，請參閱[在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/type-coercion.md)中鍵入強制。

#### 傳回值和型別

`formatDate`函式會根據指定的格式和時區，傳回指定日期值的文字表示法。 資料型別為「文字」。

>[!INFO]
>
>**範例：**&#x200B;在這些範例中，案例和網頁時區都設為`Europe/Prague`。
>
>![](assets/date&time-functions-examples-350x61.png)
>
>* `formatDate(1. Date created;MM/DD/YYYY)`
>
>    傳回2018/10/01
>
>* `formatDate(1. Date created; YYYY-MM-DD hh:mm A)`
>
>   傳回2018-10-01 09:32 AM
>
>* `formatDate(1. Date created;DD.MM.YYYY HH:mm;UTC)`
>
>    傳回01.10.2018 07:32
>
>* `formatDate(now;DD.MM.YYYY HH:mm)`
>
>    傳回19.03.2019 15:30

### [!UICONTROL parseDate （文字；格式；[時區]）]

當您有代表日期（例如`12-10-2019 20:30`或`Aug 18, 2019 10:00 AM`）的Text值，而且您想要將其轉換（剖析）為Date值（二進位電腦可讀的表示法）時，請使用此函式。 如需詳細資訊，請參閱文章[在[!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/mapping/item-data-types.md)中的專案資料型別[日期](../../workfront-fusion/mapping/item-data-types.md#date)和[文字](../../workfront-fusion/mapping/item-data-types.md#text)。

#### 參數

第二欄指出預期的型別。 如果提供不同的型別，則會套用型別強制執行。 如需詳細資訊，請參閱[在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/type-coercion.md)中鍵入強制。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>參數</th> 
   <th>預期的資料型別* </th> 
   <th>作用</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL text] </td> 
   <td>文字 </td> 
   <td> <p>將日期值轉換為文字值。 </p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL格式] </td> 
   <td>文字 </td> 
   <td> <p>可讓您使用日期/時間格式代號來指定格式。 如需詳細資訊，請參閱Adobe Workfront Fusion中日期和時間格式的<a href="../../workfront-fusion/functions/tokens-for-date-and-time-formatting.md" class="MCXref xref">代號</a>。</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>範例： </b></span></span><code>DD.MM.YYYY HH:mm</code> </p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL時區] </td> 
   <td>文字 </td> 
   <td> <p>（選用）可讓您指定用於轉換的時區。 </p> <p>如需可辨識時區的清單，請參閱Wikipedia <a href="https://en.wikipedia.org/wiki/List_of_tz_database_time_zones"> tz資料庫時區清單</a>中的「TZ資料庫名稱」欄。 函式只會將此欄中列出的值辨識為有效時區。 系統會忽略任何其他值，而改用設定檔中指定的案例時區。 如需詳細資訊，請參閱文章<a href="../../workfront-fusion/workfront-fusion-basics/change-profile-settings.md" class="MCXref xref">在Adobe Workfront Fusion中變更設定檔設定</a>。</p> <p>如果您忽略此引數，則會套用設定檔設定中指定的情境時區。</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>範例： </b></span></span><code>Europe/Prague</code>， <code>UTC</code></p> </td> 
  </tr> 
 </tbody> 
</table>

如果提供不同的型別，則會套用型別強制執行。 如需詳細資訊，請參閱[在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/type-coercion.md)中鍵入強制。

#### 傳回值和型別

此函式根據您指定的格式和時區將文字字串轉換為日期。 值的資料型別為「日期」。

>[!INFO]
>
>**範例：**&#x200B;在下列範例中，傳回的Date值是根據ISO 8601表示，但結果的資料型別為Date。
>
>* `parseDate(2016-12-28;YYYY-MM-DD)`
>
>    傳回2016-12-28T00:00:00.000Z
>
>* `parseDate(2016-12-28 16:03;YYYY-MM-DD HH:mm)`
>
>    傳回2016-12-28T16:03:00.000Z
>
>* `parseDate(2016-12-28 04:03 pm; YYYY-MM-DD hh:mm a)`
>
>    傳回2016-12-28T16:03:06.000Z
>
>* `parseDate(1482940986;X)`
>
>   傳回2016-12-28T16:03:06.000Z

### [!UICONTROL dateDifference (Date1； Date2； Unit)]

傳回代表兩個日期之間差異的數字，以指定的單位表示。

從Date1減去Date2。

為`unit`引數使用下列其中一個時間值：

* 毫秒
* 秒
* 分鐘
* 小時
* 天
* 周
* 月

若未指定單位，此函式會傳回毫秒差。

>[!INFO]
>
>**範例：**
>
>* `dateDifference(2021-05-11T18:10:00.000Z;2021-05-11T18:00:00.000Z)`
>
>    傳回`600,000`
>
>* `dateDifference(2021-05-11T18:10:00.000Z;2021-05-11T18:00:00.000Z;hours)`
>
>    傳回`4`
>
>* `dateDifference2021-06-11T18:10:00.000Z;2021-05-11T18:00:00.000Z;months)`
>
>    傳回`1`

### 其他範例

#### 如何計算每個月中每週的第n天

本節是針對[!DNL Exceljet]網頁中的[!DNL Workfront Fusion]改寫，該網頁說明如何取得一個月中的第n天。

如果您需要計算與當月第n天對應的日期（例如，第一個星期二、第三個星期五等），您可以使用下列公式：

![](assets/date&time-functions-calc-nth-day-350x31.png)

```
{{addDays(setDate(1.date; 1); 1.n * 7 - formatDate(addDays(setDate(1.date; 1); "-" + 1.dow); "E"))}}
```

公式包含下列專案：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>1.n</code> </td> 
   <td> <p> 第n天：</p> 
    <ul> 
     <li><code>1</code> （第1個星期二）</li> 
     <li><code>2</code> （第2個星期二）</li> 
     <li><code>3</code> 第3個星期二，依此類推</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td><code>2.dow</code> </td> 
   <td> <p> 星期：</p> 
    <ul> 
     <li><code>1</code> 表示星期一</li> 
     <li><code>2</code> 表示星期二</li> 
     <li><code>3</code> 表示星期三</li> 
     <li><code>4</code> 表示星期四</li> 
     <li><code>5</code> 週五</li> 
     <li><code>6</code> 代表星期六</li> 
     <li><code>7</code> 代表星期日</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td><code>1.date</code> </td> 
   <td> <p> 日期決定月份。 若要計算當月一週的第n天，請使用<code>now</code>變數。</p> </td> 
  </tr> 
 </tbody> 
</table>

如果您只想計算一個特定案例，例如每逢星期三，您就可以將公式中的專案`1.n`和`2.dow`取代為對應的數字。 對於當月的第二個星期三，您會使用下列值：

* `1.n` = `2`
* `1.dow` = `3`
* `1.date` = `now`

![](assets/nth-day-variable-value-350x33.png)

#### 說明：

* `setDate(now;1)`傳回目前月份的第一個月
* `formatDate(....;E)`傳回一週中的某天(1， 2， ... 6)

### 如何計算日期之間的天數

一種可能是使用以下運算式：

![](assets/calculate-days-between-dates-350x68.png)

```
{{round((2.value - 1.value) / 1000 / 60 / 60 / 24)}}
```

>[!NOTE]
>
>* `D1`和`D2`的值必須是日期型別值。 如果是String型別值（例如20.10.2018），請使用`parseDate()`函式將它們轉換為Date型別值。
>
>* `round()`函式適用於其中一個日期在日光節約時間期間內，而另一個日期不在日光節約時間期間的情況。 在這些情況下，時數差會少一小時或更多。 您可以將其除以24來得出非整數結果。 您會失去一小時的日光節約時間。 將平面化成圓形，這樣就不會有百分比

#### 如何計算月份的最後一天/毫秒

當您指定日期範圍時，例如在搜尋模組中，如果範圍跨越整個前一個月為關閉間隔（包括其兩個限制點的間隔），則需要計算該月的最後一天。

2019-09-01 ≤ D ≤ 2019-09-30

下列公式顯示一種計算前一個月最後一天的方法：

![](assets/last-day-prev-month.png)

```
{{addDays(setDate(now; 1); -1)}}
```

在某些情況下，您不僅需要計算當月的最後一天，還需要實際計算其最後一毫秒：

2019-09-01T00:00:00.000Z ≤ D ≤ 2019-09-30T23:59:59.999Z

此公式顯示計算前一個月最後一毫秒的一種方式：

![](assets/last-millisecond-prev-month-350x45.png)

```
{{parseDate(parseDate(formatDate(now; "YYYYMM01"); "YYYYMMDD"; "UTC") - 1; "x")}}
```

如果您需要結果來使用時區設定，請省略UTC引數：

![](assets/omit-utc-argument-350x45.png)

`{{parseDate(parseDate(formatDate(now; "YYYYMM01"); "YYYYMMDD") - 1; "x")}}`

不過，最好改用半開間隔（排除其限制點之一的間隔），改為指定下個月的第一天，並將「小於或等於」運運算元取代為「小於」，如下所示：

`2019-09-01 ≤ D < 2019-10-01`

`2019-09-01T00:00:00.000Z ≤ D < 2019-10-01T00:00:00.000Z`
