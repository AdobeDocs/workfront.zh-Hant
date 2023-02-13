---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Adobe Workfront Fusion中的路由器模組
description: 路由器模組允許您將流分支到多條路由中，並以不同方式處理每條路由中的資料。 路由器模組收到一個捆綁包後，會按照路由附加到路由器模組的順序將其轉發到每個連接的路由。
author: Becky
feature: Workfront Fusion
exl-id: 3c39c562-1cee-4f8e-89cc-0ed554079a2b
source-git-commit: e58ff769015b8c4e34b34eea653f55a296eea371
workflow-type: tm+mt
source-wordcount: '578'
ht-degree: 0%

---

# [!UICONTROL 路由器] 模組 [!DNL Adobe Workfront Fusion]

此 [!UICONTROL 路由器] 模組可讓您將流分支到多條路由，並以不同方式處理每條路由內的資料。 一次a [!UICONTROL 路由器] 模組接收一個包，它按照路由附加到的順序將它轉發到每個連接的路由 [!UICONTROL 路由器] 模組。

>[!NOTE]
>
>* 要驗證路由的順序，可以按一下 [!UICONTROL 自動對齊] 表徵圖，按從上到下的順序排列路由。
>
>  若要變更順序，請移除 [!UICONTROL 路由器] 模組，並按所需順序重新連接路由。
>
>* 路由會按順序處理，而非並行處理。 在上一條路由完全處理之前，將不會將包發送到下一條路由。
>




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
   <td>貴組織必須購買 [!DNL Adobe Workfront Fusion] 和 [!DNL Adobe Workfront] 以使用本文所述的功能。</td> 
  </tr> 
 </tbody> 
</table>

若要了解您擁有的計畫、授權類型或存取權，請聯絡您的 [!DNL Workfront] 管理員。

如需 [!DNL Adobe Workfront Fusion] 許可證，請參閱 [[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 新增 [!UICONTROL 路由器] 模組至案例

A [!UICONTROL 路由器] 可透過下列其中一種方式新增至案例：

* 如果您要連線 [!UICONTROL 路由器] 模組之後，按一下模組的右手柄，開始鍵入 **[!UICONTROL 路由器]** 要搜索，請選擇 **[!UICONTROL 流量控制]** > **[!UICONTROL 路由器]** 顯示的模組清單中。

   ![](assets/connect-the-router-350x108.png)

* 如果您想要插入 [!UICONTROL 路由器] 在兩個模組之間，按一下連接兩個模組的路由下方的扳手錶徵圖（或按一下右鍵路由），然後選擇 **[!UICONTROL 添加路由器]** 的上界。

   ![](assets/insert-router-350x191.png)

* 您可以插入 [!UICONTROL 路由器] 模組。 例如，在下圖中，要將右下角的模組連接到左上角的模組（已連接到右上角的模組），請拖動右下角模組的左手柄，並將其拖放到左上角的模組上。

   ![](assets/insert-router-automatically-350x379.png)

## 篩選器

您可以在 [!UICONTROL 路由器] 模組，以按任何其它路由來篩選包：

1. 按一下路徑中的一個點。

   ![](assets/router-click-a-dot-in-route-350x339.png)

1. 在 **[!UICONTROL 設定篩選]** 方塊，新增條件，然後按一下 **[!UICONTROL 確定]** 來儲存篩選器設定。

   ![](assets/set-up-a-filter-2-350x242.png)

如需詳細資訊，請參閱 [將篩選器新增至案例，於 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/add-a-filter-to-a-scenario.md).

## 後援路由

路由上的篩選器設定，在 [!UICONTROL 路由器] 模組包含特殊選項：後援路由：

![](assets/fallback-route-350x260.png)

啟用後，此路由將用於無法從 [!UICONTROL 路由器] 模組，因為其他路由上的篩選器會將其過濾掉。

後援路由區分為內部不同的箭頭符號 [!UICONTROL 路由器] 模組：

![](assets/arrow-sign-in-router-module-350x361.png)

## If/Else

備援路由的典型使用案例是，如果滿足條件，則使用一條路由繼續流，如果不滿足則使用另一條路由，如以下步驟所示：

1. 插入 [!UICONTROL 路由器] 模組。
1. 將兩條路由連接到 [!UICONTROL 路由器] 模組。
1. 按一下第一條路由並指定條件：

   ![](assets/set-up-a-filter-2-350x242.png)

1. 按一下第二條路由並啟用 [!UICONTROL 後退路由] 選項：

   ![](assets/enable-fallback-route-option-350x238.png)
