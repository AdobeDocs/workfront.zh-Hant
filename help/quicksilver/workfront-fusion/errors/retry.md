---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: 在 [!DNL Adobe Workfront Fusion]中重試錯誤處理
description: 在某些情況下，如果失敗的原因可能會隨時間推移而推移，則重新執行幾次失敗模組會很有用。
author: Becky
feature: Workfront Fusion
exl-id: 1058905c-6c95-4a8c-8956-e1606f1486d9
source-git-commit: a3756f9345cbc9417a6fd110306dfa50aecc81a2
workflow-type: tm+mt
source-wordcount: '683'
ht-degree: 0%

---

# 在[!DNL Adobe Workfront Fusion]中重試錯誤處理

在某些情況下，如果失敗的原因可能會隨時間推移而推移，則重新執行失敗模組會很有用。

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

## [!UICONTROL Retry]錯誤處理指示詞的因應措施

[!UICONTROL Adobe Workfront Fusion]目前不提供[!UICONTROL Retry]錯誤處理指示詞，不過可採取兩個因應措施來模擬其功能。 如需詳細資訊，請參閱[在Adobe Workfront Fusion](../../workfront-fusion/errors/directives-for-error-handling.md)中處理錯誤的指示。

### 使用[!UICONTROL Break]指示詞

1. 在案例設定面板中，啟用&#x200B;**[!UICONTROL 允許儲存未完成的執行]**&#x200B;選項。

   如需詳細資訊，請參閱 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md)中的[案例設定面板。

1. 將錯誤處理常式路由附加到模組，如[!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-handling.md)中的[錯誤處理所述。
1. 將[!UICONTROL Break]指示詞連結到錯誤處理常式路由並進行設定。

   如需詳細資訊，請參閱[!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md)中錯誤處理的[指示。

   ![](assets/break-directive-350x241.png)

#### 缺點

* 最小重試間隔為一分鐘。
* 如果模組正在處理多個套件組合且套件組合處理失敗，部分執行（僅限導致錯誤的套件）會移至不完整執行資料夾，並根據[!UICONTROL Break]指示詞設定排程重試。 但是，目前執行會繼續進行，而模組會繼續處理後續的套件組合。 您可以在[!UICONTROL 案例設定]中啟用「[!UICONTROL 循序處理]」選項，以防止案例在成功解析儲存在「未完成執行」資料夾中的執行之前再次執行。

  如需不完整執行的詳細資訊，請參閱[檢視並解決 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md)中的不完整執行。

### 使用[!UICONTROL 中繼器]模組

1. 採用&#x200B;**[!UICONTROL 中繼器]**&#x200B;模組，並將其&#x200B;**[!UICONTROL 中繼器]**&#x200B;欄位設定為最大嘗試次數。
1. 將可能失敗的模組連結至&#x200B;**[!UICONTROL 中繼器]**&#x200B;模組。
1. 將錯誤處理常式路由附加至此模組（請參閱 [!DNL Adobe Workfront Fusio]n](../../workfront-fusion/errors/error-handling.md)中的[錯誤處理）。
1. 將&#x200B;**[!UICONTROL 工具] > [!UICONTROL 睡眠]**&#x200B;模組連結到錯誤處理常式路由，並將其&#x200B;**[!UICONTROL 延遲]**&#x200B;欄位設定為嘗試之間的秒數。

1. 在&#x200B;**[!UICONTROL Tools] > [!UICONTROL 睡眠]**&#x200B;模組之後連結&#x200B;**[!UICONTROL Ignore]**&#x200B;指示詞(請參閱[指示詞，以瞭解Adobe Workfront Fusion](../../workfront-fusion/errors/directives-for-error-handling.md)中的錯誤處理)。

1. 在可能失敗的模組之後連結&#x200B;**[!UICONTROL 工具] > [!UICONTROL 設定變數]**&#x200B;模組，並將其設定為儲存模組的結果，以使用名為的變數，例如`Result`。

1. 在&#x200B;**[!UICONTROL 工具] > [!UICONTROL 設定變數]**&#x200B;之後連結&#x200B;**[!UICONTROL 陣列彙總]**&#x200B;模組，並在其Source模組欄位中選擇&#x200B;**[!DNL Repeater]**&#x200B;模組。

1. 將&#x200B;**[!UICONTROL Tools] > [!UICONTROL 取得變數]**&#x200B;模組連結至&#x200B;**[!UICONTROL 陣列彙總]**&#x200B;模組，並將其設定為取得`Result`變數的值。

1. 在&#x200B;**[!UICONTROL 中繼器]**&#x200B;模組與可能失敗的模組之間插入&#x200B;**[!UICONTROL 工具] > [!UICONTROL 取得變數]**&#x200B;模組，並設定它以取得`Result`變數的值。

1. 在此&#x200B;**[!UICONTROL 工具] > [!UICONTROL 取得變數]**&#x200B;模組與可能失敗的模組之間插入篩選器，只有在`Result`變數不存在時才能繼續。

>[!INFO]
>
>**範例：**&#x200B;以下是範例案例，其中[!UICONTROL HTTP] >[!UICONTROL 提出要求]模組代表可能失敗的模組：
>
>![](assets/http-make-request-350x116.png)
>
>如果潛在失敗模組的結果太複雜，無法儲存在簡單變數中，您可以運用資料存放區來儲存/擷取結果。 資料存放區將只包含一個記錄。 例如，記錄的索引鍵可以是`Result`。
>
>如需資料存放區的詳細資訊，請參閱 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/data-stores.md)中的[資料存放區

#### 缺點

此因應措施可能顯得太複雜，而且對操作也比較苛刻。
