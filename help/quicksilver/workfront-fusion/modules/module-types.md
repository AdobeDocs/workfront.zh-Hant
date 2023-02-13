---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: 模組類型
description: 「Adobe Workfront融合」區分了五種模組：動作模組、搜尋模組、觸發模組、匯總器及迭代器。 聚合器和迭代器適用於高級方案。
author: Becky
feature: Workfront Fusion
exl-id: 58b4aa76-6c4c-47fc-a42c-c5286da5633a
source-git-commit: e58ff769015b8c4e34b34eea653f55a296eea371
workflow-type: tm+mt
source-wordcount: '963'
ht-degree: 0%

---

# 模組類型

A[!UICONTROL Adobe Workfront Fusion] 區分五種類型的模組：動作模組、搜尋模組、觸發模組、匯總器及迭代器。 匯總器和迭代器適用於進階案例。

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
   <td>貴組織必須購買Adobe Workfront Fusion和Adobe Workfront，才能使用本文所述的功能。</td> 
  </tr> 
 </tbody> 
</table>

若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

如需 [!DNL Adobe Workfront Fusion] 許可證，請參閱 [[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 動作模組

動作模組是最常見的模組類型。 典型動作模組會傳回單一套件組合，然後傳遞至下一個模組以進行處理。

與觸發模組不同，動作模組可放置在案例的開頭、中間或結尾。 方案可包含不限數量的動作模組。

>[!INFO]
>
>**範例:**
>
>* **[!DNL Workfront]> [!UICONTROL 上傳檔案]** 將檔案傳送至 [!DNL Workfront] 並傳回其識別碼。
>* **[!UICONTROL 影像] > [!UICONTROL 調整大小]** 接收影像，將其調整為指定尺寸，並將調整後的影像傳遞到下一個操作。


動作類型有四種子類型：建立、讀取、更新和刪除。 「更新」子類型可啟用以下三個操作：

* **擦除欄位的內容**. 將欄位內容評估為清除關鍵字時(不要與 *空白*)。

   ![](assets/erase-content-of-field.png)

* **將欄位的內容維持不變**. 將欄位保留為空白，或將欄位的內容評估為空白時（透過JSON中的null表示），就會執行此操作。

   ![](assets/leave-content-field-unchanged-350x231.png)

* **取代欄位的內容**. 除上述兩種情況外，其他所有情況都會執行此操作。

>[!NOTE]
>
>* 如果您沒有看到 `erase` 關鍵字，則模組不是更新模組，或尚未更新為應用程式的最新規格。
>* &quot;[!UICONTROL 空白]「 」不會變更欄位內容。 如果需要拭除欄位，可使用下列公式：
>
>![](assets/formula-ifempty-name-erase.png)
>
>將欄位評估為空白時，目前無法將欄位維持不變。

## 搜尋模組

一般的搜尋會傳回零、一或多個套件組合，然後傳遞至下一個模組進行處理。

您可以將「搜尋」放置在案例的開頭、中間或結尾。

藍本可包含不限數量的搜尋。

>[!INFO]
>
>**範例:**
>
>**[!DNL Workfront]> [!UICONTROL 讀取相關記錄]**  讀取與您指定的搜索查詢（在特定父對象中）匹配的記錄

## 觸發模組

當指定服務發生變更時，觸發器會產生套件組合。 更改可以是建立新記錄、刪除記錄、更新記錄等。

每個觸發器都可傳回零、一或多個套件組合，然後傳遞至下一個模組以進行處理。

觸發器只能放在案例的開頭。

每個案例只能包含一個觸發器。

[!DNL Workfront Fusion] 區分兩種觸發器：輪詢觸發器和即時觸發器。

### 輪詢觸發器

輪詢觸發器會定期輪詢指定的服務，即使自上次執行以來沒有任何變更。 建議您將包含輪詢觸發器的案例排程為定期執行。 如果有 *變更*，觸發器會傳回包含變更相關資訊的套件組合。 如果沒有 *變更*，則觸發器不會輸出任何套件組合。 如需排程案例的指示，請參閱 [在中排程藍本 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/schedule-a-scenario.md).

輪詢觸發器可讓您透過Epoch面板選取應輸出的第一個套件組合。 儲存觸發器或變更觸發器設定後，面板會自動顯示。 如需詳細資訊，請參閱 [選擇觸發程式模組的起始位置 [!UICONTROL Adobe Workfront融合]](../../workfront-fusion/modules/choose-where-trigger-module-starts.md).

>[!NOTE]
>
>在Epoch面板中進行的設定只會影響模組的第一次執行。 一旦執行模組，它便記住最後輸出的束，並撤消通過紀元面板進行的設定。

>[!INFO]
>
>**範例:**
>
>* **[!DNL Workfront]> [!UICONTROL 監看記錄]** 傳回自上次執行案例後新新增的檔案
>
>* **[!DNL Google Sheets]> [!UICONTROL 監視行]** 會傳回自上次執行案例以來，使用者新增的新列


### 即時觸發

即時觸發器使服務能夠通知 [!DNL Workfront Fusion] 關於 *變更* 立即。 建議您排程包含即時觸發程式的案例，以便立即執行。 如需指示，請參閱 [排程Adobe Workfront Fusion中的案例](../../workfront-fusion/scenarios/schedule-a-scenario.md). 另請參閱 [中的即時觸發器(Webhook) [!DNL Adobe Workfront Fusion]](../../workfront-fusion/webhooks/instant-triggers-webhooks.md) 以了解如何處理傳入資料的詳細資訊。

>[!INFO]
>
>**範例:**
>
>* **[!DNL Workfront]> [!UICONTROL 觀看事件]** 在Workfront中發生特定類型的事件（例如建立任務）時，會傳回資訊。
>* **[!DNL Google Sheets]> [!UICONTROL 監看變更]** 每當儲存格更新時，都會傳回資訊。


## 匯總器

聚合器是一種模組，可將多個捆綁組合累計到一個捆綁組合中。

每個聚合器只返回一個捆綁包，然後傳遞到下一個模組以進一步處理。

您只能將整合器放在案例的中間。

方案可包含不限數量的匯總器。

>[!INFO]
>
>**範例:**
>
>* **[!UICONTROL 封存] > [!UICONTROL 建立封存]** 將接收的檔案壓縮為zip存檔
>* **[!UICONTROL CSV] > [!UICONTROL 匯總為CSV]** 將CSV檔案的多個字串合併成單一列
>* **[!UICONTROL 工具] > [!UICONTROL 文字彙總器]** 將多個字串合併為一個字串


如需詳細資訊，請參閱 [中的匯總模組 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/aggregator-module.md).

## 迭代器

迭代器是一種將陣列分割成多個獨立套件的模組。

每個迭代器都會傳回一或多個套件組合，然後傳遞至下一個模組以進行處理。

您只能將迭代程式放置在案例的中間。

藍本可包含不限數量的迭代程式。

>[!INFO]
>
>**範例:**
>
>**[!UICONTROL 電子郵件] > [!UICONTROL 檢索附件]** 將一系列附件拆分成單獨的套件

如需詳細資訊，請參閱 [中的迭代器模組 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/iterator-module.md) 和 [在中映射陣列 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-an-array.md).
