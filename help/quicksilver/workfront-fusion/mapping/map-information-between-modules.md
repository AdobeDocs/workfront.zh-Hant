---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: mapping
title: 在 [!DNL Adobe Workfront Fusion]中將資訊從一個模組對應到另一個模組
description: Adobe Workfront Fusion檔案已移至新位置。 本文已棄用，但包含新文章的連結，內容涵蓋此功能。
author: Becky
feature: Workfront Fusion
exl-id: e8d619e9-6425-4136-ac71-47d979d68a2d
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '1628'
ht-degree: 0%

---

# 在[!DNL Adobe Workfront Fusion]中將資訊從一個模組對應到另一個模組

>[!IMPORTANT]
>
>Adobe Workfront Fusion檔案已移至新位置。
>
>本文資訊可在以下文章中找到：
>
>* [將資訊從一個模組對應到另一個模組](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/map-data/map-data-from-one-to-another.html)
>
>請更新任何書籤。
>
>本文已不再更新，將於不久將來移除。

對應是將模組的輸出（結構化為專案）指派給其他模組的輸入欄位的程式。

當您按一下要插入從案例中前一個模組輸出的值的欄位時，對應面板便會顯示。 在模組內，在任何可用於對應的欄位中，您可以使用對應面板中的函式和對應專案的任何組合，以及您鍵入的靜態文字來建立公式。 這些元素可以彼此巢狀內嵌。

## 存取需求

