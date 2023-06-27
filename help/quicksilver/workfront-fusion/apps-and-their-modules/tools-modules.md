---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: 工具
description: 此 [!DNL Adobe Workfront Fusion Tools] 區段包含數個可增強您情境的實用模組。
author: Becky
feature: Workfront Fusion
exl-id: 97a68fbc-1272-43fc-b4f2-4c1c9e590741
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '2290'
ht-degree: 0%

---

# [!UICONTROL 工具]

此 [!DNL Adobe Workfront Fusion Tools] 區段包含數個可增強您情境的實用模組。

[!UICONTROL 工具] 模組可從應用程式清單或以下網址取得： [!UICONTROL 工具] 圖示 ![](assets/tools-icon-small.png) 在熒幕底部。

## 存取需求

您必須具有下列存取權才能使用本文中的功能：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計劃*</td>
  <td> <p>[！UICONTROL Pro]或更高版本</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權*</td>
   <td> <p>[！UICONTROL計畫]，[！UICONTROL工作]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] 授權**</td> 
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

## [!UICONTROL 工具] 及其欄位

* [觸發器](#triggers)
* [動作](#actions)
* [彙總](#aggregators)
* [轉換器](#transformers)

### 觸發器

#### [!UICONTROL 基本觸發器]

此模組可讓您建立自訂觸發器並定義其輸入組合。

例如，您可以將此模組用於已排程傳送至指定電子郵件地址的連絡人或任何其他清單(例如 [!UICONTROL 電子郵件] >[!UICONTROL 傳送電子郵件]，或 [!DNL Gmail] >[!UICONTROL 傳送電子郵件] 模組)，或作為您想要隨時觸發的簡單提醒。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL組合]</td> 
   <td> <p>新增陣列專案以建立自訂組合。 陣列由名稱 — 值配對組成。</p> </td> 
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

此模組會擷取先前由建立的值 [!UICONTROL 設定變數] 或 [!UICONTROL 設定多個變數] 模組。

此模組可讀取在情境中任何位置設定的變數，即使變數的設定路由與以下位置不同： [!UICONTROL 取得多個變數] 找到模組。 唯一的要求是 [!UICONTROL 工具] > [!UICONTROL 設定變數] 或 [!UICONTROL 工具] > [!UICONTROL 設定多個變數] 模組是在以下專案之前執行： [!UICONTROL 工具] > [!UICONTROL 取得多個變數] 模組。 如需有關執行模組順序的詳細資訊，請參閱 [中的路由器模組 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/router-module.md).

<table style="table-layout:auto">
    <tr>
        <td>[！UICONTROL變數]</td>
        <td>新增您想要模組取得的變數。</td>
    </tr>
    <tr>
        <td>[！UICONTROL變數名稱]</td>
        <td>針對您新增的每個變數，對應您要取得之變數的名稱。</td>
    </tr>
</table>

>[!INFO]
>
>**範例：**  以下為可能的用法 [!UICONTROL 設定]/[!UICONTROL 取得（多個）變數] 模組：
>
>* 儲存計算值以供稍後使用，即使是在不同的路由中。 當值用於多個模組且用於計算值的公式過於複雜時，這個用法很有用。
>* 若要對公式進行偵錯，請執行下列動作： 如果模組中使用的公式似乎未提供正確的結果，請複製該公式並將其貼到 [!UICONTROL 設定變數] 在相關模組之前插入的模組。 在下列動作之後，中斷與模組的連線： [!UICONTROL 設定變數] 模組並執行情境。 驗證 [!UICONTROL 設定變數] 模組的輸出、調整或簡化公式、再次執行案例，並繼續執行，直到問題解決為止。


#### [!UICONTROL 取得變數]

此模組會擷取先前由建立的值 [!UICONTROL 設定變數] 或 [!UICONTROL 設定多個變數] 模組。

此模組可讀取在情境中任何位置設定的變數，即使變數的設定路由與以下位置不同： [!UICONTROL 取得變數] 找到模組。 唯一的要求是 [!UICONTROL 工具] > [!UICONTROL 設定變數] 或 [!UICONTROL 工具] > [!UICONTROL 設定多個變數] 模組是在以下專案之前執行： [!UICONTROL 工具] > [!UICONTROL 取得變數] 模組。 如需有關執行模組順序的詳細資訊，請參閱 [中的路由器模組 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/router-module.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL變數名稱]</td> 
   <td> <p>對應您希望模組取得的變數名稱。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 增量函式]

此模組會傳回每個模組運作後以1為單位遞增的值。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL重設值]</td> 
   <td> <p>選取您希望模組增加值的時間。 </p> 
    <ul> 
     <li>[！UICONTROL After one cycle]</li> 
     <li>[！UICONTROL After one scenario run]</li> 
     <li>[！UICONTROL從不]</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**範例:**
>
>此模組的其中一個用途是實作任務、銷售機會、電子郵件等的「循環配置式」指派給群組中的使用者。 演演算法會以某種合理的順序從群組選擇受指派人，通常是從清單的頂端到底部。 當演演算法到達清單結尾時，它會在清單頂端將下一個指派給使用者，並繼續進行清單底下的指派。
>
>下列案例會在每個奇數案例執行後傳送電子郵件給第一個收件者，並在每個偶數案例執行後傳送電子郵件給第二個收件者。
>
>![](assets/example-email-350x246.gif)
>
>1. 若要建立此情境：
>1. 設定模組的 **[!UICONTROL 重設值]** 欄位設為「永不」。
>1. 設定奇數的路由。 使用等於的模數數學函式設定此路由的篩選器 `1`：
>
>   ![](assets/odd-350x459.png)
>
>  **注意**：別忘了變更 [!UICONTROL 等於] 運運算元（來自預設值） [!UICONTROL 文字] 運運算元至 [!UICONTROL 數值] 運運算元。
>
>1. 使用等於的模數數學函式設定偶數值的路徑 `0`：
>
>增量函式會在每次案例執行時新增一次。 篩選器會檢查增量並根據其值採取行動，確保電子郵件平均分配。

#### [!UICONTROL 設定多個變數]

此模組會建立可由路由中其他模組對應的變數。 變數亦可對應至 [!UICONTROL 取得變數] 或 [!UICONTROL 取得多個變數] 情境中任何路由的模組。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL變數]</td> 
   <td>新增您想要模組設定的變數。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL變數名稱] </td> 
   <td>針對每個變數，輸入變數名稱。 在其他模組中對應變數時，將顯示此名稱。 </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL變數值] </td> 
   <td>針對每個變數，輸入變數的值。 </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL變數存留期] </td> 
   <td> <p>選取您希望變數維持有效時間（保留相同的值）。</p> 
    <ul> 
     <li><strong>[！UICONTROL一個週期]</strong>：變數僅對一個週期有效。 在收到一個案例執行中的多個Webhook時非常有用（更多Webhook =更多週期）。 </li> 
     <li><strong>[！UICONTROL One execution]</strong>：變數對一個案例執行有效。 一個執行可以包含一個或多個週期。</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 設定變數]

