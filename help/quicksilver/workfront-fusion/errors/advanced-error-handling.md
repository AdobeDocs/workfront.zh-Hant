---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: 中的進階錯誤處理 [!DNL Adobe] Workfront Fusion
description: 進階錯誤處理技術包括篩選和巢狀化。
author: Becky
feature: Workfront Fusion
exl-id: 57f43fc2-23ed-44f5-8785-90739329b5ee
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '957'
ht-degree: 0%

---

# 中的進階錯誤處理 [!DNL Adobe Workfront Fusion]

進階錯誤處理技術包括篩選和巢狀化。

## 存取需求

您必須具有下列存取權才能使用本文中的功能：

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計劃*</td> 
   <td> <p>[！UICONTROL Pro]或更高版本</p> </td> 
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

## 正在篩選

錯誤處理常式路由中可能會進行兩種篩選。

* [新增篩選器至錯誤處理常式路由](#adding-a-filter-to-the-error-handler-route)
* [將後面接著篩選器的路由器新增至錯誤處理常式路由](#adding-a-router-followed-by-filters-to-the-error-handler)

### 新增篩選器至錯誤處理常式路由

您可以使用篩選器來控制哪些錯誤是由錯誤處理常式路由處理。 這可讓您僅處理特定型別的錯誤。 如果錯誤未通過篩選器，則會將其視為沒有為給定模組定義錯誤處理常式路由。

>[!INFO]
>
>**範例:**
>
>![](assets/filter-error-handling-350x238.png)

### 新增 [!UICONTROL 路由器] 後面接著錯誤處理常式的篩選器

>[!INFO]
>
>![](assets/router-filter-error-handling-350x254.png)
>
>在此範例中，錯誤發生在 [!UICONTROL 建立資料夾] 模組(A)，此模組具有規則路由和錯誤處理常式路由。 後者之後是路由器，其中一條路由具有定義特定錯誤型別（發生資料錯誤）的篩選器，而另一條路由是所有其他錯誤的預設路由。 第一個路由的結尾是 [!UICONTROL 繼續] 指示詞，其中包含從模組A恢復之情境的替代值([!UICONTROL 建立資料夾])，而第二個路由的結尾是 [!UICONTROL 復原] 立即停止案例執行的指令。

另請參閱 [中的處理錯誤 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-processing.md) 以取得有關各種錯誤型別及如何操作的進一步資訊 [!DNL Workfront Fusion] 處理並評估它們。

### 範例情境

您可以設定此範例情境，以瞭解這些篩選器如何處理錯誤。

使用現有 [!DNL Dropbox] 資料夾以上傳檔案，而非建立新檔案

如果您使用 [!UICONTROL 建立資料夾] 模組開啟 [!DNL Dropbox] 且已存在同名資料夾，模組將擲回資料錯誤，如下所示：

![](assets/dropbox-350x276.png)

完整情境：

![](assets/dropbox-scenario-350x190.png)

1. 此 [!UICONTROL 工具] > [!UICONTROL 設定變數] 模組包含資料夾名稱
1. 此 [!UICONTROL HTTP] >[!UICONTROL 取得檔案] 模組會擷取需要上傳至資料夾的檔案
1. 此 [!UICONTROL Dropbox] >[!UICONTROL 建立資料夾] 如果資料夾已存在且名稱與模組中所對應資料夾名稱相同，則模組會擲回錯誤
1. 錯誤處理常式路由（透明泡泡）包含用來篩選錯誤的路由器
1. 第一個路由是針對我們已知名為資料錯誤的指定錯誤型別：

   1. 如果發生資料錯誤，且錯誤詳細資料通過篩選器，則 [!UICONTROL Dropbox] >[!UICONTROL 列出資料夾模組中的所有檔案/子資料夾] 列出所有資料夾 [!DNL Dropbox]
   1. 後續篩選符合資料夾名稱
   1. 此 [!UICONTROL 繼續] directive會指定現有資料夾的資料夾ID和資料夾路徑，而案例執行將從 [!UICONTROL Dropbox] >[!UICONTROL 建立資料夾] 模組使用，但這次不是嘗試建立新資料夾，而是使用 [!UICONTROL 繼續] 指示移到下一個模組，並在現有資料夾中上傳檔案

1. 第二個路由適用於所有其他錯誤，且結尾為 [!UICONTROL 復原] 指示詞會導致立即停止情境

以下是第5個陳述式的詳細說明：

為了在後續模組中使用現有資料夾([!UICONTROL 上傳檔案] （如下所示），您需要將錯誤處理常式路由新增至模組，並擷取要對應至的資料夾路徑 [!UICONTROL 繼續] 指令模組如下：

![](assets/add-error-handler-route-350x113.png)

第一個路由上的篩選器設定為只處理當同名資料夾已存在時所顯示的特定錯誤（資料錯誤）：

![](assets/condition-350x327.png)

此 [!UICONTROL Dropbox] >[!UICONTROL 列出資料夾中的所有檔案] 模組已設定為傳回目標資料夾中的所有資料夾。 下列篩選器只會在我們最初嘗試建立的篩選器上傳遞（資料夾名稱儲存在33中）。 資料夾名稱專案)：

![](assets/condition2-350x193.png)

最終， [!UICONTROL 繼續] 指示詞提供資料夾路徑作為失敗模組的輸出。 請注意，資料夾ID已保留空白，因為「[!UICONTROL 上傳檔案]&#39;模組：

![](assets/flow-control-350x190.png)

## 巢狀

無論模組位於何處，都可以在所有模組（路由器除外）上建立和實施錯誤處理常式路由。 因此，可以為已經是為其他模組建立的現有錯誤處理常式路由的一部分的模組建立錯誤處理常式路由。

以下是巢狀錯誤處理常式路由的範例：

![](assets/nested-error-handling-route-350x174.png)

在此案例中，第二個錯誤處理常式路由會巢狀位於第一個錯誤處理常式路由下。 因此，如果 [!UICONTROL Dropbox] >[!UICONTROL 建立資料夾模組] 發生錯誤，執行會移至「路由1」，如果 [!UICONTROL 發生資料錯誤] 篩選器通過，下一個模組將執行，之後將執行 [!UICONTROL 繼續] 指示模組（如果錯誤未發生） [!UICONTROL Dropbox] >[!UICONTROL 列出所有檔案/子資料夾] 在資料夾模組中。

不過，如果發生錯誤，則 [!DNL Dropbox] 模組，則執行會移至錯誤處理常式路由2，並以 [!UICONTROL 忽略] 指令。 此 [!UICONTROL Resume指令] 在此情況下不會執行模組。

這是篩選和巢狀錯誤處理常式的組合。

