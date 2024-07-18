---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Adobe Workfront Fusion中的案例設定面板
description: 本文說明在您的 [!DNL Adobe Workfront Fusion] 案例中，[!UICONTROL 案例設定]面板中可用的設定。
author: Becky
feature: Workfront Fusion
exl-id: 64a7a39a-f450-4eba-b4db-f31dd22aefdc
source-git-commit: 4d9832d0870c3fccf847c3932ad4f985a62b9672
workflow-type: tm+mt
source-wordcount: '1097'
ht-degree: 0%

---

# [!DNL Adobe Workfront Fusion]中的案例設定面板

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
   <p>舊版授權需求： [！UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration]，[！UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>
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

## 開啟案例設定

1. 開啟情境編輯器，如[在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-editor.md)中的情境編輯器所述。
1. 按一下頁面左下角附近的齒輪圖示。

   ![](assets/scenario-settings-350x221.png)

   在顯示的[!UICONTROL 情境設定]面板中，您可以設定情境的各種進階設定。

## [!UICONTROL 允許儲存未完成的執行]

此選項決定在執行案例期間發生錯誤時，[!DNL Adobe Workfront Fusion]如何進行。 啟用此選項後，情境會暫停並移至[檢視並解決 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md)中未完成的執行。 這可讓您修正問題，並從情景停止的地方繼續執行。 如果停用此選項，案例執行會停止並開始倒回階段。

## [!UICONTROL 循序處理]

此選項決定當發生錯誤且案例的執行移至[檢視並解決 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md)中的未完成執行時，[!DNL Workfront Fusion]如何進行。 如果[!UICONTROL 循序處理]選項已啟用，Workfront Fusion會完全停止處理工作順序，直到解決所有未完成的執行為止。 如果[!UICONTROL 循序處理]選項已停用，則情境會根據其排程繼續執行，並伴隨重複嘗試重新執行未完成的執行。

>[!NOTE]
>
>循序處理可能會導致案例的執行延遲。 如果在即時案例觸發或排程案例設定為執行時，佇列中仍有未完成的執行，則該案例將在佇列中的所有執行完成後執行。
>
>如果您的案例不需要循序處理，建議您停用循序處理選項。

如需排程的詳細資訊，請參閱[在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/schedule-a-scenario.md)中排程情境。

## 資料是機密的

執行案例後，您可以預設顯示案例中模組處理哪些資料的相關資訊。 如果您不想儲存此資訊，請啟用[!UICONTROL 資料是機密的]選項。

如需有關顯示資訊的詳細資訊，請參閱 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-flow.md)中的[案例執行流程。

>[!IMPORTANT]
>
>如果啟用此選項，可能很難解決執行案例期間可能發生的錯誤。

## 啟用資料遺失

此選項與啟用資料遺失有關，如果[!DNL Workfront Fusion]無法將組合儲存到[的佇列檢視並解決 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md)中未完成的執行（例如，由於缺少可用空間）。 啟用此選項後，資料會遺失，以防止整體案例執行中斷。 當最高優先順序為連續執行，而傳入的錯誤資料並非很重要時，這個用法很有用。

除此之外，在執行案例時，模組有時可能會遇到大於最大允許大小的檔案。 在此情況下，[!DNL Workfront Fusion]會根據[!UICONTROL 啟用資料遺失]選項的設定進行，並顯示警告訊息。

如需檔案大小上限的詳細資訊，請參閱[關於 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/about-mapping-files.md)中的對應檔案。

如需有關警告的詳細資訊，請參閱 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-processing.md)中的[錯誤處理。

## [!UICONTROL 自動認可]

[!UICONTROL 自動認可]設定會套用至交易，並定義處理案例的方式。 如果開啟自動認可選項，每個模組上的認可階段會在完成作業階段後立即開始。 停用「自動提交」選項時，在所有模組執行作業之前，不會發生任何提交（這是預設模式）。

如需交易的詳細資訊，請參閱[案例執行、週期和階段（在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md)中）。

## 最大週期數

如果您想要避免與協力廠商服務的連線中斷，並確保所有記錄都會在單一案例執行內處理，設定更多週期可能相當實用。

* 如果案例以輪詢觸發器開始，設定會定義案例執行期間允許的最大週期數。

  如需輪詢觸發器的詳細資訊，請參閱[模組型別](../../workfront-fusion/modules/module-types.md)中的[輪詢觸發器](../../workfront-fusion/modules/module-types.md#polling)。

* 如果案例從立即觸發器開始，設定會被忽略，並且在單一案例執行期間處理所有待處理事件，每個週期一個事件。

  如需即時觸發器的詳細資訊，請參閱[模組型別](../../workfront-fusion/modules/module-types.md)中的[即時觸發器](../../workfront-fusion/modules/module-types.md#instant)。

* 如果案例不是以觸發器（即時/輪詢）開始，則一律執行指定的最大週期數。

>[!INFO]
>
>**範例：** [!DNL Workfront] > [!UICONTROL 觀看記錄]觀看新問題的出現，以及[!DNL Workfront] >[!UICONTROL 轉換物件]將新要求轉換為專案並指派適當的範本。
>
>![](assets/scenario-settings-ex-1-350x157.png)
>
>[!UICONTROL 更多週期]設定只會在您排程情境執行時套用。 當您使用[!UICONTROL 執行一次]按鈕時，會考慮循環設定。
>
>### 最大循環數設為1 （預設）
>
>![](assets/max-number-cycles-1-350x201.png)
>
>[!UICONTROL Dropbox] >[!UICONTROL 監看檔案]模組中的[!UICONTROL 最大傳回檔案數]設定為`10`。
>
>![](assets/max-number-cycles-10-350x175.png)
>
>如果將100個要求提交至[!DNL Workfront]，且[!UICONTROL 限制]欄位設為10，則在執行一個案例後仍有90個檔案未處理。 接下來10個檔案會在下一個排程案例執行中處理。
>
>### 最大循環數設為10
>
>[!UICONTROL Dropbox] >[!UICONTROL 監看檔案]模組中的[!UICONTROL 最大傳回檔案數]設定為`10`。
>
>如果新增100個檔案至Dropbox資料夾，且[!UICONTROL 傳回檔案數上限]選項設為10，則會在第一個週期處理10個檔案、在第二個週期處理下一個10個檔案、在第三個週期處理下一個10個檔案，以此類推，直到處理完所有檔案為止。
>
>所有檔案會在1個案例執行內處理。
>
>您可以在案例詳細資訊中檢視已執行的週期：
>
>![](assets/scenario-detail-350x207.png)
>
>如需此頁面的詳細資訊，請參閱 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-detail.md)中的[案例詳細資料。

## 連續錯誤數

定義停用執行案例之前連續執行嘗試的最大次數（不包括[!UICONTROL DataError]、[!UICONTROL DuplicateDataError]和[!UICONTROL ConnectionError]）。

如需有關錯誤的詳細資訊，請參閱[在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-processing.md)中處理錯誤。

>[!NOTE]
>
>如果案例以立即觸發器開始，則會忽略設定，並在發生第一個錯誤後立即停用案例。