此模組會建立變數，該變數可由路由中的其他模組對應。 變數亦可對應至 [!UICONTROL 取得變數] 或 [!UICONTROL 取得多個變數] 情境中任何路由的模組。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL變數名稱] </td> 
   <td>輸入變數名稱。 在其他模組中對應變數時，將顯示此名稱。 </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL變數存留期] </td> 
   <td> <p>選取您希望變數維持有效時間（保留相同的值）。</p> 
    <ul> 
     <li><strong>[！UICONTROL一個週期]</strong>：變數僅對一個週期有效。 在收到一個案例執行中的多個Webhook時非常有用（更多Webhook =更多週期）。 </li> 
     <li><strong>[！UICONTROL One execution]</strong>：變數對一個案例執行有效。 一個執行可以包含一個或多個週期。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL變數值] </td> 
   <td>輸入或對應變數的值。 </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 睡眠]

此模組可讓您將情境流程延遲最多300秒（5分鐘）。

例如，如果您想要降低 [!DNL target] 服務伺服器載入，或在傳送大量簡訊或電子郵件時模擬人類行為。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[！UICONTROL延遲]</p> </td> 
   <td> <p>輸入案例將暫停的秒數。</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!TIP]
>
>如果您想要將流量暫停較長的一段時間，我們建議將您的案例分割為兩個案例：
>
>* 第一個案例會包含暫停前的零件。
>* 第二個案例會包含其後的零件。
>
>第一個案例最終會將所有必要資訊連同目前的時間戳記一起儲存在資料存放區中。 第二種情況會定期檢查資料存放區中時間戳記早於預期延遲的記錄、擷取記錄、完成資料的處理，並從資料存放區中移除記錄。
>
>如需資料存放區的詳細資訊，請參閱 [中的資料存放區 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/data-stores.md).
>
>如需特定資料存放區模組的詳細資訊，請參閱 [[!UICONTROL 資料存放區] 模組](../../workfront-fusion/apps-and-their-modules/data-store-modules.md).

