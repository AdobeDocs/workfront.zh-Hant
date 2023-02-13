---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: 中的進階錯誤處理 [!DNL Adobe] Workfront融合
description: 進階的錯誤處理技術包括篩選和巢狀。
author: Becky
feature: Workfront Fusion
exl-id: 57f43fc2-23ed-44f5-8785-90739329b5ee
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '913'
ht-degree: 0%

---

# 中的進階錯誤處理 [!DNL Adobe Workfront Fusion]

進階的錯誤處理技術包括篩選和巢狀。

## 存取需求

您必須具備下列存取權才能使用本文中的功能：

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計劃*</td> 
   <td> <p>[!UICONTROL Pro]或更高版本</p> </td> 
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

## 正在篩選

在錯誤處理程式路由上可以進行兩種過濾。

* [向錯誤處理程式路由添加篩選器](#adding-a-filter-to-the-error-handler-route)
* [添加路由器，然後將篩選器添加到錯誤處理程式路由](#adding-a-router-followed-by-filters-to-the-error-handler)

### 向錯誤處理程式路由添加篩選器

您可以使用篩選器來控制哪些錯誤是由錯誤處理程式路由處理。 這可讓您僅處理特定類型的錯誤。 如果錯誤未通過篩選器，則會將其視為沒有為給定模組定義錯誤處理程式路由。

>[!INFO]
>
>**範例:**
>
>![](assets/filter-error-handling-350x238.png)

### 新增 [!UICONTROL 路由器] 後跟對錯誤處理程式的篩選器

>[!INFO]
>
>![](assets/router-filter-error-handling-350x254.png)
>
>在此範例中，錯誤發生在 [!UICONTROL 建立資料夾] 模組(A)，具有常規路由和錯誤處理路由。 後者後面是路由器，其中一條路由具有定義特定錯誤類型（資料錯誤發生）的過濾器，另一條路由是所有其他錯誤的預設路由。 第一條路由以 [!UICONTROL 繼續] 包含從模組A恢復的方案的替代值的指令([!UICONTROL 建立資料夾])，而第二條路由的結尾為 [!UICONTROL 回復] 指令，可立即停止方案執行。

請參閱 [中的錯誤處理 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-processing.md) 有關各種錯誤類型以及如何 [!DNL Workfront Fusion] 處理並評估。

### 範例案例

您可以設定此範例情境，以了解這些篩選器如何用於錯誤處理。

使用現有 [!DNL Dropbox] 上傳檔案，而非建立新檔案的資料夾

如果您使用 [!UICONTROL 建立資料夾] 模組 [!DNL Dropbox] 而且已存在同名的資料夾，模組將擲回資料錯誤，如下所示：

![](assets/dropbox-350x276.png)

完整案例：

![](assets/dropbox-scenario-350x190.png)

1. 此 [!UICONTROL 工具] > [!UICONTROL 設定變數] 模組包含資料夾名稱
1. 此 [!UICONTROL HTTP] >[!UICONTROL 取得檔案] 模組會擷取需要上傳至資料夾的檔案
1. 此 [!UICONTROL Dropbox] >[!UICONTROL 建立資料夾] 如果資料夾已存在，且名稱與模組中映射的資料夾相同，則模組會擲回錯誤
1. 錯誤處理程式路由（透明泡泡）包含用於過濾錯誤的路由器
1. 第一條路由是針對已知的、名為「資料錯誤」的指定錯誤類型：

   1. 若發生資料錯誤，且錯誤詳細資料通過篩選，則 [!UICONTROL Dropbox] >[!UICONTROL 列出資料夾模組中的所有檔案/子資料夾] 列出了 [!DNL Dropbox]
   1. 後續的篩選器符合資料夾名稱
   1. 此 [!UICONTROL 繼續] 指令指定現有資料夾的資料夾ID和資料夾路徑，並從 [!UICONTROL Dropbox] >[!UICONTROL 建立資料夾] 模組，但此次不會嘗試建立新資料夾，而是使用 [!UICONTROL 繼續] 指令，移至下一個模組並上傳現有資料夾中的檔案

1. 第二條路由適用於所有其他錯誤，結尾為 [!UICONTROL 回復] 導致立即停止方案的指令

第5份聲明的詳細說明如下：

若要在後續模組中使用現有資料夾([!UICONTROL 上傳檔案] )，則需要將錯誤處理程式路由添加到模組，並提取要映射到的資料夾路徑 [!UICONTROL 繼續] 指令模組如下：

![](assets/add-error-handler-route-350x113.png)

第一個路由上的篩選器被設定為僅處理具有相同名稱的資料夾已存在時出現的特定錯誤（資料錯誤）:

![](assets/condition-350x327.png)

此 [!UICONTROL Dropbox] >[!UICONTROL 列出資料夾中的所有檔案] 模組配置為返回目標資料夾中的所有資料夾。 下列篩選器只會傳遞原本嘗試建立的篩選器（資料夾名稱會儲存在33中）。 資料夾名稱項):

![](assets/condition2-350x193.png)

最終， [!UICONTROL 繼續] 指令將資料夾路徑作為失敗模組的輸出。 請注意，資料夾ID留空，因為「[!UICONTROL 上傳檔案]&#39;模組：

![](assets/flow-control-350x190.png)

## 巢狀

無論模組在何處，都可以在除路由器之外的所有模組上建立和實施錯誤處理程式路由。 因此，可以為已為另一個模組建立的現有錯誤處理程式路由的一部分的模組建立錯誤處理程式路由。

以下是巢狀錯誤處理程式路由的範例：

![](assets/nested-error-handling-route-350x174.png)

在這種情況下，第二錯誤處理程式路由嵌套在第一錯誤處理程式路由下。 如果 [!UICONTROL Dropbox] >[!UICONTROL 建立資料夾模組] 遇到錯誤時，執行會移至Route 1(如果 [!UICONTROL 發生資料錯誤] 會傳遞篩選，然後執行下一個模組，接著 [!UICONTROL 繼續] 指令模組（若未發生錯誤） [!UICONTROL Dropbox] >[!UICONTROL 列出所有檔案/子資料夾] 中。

不過，如果發生此錯誤 [!DNL Dropbox] 模組，則執行將移至錯誤處理程式路由2並以 [!UICONTROL 忽略] 指令。 此 [!UICONTROL 恢復指令] 在此情況下，不會執行模組。

這是篩選和嵌套錯誤處理程式的組合。

