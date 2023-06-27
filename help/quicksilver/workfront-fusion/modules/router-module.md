---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Adobe Workfront Fusion中的路由器模組
description: 路由器模組可讓您將流量分支至數個路由，並以不同方式處理每個路由中的資料。 路由器模組收到套件後，會依照路由連線至路由器模組的順序，將其轉送至每個連線的路由。
author: Becky
feature: Workfront Fusion
exl-id: 3c39c562-1cee-4f8e-89cc-0ed554079a2b
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '626'
ht-degree: 0%

---

# [!UICONTROL 路由器] 中的模組 [!DNL Adobe Workfront Fusion]

此 [!UICONTROL 路由器] 模組可讓您將流量分支至數個路由，並以不同方式處理每個路由內的資料。 一次a [!UICONTROL 路由器] 模組會接收一個束，然後依照路由附加至的順序將其轉送到每個連線的路由。 [!UICONTROL 路由器] 模組。

>[!NOTE]
>
>* 若要驗證路由的順序，您可以按一下 [!UICONTROL 自動對齊] 圖示，會根據由上到下的順序來排列路線。
>
>  若要變更順序，請移除 [!UICONTROL 路由器] 模組，並按所需順序重新連線路由。
>
>* 路由是循序處理，而非並行處理。 直到前一個路由完全處理完後，才會將套件傳送至下一個路由。
>



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

## 新增 [!UICONTROL 路由器] 模組至案例

A [!UICONTROL 路由器] 可透過下列其中一種方式新增至情境：

* 如果您想要連線 [!UICONTROL 路由器] 模組之後，按一下模組的右側控制代碼，開始輸入 **[!UICONTROL 路由器]** 以搜尋，然後選擇 **[!UICONTROL 流量控制]** > **[!UICONTROL 路由器]** 在顯示的模組清單中。

  ![](assets/connect-the-router-350x108.png)

* 如果您要插入 [!UICONTROL 路由器] 兩個模組之間的模組，按一下連線兩個模組的路由下方的扳手圖示（或用滑鼠右鍵按一下路由），然後選擇 **[!UICONTROL 新增路由器]** 功能表中的。

  ![](assets/insert-router-350x191.png)

* 您可以插入 [!UICONTROL 路由器] 模組自動。 例如，在下圖中，若要將右下角的模組連線至左上角的模組（已連線至右上角的模組），請將右下角的左側控點拖曳至左上角的模組。

  ![](assets/insert-router-automatically-350x379.png)

## 篩選器

您可以在路徑之後放置篩選器 [!UICONTROL 路由器] 模組，可像其他任何路徑一樣篩選組合：

1. 按一下路由中的其中一個點。

   ![](assets/router-click-a-dot-in-route-350x339.png)

1. 在 **[!UICONTROL 設定篩選器]** 方塊、新增條件，然後按一下 **[!UICONTROL 確定]** 以儲存篩選設定。

   ![](assets/set-up-a-filter-2-350x242.png)

如需詳細資訊，請參閱 [將篩選器新增至中的情境 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/add-a-filter-to-a-scenario.md).

## 遞補路由

路徑上的篩選設定 [!UICONTROL 路由器] 模組包含一個特殊選項：備援路由：

![](assets/fallback-route-350x260.png)

啟用時，當套件無法從繼續時，會使用此路由。 [!UICONTROL 路由器] 模組，因為其他路由上的篩選器已將其篩選掉。

「遞補繞線」的區別在於其內有不同的箭號 [!UICONTROL 路由器] 模組：

![](assets/arrow-sign-in-router-module-350x361.png)

## If/Else

遞補路由的典型使用案例是，如果滿足條件，則使用一條路由繼續流程，否則使用另一條路由，如下列步驟所示：

1. 插入 [!UICONTROL 路由器] 模組。
1. 將兩個路由都連線到 [!UICONTROL 路由器] 模組。
1. 按一下第一個繞線並指定條件：

   ![](assets/set-up-a-filter-2-350x242.png)

1. 按一下第二個路由，然後啟用 [!UICONTROL 遞補路由] 選項：

   ![](assets/enable-fallback-route-option-350x238.png)
