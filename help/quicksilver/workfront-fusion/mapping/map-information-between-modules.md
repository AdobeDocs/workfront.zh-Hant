---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: mapping
title: 將資訊從一個模組對應到 [!DNL Adobe Workfront Fusion]
description: 映射是將模組的輸出（結構化為項）分配給其他模組的輸入欄位的過程。
author: Becky
feature: Workfront Fusion
exl-id: e8d619e9-6425-4136-ac71-47d979d68a2d
source-git-commit: 97f91d663df86341a079894cff04d07c18b7bf08
workflow-type: tm+mt
source-wordcount: '1515'
ht-degree: 0%

---

# 將資訊從一個模組對應到 [!DNL Adobe Workfront Fusion]

映射是將模組的輸出（結構化為項）分配給其他模組的輸入欄位的過程。

當您按一下要在情境中插入從前一個模組輸出的值的欄位時，會顯示對應面板。 在模組內，在可用於映射的任何欄位中，可以使用映射面板中的函式和映射項的任意組合以及鍵入的靜態文本來建立公式。 這些元素可相互巢狀內。

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] （工作自動化和整合） </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>貴組織必須購買 [!DNL Adobe Workfront Fusion] 和 [!DNL Adobe Workfront] 以使用本文所述的功能。</td> 
  </tr> 
 </tbody> 
</table>

若要了解您擁有的計畫、授權類型或存取權，請聯絡您的 [!DNL Workfront] 管理員。

