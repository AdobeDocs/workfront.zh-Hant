---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
navigation-topic: apps-and-their-modules
title: 文字剖析器
description: 您可以使用文字剖析器工具來剖析要用於其他 [!DNL Adobe Workfront Fusion] 方案模組。 文本解析器不需要連接。
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 7d71cf64-4f86-42c5-81e7-8fc15333cbd7
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1010'
ht-degree: 0%

---

# [!UICONTROL 文字剖析器]

您可以使用 [!UICONTROL 文字剖析器工具] 要分析文本以用於其他 [!DNL Adobe Workfront Fusion] 方案模組。 此 [!UICONTROL 文字剖析器] 不需要連線。

## 存取需求

您必須具備下列存取權才能使用本文中的功能：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計劃*</td>
  <td> <p>[!UICONTROL Pro]或更高版本</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權*</td>
   <td> <p>[!UICONTROL計畫]、[!UICONTROL工作]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] 許可**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] （工作自動化和整合） </p> <p>[!UICONTROL [!DNL Workfront Fusion] （工作自動化）</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>貴組織必須購買 [!DNL Adobe Workfront Fusion] 和 [!DNL Adobe Workfront] 以使用本文所述的功能。</td> 
  </tr> 
 </tbody> 
</table>

若要了解您擁有的計畫、授權類型或存取權，請聯絡您的 [!DNL Workfront] 管理員。

如需 [!DNL Adobe Workfront Fusion] 許可證，請參閱 [[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!UICONTROL 文字剖析器] 模組及其欄位

設定時 [!UICONTROL 文字剖析器] 模組， [!DNL Adobe Workfront Fusion] 顯示下列欄位。 模組中的粗體標題表示必填欄位。

如果您在欄位或函式上方看到對應按鈕，則可使用它來設定該欄位的變數和函式。 如需詳細資訊，請參閱 [將資訊從一個模組對應到 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### 變形金剛

* [[!UICONTROL 從HTML取得元素]](#get-elements-from-html)
* [[!UICONTROL 從文字取得元素]](#get-elements-from-text)
* [[!UICONTROL HTML到文本]](#html-to-text)
* [[!UICONTROL 匹配模式]](#match-pattern)
* [[!UICONTROL 取代]](#replace)

#### [!UICONTROL 從HTML取得元素]

從HTML程式碼中擷取所需元素。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL即使模組找不到匹配項，仍繼續執行路由]</td> 
   <td> <p>啟用此選項，以確保若模組未傳回任何結果，則不會停止案例。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL元素類型]</td> 
   <td> <p> 選取要從HTML代碼擷取的元素類型。 </p> 
    <ul> 
     <li>[!UICONTROL影像]</li> 
     <li>[!UICONTROL連結]</li> 
     <li>[!UICONTROL iFrame元素]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROLHTML] </td> 
   <td> <p>輸入或映射要從中檢索指定元素類型的HTML代碼。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 從文字取得元素]

根據指定的模式從文本分析元素。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL輸入文本]</td> 
   <td> <p>輸入或映射要分析的文本。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL模式]</td> 
   <td> <p>選取反映要從文字剖析之元素的模式。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL忽略重複發生次數]</td> 
   <td> <p>核取此方塊可忽略重複出現的文字元素。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL HTML到文本]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROLHTML] </td> 
   <td> <p>輸入要轉換為純文字檔案的HTML代碼。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL分行符] </td> 
   <td> <p>選取新行類型（分行）。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL大寫標題]</p> </td> 
   <td> <p>啟用此選項可轉換標題標籤中括住的文字(例如 &lt;h2&gt; &lt;/h2&gt;)轉換為大寫文字。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 匹配模式]

此 [!UICONTROL 匹配模式] 模組可讓您從指定文字尋找並擷取符合搜尋模式的字串元素。 此模組使用規則運算式（也稱為regex或regexp）。

