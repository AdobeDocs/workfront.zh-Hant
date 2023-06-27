---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: Adobe Workfront Fusion中的字串函式
description: Adobe Workfront Fusion對應面板中有以下字串函式。
author: Becky
feature: Workfront Fusion
exl-id: c6676a87-2498-4de8-b877-7edc30aeabae
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '774'
ht-degree: 3%

---

# 中的字串函式 [!DNL Adobe Workfront Fusion]

## 存取需求

您必須具有下列存取權才能使用本文中的功能：

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
   <td> <p>[！UICONTROL計畫]，[！UICONTROL工作]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Adobe Workfront Fusion]授權**</td> 
   <td>
   <p>目前授權需求：否 [!DNL Workfront Fusion] 授權需求。</p>
   <p>或</p>
   <p>舊版授權需求： [！UICONTROL [!DNL Workfront Fusion] 適用於工作自動化與整合] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>
   <p>目前產品需求：如果您有[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Adobe Workfront] 計畫，您的組織必須購買 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文所述功能。 [!DNL Workfront Fusion] 包含在[！UICONTROL Ultimate]中 [!DNL Workfront] 計畫。</p>
   <p>或</p>
   <p>舊版產品需求：貴組織必須購買 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文所述功能。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

若要瞭解您擁有哪些計畫、授權型別或存取權，請聯絡您的 [!DNL Workfront] 管理員。

