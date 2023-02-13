---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: Adobe Workfront Fusion中的日期與時間函式
description: Adobe Workfront Fusion對應面板提供下列日期和時間函式。
author: Becky
feature: Workfront Fusion
exl-id: 76c63afc-4bb6-4895-9bba-6b3913ecbcf6
source-git-commit: fcaa2136310cad8ef478020a9bae34bbe5520c6d
workflow-type: tm+mt
source-wordcount: '1867'
ht-degree: 1%

---

# 日期和時間函式，於 [!DNL Adobe Workfront Fusion]

## 存取需求

您必須具備下列存取權才能使用本文中的功能：

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計劃*</td> 
   <td> <p>[!DNL Pro] 或更高</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權*</td> 
   <td> <p>[!UICONTROL計畫]、[!UICONTROL工作]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion]授權**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] （工作自動化和整合） </p><p>[!UICONTROL [!DNL Workfront Fusion] （工作自動化）</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>貴組織必須購買 [!DNL Adobe Workfront Fusion] 和 [!DNL Adobe Workfront] 以使用本文所述的功能。</td> 
  </tr> 
 </tbody> 
</table>

若要了解您擁有的計畫、授權類型或存取權，請聯絡您的 [!DNL Workfront] 管理員。

如需 [!DNL Adobe Workfront Fusion] 許可證，請參閱 [[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!UICONTROL formatDate(date;格式； [時區])]

當您有日期值時(例如 `12-10-2021 20:30`，以將其格式化為文字值，例如 `Dec 10, 2021 8:30 PM`.

例如，在相同案例中，當您需要將一個應用程式或網站服務的日期格式變更為已連線應用程式或網站服務的日期格式時，這個用法就很實用。

如需詳細資訊，請參閱 [日期](../../workfront-fusion/mapping/item-data-types.md#date) 和 [文字](../../workfront-fusion/mapping/item-data-types.md#text) 在文章中 [Adobe Workfront Fusion中的項目資料類型](../../workfront-fusion/mapping/item-data-types.md).

### 參數

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>參數</th> 
   <th>預期的資料類型* </th> 
   <th>它的作用</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL日期] </td> 
   <td>日期 </td> 
   <td> <p>將日期值轉換為文字值。 </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL格式] </td> 
   <td>文字 </td> 
   <td> <p>可讓您使用日期/時間格式化Token來指定格式。 如需詳細資訊，請參閱 <a href="../../workfront-fusion/functions/tokens-for-date-and-time-formatting.md" class="MCXref xref">日期和時間格式的代號，位於 [!DNL Adobe Workfront Fusion]</a>.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>範例: </b></span></span><code>DD.MM.YYYY HH:mm</code> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL時區] </td> 
   <td>文字 </td> 
   <td> <p>（選用）可讓您指定用於轉換的時區。 </p> <p>如需已識別時區的清單，請參閱Wikipedia中的「TZ資料庫名稱」欄 <a href="https://en.wikipedia.org/wiki/List_of_tz_database_time_zones">tz資料庫時區清單</a>. 只有此欄中列出的值會由函式辨識為有效時區。 系統會忽略任何其他值，並改用設定檔中指定的藍本時區。 如需詳細資訊，請參閱文章中的 <a href="../../workfront-fusion/workfront-fusion-basics/change-profile-settings.md" class="MCXref xref">在 [!DNL Adobe Workfront Fusion]</a>.</p> <p>如果忽略此參數，則會套用設定檔設定中指定的藍本時區。 </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>範例: </b></span></span><code>Europe/Prague</code>, <code>UTC</code></p> </td> 
  </tr> 
 </tbody> 
</table>

如果提供了不同類型，則應用類型強制。 如需詳細資訊，請參閱 [中的強制類型 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/type-coercion.md).

### 傳回值和類型

此 `formatDate` 函式會根據指定的格式和時區，傳回指定日期值的文字表示。 資料類型為Text。

>[!INFO]
>
>**範例：** 藍本和Web時區均設為 `Europe/Prague` 在這些範例中。
>
>![](assets/date&time-functions-examples-350x61.png)
>
>* `formatDate(1. Date created;MM/DD/YYYY)`
   >
   >    傳回10/01/2018
>
>* `formatDate(1. Date created; YYYY-MM-DD hh:mm A)`
   >
   >   返回2018-10-01 09:32 AM
>
>* `formatDate(1. Date created;DD.MM.YYYY HH:mm;UTC)`
   >
   >    返回01.10.2018 07:32
>
>* `formatDate(now;DD.MM.YYYY HH:mm)`
   >
   >    傳回19.03.2019 15:30


## [!UICONTROL parseDate(text;格式； [時區])]

若您有代表日期的文字值(例如 `12-10-2019 20:30` 或 `Aug 18, 2019 10:00 AM`)，而您想要將其轉換（剖析）為日期值（二進位機器可讀的表示法）。 如需詳細資訊，請參閱 [日期](../../workfront-fusion/mapping/item-data-types.md#date) 和 [文字](../../workfront-fusion/mapping/item-data-types.md#text) 在文章中 [中的項目資料類型 [!UICONTROL Adobe Workfront融合]](../../workfront-fusion/mapping/item-data-types.md).

### 參數

第二欄指出預期的類型。 如果提供了不同類型，則應用類型強制。 如需詳細資訊，請參閱 [中的強制類型 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/type-coercion.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>參數</th> 
   <th>預期的資料類型* </th> 
   <th>它的作用</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL文本] </td> 
   <td>文字 </td> 
   <td> <p>將日期值轉換為文字值。 </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL格式] </td> 
   <td>文字 </td> 
   <td> <p>可讓您使用日期/時間格式化Token來指定格式。 如需詳細資訊，請參閱 <a href="../../workfront-fusion/functions/tokens-for-date-and-time-formatting.md" class="MCXref xref">Adobe Workfront Fusion中日期和時間格式的代號</a>.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>範例: </b></span></span><code>DD.MM.YYYY HH:mm</code> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL時區] </td> 
   <td>文字 </td> 
   <td> <p>（選用）可讓您指定用於轉換的時區。 </p> <p>如需已識別時區的清單，請參閱Wikipedia中的「TZ資料庫名稱」欄 <a href="https://en.wikipedia.org/wiki/List_of_tz_database_time_zones">tz資料庫時區清單</a>. 只有此欄中列出的值會由函式辨識為有效時區。 系統會忽略任何其他值，並改用設定檔中指定的藍本時區。 如需詳細資訊，請參閱文章中的 <a href="../../workfront-fusion/workfront-fusion-basics/change-profile-settings.md" class="MCXref xref">變更Adobe Workfront Fusion中的設定檔設定</a>.</p> <p>如果忽略此參數，則會套用設定檔設定中指定的藍本時區。</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>範例: </b></span></span><code>Europe/Prague</code>, <code>UTC</code></p> </td> 
  </tr> 
 </tbody> 
