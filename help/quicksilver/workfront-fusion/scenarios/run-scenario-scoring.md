---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: 執行案例評分專家
description: 管理 [!DNL Adobe Workfront Fusion]中鎖定的案例
author: Becky
feature: Workfront Fusion
hide: true
hidefromtoc: true
source-git-commit: ed100c6ba32a6fbff6fa68ac7a4bfb38db861b17
workflow-type: tm+mt
source-wordcount: '295'
ht-degree: 0%

---

# 在Adobe Workfront Fusion中執行情境評分專家

情境評分專家可協助您確保情境的設定方式遵循最佳實務。 它會檢查您的情境並提供其結構和組織的建議。

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
  <td> <p>[！UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p><p>[！UICONTROL [!DNL Workfront Fusion] for Work Automation] </p>  </td>    </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>您的組織必須購買[!DNL Adobe Workfront Fusion]和[!DNL Adobe Workfront]，才能使用本文所述的功能。</td> 
  </tr> 
 </tbody> 
</table>

若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的[!DNL Workfront]管理員。

如需[!DNL Adobe Workfront Fusion]授權的相關資訊，請參閱[[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md)。

執行案例評分專家

1. 按一下左側面板中的&#x200B;**[!UICONTROL 案例]**&#x200B;索引標籤。
1. 選取您要執行「案例評分專家」的案例。
1. 按一下情境上的任何位置，以輸入情境編輯器。
1. 按一下畫面底部附近的情境評分專家圖示![情境評分專家](assets/scoring-expert-icon.png)。

   「情境評分專家」面板隨即開啟。
1. 按一下&#x200B;**評估**。

情境評分專家傳回滿分10分，並顯示哪些檢查通過或失敗。 如果檢查失敗，案例評分專家會提供建議，說明如何確保案例符合這些檢查。

![案例分數](assets/scenario-score.png)

## 案例評分檢查

「情境評分專家」會使用以下檢查：

* 案例必須命名為。
* 所有模組都必須加上標籤。
* 此案例必須依設定的排程執行。

  如需指示，請參閱[排程情境](/help/quicksilver/workfront-fusion/scenarios/schedule-a-scenario.md)。
* 情境藍圖大小必須小於5 MB。

  如需詳細資訊，請參閱[融合效能護欄](/help/quicksilver/workfront-fusion/get-started/fusion-performance-guardrails.md#scenarios)。
* 若使用Workfront即時觸發程式模組，則必須加以篩選。

  如需指示，請參閱 [!DNL Workfront] > [!UICONTROL 觀看活動]模組](/help/quicksilver/workfront-fusion/apps-and-their-modules/workfront-modules.md#event-subscription-filters-in-the-workfront--watch-events-module)中的[活動訂閱篩選器。





