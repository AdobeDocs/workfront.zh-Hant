---
content-type: overview
product-area: portfolios
navigation-topic: portfolio-optimizer
title: Portfolio最佳化工具分數概述
description: 您可以在Portfolio最佳化工具中找到Portfolio最佳化工具分數。 它會顯示在每個專案的[!UICONTROL 分數]欄中。 這代表投資組合中每個專案的分數。
author: Alina
feature: Work Management, Strategic Planning
exl-id: 4451b1a3-57ae-4c66-a6a1-a85bd51a1648
source-git-commit: 00e58ea9a207037b701e1be010c2c4c2995d60e0
workflow-type: tm+mt
source-wordcount: '726'
ht-degree: 0%

---

# [!UICONTROL Portfolio最佳化工具]分數的總覽

<!--Audited: 01/2025-->

您可以在[!UICONTROL Portfolio最佳化工具]中找到[!UICONTROL Portfolio最佳化工具]分數。 它會顯示在每個專案的&#x200B;**[!UICONTROL 分數]**&#x200B;欄中。 這代表投資組合中每個專案的分數。

如需有關找到[!UICONTROL Portfolio最佳化工具]的資訊，請參閱文章[[!UICONTROL Portfolio最佳化工具]概覽](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md)。

有關[!DNL Adobe Workfront]如何使用專案分數和其他專案資訊來最佳化[!UICONTROL Portfolio最佳化工具]中的專案的資訊，請參閱[最佳化Portfolio最佳化工具中的專案](../../../manage-work/portfolios/portfolio-optimizer/optimize-projects-in-portfolio-optimizer.md)。

## [!UICONTROL 校準分數]與[!UICONTROL Portfolio最佳化工具分數]之間的差異

一致性分數和專案的投資組合最佳化工具分數之間有所差異。

專案的對齊分數是根據完成計分卡後獲得的點數來計算。 然後，會使用此分數來決定產品組合校準分數。 對齊分數會以百分比顯示。

專案的對齊分數會顯示在[!UICONTROL Portfolio最佳化工具]的&#x200B;**[!UICONTROL 對齊]**&#x200B;欄位或[!UICONTROL 業務案例摘要]的[!UICONTROL 對齊]欄位中。

![](assets/business-case-summary-aligned-field-highlighted.png)

![](assets/project-alignment-score-portfolio-optimizer-highlighted-350x174.png)

如需有關產生專案對齊分數的詳細資訊，請參閱文章[將計分卡套用至專案並產生對齊分數](../../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md)。

[!UICONTROL 專案組合最佳化工具]分數是在[!UICONTROL Portfolio最佳化工具]中自動計算的排名，專案可依此排定優先順序。 專案組合最佳化工具分數會顯示為指標圖示，並附上數字，且會顯示在[!UICONTROL Portfolio最佳化工具]的&#x200B;**[!UICONTROL 分數]**&#x200B;欄中。

>[!NOTE]
>
>專案只有完成業務案例後，才能在[!UICONTROL Portfolio最佳化工具]中評分。 如需有關完成業務案例的詳細資訊，請參閱文章[[!UICONTROL 為專案建立業務案例]](../../../manage-work/projects/define-a-business-case/create-business-case.md)。

![](assets/portfolio-optimizer-project-score-highlighted-350x132.png)

系統會根據下列類別的重要性來計算每個專案的分數：

* [!UICONTROL 成本]
* [!UICONTROL 對齊方式]
* [!UICONTROL 淨值]
* [!UICONTROL 利益風險]
* [!UICONTROL ROI]

## 計算[!UICONTROL Portfolio最佳化工具]分數

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: This was edited based on this issue, per Anna: https://hub.workfront.com/issue/603d0c58000095ea0bc00ce5e2110693/overview)</p>
-->

[!DNL Workfront]使用[!UICONTROL Portfolio最佳化工具]產生分數，這是協助專案優先順序排定的排名。 投資組合中的值是根據輸入到專案業務案例中的值，並用於計算專案的分數。 分數較高的專案可視為較重要，並可將它們排定優先順序以首先完成。

若要瞭解專案排名，請執行下列動作：

1. 移至[!UICONTROL Portfolio最佳化工具]。
1. 將滑鼠指標停留在排名圖示上，即可檢視專案的投資組合最佳化工具分數。

![ranking_icon_in_portfolio_optimizer_new.png](assets/ranking-icon-in-portfolio-optimizer-new-350x160.png)

計算分數的演演算法會考量專案業務案例中概述的值及其攜帶的權重。 這會提供最佳化工具中每個專案的分數，並將分數標準化，因此總是會有一個專案分數為100。 這會為最佳專案提供高分。

>[!BEGINSHADEBOX]

**範例**

例如，如果您將[!UICONTROL 較高對齊度]設為唯一要考慮的因素，則具有最高對齊度的專案會獲得100分。

>[!ENDSHADEBOX]

以下是您可對專案進行評分的條件：

* [!UICONTROL 成本]
* [!UICONTROL 對齊方式]
* [!UICONTROL 值]
* [!UICONTROL 利益風險]
* [!UICONTROL ROI]

![](assets/optimizer-sliding-value-options-350x77.png)

如需如何最佳化投資組合中專案的詳細資訊，請參閱[!UICONTROL Portfolio最佳化工具]](../../../manage-work/portfolios/portfolio-optimizer/optimize-projects-in-portfolio-optimizer.md)中的[最佳化專案。

組態面板上的每個條件（[!UICONTROL 成本]、[!UICONTROL 一致性]、[!UICONTROL ROI]、[!UICONTROL 淨值]、[!UICONTROL 利益風險]）會根據您選取的專案，賦予其在0到100範圍內的權重。

對於具有完整業務案例的每個專案，會使用下列公式產生每個條件的分數：

```
Score Per Criteria = (Project Value For The Criteria - AVG(all the project values for this criteria)) / Standard Deviation of that value for that project
```

**範例：**&#x200B;針對專案A的[!UICONTROL 對齊分數]，您將擁有下列專案：

```
Alignment Score = (Project A Alignment Score - AVG (of all the project Alignments)) / Standard Deviation of alignment score for that project
```

計算完所有的[!UICONTROL 每個條件的分數]後，您就可以考慮其權重來新增它們，以取得每個專案的完整分數。 專案分數使用下列公式計算：

```
Score = Cost Score * Cost Weight + Alignment Score * Alignment Weight + ROI Score * ROI Weight + Net Value Score * Net Value Weight + Risk Score * Risk Weight
```

針對專案成本和[!UICONTROL 風險]，邏輯與其他條件運作方式相反：如果您希望[!UICONTROL 低成本]對您很重要，它不會增加，但會降低`Cost Score * Cost Weight`的專案整體分數。

計算每個專案的分數後，會依照下列方式為專案定義[!UICONTROL 最佳化分數]：

1. 已定義[!UICONTROL 最小]和[!UICONTROL 最大]分數。
1. 會計算這些值之間的範圍。
1. 針對每個專案，會使用下列公式計算[!UICONTROL 最佳化分數]：

   ```
   Optimization Score = Rounded ((Score - Minimum / Range)*100)
   ```