</table>

如果提供了不同類型，則應用類型強制。 如需詳細資訊，請參閱 [中的強制類型 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/type-coercion.md).

### 傳回值和類型

此函式會根據您指定的格式和時區，將文字字串轉換為日期。 值的資料類型為Date。

>[!INFO]
>
>**範例：** 在以下示例中，返回的Date值是根據ISO 8601表示的，但結果的資料類型是Date。
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
>  傳回2016-12-28T16:03:06.000Z

## [!UICONTROL addDays(date;數字)] {#adddays-date-number}

傳回新日期，因為將指定天數新增至日期。 要減去天數，請輸入負數。

>[!INFO]
>
>**範例:**
>
>* `addDays(2016-12-08T15:55:57.536Z;2)`
   >
   >    傳回2016-12-10T15:55:57.536Z
>
>* `addDays(2016-12-08T15:55:57.536Z;-2)`
   >
   >    傳回2016-12-6T15:55:57.536Z


## [!UICONTROL addHours(date;數字)] {#addhours-date-number}

傳回將指定小時數新增至日期的新日期。 要減去小時數，請輸入負數。

>[!INFO]
>
>**範例:**
>
>* `addHours(2016-12-08T15:55:57.536Z; 2)`
   >
   >    傳回2016-12-08T17:55:57.536Z
