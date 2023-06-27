---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: 模組型別
description: 「Adobe Workfront Fusion區分五種模組：動作模組、搜尋模組、觸發模組、彙總器和疊代器。 彙總器和迭代器適用於進階情況。」
author: Becky
feature: Workfront Fusion
exl-id: 58b4aa76-6c4c-47fc-a42c-c5286da5633a
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '973'
ht-degree: 0%

---

# 模組型別

A[!UICONTROL Adobe Workfront Fusion] 區分五種模組：動作模組、搜尋模組、觸發模組、彙總器和疊代器。 「彙總」和「疊代」適用於進階案例。

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
   <td>您的組織必須購買Adobe Workfront Fusion和Adobe Workfront，才能使用本文所述的功能。</td> 
  </tr> 
 </tbody> 
</table>

若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的Workfront管理員。

有關以下專案的資訊： [!DNL Adobe Workfront Fusion] 授權，請參閱 [[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 動作模組

動作模組是最常見的模組型別。 典型動作模組會傳回單一組合，然後傳至下一個模組進行處理。

和觸發模組不同，動作模組可以放置在情境的開頭、中間或結尾。 案例可以包含不限數量的動作模組。

>[!INFO]
>
>**範例:**
>
>* **[!DNL Workfront]> [!UICONTROL 上傳檔案]** 傳送檔案至 [!DNL Workfront] 並傳回其識別碼。
>* **[!UICONTROL 影像] > [!UICONTROL 調整大小]** 接收影像、將影像大小調整為指定尺寸，然後將調整大小的影像傳遞給下一個動作。

動作型別有四個子型別：建立、讀取、更新和刪除。 「更新」子型別可啟用下列三個作業：

* **清除欄位內容**. 評估欄位的內容以清除關鍵字（不要混淆）時，就會發生此操作 *空白*)。

  ![](assets/erase-content-of-field.png)

* **欄位的內容維持不變**. 當欄位留空或欄位內容評估為空白（透過JSON中的null表示）時，就會發生此操作。

  ![](assets/leave-content-field-unchanged-350x231.png)

* **取代欄位內容**. 除了上述兩種情況外，此操作還會發生在所有其他情況下。

>[!NOTE]
>
>* 如果您沒有看到 `erase` 關鍵字在對映面板中，模組不是更新模組，或尚未更新至應用程式的最新規格。
>* &quot;[!UICONTROL 空白]」不會變更欄位內容。 如果需要拭除欄位，可使用下列公式：
>
>![](assets/formula-ifempty-name-erase.png)
>
>在內容評估為空白時，目前無法讓欄位保持不變。

## 搜尋模組

典型的搜尋會傳回零、一或多個組合，然後傳至下一個模組進行處理。

您可以將搜尋放在情境的開頭、中間或結尾。

案例可以包含不限數量的搜尋。

>[!INFO]
>
>**範例:**
>
>**[!DNL Workfront]> [!UICONTROL 讀取相關記錄]**  讀取符合指定搜尋查詢的記錄（在特定父物件中）

## 觸發器模組

指定服務發生變更時，觸發器會產生組合。 變更可以是建立新記錄、刪除記錄、更新記錄等。

每個觸發器可傳回零、一或多個組合，然後傳至下一個模組進行處理。

觸發器只能放在情境的開頭。

每個案例只能包含一個觸發器。

[!DNL Workfront Fusion] 區分兩種型別的觸發器：輪詢觸發器和即時觸發器。

### 輪詢觸發程式

輪詢觸發程式會定期輪詢指定服務，即使自上次執行以來未曾有任何變更。 我們建議您排程包含輪詢觸發器的情境，以定期執行。 如果有 *變更*，觸發器會傳回包含變更相關資訊的套件組合。 如果沒有 *變更*，觸發器不會輸出任何組合。 如需排程情境的說明，請參閱 [排程情境於 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/schedule-a-scenario.md).

輪詢觸發器可讓您選取它們應透過Epoch面板輸出的第一個組合。 儲存觸發器或變更觸發器設定後，面板會自動顯示。 如需詳細資訊，請參閱 [選擇觸發程式模組的開始位置 [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/modules/choose-where-trigger-module-starts.md).

>[!NOTE]
>
>在Epoch面板中進行的設定只會影響模組的第一次執行。 執行模組後，它會記住最後輸出的組合，並使得透過epoch面板所做的設定失效。

>[!INFO]
>
>**範例:**
>
>* **[!DNL Workfront]> [!UICONTROL 觀看記錄]** 傳回自上次執行案例後新增的檔案
>
>* **[!DNL Google Sheets]> [!UICONTROL 觀看列]** 傳回自上次執行案例以來使用者新增的新列

### 即時觸發程式

即時觸發器讓服務能夠通知 [!DNL Workfront Fusion] 關於 *變更* 立即。 我們建議您排程包含立即觸發器的情境以立即執行。 如需指示，請參閱 [在Adobe Workfront Fusion中排程情境](../../workfront-fusion/scenarios/schedule-a-scenario.md). 另請參閱 [中的即時觸發器(Webhook) [!DNL Adobe Workfront Fusion]](../../workfront-fusion/webhooks/instant-triggers-webhooks.md) 以取得如何處理傳入資料的詳細資訊。

>[!INFO]
>
>**範例:**
>
>* **[!DNL Workfront]> [!UICONTROL 觀看活動]** 在Workfront中發生特定型別事件時（例如建立任務），會傳回資訊。
>* **[!DNL Google Sheets]> [!UICONTROL 觀看變更]** 每當儲存格更新時，就會傳回資訊。

## 彙總

彙總器是一種模組，可將多個套件組合累積至單一套件組合中。

每個彙總器僅傳回一個組合，然後傳至下一個模組以供進一步處理。

您只能在情境的中間放置彙總。

案例可以包含無限數量的彙總。

>[!INFO]
>
>**範例:**
>
>* **[!UICONTROL 封存] > [!UICONTROL 建立封存]** 將收到的檔案壓縮成zip封存
>* **[!UICONTROL CSV] > [!UICONTROL 彙總至CSV]** 將CSV檔案中的多個字串合併為單一列
>* **[!UICONTROL 工具] > [!UICONTROL 文字彙總]** 將數個字串結合為單一字串

如需詳細資訊，請參閱 [中的彙總模組 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/aggregator-module.md).

## 迭代器

疊代器是一種將陣列分割成多個獨立套件的模組。

每個迭代器都會傳回一或多個組合，然後傳至下一個模組進行處理。

您只能在情境的中間放置疊代器。

案例可以包含不限數量的迭代器。

>[!INFO]
>
>**範例:**
>
>**[!UICONTROL 電子郵件] > [!UICONTROL 擷取附件]** 將附件陣列分割為個別的組合

如需詳細資訊，請參閱 [中的疊代器模組 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/iterator-module.md) 和 [將陣列對應 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-an-array.md).