### 彙總

* [[!UICONTROL 數值彙總]](#numeric-aggregator)
* [[!UICONTROL 表格彙總]](#table-aggregator)
* [[!UICONTROL 文字彙總]](#text-aggregator)

#### [!UICONTROL 數值彙總]

此模組可讓您擷取數值，然後套用其中一個選取的函式(SUM、AVG、COUNT、MAX、MIN)，並在一個套件中傳回結果。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[！UICONTROL來源模組]</p> </td> 
   <td> <p>選取您要從中彙總欄位的模組。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[！UICONTROL彙總函式]</p> </td> 
   <td> <p>選取您要用來彙總值的函式。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[！UICONTROL Group by]</p> </td> 
   <td> <p>定義要將彙總輸出分組依據的運算式。 此運算式可包含一或多個對應專案。 然後使用此運算式的值將彙總的資料分隔成群組。 每個群組都會輸出為個別的組合，並附有索引鍵（運算式）和值（彙總值）。 您可以在後續模組中將該索引鍵當作篩選條件使用。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL在空白彙總後停止處理]</td> 
   <td>啟用此選項可在沒有結果時停止情境。</td> 
  </tr> 
  <tr> 
   <td> <p>[！UICONTROL值]</p> </td> 
   <td> <p>輸入或對應您要彙總的值。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 表格彙總]

此模組會使用指定的欄和列分隔符號（可讓您建立表格），將所接收資料包的所選欄位中的值合併到單一資料包中。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[！UICONTROL來源模組]</p> </td> 
   <td> <p>選取您要從中彙總欄位的模組。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL彙總欄位]</td> 
   <td> <p> 從上面選取的模組中選取包含您要彙總至一個組合中的值的欄位。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[！UICONTROL欄分隔符號]</p> </td> 
   <td> <p>選取或輸入將分隔結果束中欄位值欄的分隔符號型別。 如果您選取[！UICONTROL其他]，請在分隔符號欄位中輸入用來分隔值的字元。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[！UICONTROL列分隔符號]</p> </td> 
   <td> <p>選取或輸入將分隔結果束中欄位值列的分隔符號型別。 如果您選取[！UICONTROL其他]，請在分隔符號欄位中輸入用來分隔值的字元。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[！UICONTROL Group by]</p> </td> 
   <td> <p>定義要將彙總輸出分組依據的運算式。 此運算式可包含一或多個對應專案。 之後，會使用此運算式的值將彙總的資料分隔成群組。 每個群組都會輸出為個別的組合，並附有索引鍵（運算式）和值（彙總值）。 您可以在後續模組中將該索引鍵當作篩選條件使用。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL在空白彙總後停止處理]</td> 
   <td>選取此選項可在沒有結果時停止情境。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 文字彙總]