>
>* `addHours(2016-12-08T15:55:57.536Z;-2)`
   >
   >    傳回2016-12-08T13:55:57.536Z


## [!UICONTROL addMinutes(date;數字)] {#addminutes-date-number}

將指定的分鐘數新增至日期，以傳回新日期。 要減去分鐘，請輸入負數。

>[!INFO]
>
>**範例:**
>
>* `addMinutes(2016-12-08T15:55:57.536Z;2)`
   >
   >    傳回2016-12-08T15:57:57.536Z
>
>* `addMinutes(2016-12-08T15:55:57.536Z;-2)`
   >
   >    傳回2016-12-08T15:53:57.536Z


## [!UICONTROL addMonths(date;數字)] {#addseconds-date-number}

傳回將指定月數新增至日期的新日期。 要減去月份，請輸入負數。

>[!INFO]
>
>**範例:**
>
>* `addMonths(2016-08-08T15:55:57.536Z;2)`
   >
   >    傳回2016-10-08T15:55:57.536Z
>
>* `addMonths(2016-08-08T15:55:57.536Z;-2)`
   >
   >    傳回2016-06-08T15:55:57.536Z


## [!UICONTROL addSeconds(date;數字)]

將指定的秒數新增至日期後，傳回新日期。 要減去秒數，請輸入負數。

>[!INFO]
>
>**範例:**
>
>* `addSeconds(2016-12-08T15:55:57.536Z;2)`
   >
   >   傳回2016-12-08T15:55:59.536Z
>
>* `addSeconds(2016-12-08T15:55:57.536Z;-2)`
   >
   >   傳回2016-12-08T15:55:55.536Z


## [!UICONTROL addYears(date;數字)]

將指定的年數新增至日期，以傳回新日期。 要減去年，請輸入負數。

>[!INFO]
>
>**範例:**
>
>* `addYears(2016-08-08T15:55:57.536Z;2)`
   >
   >    傳回2018-08-08T15:55:57.536Z
>
>* `addYears(2016-12-08T15:55:57.536Z; -2)`
   >
   >    傳回2014-08-08T15:55:57.536Z


## [!UICONTROL setSecond(date;數字)]

此函式會傳回新日期，並以參數中指定的秒數表示。

指定0到59之間的數字。 如果數字超出該範圍，則函式會從前一分鐘（對於負數）或後一分鐘（對於正數）返回一秒。

