---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Adobe Workfront Fusion中的案例設定面板
description: 本文說明 [!UICONTROL 藍本設定] 面板 [!DNL Adobe Workfront Fusion] 方案。
author: Becky
feature: Workfront Fusion
exl-id: 64a7a39a-f450-4eba-b4db-f31dd22aefdc
source-git-commit: 59941ea1ce523a0d1036138a83f771b058049b34
workflow-type: tm+mt
source-wordcount: '968'
ht-degree: 0%

---

# 中的藍本設定面板 [!DNL Adobe Workfront Fusion]

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] （工作自動化和整合） </p><p>[!UICONTROL [!DNL Workfront Fusion] （工作自動化） </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>貴組織必須購買 [!DNL Adobe Workfront Fusion] 和 [!DNL Adobe Workfront] 以使用本文所述的功能。</td> 
  </tr> 
 </tbody> 
</table>

若要了解您擁有的計畫、授權類型或存取權，請聯絡您的 [!DNL Workfront] 管理員。

如需 [!DNL Adobe Workfront Fusion] 許可證，請參閱 [[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 開啟藍本設定

1. 開啟案例編輯器，如 [中的案例編輯器 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-editor.md).
1. 按一下頁面左下角附近的齒輪圖示。

   ![](assets/scenario-settings-350x221.png)

   在 [!UICONTROL 藍本設定] 面板隨即顯示，您可以為藍本配置各種進階設定。

## [!UICONTROL 允許儲存不完整的執行]

此選項決定如何 [!DNL Adobe Workfront Fusion] 執行情境期間發生錯誤時繼續。 啟用此選項後，案例會暫停並移至 [在中檢視並解決未完成的執行 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md). 這可讓您修正問題，並從情境停止的位置繼續執行。 如果禁用此選項，則方案運行將停止，並啟動回滾階段。

## [!UICONTROL 循序處理]

此選項決定如何 [!DNL Workfront Fusion] 發生錯誤並將執行案例移至 [在中檢視並解決未完成的執行 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md). 若 [!UICONTROL 循序處理] 選項，則Workfront Fusion會完全停止處理任務序列，直到所有未完成的執行都解決為止。 若 [!UICONTROL 循序處理] 選項已停用，則情境會根據其排程繼續執行，並會重複嘗試重新執行不完整的執行。

如需排程的詳細資訊，請參閱 [在中排程藍本 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/schedule-a-scenario.md).

## 資料是機密的

執行案例後，您預設可顯示案例中模組所處理資料的相關資訊。 如果您不想儲存此資訊，請啟用 [!UICONTROL 資料是機密的] 選項。

如需顯示資訊的詳細資訊，請參閱 [中的方案執行流程 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-flow.md).

>[!IMPORTANT]
>
>如果啟用此選項，可能很難解決執行案例期間可能發生的錯誤。

## 啟用資料丟失

如果 [!DNL Workfront Fusion] 無法將套件組合儲存到 [在中檢視並解決未完成的執行 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md) （例如，由於缺乏可用空間）。 啟用此選項後，資料會遺失，以防止整體情境執行中斷。 對於最高優先順序為持續執行且傳入的錯誤資料不重要的情況，這很有用。

除此之外，執行案例時，模組有時會遇到大於允許大小上限的檔案。 在這種情況下， [!DNL Workfront Fusion] 收益，根據 [!UICONTROL 啟用資料丟失] 選項和警告訊息。

有關最大檔案大小的詳細資訊，請參見 [關於在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/about-mapping-files.md).

有關警告的詳細資訊，請參閱 [中的錯誤處理 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-processing.md).

## [!UICONTROL 自動提交]

此 [!UICONTROL 自動提交] 設定會套用至交易，並定義處理案例的方式。 如果「自動提交」選項處於開啟狀態，則每個模組的提交階段在完成操作階段後立即開始。 禁用「自動提交」選項後，在對所有模組執行操作（這是預設模式）之前，不會執行提交。

有關交易的詳細資訊，請參閱 [中的方案執行、週期和階段 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

## 最大循環數

如果您想要防止第三方服務的連線中斷，並確保在一個案例執行中處理所有記錄，設定更多週期會很有用。

* 如果情境以輪詢觸發器開頭，則設定會定義在執行情境期間允許的最大循環數。

   如需輪詢觸發器的詳細資訊，請參閱 [輪詢觸發器](../../workfront-fusion/modules/module-types.md#polling) in [模組類型](../../workfront-fusion/modules/module-types.md).

* 如果情境以立即觸發開始，則會忽略設定，並在單一情境執行期間處理所有待定事件，每個週期處理一個事件。

   有關即時觸發器的詳細資訊，請參閱 [即時觸發](../../workfront-fusion/modules/module-types.md#instant) in [模組類型](../../workfront-fusion/modules/module-types.md).

* 如果情境不是以觸發器（即時/輪詢）開頭，則一律會執行指定的最大循環數。

>[!INFO]
>
>**範例：**  [!DNL Workfront] > [!UICONTROL 監視記錄] 監視傳入的新問題，以及 [!DNL Workfront] >[!UICONTROL 轉換物件] 將新請求轉換為專案，並為其指派適當的範本。
>
>![](assets/scenario-settings-ex-1-350x157.png)
>
>A [!UICONTROL 更多週期] 只有在排程方案執行時，才會套用設定。 若您使用 [!UICONTROL 執行一次] 按鈕，則會考慮週期設定。
>
>### 最大循環數設為1（預設值）
>
>![](assets/max-number-cycles-1-350x201.png)
>
>此 [!UICONTROL 返回檔案的最大數量] 在 [!UICONTROL Dropbox] >[!UICONTROL 監看檔案] 模組設為 `10`.
>
>![](assets/max-number-cycles-10-350x175.png)
>
>如果100個請求已提交至 [!DNL Workfront]，和 [!UICONTROL 限制] 欄位設為10，則90個檔案在某個案例執行後會保留為未處理。 接下來10個檔案會在下一個排程的案例執行中處理。
>
>### 最大循環數設為10
>
>此 [!UICONTROL 返回檔案的最大數量] 在 [!UICONTROL Dropbox] >[!UICONTROL 監看檔案] 模組設為 `10`.
>
>如果有100個檔案新增至Dropbox資料夾，且 [!UICONTROL 返回檔案的最大數量] 選項設為10，然後在第一個週期處理10個檔案，第二個週期處理下一個10個檔案，第三個週期處理下一個10個檔案，依此類推，直到處理所有檔案。
>
>所有檔案都會在1個案例執行中處理。
>
>您可以在方案詳細資訊中查看已執行的週期：
>
>![](assets/scenario-detail-350x207.png)
>
>如需此頁面的詳細資訊，請參閱 [中的方案詳細資料 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-detail.md).

## 連續錯誤數

定義在情境執行被停用前連續執行嘗試的最大數量(不包括 [!UICONTROL DataError], [!UICONTROL DuplicateDataError] 和 [!UICONTROL 連接錯誤])。

如需錯誤的詳細資訊，請參閱 [中的錯誤處理 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-processing.md).

>[!NOTE]
>
>如果情境以立即觸發開始，則會忽略設定，並在發生第一個錯誤後立即停用情境。