如需 [!DNL Adobe Workfront Fusion] 許可證，請參閱 [[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 套件和項目

模組的操作將生成零、一個或多個包作為其輸出。 套件組合包含一或多個項目。

要探索模組的輸出，請執行以下操作：

1. 按一下 **[!UICONTROL 執行一次]** 來執行模組。
1. 按一下模組上方的泡泡。

   隨即顯示包含模組所有階段的記錄。 您可以在 **[!UICONTROL 輸出]** 標題。 每個套件都包含其項目和每個項目的值。

>[!INFO]
>
>**範例：** 此範例顯示模組 [!UICONTROL 電子郵件] > [!UICONTROL 觀看電子郵件]. 您可以看到，它執行了1項操作，產生包含各種項目的單一套件組合，例如 `Date`, `Email ID (UID)`, `size`等。
>
>![](assets/watch-emails-350x298.png)

>[!NOTE]
>
>包在 [!UICONTROL 迭代器] 和 [!UICONTROL 匯總器] 無法存取 [!UICONTROL 匯總器] 模組。

## 對應項目

在您建立了一系列模組後，通過連結其中的兩個或多個模組，每個模組都可以處理前面模組輸出的項的值。

要將項目分配給模組的輸入欄位，請執行以下操作：

1. 按一下應處理前一模組或模組輸出的模組。
1. 在顯示的「模組設定」面板中，按一下您要使用前一個模組輸出項目值的欄位。

   「對應」面板隨即開啟。

1. 從對應面板按一下項目，將其插入欄位中。
1. （可選）要在映射面板中搜索特定欄位，請按一下映射面板搜索欄，然後鍵入要搜索的詞。 當欄位出現在清單中時，按一下該欄位。

   搜尋結果包含搜尋詞，且不區分大小寫。

如需詳細資訊，請參閱 [在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/configure-a-modules-settings.md).

## 公式

您可以將多個項目映射到一個欄位，將它們與文字（固定值）結合，然後使用運算子和函式來構建複雜的公式：

![](assets/operators-and-functions-350x187.png)

您可以在對應面板的其中一個索引標籤下找到函式和運算子。

![](assets/functions-toolbar-350x189.png)

第一個標籤 ![](assets/toolbar-icon-functions-you-map-from-other-modules.png) （在開啟面板時顯示）會顯示您可從其他模組對應的項目。

其他索引標籤包含下列類型的函式：

* **一般函式** ![](assets/toolbar-icon-general-function.png)  — 請參閱 [中的一般函式 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/general-functions.md) 以取得更多資訊。

* **數學函式** ![](assets/toolbar-icon-math-functions.png)  — 請參閱 [中的數學函式 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/math-functions.md) 以取得更多資訊。

* **文本和二進位函式** ![](assets/toolbar-icon-text&binary-functions.png)  — 請參閱 [中的字串函式 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/string-functions.md) 以取得更多資訊。

* **日期和時間** ![](assets/toolbar-icon-date&time-functions.png)  — 請參閱 [日期和時間函式，於 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/date-and-time-functions.md) 以及以下文章以取得詳細資訊。

   * [日期和時間格式的代號，位於 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/tokens-for-date-and-time-formatting.md)
   * [Adobe Workfront Fusion中用於日期和時間剖析的代號](../../workfront-fusion/functions/tokens-for-date-and-time-parsing.md)

* **使用陣列的功能** ![](assets/toolbar-icon-functions-for-arrays.png)  — 請參閱 [中的陣列函式 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/array-functions.md) 以取得更多資訊。

>[!TIP]
>
>建立要在其他欄位中重複使用的複雜公式時，可以按一下包含組合的欄位，使用Command-A或Ctrl-A選擇它，然後複製它並貼到其他欄位中。

如需使用函式對應項目的詳細資訊，請參閱 [在中使用函式映射項目 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/map-using-functions.md).

## 集合

某些項目可包含多種類型的多個值。 這些是集合類型項目。

您可以識別 [!UICONTROL 集合] 按項目標籤右側顯示的小黑色矩形鍵入項目，並自動展開子項目清單：

![](assets/collection.png)

>[!NOTE]
>
>在大多數情況下，您會對應集合的子項目，而非代表整個集合的項目。

如需集合的詳細資訊，請參閱 [中的項目資料類型 [!UICONTROL Adobe Workfront融合]](../../workfront-fusion/mapping/item-data-types.md)

## 陣列

有些項目可以包含相同類型的多個元素。 這些是陣列類型項目。

您可以依項目標籤結尾的方括弧來識別陣列類型項目。 按一下項目標籤右側的小黑色矩形，以顯示元素的項目：

![](assets/array.png)

如需陣列的詳細資訊，請參閱 [中的項目資料類型 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/item-data-types.md)

### 映射陣列的第一個元素

如果映射陣列 `Recipient name` 項目，欄位中會顯示如下：

![](assets/map-array-1st-element.png)

方括弧中的數字是一個索引，可確定將使用陣列的哪個元素。 預設會設為1。

### 映射陣列的第n個元素

如果要存取其他元素，請按一下方括弧並編輯索引值：

![](assets/access-another-element.png)

### 使用指定的鍵映射陣列的元素

有些陣列包含數個包含索引鍵和值項目的集合。 這些通常是各種中繼資料、屬性等。

下列範例顯示 [!DNL Jira] 應用程式。

![](assets/output-of-jira-app-350x100.png)

在此範例中，我們會從特定附件的附件陣列取得檔案名稱，其ID為10108。

輸出來自 [!DNL Jira] 看起來像這樣：

![](assets/output-from-jira-350x261.png)

通常的需求是根據元素的指定索引鍵值來尋找元素，並從值項目中取得對應的值。 這可以通過採用 `map()` 和 `get()` 函式。

以下是公式的詳細劃分：

1. 的第一個參數 `map()` 函式是整個陣列項目。
1. 第二個參數是值項目的原始名稱。 若要取得原始名稱，請將滑鼠移至 [!UICONTROL 映射] 面板：

   ![](assets/obtain-raw-name-350x124.png)

   >[!NOTE]
   >
   >所有參數都區分大小寫。 即使在此特定範例中，項目的標籤與其原始名稱僅大小寫不同，仍有必要使用原始名稱，與標籤Value相比，原始名稱全部為小寫值。

1. 第3個參數是關鍵項的原始名稱：

   ![](assets/3rd-parameter-350x166.png)

1. 第4個參數是給定的鍵值。

因為 `map()` 函式會傳回陣列（因為可能會有更多元素具有指定的索引鍵值），因此必須套用 `get()` 函式來取得其第一個元素：

* 此 `get()` 函式是 `map()` 函式。

* 第2個參數是元素的索引 — 1。

如需 `map()` 函式，請參閱 [中的陣列函式 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/array-functions.md).

如需 `get()` 函式，請參閱 [中的一般函式 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/general-functions.md).

## 將元素轉換為一系列套件組合

陣列可透過 [!UICONTROL 迭代器] 模組。 如需詳細資訊，請參閱 [[!UICONTROL 迭代器] 模組 [!UICONTROL Adobe Workfront融合]](../../workfront-fusion/modules/iterator-module.md).

![](assets/series-of-bundles-350x169.png)

## 疑難排解

### 映射面板中缺少項

對於每個模組，對應面板會顯示由模組作者列出的所有輸出項目。 在某些情況下，此清單可能因各種原因而不完整，而且可能缺少某些項目。 [!DNL Workfront Fusion] 在情境編輯器中執行模組時，可以自動找出遺失的輸出項目。 確切的程式會因模組的類型而稍有不同：

#### 即時觸發

1. 以滑鼠右鍵按一下模組，然後按一下 **[!UICONTROL 僅運行此模組]** 在顯示的功能表中。

   如果沒有排入佇列的WebHook，模組會等待新WebHook處理。

1. 產生網頁鈎點。

   例如，網頁鈎點模組 **[!DNL Slack]>[!UICONTROL 監聽新事件]** （會監視通道中的新通道訊息）會傳送訊息至通道。

1. 當模組完成執行時，按一下模組上方的泡泡以探索其完整輸出。

   映射面板將包含在模組輸出中發現的所有項目。

#### 輪詢觸發器

1. 以滑鼠右鍵按一下模組，然後按一下 **[!UICONTROL 僅運行此模組]** 在顯示的功能表中。
1. 如果沒有輸出，請按一下 **[!UICONTROL 選擇要開始的位置]** 並調整設定。
1. 如果沒有要處理的事件，請建立一個事件，然後返回步驟2。

   例如，網頁鈎點模組 **[!UICONTROL Gmail] >[!UICONTROL 觀看電子郵件]** 傳送電子郵件至模組正在觀看的資料夾。

1. 當模組完成執行時，按一下模組上方的泡泡以探索其完整輸出。

   映射面板現在包含模組輸出中探索到的所有項目。

#### 其他模組

您可以選擇執行：

* 整個案例（或僅包含模組的部分）

   如果您的案例以觸發器開頭，請參閱 [即時觸發](#instant-trigger) 或 [輪詢觸發器](#polling-trigger) 一節。

* 只有單一模組

如果您選擇僅執行單一模組：

1. 以滑鼠右鍵按一下模組，然後按一下 **[!UICONTROL 僅運行此模組]** 在顯示的功能表中……
1. 提供輸入項目的範例值，然後按一下 **[!UICONTROL 確定]** .
1. 當模組完成執行時，按一下模組上方的泡泡以探索其完整輸出。

   映射面板現在包含模組輸出中探索到的所有項目。
