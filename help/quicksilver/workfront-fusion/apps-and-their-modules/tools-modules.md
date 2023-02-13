---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: 工具
description: 此 [!DNL Adobe Workfront Fusion Tools] 小節包含數個可增強案例的實用模組。
author: Becky
feature: Workfront Fusion
exl-id: 97a68fbc-1272-43fc-b4f2-4c1c9e590741
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '2246'
ht-degree: 0%

---

# [!UICONTROL 工具]

此 [!DNL Adobe Workfront Fusion Tools] 小節包含數個可增強案例的實用模組。

[!UICONTROL 工具] 模組可從應用程式清單或 [!UICONTROL 工具] 圖示 ![](assets/tools-icon-small.png) 在螢幕底部。

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] （工作自動化和整合） </p> <p>[!UICONTROL [!DNL Workfront Fusion] （工作自動化） </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>貴組織必須購買 [!DNL Adobe Workfront Fusion] 和 [!DNL Adobe Workfront] 以使用本文所述的功能。</td> 
  </tr>
 </tbody> 
</table>

若要了解您擁有的計畫、授權類型或存取權，請聯絡您的 [!DNL Workfront] 管理員。

如需 [!DNL Adobe Workfront Fusion] 許可證，請參閱 [[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!UICONTROL 工具] 和田地

* [觸發器](#triggers)
* [動作](#actions)
* [匯總器](#aggregators)
* [變形金剛](#transformers)

### 觸發器

#### [!UICONTROL 基本觸發]

此模組可讓您建立自訂觸發程式並定義其輸入套件組合。

例如，您可以將此模組用於聯繫人，或計畫發送到指定電子郵件地址的任何其他清單(如 [!UICONTROL 電子郵件] >[!UICONTROL 傳送電子郵件]，或 [!DNL Gmail] >[!UICONTROL 傳送電子郵件] 模組)，或作為簡單提醒，可隨時觸發。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL套件]</td> 
   <td> <p>透過新增陣列項目來建立自訂套件組合。 陣列由名稱 — 值組組成。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 動作

* [[!UICONTROL 取得多個變數]](#get-multiple-variables)
* [[!UICONTROL 取得變數]](#get-variable)
* [[!UICONTROL 增量函式]](#increment-function)
* [[!UICONTROL 設定多個變數]](#set-multiple-variables)
* [[!UICONTROL 設定變數]](#set-variable)
* [[!UICONTROL 睡眠]](#sleep)

#### [!UICONTROL 取得多個變數]

此模組會擷取先前由 [!UICONTROL 設定變數] 或 [!UICONTROL 設定多個變數] 模組。

此模組可讀取在案例中任何位置設定的變數，即使變數的設定路徑與 [!UICONTROL 取得多個變數] 模組的位置。 唯一的要求是 [!UICONTROL 工具] > [!UICONTROL 設定變數] 或 [!UICONTROL 工具] > [!UICONTROL 設定多個變數] 模組在 [!UICONTROL 工具] > [!UICONTROL 取得多個變數] 模組。 如需模組執行順序的詳細資訊，請參閱 [路由器模組 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/router-module.md).

<table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL變數]</td>
        <td>新增您要模組取得的變數。</td>
    </tr>
    <tr>
        <td>[!UICONTROL變數名稱]</td>
        <td>對於您新增的每個變數，對應您要取得的變數名稱。</td>
    </tr>
</table>

>[!INFO]
>
>**範例：**  以下是 [!UICONTROL 設定]/[!UICONTROL 取得（多個）變數] 模組：
>
>* 儲存計算值以供稍後使用，即使在不同路由中亦然。 當值用於多個模組，且計算值的公式過於複雜時，這個用法很有用。
>* 調試公式。 如果模組中使用的公式似乎未提供正確的結果，請複製公式並貼到 [!UICONTROL 設定變數] 在相關模組之前插入的模組。 在 [!UICONTROL 設定變數] 模組並執行案例。 驗證 [!UICONTROL 設定變數] 模組的輸出、調整或簡化公式、再次執行情境，並繼續執行，直到問題解決為止。



#### [!UICONTROL 取得變數]

此模組會擷取先前由 [!UICONTROL 設定變數] 或 [!UICONTROL 設定多個變數] 模組。

此模組可讀取在案例中任何位置設定的變數，即使變數的設定路徑與 [!UICONTROL 取得變數] 模組的位置。 唯一的要求是 [!UICONTROL 工具] > [!UICONTROL 設定變數] 或 [!UICONTROL 工具] > [!UICONTROL 設定多個變數] 模組在 [!UICONTROL 工具] > [!UICONTROL 取得變數] 模組。 如需模組執行順序的詳細資訊，請參閱 [路由器模組 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/router-module.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL變數名稱]</td> 
   <td> <p>對應您要模組取得的變數名稱。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 增量函式]

此模組會傳回在每個模組執行作業後以1為單位遞增的值。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL重置值]</td> 
   <td> <p>選取何時要讓模組增加值。 </p> 
    <ul> 
     <li>[!UICONTROL在一個循環後]</li> 
     <li>[!UICONTROL在一個方案運行後]</li> 
     <li>[!UICONTROL從不]</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**範例:**
>
>模組的用途之一，是對群組中的使用者實作任務、銷售機會、電子郵件等的「循環」指派。 演算法會以合理順序從群組中選擇受指派者，通常從清單的頂端到底部。 當演算法達到清單結尾時，它會將下一個指派給清單頂端的使用者，並繼續在清單下進行指派。
>
>以下情形會在每次奇數方案執行後傳送電子郵件給第一個收件者，並在每次偶數方案執行後傳送電子郵件給第二個收件者。
>
>![](assets/example-email-350x246.gif)
>
>1. 若要建立此案例：
>1. 設定模組的 **[!UICONTROL 重設值]** 欄位為「永不」。
>1. 為奇數值設定路由。 使用等於的模數數學函式設定此路由的篩選器 `1`:

>
>   ![](assets/odd-350x459.png)
>
>  **附註**:別忘了變更 [!UICONTROL 等於] 運算子 [!UICONTROL 文字] 運算子 [!UICONTROL 數值] 運算元。
>
>1. 使用等於的模數數學函式設定偶數值的路由 `0`:
>
>每次執行案例時，增量函式會新增一個。 篩選器會檢查增量並對其值採取行動，確保電子郵件均勻分佈。

#### [!UICONTROL 設定多個變數]

此模組會建立可由路由中的其他模組映射的變數。 變數也可對應至 [!UICONTROL 取得變數] 或 [!UICONTROL 取得多個變數] 方案中任何路由的模組。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL變數]</td> 
   <td>新增您要模組設定的變數。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL變數名稱] </td> 
   <td>為每個變數輸入變數名稱。 在其他模組中對應變數時，將顯示此名稱。 </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL變數值] </td> 
   <td>對於每個變數，輸入變數的值。 </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL變數期限] </td> 
   <td> <p>選取要讓變數維持有效的時間（保留相同的值）。</p> 
    <ul> 
     <li><strong>[!UICONTROL單週期]</strong>:變數對一個循環有效。 當收到一個案例執行中的多個Webhook時非常有用（更多Webhook =更多週期）。 </li> 
     <li><strong>[!UICONTROL One Execution]</strong>:變數對一個案例執行有效。 一個執行可包含一或多個週期。</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 設定變數]

此模組會建立一個變數，該變數可由路由中的其他模組映射。 變數也可對應至 [!UICONTROL 取得變數] 或 [!UICONTROL 取得多個變數] 方案中任何路由的模組。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL變數名稱] </td> 
   <td>輸入變數名稱。 在其他模組中對應變數時，將顯示此名稱。 </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL變數期限] </td> 
   <td> <p>選取要讓變數維持有效的時間（保留相同的值）。</p> 
    <ul> 
     <li><strong>[!UICONTROL單週期]</strong>:變數對一個循環有效。 當收到一個案例執行中的多個Webhook時非常有用（更多Webhook =更多週期）。 </li> 
     <li><strong>[!UICONTROL One Execution]</strong>:變數對一個案例執行有效。 一個執行可包含一或多個週期。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL變數值] </td> 
   <td>輸入或對應變數的值。 </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 睡眠]

