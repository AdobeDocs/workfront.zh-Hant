---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: 重試錯誤處理 [!DNL Adobe Workfront Fusion]
description: 在某些情況下，如果失敗的原因可能隨時間流逝而發生，則重新執行幾次失敗模組會很有用。
author: Becky
feature: Workfront Fusion
exl-id: 1058905c-6c95-4a8c-8956-e1606f1486d9
source-git-commit: a3756f9345cbc9417a6fd110306dfa50aecc81a2
workflow-type: tm+mt
source-wordcount: '683'
ht-degree: 0%

---

# 重試錯誤處理 [!DNL Adobe Workfront Fusion]

在某些情況下，如果失敗的原因可能隨時間流逝而發生，則重新執行失敗模組會很有用。

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
   <td>
   <p>目前產品需求：如果您有[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Adobe Workfront] 計畫，您的組織必須購買 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文所述功能。 [!DNL Workfront Fusion] 包含在[！UICONTROL Ultimate]中 [!DNL Workfront] 計畫。</p>
   <p>或</p>
   <p>舊版產品需求：貴組織必須購買 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文所述功能。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

若要瞭解您擁有哪些計畫、授權型別或存取權，請聯絡您的 [!DNL Workfront] 管理員。

有關以下專案的資訊： [!DNL Adobe Workfront Fusion] 授權，請參閱 [[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 變通辦法 [!UICONTROL 重試] 錯誤處理指示詞

[!UICONTROL Adobe Workfront Fusion] 目前不提供 [!UICONTROL 重試] 錯誤處理指示詞，不過可以使用兩個變通方法模擬其功能。 如需詳細資訊，請參閱 [Adobe Workfront Fusion中錯誤處理的指示](../../workfront-fusion/errors/directives-for-error-handling.md).

### 使用 [!UICONTROL 中斷] 指令

1. 在案例設定面板中，啟用 **[!UICONTROL 允許儲存未完成的執行]** 選項。

   如需詳細資訊，請參閱 [中的案例設定面板 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md).

1. 將錯誤處理常式路由附加至模組，如所述 [中的錯誤處理 [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-handling.md).
1. 連結 [!UICONTROL 中斷] 指示錯誤處理常式路由並加以設定。

   如需詳細資訊，請參閱 [中用於錯誤處理的指令 [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md).

   ![](assets/break-directive-350x241.png)

#### 缺點

* 最小重試間隔為一分鐘。
* 如果模組正在處理多個套件組合且套件組合處理失敗，則會將部分執行（僅限導致錯誤的套件）移至不完整執行資料夾，並根據排程重試 [!UICONTROL 中斷] 指示詞設定。 不過，目前執行會繼續，而模組會繼續處理後續的組合。 您可以啟用「 」[!UICONTROL 循序處理]中的「 」選項 [!UICONTROL 案例設定] 以防止案例再次執行，直到成功解析儲存在未完成執行資料夾中的執行為止。

  如需不完整執行的詳細資訊，請參閱 [在中檢視和解決未完成的執行 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

### 使用 [!UICONTROL 中繼器] 模組

1. 採用 **[!UICONTROL 中繼器]** 模組並設定其 **[!UICONTROL 重複]** 欄位至最大嘗試次數。
1. 將可能失敗的模組連結至 **[!UICONTROL 中繼器]** 模組。
1. 將錯誤處理常式路由附加至此模組(請參閱 [中的錯誤處理 [!DNL Adobe Workfront Fusio]n](../../workfront-fusion/errors/error-handling.md))。
1. 連結 **[!UICONTROL 工具] > [!UICONTROL 睡眠]** 模組到錯誤處理常式路由並設定其 **[!UICONTROL 延遲]** 欄位中輸入兩次嘗試之間的秒數。

1. 連結 **[!UICONTROL 忽略]** 指示詞位於 **[!UICONTROL 工具] > [!UICONTROL 睡眠]** 模組(請參閱 [Adobe Workfront Fusion中錯誤處理的指示](../../workfront-fusion/errors/directives-for-error-handling.md))。

1. 連結 **[!UICONTROL 工具] > [!UICONTROL 設定變數]** 在可能失敗的模組後面加上模組，並將其設定為將模組結果儲存在名為的變數中，例如， `Result`.

1. 連結 **[!UICONTROL 陣列彙總]** 之後的模組 **[!UICONTROL 工具] > [!UICONTROL 設定變數]** 並選擇 **[!DNL Repeater]** 模組在其來源模組欄位中。

1. 連結 **[!UICONTROL 工具] > [!UICONTROL 取得變數]** 模組至 **[!UICONTROL 陣列彙總]** 模組並進行設定，以取得 `Result` 變數。

1. 插入 **[!UICONTROL 工具] > [!UICONTROL 取得變數]** 模組介於 **[!UICONTROL 中繼器]** 模組和可能失敗的模組，並將其設定為取得 `Result` 變數。

1. 在此之間插入篩選器 **[!UICONTROL 工具] > [!UICONTROL 取得變數]** 模組與可能失敗的模組僅在 `Result` 變數不存在。

>[!INFO]
>
>**範例：** 以下是範例情境： [!UICONTROL HTTP] >[!UICONTROL 提出要求] 模組代表可能失敗的模組：
>
>![](assets/http-make-request-350x116.png)
>
>如果可能失敗的模組結果太複雜，無法儲存在簡單變數中，您可以利用資料存放區來儲存/擷取結果。 資料存放區將只包含一個記錄。 例如，記錄的鍵可以是 `Result`.
>
>如需資料存放區的詳細資訊，請參閱 [中的資料存放區 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/data-stores.md)

#### 缺點

此因應措施可能顯得太複雜，對作業的要求也更高。
