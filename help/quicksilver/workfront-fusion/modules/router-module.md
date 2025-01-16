---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Adobe Workfront Fusion中的路由器模組
description: Adobe Workfront Fusion檔案已移至新位置。 本文已棄用，但包含新文章的連結，內容涵蓋此功能。
author: Becky
feature: Workfront Fusion
exl-id: 3c39c562-1cee-4f8e-89cc-0ed554079a2b
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '659'
ht-degree: 0%

---

# [!DNL Adobe Workfront Fusion]中的[!UICONTROL 路由器]模組

>[!IMPORTANT]
>
>Adobe Workfront Fusion檔案已移至新位置。
>
>本文資訊可在以下文章中找到：
>
>* [新增路由器模組並設定路由](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/add-modules/router-module.html)
>
>請更新任何書籤。
>
>本文已不再更新，將於不久將來移除。

[!UICONTROL 路由器]模組可讓您將流量分支為數個路由，並以不同方式處理每個路由中的資料。 一旦[!UICONTROL 路由器]模組收到套件組合，它會依照路由附加至[!UICONTROL 路由器]模組的順序將其轉送至每個連線的路由。

>[!NOTE]
>
>* 若要驗證路由的順序，您可以按一下[!UICONTROL 自動對齊]圖示，該圖示會根據由上到下的順序來排列路由。
>
>  若要變更順序，請移除[!UICONTROL 路由器]模組，然後依照所需的順序重新連線路由。
>
>* 路由會循序處理，而非並行處理。 直到前一個路由完全處理完後，才會將束傳送到下一個路由。
>



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

## 正在將[!UICONTROL 路由器]模組新增至情境

[!UICONTROL 路由器]可透過下列其中一種方式新增至情境：

* 如果您要在模組之後連線[!UICONTROL 路由器]模組，請按一下模組的右邊控制代碼，開始輸入&#x200B;**[!UICONTROL 路由器]**&#x200B;進行搜尋，然後在顯示的模組清單中選擇&#x200B;**[!UICONTROL 流量控制]** > **[!UICONTROL 路由器]**。

  ![](assets/connect-the-router-350x108.png)

* 若要在兩個模組之間插入[!UICONTROL 路由器]模組，請按一下連線兩個模組的路由下方的扳手圖示（或用滑鼠右鍵按一下路由），然後從功能表中選擇&#x200B;**[!UICONTROL 新增路由器]**。

  ![](assets/insert-router-350x191.png)

* 您可以自動插入[!UICONTROL 路由器]模組。 例如，在下圖中，若要將右下角的模組連線至左上角的模組（已連線至右上角的模組），請將右下角的左側控點拖曳至左上角的模組。

  ![](assets/insert-router-automatically-350x379.png)

## 篩選器

您可以在[!UICONTROL 路由器]模組之後的路由上放置篩選器，以像任何其他路由上一樣篩選組合：

1. 按一下路由中的其中一個點。

   ![](assets/router-click-a-dot-in-route-350x339.png)

1. 在&#x200B;**[!UICONTROL 設定顯示的篩選器]**&#x200B;方塊中，新增條件，然後按一下&#x200B;**[!UICONTROL 確定]**&#x200B;以儲存篩選器設定。

   ![](assets/set-up-a-filter-2-350x242.png)

如需詳細資訊，請參閱[將篩選器新增至 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/add-a-filter-to-a-scenario.md)中的情境。

## 遞補路由

[!UICONTROL 路由器]模組之後的路由上的篩選器設定包含一個特殊選項：遞補路由：

![](assets/fallback-route-350x260.png)

啟用時，此路由用於組合無法透過任何其他路由從[!UICONTROL 路由器]模組繼續的情況下，因為其他路由上的篩選器已將其篩選掉。

在[!UICONTROL 路由器]模組中有一個不同的箭號來區分遞補路由：

![](assets/arrow-sign-in-router-module-350x361.png)

## If/Else

遞補路由的典型使用案例是，如果滿足條件，則使用一條路由繼續流程，否則使用另一條路由，如下列步驟所示：

1. 在您的情境中插入[!UICONTROL 路由器]模組。
1. 將兩個路由都連線到[!UICONTROL 路由器]模組。
1. 按一下第一個路由並指定條件：

   ![](assets/set-up-a-filter-2-350x242.png)

1. 按一下第二個路由並啟用[!UICONTROL 遞補路由]選項：

   ![](assets/enable-fallback-route-option-350x238.png)