此模組可讓您將案例流程延遲最多300秒（5分鐘）。

例如，如果您想要降低 [!DNL target] 在傳送大量簡訊或電子郵件時，服務伺服器載入或模擬人的行為。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!UICONTROL延遲]</p> </td> 
   <td> <p>輸入方案將暫停的秒數。</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!TIP]
>
>如果您想要將流程暫停較長的時間，建議您將案例分割為兩個案例：
>
>* 第一個案例會包含暫停前的部分。
>* 第二種情況會包含後面的部分。
>
>第一種情況最終會將所有必要資訊連同當前時間戳一起儲存在資料儲存中。 第二個方案將定期檢查資料儲存中是否有時間戳早於預定延遲的記錄，檢索記錄，完成資料的處理並從資料儲存中刪除記錄。
>
>如需資料存放區的詳細資訊，請參閱 [資料儲存於 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/data-stores.md).
>
>如需特定資料儲存模組的詳細資訊，請參閱 [[!UICONTROL 資料儲存] 模組](../../workfront-fusion/apps-and-their-modules/data-store-modules.md).

### 匯總器

* [[!UICONTROL 數值匯總器]](#numeric-aggregator)
* [[!UICONTROL 表聚合器]](#table-aggregator)
* [[!UICONTROL 文字彙總器]](#text-aggregator)

#### [!UICONTROL 數值匯總器]

此模組可讓您擷取數值，然後套用其中一個選取的函式(SUM、AVG、COUNT、MAX、MIN)，並將結果傳回至一個套件中。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!UICONTROL源模組]</p> </td> 
   <td> <p>選取要匯總欄位的模組。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL聚合函式]</p> </td> 
   <td> <p>選取您要用來匯總值的函式。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL組依據]</p> </td> 
   <td> <p>定義要將匯總輸出分組的表達式。 此運算式可包含一或多個已對應項目。 然後，使用此運算式的值將匯總的資料分成群組。 每個群組會以獨立套件的形式輸出，其中包含鍵值（評估的運算式）和值（匯總值）。 您可以在後續模組中將索引鍵當作篩選器。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL在空聚合後停止處理]</td> 
   <td>啟用此選項可在沒有結果時停止方案。</td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL值]</p> </td> 
   <td> <p>輸入或映射要匯總的值。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 表聚合器]