如果您需要指定範圍以外的數字，建議您使用[!UICONTROL  addSeconds]，如上一節所述 [addSeconds(date;數字)](#addseconds-date-number).

>[!INFO]
>
>**範例:**
>
>* `setSecond(2015-10-07T11:36:39.138Z;10)`
   >
   >    傳回2015-10-07T11:36:10.138Z
>
>* `setSecond(2015-10-07T11:36:39.138Z; 6)`
   >
   >    傳回2015-10-07T11:37:01.138Z


## [!UICONTROL setMinute(date;數字)]

此函式會傳回新日期，並在參數中指定分鐘。

指定0到59之間的數字。 如果數字超出該範圍，則函式會從前一小時（對於負數）或後一小時（對於正數）返回一分鐘。

如果您需要指定範圍以外的數字，建議您使用addMinutes，如上所述： [addMinutes(date;數字)](#addminutes-date-number).

>[!INFO]
>
>**範例:**
>
>* `setMinute(2015-10-07T11:36:39.138Z;10)`
   >
   >    傳回2015-10-07T11:10:39.138Z
>
>* `setMinute(2015-10-07T11:36:39.138Z;61)`
   >
   >    傳回2015-10-07T12:01:39.138Z


## [!UICONTROL setHour(date;數字)]

此函式會傳回新日期，並在參數中指定小時。

指定0到23之間的數字。 如果數字超出此範圍，函式會從前一天（對於負數）或後一天（對於正數）傳回一小時。

如果您需要指定範圍以外的數字，建議您使用addHours，如上所述： [addHours(date;數字)](#addhours-date-number).

>[!INFO]
>
>**範例:**
>
>* `setHour(2015-08-07T11:36:39.138Z;6)`
   >
   >   傳回2015-08-07T06:36:39.138Z
>
>* `setHour(2015-08-07T11:36:39.138;-6)`
   >
   >    傳回2015-08-06T18:36:39.138Z


## [!UICONTROL setDay(date;日數/名稱（英文）]

此函式會傳回新日期，並在參數中指定日期。

您可以使用此函式設定一週中的某天，其中週日為1，週六為7。 如果您指定從1到7的數字，則產生的日期在目前（星期日到星期六）周內。 如果數字超出該範圍，則函式會傳回前一週（對於負數）或後一週（對於正數）的一天。

如果您需要指定範圍以外的數字，建議您使用addDays，如上所述： [addDays(date;數字)](#adddays-date-number).

>[!INFO]
>
>**範例:**
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


## [!UICONTROL setDate(date;數字)]

此函式會傳回新日期，並在參數中指定月份的某天。

指定從1到31的數字。 如果數字超出此範圍，則函式會傳回上個月（負數）或後續月（正數）的某天。

>[!INFO]
>
>**範例:**
>
>* `setDate(2015-08-07T11:36:39.138Z;5)`
   >
   >   傳回2015-08-05T11:36:39.138Z
>
>* `setDate(2015-08-07T11:36:39.138Z;32)`
   >
   >   傳回2015-09-01T11:36:39.138Z


## [!UICONTROL setMonth(date;月份編號/名稱（英文）]

此函式會傳回新日期，並在參數中指定月份。

指定從1到12的數字。 如果數字超出此範圍，函式會傳回前一年（負數）或後一年（正數）的月份。

>[!INFO]
>
>**範例:**
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


## [!UICONTROL setYear(date;數字)]

傳回參數中指定年份的新日期。

>[!INFO]
>
>**範例:**
>
>* `setYear(2015-08-07T11:36:39.138Z;2017)`
   >
   >   傳回2017-08-07T11:36:39.138Z


## [!UICONTROL dateDifference(Date1;日期2;單位)]

傳回代表兩個日期之間差異的數字，以指定單位表示。

從Date1中減去Date2。

請將下列其中一個時間值用於 `unit` 參數：

* 毫秒
* 秒
* 分鐘
* 小時
* 日
* 周
* 月

如果未指定任何單位，則函式將返回以毫秒為單位的差值。

>[!INFO]
>
>**範例:**
>
>* `dateDifference(2021-05-11T18:10:00.000Z;2021-05-11T18:00:00.000Z)`
   >
   >    傳回 `600,000`
>
>* `dateDifference(2021-05-11T18:10:00.000Z;2021-05-11T18:00:00.000Z;hours)`
   >
   >    傳回 `4`
>
>* `dateDifference2021-06-11T18:10:00.000Z;2021-05-11T18:00:00.000Z;months)`
   >
   >    傳回 `1`


## 其他範例

### 如何計算月中的第n天

本節適用於 [!DNL Workfront Fusion] 從 [!DNL Exceljet] 說明如何在一個月內取得第n天的網頁。

如果您需要計算與月中第n天（例如，第一個星期二、第三個星期五等）對應的日期，可以使用下列公式：

![](assets/date&time-functions-calc-nth-day-350x31.png)

```
{{addDays(setDate(1.date; 1); 1.n * 7 - formatDate(addDays(setDate(1.date; 1); "-" + 1.dow); "E"))}}
```

公式包含下列項目：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>1.n</code> </td> 
   <td> <p> 第n天：</p> 
    <ul> 
     <li><code>1</code> 1日星期二</li> 
     <li><code>2</code> 2日</li> 
     <li><code>3</code> 3個星期二，等等</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td><code>2.dow</code> </td> 
   <td> <p> 星期：</p> 
    <ul> 
     <li><code>1</code> 星期一</li> 
     <li><code>2</code> 星期二</li> 
     <li><code>3</code> 為星期三</li> 
     <li><code>4</code> 星期四</li> 
     <li><code>5</code> 星期五</li> 
     <li><code>6</code> 為星期六</li> 
     <li><code>7</code> 為星期日</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td><code>1.date</code> </td> 
   <td> <p> 日期決定月份。 若要計算當月的第n天，請使用 <code>now</code> 變數。</p> </td> 
  </tr> 
 </tbody> 
</table>

如果您只想計算一個特定案例，例如，每隔一個星期三，您就可以取代項目 `1.n` 和 `2.dow` 在公式中具有對應數字。 對於當月的第二個星期三，您會使用下列值：

* `1.n` = `2`
* `1.dow` = `3`
* `1.date` = `now`

![](assets/nth-day-variable-value-350x33.png)

### 說明：

* `setDate(now;1)` 當月初傳回
* `formatDate(....;E)` 傳回星期(1、2、.. 6)

## 如何計算日期之間的天數

一種可能性是使用下列運算式：

![](assets/calculate-days-between-dates-350x68.png)

```
{{round((2.value - 1.value) / 1000 / 60 / 60 / 24)}}
```

>[!NOTE]
>
>* 值 `D1`和 `D2` 為日期類型值。 如果它們是字串類型值(例如20.10.2018)，請使用 `parseDate()` 功能，將其轉換為日期類型值。
>
>* 此 `round()` 函式適用於其中一個日期落在日光節約時間期間內，而另一個日期不在時。 在這些情況下，小時數的差異會少一小時或更久。 對於非整數結果，可以將其除以24。 你失去了一小時夏令時。 四捨五入會拼合，因此您沒有百分比


### 如何計算每月的最後一天/毫秒

當您指定日期範圍時（例如在搜尋模組中），如果範圍以關閉間隔（包括兩個限制點的間隔）涵蓋前一個月的整個時間範圍，則需要計算該月的最後一天。

2019-09-01 ≤ D ≤ 2019-09-30

下列公式說明如何計算前一個月的最後一天：

![](assets/last-day-prev-month.png)

```
{{addDays(setDate(now; 1); -1)}}
```

在某些情況下，您不僅需要計算每個月的最後一天，還需要計算最後一毫秒：

2019-09-01T00:00:00.000Z ≤ D ≤ 2019-09-30T23:59:59.999Z

此公式說明如何計算前一個月的最後毫秒：

![](assets/last-millisecond-prev-month-350x45.png)

```
{{parseDate(parseDate(formatDate(now; "YYYYMM01"); "YYYYMMDD"; "UTC") - 1; "x")}}
```

如果需要使用時區設定的結果，請忽略UTC參數：

![](assets/omit-utc-argument-350x45.png)

`{{parseDate(parseDate(formatDate(now; "YYYYMM01"); "YYYYMMDD") - 1; "x")}}`

不過，最好使用半開間隔（排除其中一個限制點的間隔），指定下個月的第一天，並以「小於」取代「小於或等於」運算子，如下所示：

`2019-09-01 ≤ D < 2019-10-01`

`2019-09-01T00:00:00.000Z ≤ D < 2019-10-01T00:00:00.000Z`