規則運算式是字元的序列，其中每個字元都是具有特殊意義的超字元，或是具有常值意義的規則字元。 這些字元和超字元可識別可用於搜尋文字的模式。 例如，如果要搜索名稱，可以設定一個規則表達式來搜索由兩個連續單片語成的模式，這兩個單詞以大寫字母開頭。 規則運算式是搜尋和操控文字的強大工具。

對規則運算式的討論不在本文的討論範圍內。 建議下列資源：

* 有關超字元的完整清單，請參見 [規則運算式](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Regular_Expressions) 在MDN網頁檔案中。
* 如需如何建立規則運算式的教學課程，建議您 [RegexOne](https://regexone.com/).
* 若要試用規則運算式，建議您 [規則運算式101](https://regex101.com/) 網站。 在左側面板中選擇ECMAScript(JavaScript)FLAVOR。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL模式] </td> 
   <td> <p>輸入規則運算式模式。 </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>範例： </b></span></span> <code>[+-]?(\d+(\.\d+)?|\.\d+)([eE][+-]?\d+)?</code> 提供的文本中提取所有數字。</p> <p>備註:  <p>該模式應在括弧中至少包含一個捕獲組 <code>()</code>. 如果模式不包含任何捕獲組，則輸出包為空。</p> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL全局匹配]</td> 
   <td> <p>啟用此選項可檢索文本中的所有匹配項。 每個匹配都以單獨的捆綁輸出。 如果此選項已停用，模組只會擷取第一個項目。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL區分大小寫]</td> 
   <td> <p> 啟用此模組的選項，將文字視為區分大小寫。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL多行] </td> 
   <td> <p>啟用此選項可確保開頭和結尾超字元(<code>^</code> 和 <code>$</code>)會比對每行的開頭或結尾，而不只是整個輸入字串的開頭或結尾。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL單行]</td> 
   <td>啟用此選項可確保期間(.) 匹配新行字元(<code>\n</code>)。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL即使模組未返回任何結果，仍繼續執行路由]</td> 
   <td> <p>啟用此選項，以確保若模組未傳回任何結果，則不會停止案例。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL文本] </td> 
   <td> <p>輸入或映射要匹配模式的文本。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 取代]

搜索輸入的文本以查找指定值或規則表達式，並將結果替換為新值。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL模式] </td> 
   <td> <p>輸入搜索詞。 您也可以使用規則運算式。 如需規則運算式的詳細資訊，請參閱 <a href="#match-pattern" class="MCXref xref">[!UICONTROL匹配模式]</a> 模組。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL新值]</td> 
   <td> <p> 輸入一個值以替換搜索詞。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL全局匹配]</td> 
   <td> <p>啟用此選項可檢索文本中的所有匹配項。 每個匹配都以單獨的捆綁輸出。 如果此選項已停用，模組只會擷取第一個項目。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL區分大小寫]</td> 
   <td> <p> 啟用此模組的選項，將文字視為區分大小寫。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL多行] </td> 
   <td> <p>啟用此選項可確保開頭和結尾超字元(<code>^</code> 和 <code>$</code>)會比對每行的開頭或結尾，而不只是整個輸入字串的開頭或結尾。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL單行]</td> 
   <td>啟用此選項可確保期間(.) 匹配新行字元(<code>\n</code>)。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL文本] </td> 
   <td> <p>輸入要搜索的文本。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 資料刮除

資料刮取（有時稱為網頁刮取、資料擷取或網頁擷取）是從網站收集資料，並儲存於您本機資料庫或試算表的程式。 如果您想從網站上消除資料，但不熟悉規則運算式，則可使用資料刮除工具：

* [Apify](https://apify.com/)
* [2019年最佳資料刮削工具](https://www.octoparse.com/blog/best-data-scraping-tools-for-2019-top-10-reviews)

如果資料刮除工具提供REST API，您可以透過我們通用的API連線 [[!UICONTROL HTTP] 模組](../../workfront-fusion/apps-and-their-modules/http-modules/http-modules-1.md) 和 [Webhook](../../workfront-fusion/apps-and-their-modules/webhooks-updated.md) 模組。
