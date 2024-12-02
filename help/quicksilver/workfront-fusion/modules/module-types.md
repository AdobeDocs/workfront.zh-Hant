---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: 模組型別
description: Adobe Workfront Fusion區分五種模組：動作模組、搜尋模組、觸發模組、彙總器和疊代器。 「彙總」和「疊代」適用於進階案例。
author: Becky
feature: Workfront Fusion
exl-id: 58b4aa76-6c4c-47fc-a42c-c5286da5633a
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '973'
ht-degree: 0%

---

# 模組型別

A[!UICONTROL adobe Workfront Fusion]會區分五種模組：動作模組、搜尋模組、觸發模組、彙總器和疊代器。 「彙總」和「疊代」適用於進階案例。

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
   <td>您的組織必須購買Adobe Workfront Fusion以及Adobe Workfront，才能使用本文所述的功能。</td> 
  </tr> 
 </tbody> 
</table>

若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的Workfront管理員。

如需[!DNL Adobe Workfront Fusion]授權的相關資訊，請參閱[[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md)。

## 動作模組

動作模組是最常見的模組型別。 典型動作模組會傳回單一套件，然後傳至下一個模組進行處理。

和觸發模組不同，動作模組可以放置在情境的開頭、中間或結尾。 案例可以包含不限數量的動作模組。

>[!INFO]
>
>**範例：**
>
>* **[!DNL Workfront]> [!UICONTROL 上傳檔案]**&#x200B;會將檔案傳送至[!DNL Workfront]並傳回其識別碼。
>* **[!UICONTROL 影像] > [!UICONTROL 調整大小]**&#x200B;會收到影像，將其調整為指定的尺寸，然後將調整大小的影像傳遞到下一個動作。

動作型別有四種子型別：建立、讀取、更新和刪除。 「更新」子型別可啟用下列三個作業：

* **清除欄位**&#x200B;的內容。 當欄位內容評估為清除關鍵字（不要與&#x200B;*empty*&#x200B;混淆）時，就會發生此作業。

  ![](assets/erase-content-of-field.png)

* **保留欄位的內容不變**。 當欄位留空或欄位內容評估為空白（透過JSON中的Null表示）時，會發生此作業。

  ![](assets/leave-content-field-unchanged-350x231.png)

* **取代欄位**&#x200B;的內容。 除了上述兩種情況外，此操作還會發生在其他所有情況中。

>[!NOTE]
>
>* 如果您在對應面板中看不到`erase`關鍵字，表示模組不是更新模組，或模組尚未更新為應用程式的最新規格。
>* &quot;[!UICONTROL Empty]&quot;不會變更欄位內容。 如果必須拭除欄位，您可以使用下列公式：
>
>![](assets/formula-ifempty-name-erase.png)
>
>在內容評估為空白時保持欄位不變，目前是不可能的。

## 搜尋模組

典型的搜尋會傳回零、一或多個組合，然後傳至下一個模組進行處理。

您可以將搜尋放置在情境的開頭、中間或結尾。

案例可以包含不限數量的搜尋。

>[!INFO]
>
>**範例：**
>
>**[!DNL Workfront]> [!UICONTROL 讀取相關記錄]**&#x200B;會讀取符合您指定之搜尋查詢的記錄（在特定父物件中）

## 觸發模組

指定服務發生變更時，觸發器便會產生組合。 變更可以是建立新記錄、刪除記錄、更新記錄等。

每個觸發器可傳回零、一或多個組合，接著再傳至下一個模組進行處理。

觸發器只能放置在情境的開頭。

每個案例只能包含一個觸發器。

[!DNL Workfront Fusion]會區分兩種型別的觸發器：輪詢觸發器和即時觸發器。

### 輪詢觸發程式

輪詢觸發程式會定期輪詢指定的服務，即使自上次執行以來未曾變更也是如此。 我們建議您排程包含輪詢觸發器的情境，以定期執行。 如果發生&#x200B;*變更*，觸發器會傳回包含變更相關資訊的組合。 如果沒有&#x200B;*變更*，則觸發器不會輸出任何組合。 如需排程情境的說明，請參閱[在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/schedule-a-scenario.md)中排程情境。

輪詢觸發器可讓您選取它們應透過Epoch面板輸出的第一個套件。 儲存觸發器或變更觸發器設定後，面板會自動顯示。 如需詳細資訊，請參閱[選擇觸發程式模組在[!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/modules/choose-where-trigger-module-starts.md)中的開始位置。

>[!NOTE]
>
>在Epoch面板中進行的設定只會影響模組的第一次執行。 執行模組後，它會記住最後輸出的組合，並使得透過Epoch面板進行的設定失效。

>[!INFO]
>
>**範例：**
>
>* **[!DNL Workfront]> [!UICONTROL 觀看記錄]**&#x200B;會傳回自上次執行情境後新增的檔案
>
>* **[!DNL Google Sheets]> [!UICONTROL 觀看列]**&#x200B;傳回自上次執行案例以來使用者新增的新列

### 即時觸發程式

即時觸發程式可讓服務立即通知[!DNL Workfront Fusion]發生&#x200B;*變更*。 我們建議您排程包含立即觸發器的情境，以便立即執行。 如需指示，請參閱[在Adobe Workfront Fusion中排程情境](../../workfront-fusion/scenarios/schedule-a-scenario.md)。 另請參閱 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/webhooks/instant-triggers-webhooks.md)中的[即時觸發程式(webhook)，以取得如何處理傳入資料的詳細資訊。

>[!INFO]
>
>**範例：**
>
>* **[!DNL Workfront]> [!UICONTROL 觀看活動]**&#x200B;會在Workfront中發生特定型別的活動時（例如建立工作），傳回資訊。
>* **[!DNL Google Sheets]> [!UICONTROL 每次更新儲存格時，觀看變更]**&#x200B;都會傳回資訊。

## 彙總

彙總是一種模組，可將多個套件累積至單一套件組合中。

每個彙總器僅傳回一個組合，然後傳至下一個模組以供進一步處理。

您只能在情境的中間放置彙總。

案例可以包含不限數量的彙總。

>[!INFO]
>
>**範例：**
>
>* **[!UICONTROL 封存] > [!UICONTROL 建立封存]**&#x200B;將收到的檔案壓縮成zip封存
>* **[!UICONTROL CSV] > [!UICONTROL 彙總至CSV]**&#x200B;會將CSV檔案中的多個字串合併為一列
>* **[!UICONTROL 工具] > [!UICONTROL 文字彙總]**&#x200B;將數個字串合併為一個字串

如需詳細資訊，請參閱 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/aggregator-module.md)中的[彙總模組。

## 迭代器

疊代器是一種將陣列分割成多個獨立套件的模組。

每個疊代器會傳回一或多個組合，然後傳至下一個模組進行處理。

您只能在情境的中間放置疊代器。

案例可以包含不限數量的迭代器。

>[!INFO]
>
>**範例：**
>
>**[!UICONTROL 電子郵件] > [!UICONTROL 擷取附件]**&#x200B;將附件陣列分成不同的組合

如需詳細資訊，請參閱 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/iterator-module.md)中的[疊代器模組，以及 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-an-array.md)中的[對應陣列。