此模組將來自所接收套裝的選定欄位的值合併至單一套裝。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[！UICONTROL來源模組]</p> </td> 
   <td> <p>選取您要從中彙總欄位的模組。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[！UICONTROL列分隔符號]</p> </td> 
   <td> <p>選取或輸入將分隔結果束中欄位值列的分隔符號型別。 如果您選取[！UICONTROL其他]，請在分隔符號欄位中輸入用來分隔值的字元。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[！UICONTROL Group by]</p> </td> 
   <td> <p>定義包含一或多個對應專案的運算式。 使用相同運算式的值在「群組」底下分隔彙總的資料。 每個群組都會輸出為單獨的組合，其中包含具有評估運算式和彙總文字的索引鍵。 透過這樣做，您可以在後續模組中將該索引鍵當作篩選條件使用。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL文字]</td> 
   <td> <p> 輸入或對應您要模組彙總的文字。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL在空白彙總後停止處理]</td> 
   <td>選取此選項可在沒有結果時停止情境。</td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**範例：** 您可以使用文字彙總將更多值（例如客戶名稱或附註）插入單一套件組合中，並傳送包含電子郵件內文或電子郵件主旨中所有值的電子郵件。

### 轉換器

* [[!UICONTROL 撰寫字串]](#compose-a-string)
* [[!UICONTROL 轉換文字的編碼]](#convert-the-encoding-of-the-text)
* [[!UICONTROL 切換]](#switch)

#### [!UICONTROL 撰寫字串]

將任何值轉換為字串資料型別（文字）。 對應時（例如二進位資料），可讓對應更容易。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL文字]</td> 
   <td> <p>輸入或對應您要轉換為文字的資料。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 轉換文字的編碼]

將輸入的輸入文字（或二進位資料）轉換為選取的編碼。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[！UICONTROL輸入資料]</p> </td> 
   <td> <p>輸入或對應您要轉換的內容。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL Input data codepage]</td> 
   <td> <p>選取輸入資料的編碼型別。 </p> </td> 
  </tr> 
  <tr> 
   <td> <p>[！UICONTROL Output data codepage]</p> </td> 
   <td> <p>選取目標（輸出）資料的編碼型別。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 切換]

檢查輸入值，找出與提供的值清單相符的專案。 根據結果傳回輸出。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[！UICONTROL輸入]</p> </td> 
   <td> <p>輸入您要計算的運算式。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL使用規則運算式來比對]</td> 
   <td> <p>啟用此選項以使用規則運算式。 模組會根據規則運算式來判斷案例，而非完全相符。</p> 
    <div> 
     <p>規則運算式是字元序列，其中每個字元都是具有特殊含義的中繼字元，或是具有常值含義的規則字元。 這些字元和中繼字元會識別可用來搜尋文字的模式。 例如，如果您想要搜尋名稱，可以設定規則運算式來搜尋由兩個以大寫字母開頭的連續字片語成的模式。 規則運算式是搜尋和處理文字的強大工具。</p> 
     <p>有關規則運算式的討論不在本文的討論範圍內。 我們建議使用下列資源：</p> 
     <ul> 
      <li>如需中繼字元的完整清單，請參閱 <a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Regular_Expressions">規則運算式</a> 在MDN網頁檔案中。</li> 
      <li>如需如何建立規則運算式的教學課程，我們建議 <a href="https://regexone.com/">Regexone</a>.</li> 
      <li>若要實驗規則運算式，我們建議 <a href="https://regex101.com/">規則運算式101</a> 網站。 在左側面板中選取ECMAScript (JavaScript) FLAVOR。</li> 
     </ul> 
    </div> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL大小寫] </td> 
   <td> <p>如果輸入包含輸入到[！UICONTROL模式]欄位的值，則會傳回輸入到[！UICONTROL輸出]欄位的值。</p> <p>如果輸入不符合您在[！UICONTROL模式]欄位中設定的任何值，則會發生下列其中一種情況：</p> 
    <ul> 
     <li>傳回[！UICONTROL Else]欄位的值</li> 
     <li>如果[！UICONTROL Else]欄位中沒有值，則不會傳回任何輸出。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td> <p>[！UICONTROL Else]</p> </td> 
   <td> <p>輸入當不符合案例欄位中設定的條件時傳回的值。 </p> </td> 
  </tr> 
 </tbody> 
</table>
