---
content-type: overview
product-area: portfolios
navigation-topic: portfolio-optimizer
title: Portfolio優化程式分數概觀
description: 您可以在Portfolio優化程式中找到Portfolio優化程式分數。 它會顯示在 [!UICONTROL 分數] 欄。 這代表產品組合中每個專案的分數。
author: Alina
feature: Work Management, Strategic Planning
exl-id: 4451b1a3-57ae-4c66-a6a1-a85bd51a1648
source-git-commit: b6defd7dba91a06feb365ead74bd9c48f5165c77
workflow-type: tm+mt
source-wordcount: '727'
ht-degree: 1%

---

# 概觀 [!UICONTROL Portfolio優化程式] 分數

您可以找到 [!UICONTROL Portfolio優化程式] 在 [!UICONTROL Portfolio優化程式]. 它會顯示在 **[!UICONTROL 分數]** 欄。 這代表產品組合中每個專案的分數。

如需關於找到 [!UICONTROL Portfolio優化程式]，請參閱文章 [[!UICONTROL Portfolio優化程式] 概述](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md).

如需如何 [!DNL Adobe Workfront] 使用專案分數和其他專案資訊來最佳化 [!UICONTROL Portfolio優化程式]，請參閱 [在Portfolio優化程式中最佳化專案](../../../manage-work/portfolios/portfolio-optimizer/optimize-projects-in-portfolio-optimizer.md).

## 差異 [!UICONTROL 對齊分數] 和 [!UICONTROL Portfolio優化程式分數]

項目的對齊分數與產品組合優化程式分數之間存在差異。

專案的對齊分數會根據完成計分卡後取得的點數計算。 然後，系統會使用此分數來判斷產品組合對齊分數。 對齊分數會以百分比顯示。\
專案的對齊分數會顯示在 **[!UICONTROL 對齊方式]** 欄 [!UICONTROL Portfolio優化程式] 或 [!UICONTROL 對齊方式] 欄位 [!UICONTROL 業務案例摘要].

![](assets/business-case-summary-aligned-field-highlighted.png)

![](assets/project-alignment-score-portfolio-optimizer-highlighted-350x174.png)

如需有關產生專案對齊分數的詳細資訊，請參閱文章 [將計分卡套用至專案並產生對齊分數](../../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md).

此 [!UICONTROL 產品組合優化程式] 分數是自動在 [!UICONTROL Portfolio優化程式] 可優先處理項目。 產品組合最佳化程式分數會以指標圖示的形式顯示，並附上數字，並顯示在 **[!UICONTROL 分數]** 欄 [!UICONTROL Portfolio優化程式].

>[!NOTE]
>
>專案可在 [!UICONTROL Portfolio優化程式] 只有在其業務案例已完成時。 如需完成商業案例的詳細資訊，請參閱文章 [[!UICONTROL 建立業務案例] 的](../../../manage-work/projects/define-a-business-case/create-business-case.md).

![](assets/portfolio-optimizer-project-score-highlighted-350x132.png)

每個專案的分數會根據下列類別的重要性計算：

* [!UICONTROL 成本]
* [!UICONTROL 校準]
* [!UICONTROL 淨值]
* [!UICONTROL 收益風險]
* [!UICONTROL ROI]

## 計算 [!UICONTROL Portfolio優化程式] 分數

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: This was edited based on this issue, per Anna: https://hub.workfront.com/issue/603d0c58000095ea0bc00ce5e2110693/overview)</p>
-->

[!DNL Workfront] 會使用 [!UICONTROL Portfolio優化程式] 這是協助確定項目優先順序的排名。 產品組合中的值是基於在項目業務案例中輸入的值，用於計算項目的分數。 得分較高的項目可被認為更重要，可優先完成這些項目。

若要了解專案的排名，請執行下列動作：

1. 前往 [!UICONTROL Portfolio優化程式].
1. 將滑鼠指標暫留在排名圖示上，即可查看專案的產品組合最佳化程式分數。

![ranking_icon_in_portfolio_optimizer_new_png](assets/ranking-icon-in-portfolio-optimizer-new-350x160.png)

計算分數的演算法會考慮專案商業案例中概述的值，以及其所承載的加權。 它會為優化程式中的每個項目提供分數，並將該分數標準化，以便總有一個分數為100的項目。 這可為最佳專案帶來高分。

**範例：** 例如，若您將 [!UICONTROL 高對齊度] 唯一需要考慮的因素是，對齊率最高的專案得分為100。

以下是您可依據對專案評分的條件：

* [!UICONTROL 成本]
* [!UICONTROL 校準]
* [!UICONTROL 值]
* [!UICONTROL 收益風險]
* [!UICONTROL ROI]

![](assets/optimizer-sliding-value-options-350x77.png)

如需如何最佳化產品組合中專案的相關資訊，請參閱 [在 [!UICONTROL Portfolio優化程式]](../../../manage-work/portfolios/portfolio-optimizer/optimize-projects-in-portfolio-optimizer.md).

設定面板上的每個條件([!UICONTROL 成本], [!UICONTROL 對齊方式], [!UICONTROL ROI], [!UICONTROL 淨值], [!UICONTROL 收益風險])會根據您選取的項目，在0-100範圍內指定其加權。

對於具有完整商業案例的每個專案，系統會使用下列公式產生每個條件的分數：

```
Score Per Criteria = (Project Value For The Criteria - AVG(all the project values for this criteria)) / Standard Deviation of that value for that project
```

**範例：** 若 [!UICONTROL 對齊分數] 針對專案A，您會有下列項目：

```
Alignment Score = (Project A Alignment Score - AVG (of all the project Alignments)) / Standard Deviation of alignment score for that project
```

一旦你擁有了 [!UICONTROL 每個條件的分數] 計算後，您可考慮其權重將其加入，以取得每個專案的完整分數。 專案分數會使用下列公式計算：

```
Score = Cost Score * Cost Weight + Alignment Score * Alignment Weight + ROI Score * ROI Weight + Net Value Score * Net Value Weight + Risk Score * Risk Weight
```

就項目成本和 [!UICONTROL 風險] 邏輯與其他條件的運作方式相反：如果您想要 [!UICONTROL 低成本] 對您來說很重要，它不會增加但會降低專案的整體分數，依 `Cost Score * Cost Weight`.

計算每個專案的分數後， [!UICONTROL 最佳化分數] 會以下列方式為專案定義：

1. [!UICONTROL 最低] 和 [!UICONTROL 最大值] 分數已定義。
1. 系統會計算這些值之間的範圍。
1. 對於每個專案， [!UICONTROL 最佳化分數] 是使用下列公式計算：

   ```
   Optimization Score = Rounded ((Score - Minimum / Range)*100)
   ```
