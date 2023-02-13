---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: 中的錯誤處理 [!DNL Adobe Workfront Fusion]
description: 執行案例期間有時會發生錯誤。 當服務因無法連線至服務或驗證失敗而無法使用時，通常會發生此情況。 本文探討您可能遇到的常見錯誤。
author: Becky
feature: Workfront Fusion
exl-id: 468d7460-3853-4016-bff9-b9d3b87198ed
source-git-commit: 97f91d663df86341a079894cff04d07c18b7bf08
workflow-type: tm+mt
source-wordcount: '1191'
ht-degree: 0%

---

# 中的錯誤處理 [!DNL Adobe Workfront Fusion]

執行案例期間有時會發生錯誤。 當服務因無法連線至服務或驗證失敗而無法使用時，通常會發生此情況。 本文探討您可能遇到的常見錯誤。

[!DNL Adobe Workfront Fusion] 區分幾種基本錯誤類型。 根據發生的錯誤類型，其反應會不同。

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] （工作自動化和整合） </p><p>[!UICONTROL [!DNL Workfront Fusion] （工作自動化）</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>貴組織必須購買 [!DNL Adobe Workfront Fusion] 和 [!DNL Adobe Workfront] 以使用本文所述的功能。</td> 
  </tr> 
 </tbody> 
</table>

若要了解您擁有的計畫、授權類型或存取權，請聯絡您的 [!DNL Workfront] 管理員。

如需 [!DNL Adobe Workfront Fusion] 許可證，請參閱 [[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 連接錯誤

`ConnectionError`

連線錯誤是最常見的錯誤之一，通常是由於各種原因（過載、維護、中斷等）而無法使用第三方服務所造成。 此錯誤的預設處理方式取決於遇到的模組：

* 如果錯誤發生在第一個模組，則會以警告訊息終止執行情境。 [!DNL Workfront Fusion] 接著，會以增加的時間間隔重複嘗試重新執行情境（以下說明）。 如果所有嘗試都失敗， [!DNL Workfront Fusion] 停用案例。
* 如果連接錯誤發生在第一個模組以外的其他模組上，則後續步驟取決於 [允許儲存不完整的執行](../../workfront-fusion/scenarios/scenario-settings-panel.md#allow) 方案進階設定中的選項：

   * 如果啟用此選項，則會將方案的執行移至 [!UICONTROL 未完成執行] 資料夾 [!DNL Workfront Fusion] 不斷嘗試以增加的時間間隔重新執行情境。 如果所有嘗試都失敗，則執行會保留在 [在中檢視並解決未完成的執行 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md) 資料夾等待用戶手動解析。
   * 如果禁用了該選項，則方案的執行將以錯誤結束，然後是回滾階段。 [!DNL Workfront Fusion] 然後，以增加的時間間隔反複嘗試重新執行情境。 如果所有嘗試都失敗， [!DNL Workfront Fusion] 停用案例。

### 增加時間間隔

錯誤發生時多次增加兩次嘗試之間的時間間隔的算法稱為指數回退。 增加的時間間隔設定如下：

1. 10 分鐘
1. 1 小時
1. 3 小時
1. 12 小時
1. 24 小時

時間間隔增加的主要原因 [!DNL Workfront Fusion] 是為了防止頻繁執行的情況對反複失敗的嘗試執行佔用操作。

>[!INFO]
>
>**範例:**
>
>案例包含 [!DNL Google Sheets] 觸發 [!UICONTROL 監視行]. [!DNL Google Sheets] 因為維護，在 [!DNL Workfront Fusion] 會啟動情境，因此無法擷取新列。 情境會在10分鐘內停止並再次嘗試。 由於此時間範圍內服務繼續不可用， [!DNL Workfront Fusion] 仍無法取得新列的相關資訊。 方案的下次執行排程為1小時後。 [!DNL Google Sheets] 此時間內可再次使用，且案例成功執行。

## 資料錯誤

`DataError`

當項目不正確對應，且未通過在 [!DNL Workfront Fusion] 使用的第三方服務的側面或側面。 如需詳細資訊，請參閱 [將資訊從一個模組對應到 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

如果發生此錯誤，則情境（直到模組失敗的位置）會移至不完整的執行資料夾，您可在其中疑難排解問題。 但是，情境不會停止，並會繼續根據其排程執行。 若要在出現「資料錯誤」時停止執行案例，請在「案例設定」面板中啟用「循序處理」選項。

如果您尚未啟用 [!UICONTROL 允許儲存不完整的執行] 選項，方案的執行將終止並出現錯誤，並執行回滾。

有關未完成執行的資訊，請參閱 [檢視並解決Adobe Workfront Fusion中的不完整執行](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

如需情節設定面板的相關資訊，請參閱 [Adobe Workfront Fusion中的案例設定面板](../../workfront-fusion/scenarios/scenario-settings-panel.md).

如需排程的相關資訊，請參閱 [排程Adobe Workfront Fusion中的案例](../../workfront-fusion/scenarios/schedule-a-scenario.md).

## 重複資料錯誤

`DuplicateDataError`

若 [!DNL Workfront Fusion] 嘗試將相同套件插入兩次不允許重複資料的服務，會產生重複資料錯誤。 如果發生此錯誤， [!DNL Workfront Fusion] 會以與處理資料錯誤相同的方式進行。

## 訪問令牌錯誤無效

`InvalidAccessTokenError`

當 [!DNL Workfront Fusion] 無法訪問在第三方服務中註冊的帳戶。 這通常發生在您撤銷 [!DNL Workfront Fusion] 在指定服務的管理中，但相關情況會依排程持續執行。

如果發生此錯誤，則會立即停止執行情境。 從發生錯誤的模組開始的其餘方案會移至不完整的執行資料夾。

有關未完成執行的資訊，請參閱 [在中檢視並解決未完成的執行 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

## 速率限制錯誤

`RateLimitError`

如果超過給定服務設定的限制，則生成速率限制錯誤。 如果發生此錯誤， [!DNL Workfront Fusion] 會以與連線錯誤相同的方式進行。 如需詳細資訊，請參閱 [連接錯誤](#connection-error).

## 資料錯誤不完整

`IncompleteDataError`

只有觸發器才會發生不完整的資料錯誤。 如果觸發器無法從指定服務下載所需資料，則會產生此錯誤。

如果藍本終止，且 `IncompleteDataError`，其進一步行為將取決於其設定 [!UICONTROL 連續錯誤的最大數量]. 如需詳細資訊，請參閱 [連續錯誤數](../../workfront-fusion/scenarios/scenario-settings-panel.md#number) 在文章中 [Adobe Workfront Fusion中的案例設定面板](../../workfront-fusion/scenarios/scenario-settings-panel.md).

>[!INFO]
>
>**範例：** 情境具有 [!DNL Workfront] 觸發 [!UICONTROL 監視記錄] 設定為監視文檔。 當您上傳大型檔案（例如長視訊）時，會執行此案例。 因為 [!UICONTROL Workfront融合] 嘗試在視訊仍上傳至Workfront時下載，情境會以 `IncompleteDataError`.

## 運行時錯誤

`RuntimeError`

如果執行案例期間出現任何其他錯誤（如上所述），則會回報為 `RunTimeError`.

如果藍本終止，且 `RuntimeError`，其進一步行為將取決於其設定 [!UICONTROL 連續錯誤的最大數量]. 如需詳細資訊，請參閱 [連續錯誤數](../../workfront-fusion/scenarios/scenario-settings-panel.md#number) 在文章中 [Adobe Workfront Fusion中的案例設定面板](../../workfront-fusion/scenarios/scenario-settings-panel.md).

>[!NOTE]
>
>如果情境以即時觸發開始，則 [!UICONTROL 連續錯誤的最大數量] 會忽略，且第一個錯誤發生後，會立即停用情境。 如需詳細資訊，請參閱 [即時觸發](../../workfront-fusion/modules/module-types.md#instant) 在文章中 [模組類型](../../workfront-fusion/modules/module-types.md).

## 不一致錯誤

`InconsistencyError`

如果在提交或回滾階段期間出現上述任何錯誤，則方案將終止並出現「不一致錯誤」。 如需詳細資訊，請參閱 [中的方案執行、週期和階段 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

如果情境中出現此錯誤，則立即停止執行情境。

## 警告

執行情境時，您可能會收到警告，通知您有問題。 但是，這並不會阻止方案成功完成。

例如，超過允許的檔案大小上限時，可能會出現警告，且 [!UICONTROL 啟用資料丟失] 選項。 如需詳細資訊，請參閱 [啟用資料丟失](../../workfront-fusion/scenarios/scenario-settings-panel.md#enable) 在文章中 [Adobe Workfront Fusion中的案例設定面板](../../workfront-fusion/scenarios/scenario-settings-panel.md).