此模組使用指定的列和行分隔符（允許您建立表）將接收包的選定欄位中的值合併到單個包中。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!UICONTROL源模組]</p> </td> 
   <td> <p>選取要匯總欄位的模組。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL聚合欄位]</td> 
   <td> <p> 從上方選取的模組中選取欄位，其中包含您要匯總至單一套件組合的值。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL列分隔符]</p> </td> 
   <td> <p>選擇或輸入分隔符類型，該分隔符將分隔生成的包中的欄位值列。 如果選擇[!UICONTROL其他]，請在分隔符欄位中輸入要用來分隔值的字元。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL行分隔符]</p> </td> 
   <td> <p>選擇或輸入分隔符類型，該分隔符將分隔生成的包中的欄位值行。 如果選擇[!UICONTROL其他]，請在分隔符欄位中輸入要用來分隔值的字元。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL組依據]</p> </td> 
   <td> <p>定義要將匯總輸出分組的表達式。 此運算式可包含一或多個已對應項目。 然後，使用此運算式的值，將匯總的資料分組。 每個群組會以獨立套件的形式輸出，其中包含鍵值（評估的運算式）和值（匯總值）。 您可以在後續模組中將索引鍵當作篩選器。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL在空聚合後停止處理]</td> 
   <td>選取此選項，在沒有結果時停止方案。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 文字彙總器]

