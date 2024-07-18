---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: 在 [!DNL Adobe Workfront Fusion]中處理時發生錯誤
description: 有時候，執行情境期間可能會發生錯誤。 如果服務因無法連線至服務而無法使用，或驗證失敗，通常就會發生這種情況。 本文會討論您可能會遇到的常見錯誤。
author: Becky
feature: Workfront Fusion
exl-id: 468d7460-3853-4016-bff9-b9d3b87198ed
source-git-commit: a3756f9345cbc9417a6fd110306dfa50aecc81a2
workflow-type: tm+mt
source-wordcount: '1246'
ht-degree: 1%

---

# 在[!DNL Adobe Workfront Fusion]中處理時發生錯誤

有時候，執行情境期間可能會發生錯誤。 如果服務因無法連線至服務而無法使用，或驗證失敗，通常就會發生這種情況。 本文會討論您可能會遇到的常見錯誤。

[!DNL Adobe Workfront Fusion]會區分幾種基本錯誤型別。 其反應會因發生的錯誤型別而異。

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

## 連線錯誤

`ConnectionError`

連線錯誤是最常見的錯誤之一，通常是因為多種原因（超載、維護、中斷等）導致協力廠商服務無法使用。 此錯誤的預設處理方式取決於發生錯誤的模組：