您必須具有下列存取權才能使用本文中的功能：

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] 計畫*</td> 
   <td> <p>[!DNL Pro] 或更高</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權*</td> 
   <td> <p>[！UICONTROL計畫]，[！UICONTROL工作]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Adobe Workfront Fusion]授權**</td> 
   <td>
   <p>目前授權需求：無[!DNL Workfront Fusion]授權需求。</p>
   <p>或</p>
   <p>舊版授權需求：[！UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>
   <p>目前產品需求：如果您有[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Adobe Workfront]計畫，您的組織必須購買[!DNL Adobe Workfront Fusion]及[!DNL Adobe Workfront]，才能使用本文所述的功能。 [!DNL Workfront Fusion]包含在[！UICONTROL Ultimate] [!DNL Workfront]計畫中。</p>
   <p>或</p>
   <p>舊版產品需求：您的組織必須購買[!DNL Adobe Workfront Fusion]及[!DNL Adobe Workfront]，才能使用本文所述的功能。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的[!DNL Workfront]管理員。

如需[!DNL Adobe Workfront Fusion]授權的相關資訊，請參閱[[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md)。

## 套件組合和專案

模組的操作會產生零、一或多個套件組合作為其輸出。 組合包含一或多個專案。

若要探索模組的輸出：

1. 按一下&#x200B;**[!UICONTROL 執行一次]**&#x200B;以執行模組。
1. 按一下模組上方的泡泡。

   包含模組所有階段的記錄檔隨即顯示。 您可以在&#x200B;**[!UICONTROL 輸出]**&#x200B;標題下找到模組作業階段輸出的組合或組合。 每個束都包含其專案和每個專案的值。

>[!INFO]
>
>**範例：**&#x200B;此範例顯示模組[!UICONTROL 電子郵件] > [!UICONTROL 觀看電子郵件]。 您可以看到它執行了1個作業，產生包含各種專案（例如`Date`、`Email ID (UID)`、`size`等）的單一組合。
>
>![](assets/watch-emails-350x298.png)

>[!NOTE]
>
>封裝在[!UICONTROL 疊代器]和[!UICONTROL 彙總]之間的模組的輸出無法在[!UICONTROL 彙總]模組之外存取。

## 對應專案

當您連結兩個或多個模組來建立一系列模組後，每個模組都可以處理其前面的模組所輸出的專案值。

若要將專案指派給模組的輸入欄位：

1. 按一下應處理先前一個或多個模組輸出的模組。
1. 在顯示的「模組設定」面板中，按一下您要使用先前模組輸出之專案值的欄位。

   對應面板隨即開啟。

1. 按一下對應面板中的專案以將其插入欄位中。
1. （可選）若要搜尋對應面板中的特定欄位，請按一下對應面板搜尋列，然後輸入您要搜尋的字詞。 當欄位出現在清單中時，按一下該欄位。

   搜尋結果包含搜尋字詞，且不區分大小寫。

如需詳細資訊，請參閱[在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/configure-a-modules-settings.md)中設定模組的設定。

## 公式

您可以將多個專案對應到一個欄位中，將它們與常值（固定值）結合，然後使用運運算元和函式來建立複雜的公式：

![](assets/operators-and-functions.png)

您可以在對應面板的其中一個標籤下找到函式和運運算元。

![](assets/functions-toolbar-350x189.png)

第一個標籤![](assets/toolbar-icon-functions-you-map-from-other-modules.png) （在開啟面板時顯示）會顯示您可以從其他模組對應的專案。

其他標籤包含下列型別的函式：

* **一般函式** ![](assets/toolbar-icon-general-function.png) — 如需詳細資訊，請參閱 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/general-functions.md)中的[一般函式。

* **數學函式** ![](assets/toolbar-icon-math-functions.png) — 如需詳細資訊，請參閱 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/math-functions.md)中的[數學函式。

* **文字和二進位函式** ![](assets/toolbar-icon-text&binary-functions.png) — 如需詳細資訊，請參閱 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/string-functions.md)中的[字串函式。

* **日期與時間** ![](assets/toolbar-icon-date&time-functions.png) — 如需詳細資訊，請參閱 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/date-and-time-functions.md)中的[日期與時間函式，以及下列文章。

   * [ [!DNL Adobe Workfront Fusion]中日期和時間格式的Token](../../workfront-fusion/functions/tokens-for-date-and-time-formatting.md)
   * [Adobe Workfront Fusion中日期和時間剖析的權杖](../../workfront-fusion/functions/tokens-for-date-and-time-parsing.md)

* **使用陣列的函式** ![](assets/toolbar-icon-functions-for-arrays.png) — 如需詳細資訊，請參閱 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/array-functions.md)中的[陣列函式。

>[!TIP]
>
>當您建立要在其他欄位中重複使用的複雜公式時，可以按一下包含組合的欄位，使用Command-A或Ctrl-A來選取它，然後將其複製並貼到其他欄位中。

如需有關使用函式對應專案的詳細資訊，請參閱[在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/map-using-functions.md)中使用函式對應專案。

## 集合

有些專案可以包含多種型別的多個值。 這些是集合型別專案。

您可以透過專案標籤右側顯示的黑色小矩形及其自動展開的子專案清單來識別[!UICONTROL 集合]型別專案：

![](assets/collection.png)

>[!NOTE]
>
>在大多數情況下，會對映集合的子專案，而非代表整個集合的專案。

如需集合的詳細資訊，請參閱[!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/mapping/item-data-types.md)中的[專案資料型別

## 陣列

某些專案可以包含相同型別的多個元素。 這些是陣列型別專案。

您可以藉由專案標籤結尾的方括弧來識別陣列型別專案。 按一下專案標籤右側的黑色小矩形，以顯示專案的專案：

![](assets/array.png)

如需有關陣列的詳細資訊，請參閱 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/item-data-types.md)中的[專案資料型別

### 對應陣列的第一個元素

如果您對應陣列的`Recipient name`專案，它會顯示在「 」欄位中，如下所示：

![](assets/map-array-1st-element.png)

方括弧中的數字是決定要使用陣列中哪個元素的索引。 預設為1。

### 對應陣列的第n個元素

如果您想要存取其他元素，請按一下方括弧並編輯索引值：

![](assets/access-another-element.png)

### 使用指定索引鍵對應陣列的元素

某些陣列包含數個具有索引鍵和值專案的集合。 這些通常是各種中繼資料、屬性等。

下列範例顯示[!DNL Jira]應用程式的輸出。

![](assets/output-of-jira-app-350x100.png)

在此範例中，我們會從ID為10108的特定附件的附件陣列中取得檔案名稱。

來自[!DNL Jira]的輸出如下所示：

![](assets/output-from-jira-350x261.png)

一般的要求是根據元素的指定索引鍵值來尋找元素，並從值專案中取得對應的值。 這可以用採用`map()`和`get()`函式組合的公式來達成。

以下是公式的詳細劃分：

1. `map()`函式的第一個引數是整個陣列專案。
1. 第二個引數是值專案的原始名稱。 若要取得原始名稱，請將游標停留在[!UICONTROL 對應]面板中的專案上：

   ![](assets/obtain-raw-name-350x124.png)

   >[!NOTE]
   >
   >所有引數都區分大小寫。 即使在此特定範例中，專案的標籤與只有大寫的原始名稱不同，仍有必要使用原始名稱，這是與標籤Value相反的所有小寫值。

1. 第三個引數是關鍵專案的原始名稱：

   ![](assets/3rd-parameter-350x166.png)

1. 第4個引數是指定的機碼值。

由於`map()`函式傳回陣列（因為可能有更多具有指定索引鍵值的元素），所以必須套用`get()`函式才能取得其第一個元素：

* `get()`函式的第1個引數是`map()`函式的結果。

* 第二個引數是元素的索引 — 一個。

如需`map()`函式的詳細資訊，請參閱 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/array-functions.md)中的[陣列函式。

如需`get()`函式的詳細資訊，請參閱 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/general-functions.md)中的[一般函式。

## 將元素轉換為一系列組合

可以使用[!UICONTROL 疊代器]模組將陣列轉換為一系列組合。 如需詳細資訊，請參閱[!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/modules/iterator-module.md)中的[[!UICONTROL 迭代器]模組。

![](assets/series-of-bundles-350x169.png)

## 疑難排解

### 對應面板中缺少專案

對於每個模組，對應面板會顯示所有輸出專案，由模組的作者列出。 在某些情況下，由於各種原因，此清單可能不完整，並且可能缺少某些專案。 當您在案例編輯器中執行模組時，[!DNL Workfront Fusion]可以自動探索遺漏的輸出專案。 確切的程式會因模組的型別而稍有不同：

#### 即時觸發

1. 在模組上按一下滑鼠右鍵，然後在顯示的功能表中按一下&#x200B;**[!UICONTROL 僅執行此模組]**。

   如果沒有已排入佇列的Webhook，模組會等待新的Webhook處理。

1. 產生webhook。

   例如，webhook模組&#x200B;**[!DNL Slack]>[!UICONTROL 聆聽新事件]** （會觀看頻道中的新頻道訊息）傳送訊息至頻道。

1. 當模組完成執行時，按一下模組上方的泡泡圖示，以探索其完整輸出。

   對應面板將包含在模組輸出中發現的所有專案。

#### 輪詢觸發程式

1. 在模組上按一下滑鼠右鍵，然後在顯示的功能表中按一下&#x200B;**[!UICONTROL 僅執行此模組]**。
1. 如果沒有輸出，請按一下&#x200B;**[!UICONTROL 選擇開始位置]**&#x200B;並調整設定。
1. 如果沒有要處理的事件，請建立一個事件並返回步驟2。

   例如，webhook模組&#x200B;**[!UICONTROL Gmail] >[!UICONTROL 觀看電子郵件]**&#x200B;傳送電子郵件至模組正在觀看的資料夾。

1. 當模組完成執行時，按一下模組上方的泡泡圖示，以探索其完整輸出。

   對應面板現在包含模組輸出中探索到的所有專案。

#### 其他模組

您可以選擇執行：

* 整個情境（或僅包含模組的部分）

  如果您的案例以觸發程式開始，請參閱上面的[立即觸發程式](#instant-trigger)或[輪詢觸發程式](#polling-trigger)區段。

* 只有單一模組

如果您選擇只執行單一模組：

1. 在模組上按一下滑鼠右鍵，然後在顯示的功能表中按一下&#x200B;**[!UICONTROL [僅執行此模組]]**。
1. 提供輸入專案的範例值，然後按一下&#x200B;**[!UICONTROL 確定]** 。
1. 當模組完成執行時，按一下模組上方的泡泡圖示，以探索其完整輸出。

   對應面板現在包含模組輸出中探索到的所有專案。