此模組將接收套件組合的選定欄位中的值合併到單個套件組合中。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!UICONTROL源模組]</p> </td> 
   <td> <p>選取要匯總欄位的模組。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL行分隔符]</p> </td> 
   <td> <p>選擇或輸入分隔符類型，該分隔符將分隔生成的包中的欄位值行。 如果選擇[!UICONTROL其他]，請在分隔符欄位中輸入要用來分隔值的字元。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL組依據]</p> </td> 
   <td> <p>定義包含一或多個已對應項目的運算式。 匯總的資料在具有相同運算式值的「群組」下分隔。 每個組輸出為一個單獨的包，包含一個鍵，其中包含已評估的表達式和聚合文本。 執行此操作後，您就可以在後續模組中使用索引鍵作為篩選器。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL文本]</td> 
   <td> <p> 輸入或對應您要模組匯總的文字。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL在空聚合後停止處理]</td> 
   <td>選取此選項，在沒有結果時停止方案。</td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**範例：** 您可以使用文字彙總器將更多值（例如客戶名稱或附註）插入單一套件，並傳送包含電子郵件內文或電子郵件主旨中所有值的電子郵件。

### 變形金剛

* [[!UICONTROL 撰寫字串]](#compose-a-string)
* [[!UICONTROL 轉換文字的編碼]](#convert-the-encoding-of-the-text)
* [[!UICONTROL 交換機]](#switch)

#### [!UICONTROL 撰寫字串]

將任何值轉換為字串資料類型（文字）。 這可讓對應更輕鬆，例如二進位資料。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL文本]</td> 
   <td> <p>輸入或映射要轉換為文本的資料。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 轉換文字的編碼]

將輸入的輸入文本（或二進位資料）轉換為所選編碼。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!UICONTROL輸入資料]</p> </td> 
   <td> <p>輸入或對應您要轉換的內容。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL輸入資料代碼頁]</td> 
   <td> <p>選取輸入資料的編碼類型。 </p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL輸出資料代碼頁]</p> </td> 
   <td> <p>選取目標（輸出）資料的編碼類型。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 交換機]

檢查輸入值是否與提供的值清單匹配。 根據結果傳回輸出。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!UICONTROL輸入]</p> </td> 
   <td> <p>輸入要評估的表達式。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL使用規則運算式來比對]</td> 
   <td> <p>啟用此選項可使用規則運算式。 模組會根據規則運算式來判斷大小寫，而非完全相符。</p> 
    <div> 
     <p>規則運算式是字元的序列，其中每個字元都是具有特殊意義的超字元，或是具有常值意義的規則字元。 這些字元和超字元可識別可用於搜尋文字的模式。 例如，如果要搜索名稱，可以設定一個規則表達式來搜索由兩個連續單片語成的模式，這兩個單詞以大寫字母開頭。 規則運算式是搜尋和操控文字的強大工具。</p> 
     <p>對規則運算式的討論不在本文的討論範圍內。 建議下列資源：</p> 
     <ul> 
      <li>有關超字元的完整清單，請參見 <a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Regular_Expressions">規則運算式</a> 在MDN網頁檔案中。</li> 
      <li>如需如何建立規則運算式的教學課程，建議您 <a href="https://regexone.com/">RegexOne</a>.</li> 
      <li>若要試用規則運算式，建議您 <a href="https://regex101.com/">規則運算式101</a> 網站。 在左側面板中選擇ECMAScript(JavaScript)FLAVOR。</li> 
     </ul> 
    </div> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL案例] </td> 
   <td> <p>如果輸入包含輸入到[!UICONTROL模式]欄位的值，則返回輸入到[!UICONTROL輸出]欄位的值。</p> <p>如果輸入與您在[!UICONTROL模式]欄位中設定的任何值不匹配，則會發生以下情況之一：</p> 
    <ul> 
     <li>系統會傳回[!UICONTROL Else]欄位的值</li> 
     <li>如果[!UICONTROL Else]欄位中沒有值，則不返回任何輸出。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Else]</p> </td> 
   <td> <p>輸入在「案例」欄位中設定的條件不符合時傳回的值。 </p> </td> 
  </tr> 
 </tbody> 
</table>
