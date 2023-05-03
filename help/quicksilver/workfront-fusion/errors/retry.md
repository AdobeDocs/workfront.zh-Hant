---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: 重試錯誤處理(在 [!DNL Adobe Workfront Fusion]
description: 在某些情況下，如果故障原因可能會隨著時間而過去，重新執行失敗模組幾次會很有幫助。
author: Becky
feature: Workfront Fusion
exl-id: 1058905c-6c95-4a8c-8956-e1606f1486d9
source-git-commit: 184033c8957e955b3011f7e0845a73029f6b7aba
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# 重試錯誤處理(在 [!DNL Adobe Workfront Fusion]

在某些情況下，如果故障原因可能會隨著時間而過去，則重新執行故障模組會很有幫助。

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

## 解決方法 [!UICONTROL 重試] 錯誤處理指令

[!UICONTROL Adobe Workfront融合] 目前不提供 [!UICONTROL 重試] 錯誤處理指令，但可採用兩種解決方法來模擬其功能。 如需詳細資訊，請參閱 [Adobe Workfront Fusion錯誤處理指示](../../workfront-fusion/errors/directives-for-error-handling.md).

### 使用 [!UICONTROL 插播] 指令

1. 在情節設定面板中，啟用 **[!UICONTROL 允許儲存不完整的執行]** 選項。

   如需詳細資訊，請參閱 [中的藍本設定面板 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md).

1. 將錯誤處理程式路由附加到模組，如 [錯誤處理 [!UICONTROL Adobe Workfront融合]](../../workfront-fusion/errors/error-handling.md).
1. 連結 [!UICONTROL 插播] 指令到錯誤處理程式路由並進行配置。

   如需詳細資訊，請參閱 [錯誤處理指令 [!UICONTROL Adobe Workfront融合]](../../workfront-fusion/errors/directives-for-error-handling.md).

   ![](assets/break-directive-350x241.png)

#### 缺點

* 最小重試間隔為1分鐘。
* 如果模組正在處理多個套件組合，且套件組合的處理失敗，則部分執行（僅導致錯誤的套件組合）會移至不完整的執行資料夾，並根據 [!UICONTROL 插播] 指令設定。 但是，當前執行將繼續，而模組將繼續處理後續的包。 您可以啟用「[!UICONTROL 循序處理]」選項 [!UICONTROL 藍本設定] 以防止在Incomplete executions資料夾中儲存的執行已成功解析之前再次執行方案。

   有關未完成執行的詳細資訊，請參見 [在中檢視並解決未完成的執行 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

### 使用 [!UICONTROL 中繼器] 模組

1. 採用 **[!UICONTROL 中繼器]** 模組及其設定 **[!UICONTROL 重複]** 欄位至最大嘗試次數。
1. 將可能失敗的模組連結至 **[!UICONTROL 中繼器]** 模組。
1. 將錯誤處理程式路由附加到此模組(請參閱 [錯誤處理 [!DNL Adobe Workfront Fusio]n](../../workfront-fusion/errors/error-handling.md))。
1. 連結 **[!UICONTROL 工具] > [!UICONTROL 睡眠]** 模組到錯誤處理程式路由並設定其 **[!UICONTROL 延遲]** 欄位至兩次嘗試之間的秒數。

1. 連結 **[!UICONTROL 忽略]** 指令之後 **[!UICONTROL 工具] > [!UICONTROL 睡眠]** 模組(請參閱 [Adobe Workfront Fusion錯誤處理指示](../../workfront-fusion/errors/directives-for-error-handling.md))。

1. 連結 **[!UICONTROL 工具] > [!UICONTROL 設定變數]** 模組在可能發生故障的模組之後，並將其設定為儲存模組的結果，並產生一個名為的變數，例如 `Result`.

1. 連結 **[!UICONTROL 陣列聚合器]** 模組之後 **[!UICONTROL 工具] > [!UICONTROL 設定變數]** 並選擇 **[!DNL Repeater]** 模組。

1. 連結 **[!UICONTROL 工具] > [!UICONTROL 取得變數]** 模組 **[!UICONTROL 陣列聚合器]** 模組並加以設定，以取得 `Result` 變數。

1. 插入 **[!UICONTROL 工具] > [!UICONTROL 取得變數]** 模組介於 **[!UICONTROL 中繼器]** 模組和可能失敗的模組，並加以設定，以取得 `Result` 變數。

1. 在此之間插入篩選器 **[!UICONTROL 工具] > [!UICONTROL 取得變數]** 模組和可能失敗的模組只在 `Result` 變數不存在。

>[!INFO]
>
>**範例：** 以下是範例案例，其中 [!UICONTROL HTTP] >[!UICONTROL 提出請求] 模組代表可能失敗的模組：
>
>![](assets/http-make-request-350x116.png)
>
>如果可能發生故障的模組的結果太複雜，無法儲存在簡單變數中，您可以使用資料儲存來儲存/擷取結果。 資料儲存區只包含一條記錄。 例如，記錄的密鑰可以是， `Result`.
>
>如需資料存放區的詳細資訊，請參閱 [資料儲存於 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/data-stores.md)

#### 缺點

此解決方法看起來可能有點過於複雜，而且在操作方面要求更高。