* 如果第一個模組發生錯誤，則會終止案例的執行並顯示警告訊息。 然後[!DNL Workfront Fusion]會不斷嘗試以遞增的時間間隔重新執行案例（如下所述）。 如果所有嘗試都失敗，[!DNL Workfront Fusion]會停用此情境。
* 如果連線錯誤發生在第一個模組以外的其他模組，則後續步驟取決於情境進階設定中的[允許儲存不完整的執行](../../workfront-fusion/scenarios/scenario-settings-panel.md#allow)選項：

   * 如果啟用此選項，則情境的執行會移至[!UICONTROL 未完成執行]資料夾，其中[!DNL Workfront Fusion]會不斷嘗試以遞增的時間間隔重新執行情境。 如果所有嘗試都失敗，執行將保留在「未完成執行」資料夾中，等待使用者手動解析。

     如需不完整執行的詳細資訊，請參閱[檢視並解決 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md)中的不完整執行。
   * 如果停用此選項，則案例的執行會以錯誤結束，然後是復原階段。 然後[!DNL Workfront Fusion]會不斷嘗試以遞增的時間間隔重新執行案例。 如果所有嘗試都失敗，[!DNL Workfront Fusion]會停用此情境。

### 增加時間間隔

當發生錯誤時，以倍增方式增加兩次嘗試之間的時間間隔的演演算法稱為指數輪詢。 遞增時間間隔的設定如下：

1. 10 分鐘
1. 1 小時
1. 3 小時
1. 12 小時
1. 24 小時

在[!DNL Workfront Fusion]中使用遞增時間間隔的主要原因是為了防止經常執行的案例在多次失敗的嘗試中消耗作業。

>[!INFO]
>
>**範例：**
>
>案例包含[!DNL Google Sheets]觸發器[!UICONTROL 觀察資料列]。 由於在[!DNL Workfront Fusion]啟動案例時進行維護，[!DNL Google Sheets]在30分鐘內無法使用，因此無法擷取新列。 此情境會停止，並在10分鐘後重試。 因為[!DNL Google Sheets]仍然無法使用，[!DNL Workfront Fusion]仍無法取得新資料列的資訊。 此情境的下一次執行排程在1小時內。 [!DNL Google Sheets]此時再次可用，情境已成功執行。

## 資料錯誤

`DataError`

當專案未正確對應且未通過在[!DNL Workfront Fusion]端或使用的協力廠商服務端執行的驗證時，會產生資料錯誤。

如果發生此錯誤，則會將場景（最多到模組失敗的位置）移至不完整執行資料夾，您可以在其中疑難排解問題。 不過，此情境不會停止並繼續根據其排程執行。 若要在資料錯誤出現時停止執行案例，請啟用「案例設定」面板中的循序處理選項。

如果您尚未啟用案例設定中的[!UICONTROL 允許儲存不完整的執行]選項，則案例的執行會因錯誤而終止，並會執行復原。

如需對應的詳細資訊，請參閱[在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md)中將資訊從一個模組對應到另一個模組。

如需有關未完成執行的資訊，請參閱[在Adobe Workfront Fusion中檢視及解決未完成的執行](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md)。

如需情境設定面板的詳細資訊，請參閱[Adobe Workfront Fusion中的情境設定面板](../../workfront-fusion/scenarios/scenario-settings-panel.md)。

如需排程的相關資訊，請參閱[在Adobe Workfront Fusion中排程情境](../../workfront-fusion/scenarios/schedule-a-scenario.md)。

## 重複資料錯誤

`DuplicateDataError`

如果[!DNL Workfront Fusion]嘗試將相同的組合插入不允許重複資料的服務兩次，則會產生重複資料錯誤。 如果發生此錯誤，[!DNL Workfront Fusion]會以處理資料錯誤的方式進行。

## 無效的存取Token錯誤

`InvalidAccessTokenError`

當[!DNL Workfront Fusion]無法存取您向協力廠商服務註冊的帳戶時，會發生無效的存取權杖錯誤。 這通常發生在您在管理指定服務時撤銷[!DNL Workfront Fusion]的存取權時，但相關案例會依排程繼續執行。

如果發生此錯誤，案例的執行就會立即停止。 從發生錯誤的模組開始的其餘情境會移至不完整執行資料夾。

如需有關未完成執行的資訊，請參閱[檢視並解決 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md)中的未完成執行。

## 速率限制錯誤

`RateLimitError`

如果超過指定服務設定的限制，就會產生速率限制錯誤。 如果發生此錯誤，[!DNL Workfront Fusion]會以與連線錯誤相同的方式進行。

如需詳細資訊，請參閱[連線錯誤](#connection-error)。

## 不完整的資料錯誤

`IncompleteDataError`

只有觸發器會發生不完整的資料錯誤。 如果觸發器無法從指定服務下載所需資料，則會產生此錯誤。

如果案例以`IncompleteDataError`結束，其進一步的行為將取決於其設定[!UICONTROL 最大連續錯誤數]。

如需詳細資訊，請參閱文章[Adobe Workfront Fusion中的案例設定面板](../../workfront-fusion/scenarios/scenario-settings-panel.md)中的[連續錯誤數](../../workfront-fusion/scenarios/scenario-settings-panel.md#number)。

>[!INFO]
>
>**範例：**
>
>案例已將[!DNL Workfront]觸發器[!UICONTROL 觀看記錄]設定為觀看檔案。 此情境會在您上傳大型檔案（例如長影片）時執行。 由於[!UICONTROL Workfront Fusion]嘗試在視訊仍在上傳至Workfront時下載視訊，因此情境會以`IncompleteDataError`終止。

## 執行階段錯誤

`RuntimeError`

如果在案例執行期間出現任何其他錯誤（未提及），則會將其回報為`RunTimeError`。

如果案例以`RuntimeError`結束，其進一步的行為將取決於其設定[!UICONTROL 最大連續錯誤數]。 如需詳細資訊，請參閱文章[Adobe Workfront Fusion中的案例設定面板](../../workfront-fusion/scenarios/scenario-settings-panel.md)中的[連續錯誤數](../../workfront-fusion/scenarios/scenario-settings-panel.md#number)。

>[!NOTE]
>
>如果案例以立即觸發開始，則會忽略[!UICONTROL 最大連續錯誤數]的設定，一旦發生第一個錯誤，就會立即停用案例。 如需詳細資訊，請參閱文章[模組型別](../../workfront-fusion/modules/module-types.md)中的[立即觸發程式](../../workfront-fusion/modules/module-types.md#instant)。

## 不一致性錯誤

`InconsistencyError`

如果上述任何錯誤發生在認可或復原階段，案例會以不一致錯誤終止。 如需詳細資訊，請參閱 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md)中的[案例執行、週期和階段。

如果此錯誤出現在案例中，案例的執行會立即停止。

## 警告

執行案例時，您可能會收到警告訊息，通知您發生問題。 但是，這不會阻止案例成功完成。

例如，當超過允許的檔案大小上限，且[!UICONTROL 啟用資料遺失]選項停用時，可能會出現警告。 如需詳細資訊，請參閱文章[Adobe Workfront Fusion中的案例設定面板](../../workfront-fusion/scenarios/scenario-settings-panel.md)中的[啟用資料遺失](../../workfront-fusion/scenarios/scenario-settings-panel.md#enable)。