有關以下專案的資訊： [!DNL Adobe Workfront Fusion] 授權，請參閱 [[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!UICONTROL ascii (文字； [移除變音符號])]

移除文字字串中的所有非ascii字元。

>[!INFO]
>
>**範例:**
>
>* `ascii(` `Wěošrčkřfžrýoáníté` `)`
>
>   傳回： [!DNL Workfront]
>
>* `ascii(` `ěščřž` `;` `true` `)`
>
>   傳回： [!UICONTROL escrz]

## [!UICONTROL base64 （文字）]

將文字轉換為base64。

>[!INFO]
>
>**範例:**
>
>`base64( workfront )`
>
>傳回： d29ya2Zyb250==

## [!UICONTROL 大寫（文字）]

將文字字串中的第一個字元轉換為大寫。

>[!INFO]
>
>**範例:**
>
>`capitalize( workfront )`
>
>傳回： [!DNL Workfront]

## 包含（文字；搜尋字串）

驗證文字是否包含搜尋字串。

>[!INFO]
>
>**範例:**
>
>* `contains( Hello World ; Hello )`
>
>   傳回： [!UICONTROL true]
>
>* `contains( Hello World ; Bye )`
>
>   傳回： [!UICONTROL false]

## [!UICONTROL decodeURL （文字）]

將URL中的特殊字元解碼為文字。

>[!INFO]
>
>**範例:**
>`decodeURL( Automate%20your%20workflow )`
>
>傳回： [!UICONTROL 自動化您的工作流程]

## [!UICONTROL encodeURL （文字）]

將某些文字中的特殊字元編碼為有效的URL位址。

## [!UICONTROL escapeHTML （文字）]

逸出文字中的所有HTML標籤。

>[!INFO]
>
>**範例:**
>
>`escapeHTML( <b>Hello</b> )`
>
> 傳回： `&lt;b&gt;Hello&lt;/b&gt;`

## [!UICONTROL escapeMarkdown(text)]

逸出文字中的所有Markdown標籤。

>[!INFO]
>
>**範例:**
>
>`escapeMarkdown( # Header )`
>
>傳回： `&#35; Header`

## [!DNL indexOf (string; value; [start])]

傳回指定值在字串中第一次出現的位置。 如果搜尋的值不存在，此方法會傳回&#39;-1&#39;。 起始值表示字串中開始搜尋的位置。

>[!INFO]
>
>**範例:**
>
>* `indexOf( Workfront ; o )`
>
>   傳回： 1
>
>* `indexOf( Workfront ; x )`
>
>   傳回： -1
>
>* `indexOf( Workfront ; o ; 3 )`
>
>   傳回： 6

## [!UICONTROL 長度（文字或緩衝區）]

傳回文字字串長度（字元數）或二進位緩衝區（緩衝區大小，以位元組為單位）。

>[!INFO]
>
>**範例:**
>
>`length( hello )`
>
>傳回： 5

## [!UICONTROL lower (text)]

將文字字串中的所有字母字元轉換為小寫。

>[!INFO]
>
>**範例:**
>
>`lower( Hello )`
>
>傳回： hello

## [!UICONTROL md5 （文字）]

計算字串的md5雜湊。

>[!INFO]
>
>**範例:**
>
>`md5( Workfront )`
>
>傳回： `1448bbbeaa7a9b8091d426999f1f666b`

## [!UICONTROL 取代（文字；搜尋字串；取代字串）]

以新字串取代搜尋字串。

>[!INFO]
>
>**範例:**
>
>`replace( Hello World ; Hello ; Hi )`
>
>傳回： [!UICONTROL Hi World]

規則運算式(包含在 `/.../`)可作為搜尋字串使用，並搭配使用各種標幟(例如 `g`， `i`， `m`)已附加：

>[!INFO]
>
>**範例:**
>
>![](assets/replace---1-350x31.png)
>
>這些數字X X X X全部取代為X

取代字串可包含下列特殊取代模式：

* `$&` 插入相符的子字串。
* `$n` 其中n是小於100的正整數，插入第n個以括弧括住的子符合字串。 此索引為1。

>[!INFO]
>
>**範例:**
>
>![](assets/variable-value-350x63.png)
>
>傳回：電話號碼 `+420777111222`
>>
>![](assets/variable-value---2-350x55.png)
>
>傳回：電話號碼： `+420777111222`

>[!CAUTION]
>
>請勿使用已命名的擷取群組，例如 `/ is (?<number>\d+)/` 在取代字串引數中。 這樣做會導致錯誤。

如需規則運算式的詳細資訊，請參閱 [文字剖析器](../../workfront-fusion/apps-and-their-modules/text-parser.md).

## [!UICONTROL sha1 (文字； [編碼]； [金鑰])]

計算字串的sha1雜湊。 如果指定機碼引數，則會傳回sha1 HMAC雜湊。 支援的編碼：「hex」（預設）、「base64」或「latin1」。

>[!INFO]
>
>**範例:**
>
>`sha1( workfront )`
>
>傳回： b2b30b8ae1f9e5b40fbb0696eaabdbfd8d0c087f

## [!UICONTROL sha256 (文字； [編碼]； [金鑰])]

計算字串的sha256雜湊。 如果指定機碼引數，則會傳回sha256 HMAC雜湊。 支援的編碼：「hex」（預設）、「base64」或「latin1」。>

>[!INFO]
>
>**範例:**
>
>`sha256( workfront )`
>
>傳回： ed3d7397eec7b94453035b67ba4468c883ee3bedeb57137f7371f2e0cf5e2bbc

## [!UICONTROL sha512 (文字； [輸出編碼]； [金鑰]； [金鑰編碼])]

計算字串的sha512雜湊。 如果指定機碼引數，則會傳回sha512 HMAC雜湊。

支援的編碼：

* &quot;[!UICONTROL 十六進位]「 （預設）
* &quot;[!UICONTROL base64]&quot;
* &quot;[!UICONTROL latin1]&quot;

支援的金鑰編碼：

* &quot;[!UICONTROL 文字]「 （預設）
* &quot;[!UICONTROL 十六進位]&quot;
* &quot;[!UICONTROL base64]「或」[!UICONTROL 二進位]&quot;

使用&quot;[!UICONTROL 二進位]「金鑰編碼，金鑰必須是緩衝區，而不是字串。

>[!INFO]
>
>**範例:**
>
>`sha512(workfront)`
>
>傳回： 789ae41b9456357e4f27c6a09956a767abbb8d80b206003ffdd1e94dbc687cd119b85e1e19db58bb44b234493af35fd431639c0345aadf2cf7ec26e9f4a7fb19

## [!UICONTROL 分割（文字；分隔符號）]

藉由將字串分割為子字串，將字串分割為字串陣列。

>[!INFO]
>
>**範例:**
>
>`split( John, George, Paul ; , )`

## [!UICONTROL startcase （文字）]

每個字詞的第一個字母都會變成大寫，其他字母則會變成小寫。

>[!INFO]
>
>**範例:**
>`startcase( hello WORLD )`
>
>傳回： [!UICONTROL Hello World]

## [!UICONTROL stripHTML （文字）]

從文字中移除所有HTML標籤。

>[!INFO]
>
>**範例:**
>
>`stripHTML( <b>Hello</b> )`
>
>傳回： Hello

## [!UICONTROL 子字串（文字；開始；結束）]

傳回「開始」位置和「結束」位置之間的文字字串部分。

>[!INFO]
>
>**範例:**
>
>* `substring( Hello ; 0 ; 3)`
>
>   傳回：高度
>
>* `substring( Hello ; 1 ; 3 )`
>
>   傳回： el

## [!UICONTROL toBinary （值）]

將任何值轉換為二進位資料。

您也可以指定編碼作為第二個引數，以將十六進位或base64的二進位轉換套用至二進位資料。

>[!INFO]
>
>**範例:**
>
>* `toBinary( Workfront )`
>
>   傳回： 57 6f 72 6b 66 72 6f 6e 74
>
>* `toBinary( V29ya2Zyb250 ; base64 )`
>
>   傳回： 57 6f 72 6b 66 72 6f 6e 74

## [!UICONTROL toString （值）]

將任何值轉換為字串。

## [!UICONTROL trim （文字）]

移除文字開頭或結尾的空格字元。

## [!UICONTROL upper （文字）]

將文字字串中的所有字母字元轉換為大寫。

>[!INFO]
>
>**範例:**
>
>`upper( Hello )`
>
>傳回： [!UICONTROL 您好]
