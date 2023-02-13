---
content-type: overview
product-area: portfolios
navigation-topic: portfolio-optimizer
title: Portfolio優化程式概述
description: 此 [!UICONTROL Portfolio優化程式] 是用於項目評估和比較的工具。 審核和比較分配給產品組合的項目的業務案例值的過程是產品組合經理如何排列項目優先順序並為組織生成最大價值。
author: Alina
feature: Work Management, Strategic Planning
exl-id: 1e48a24c-65de-49c2-85a8-dc931ac40c52
source-git-commit: 4440fc50e988da6e446fd9a3195ae94f978b4b74
workflow-type: tm+mt
source-wordcount: '1654'
ht-degree: 0%

---

# [!UICONTROL Portfolio優化程式] 概述

此 [!UICONTROL Portfolio優化程式] 是用於項目評估和比較的工具。 審查和比較的過程 [!UICONTROL 業務案例] 指派給產品組合之專案的值，是產品組合經理如何為專案排定優先順序，並為組織產生最大價值。

此 [!UICONTROL 產品組合優化程式] 是提供一個介面，通過該介面，投資組合經理、指導委員會或產品管理辦公室可以查看有關每個項目的業務案例的摘要資訊。 然後，可以根據戰略價值和目標或根據其總體得分來確定項目的優先順序。

此 [!UICONTROL Portfolio優化程式] 只有在您已完成下列必要條件時，才能協助您：


* 此 [!UICONTROL 業務案例] 已經完成了。 如需詳細資訊，請參閱 [定義業務案例](../../projects/define-a-business-case/define-business-case.md).
* 在要複查的項目的「項目詳細資訊」部分的「項目概覽」區域中定義了一個產品組合
* 您已為要複查的項目指明了項目預算和計畫福利。 「固定成本」和「固定收入」是可選項，但可添加附加值。 如需詳細資訊，請參閱 [項目財務欄位](../../projects/project-finances/project-finances-overview-1.md).


如需關於找到 [!UICONTROL Portfolio優化程式]，請參閱 [找出 [!UICONTROL Portfolio優化程式]](../../../manage-work/portfolios/portfolio-optimizer/locate-portfolio-optimizer.md).

## 財務 [!UICONTROL Portfolio優化程式]

* [在 [!UICONTROL Portfolio優化程式]](#the-financial-areas-in-the-portfolio-optimizer)
* [中的財務欄位 [!UICONTROL Portfolio優化程式]](#the-financial-fields-in-the-portfolio-optimizer)

使用 [!UICONTROL Portfolio優化程式].

使用 [!UICONTROL Portfolio優化程式]:

* 專案在完成時各會獲得分數 [!UICONTROL 業務案例] 會根據 [!UICONTROL Portfolio優化程式]. 例如，低成本或高對齊項目獲得較高的分數。

   如需有關計算專案的產品組合最佳化程式分數的詳細資訊，請參閱文章 [概觀 [!UICONTROL Portfolio優化程式] 分數](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-score.md).

* 本公司之財務計算 [!UICONTROL Portfolio優化程式] 使用 [!UICONTROL 預算成本] 在 [!UICONTROL 業務案例] 的URL。
* 您可以在 [!UICONTROL Portfolio優化程式]，並考慮其所有相關資訊。 這包括財務資料、計分卡的一致性、ROI等。

### 在 [!UICONTROL Portfolio優化程式] {#the-financial-areas-in-the-portfolio-optimizer}

您可以在以下區域查看財務資訊： [!UICONTROL Portfolio優化程式]:

* **[!UICONTROL Portfolio標題]**:此區域顯示從產品組合中的所有項目收集的財務資訊。 它會顯示在Portfolio物件的每個標籤上。
* **[!UICONTROL Portfolio選定項目的財務]**:此區域顯示從以下項目中選取的項目收集的財務資訊： [!UICONTROL Portfolio優化程式]. 您可以添加或刪除項目，並通過查看此區域中的資訊了解這將如何影響產品組合的財務。
* **[!UICONTROL 項目財務]**:此區域會顯示 [!UICONTROL Portfolio優化程式].

### 中的財務欄位 [!UICONTROL Portfolio優化程式] {#the-financial-fields-in-the-portfolio-optimizer}

下列財務欄位顯示在 [!UICONTROL Portfolio優化程式]:

* [Portfolio標題](#portfolio-header)
* [Portfolio選定項目的財務](#portfolio-finances-for-selected-projects)

#### Portfolio標題 {#portfolio-header}

![](assets/portfolio-header-nwe-350x14.png)

[!DNL Adobe Workfront] 使用狀態僅等於的項目的資訊來計算產品組合題頭中的財務欄位 [!UICONTROL 已核准] 或 [!UICONTROL 目前].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>欄位名稱</strong> </th> 
   <th><strong>說明</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL準時]</td> 
   <td> <p>產品組合中被視為[!UICONTROL On Time]的項目百分比。 這可從Portfolio內的任何索引標籤看到。</p> <p>專案時，專案會視為[!UICONTROL On Time] <strong>[!UICONTROL條件]</strong> is <strong>目標上的[!UICONTROL]</strong>. <br>如需[!UICONTROL專案條件]的詳細資訊，請參閱文章 <a href="../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md" class="MCXref xref">專案條件和條件類型概觀</a>.</p> <p>此 <strong>[!UICONTROL準時]</strong> 百分比是使用下列公式計算：</p> <p><em>[!UICONTROL On TimePortfolio百分比] = [!UICONTROL On Time]項目數/ [!UICONTROL當前]或[!UICONTROL已批准]狀態中的項目總數</em> </p> </td> 
  </tr> 
  <tr> 
   <td>[！預算上的UICONTROL]</td> 
   <td> <p>產品組合中被視為[!UICONTROL On Budget]的項目百分比。 這可從[!UICONTROLPortfolio]內的任何標籤看到。</p> <p>專案包括 <strong>[！預算上的UICONTROL]</strong> 未超過預定預算時。 <br>如需專案預算的詳細資訊，請參閱文章 <a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref">項目財務區域中的[!UICONTROL管理]資訊</a>.</p> <p>[!UICONTROL預算上]百分比是使用下列公式計算的：</p> <p><em>[！預算Portfolio百分比上的UICONTROL] =預算上的[!UICONTROL]項目數/項目總數 </em><em>處於[!UICONTROL當前]或[!UICONTROL已批准]狀態</em> </p> </td> 
  </tr> 
  <tr> 
   <td>ROI（針對產品組合）</td> 
   <td> <p>此組合的[!UICONTROL投資回報](ROI)的計算方法是考慮[!UICONTROLPortfolio]的[!UICONTROL優勢]合計和項目的[!UICONTROL預算成本]合計。 這可從Portfolio內的任何索引標籤看到。</p> <p>PortfolioROI值是使用下列公式計算：</p> <p><em>PortfolioROI =（[!UICONTROL總收益] - [!UICONTROL總預算成本]）/ [!UICONTROL總成本] x 100</em> </p> <p>如需如何計算專案投資報酬率的詳細資訊，請參閱文章 <a href="../../../manage-work/projects/project-finances/calculate-roi.md" class="MCXref xref">計算投資回報(ROI)</a> .</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL對齊]或[!UICONTROL對齊分數] </td> 
   <td> <p>完成專案[!UICONTROL商業案例]中的[!UICONTROL計分卡]後計算的所有[!UICONTROL專案對齊分數]值的平均值。 每個項目的對齊分數會列在[!UICONTROLPortfolio優化程式]的[!UICONTROL對齊]列中。 這可從產品組合內的任何索引標籤看到。</p> <p>如需產生專案對齊分數的詳細資訊，請參閱文章 <a href="../../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md" class="MCXref xref">將計分卡套用至專案並產生對齊分數</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL淨值]</td> 
   <td> <p>產品組合中所有專案的所有[!UICONTROL淨值]之和。 這可從產品組合內的任何索引標籤看到。</p> <p>如需如何為專案計算[!UICONTROL淨值]的詳細資訊，請參閱文章 <a href="../../../manage-work/projects/project-finances/calculate-net-value.md" class="MCXref xref">計算淨值</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Portfolio選定項目的財務 {#portfolio-finances-for-selected-projects}

![](assets/portfolio-finances-for-selected-projects-in-optimizer-nwe-350x29.png)

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>欄位名稱</strong> </th> 
   <th> <p><strong>說明</strong> </p> <p> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL項目數]</td> 
   <td> <p>產品組合中作用中專案的總數。 在產品組合中被視為有效的專案可以處於下列任何狀態：</p> 
    <ul> 
     <li>[!UICONTROL當前]</li> 
     <li>[!UICONTROL規劃]</li> 
     <li>[!UICONTROL已批准]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL預算]</td> 
   <td>您可以手動更新此欄位，以指出整個產品組合的總預算。 此預算用於產品組合內的所有專案。 </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL剩餘]</td> 
   <td> <p>組合內所有項目的所有[!UICONTROL預算成本]之後的剩餘預算已從組合預算中扣除。</p> <p>[!UICONTROL剩餘Portfolio預算]使用以下公式計算：</p> <p><em>[!UICONTROL剩餘Portfolio預算] = [!UICONTROL總Portfolio預算] — 所有Portfolio項目的[!UICONTROL預算成本]合計</em> </p> <p>組合中所有項目的[!UICONTROL預算成本]總體值在「預算」欄位下的指標欄中表示。 </p> <p>如需追蹤專案成本的詳細資訊，請參閱文章<a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">追蹤成本</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL總成本]</td> 
   <td> <p>[!UICONTROLPortfolio優化程式]中顯示的所有項目的成本總和。 每個項目的成本與項目的[!UICONTROL預算成本]相同，它顯示在[!UICONTROL業務案例摘要]中。 </p> <p>有關[!UICONTROL業務案例]中項目的財務欄位的詳細資訊，請參閱文章中的「了解業務案例中的財務欄位」一節 <a href="../../../manage-work/projects/define-a-business-case/create-business-case.md" class="MCXref xref">為項目建立業務案例 </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL風險] </td> 
   <td> <p>產品組合中所有項目的所有[!UICONTROL潛在風險成本]的總和。 每個項目的[!UICONTROL潛在風險成本]列在[!UICONTROLPortfolio優化程式]的[!UICONTROL風險]列中。 </p> <p>有關計算項目風險的詳細資訊，請參閱文章 <a href="../../../manage-work/projects/project-finances/potential-risk-cost.md" class="MCXref xref">計算潛在風險成本 </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL優勢]</td> 
   <td> <p>產品組合中所有項目的所有[!UICONTROL計畫福利]值的總和。 每個項目的「計畫福利」值列在[!UICONTROLPortfolio優化程式]的[!UICONTROL福利]列中。 </p> <p>如需專案[!UICONTROL計畫效益]的詳細資訊，請參閱文章 <a href="../../../manage-work/projects/project-finances/project-planned-benefit.md" class="MCXref xref">項目計畫收益概覽</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL風險對淨值]指標</td> 
   <td> <p>考量[!UICONTROL潛在風險]值，同時考慮產品組合中所有項目提供的[!UICONTROL淨值]。 要在產品組合內實現最高效率，您希望看到[!UICONTROL風險]指標較低，而[!UICONTROL淨值]指標較高。 </p> <p>有關計算[!UICONTROL淨值]風險的詳細資訊，請參閱文章 <a href="../../../manage-work/portfolios/portfolio-optimizer/calculate-risk-to-net-value-in-portfolio.md" class="MCXref xref">計算投資組合中的淨值風險</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 自訂 [!UICONTROL Portfolio優化程式]

您只能自訂 [!UICONTROL Portfolio優化程式] 使用設定來變更清單中的資訊。

下列圖示和選項適用於 [!UICONTROL Portfolio優化程式]:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Portfolio優化程式中的圖示</td> 
   <td>名稱</td> 
   <td>函數</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/nwe-set-priority-icon.png"> </td> 
   <td>[!UICONTROL設定項目優先順序]</td> 
   <td>當您想要儲存專案順序時，請根據其優先順序使用此圖示。 </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/nwe-optimize-icon-in-optimizer.png"> </td> 
   <td>[!UICONTROL優化產品組合]</td> 
   <td>使用此表徵圖可根據項目的下列財務值優化產品組合：
    <ul>
     <li>[!UICONTROL成本]</li>
     <li>[!UICONTROL對齊]</li>
     <li>[!UICONTROL值]</li>
     <li>[!UICONTROL受益風險]</li>
     <li>[!UICONTROL ROI]</li>
    </ul><p>如需最佳化產品組合的詳細資訊，請參閱文章 <a href="../../../manage-work/portfolios/portfolio-optimizer/optimize-projects-in-portfolio-optimizer.md" class="MCXref xref">在[!UICONTROLPortfolio優化程式]中優化項目 </a>.</p></td> 
  </tr> 
  <tr> 
   <td> <img src="assets/nwe-undo-redo-icons-optimizer.png"> </td> 
   <td>[!UICONTROL撤消]/ [!UICONTROL重做]表徵圖</td> 
   <td>使用這些表徵圖可以取消或重做您在保存前對[!UICONTROLPortfolio優化程式]所做的更改。</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/hide-show-unselected-portfolio-optimizer-142x74.png" alt="hide_show_unselected_portfolio_optimizer.png" style="width: 142;height: 74;"> </td> 
   <td>[!UICONTROL顯示]/ [!UICONTROL隱藏未選中]項目</td> 
   <td>使用這些圖示來顯示或隱藏您未勾選之作品集中的專案。</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/nwe-export-optimizer-icon-350x173.png" style="width: 350;height: 173;"> </td> 
   <td>[!UICONTROL導出] </td> 
   <td> <p>使用此表徵圖可導出[!UICONTROLPortfolio優化程式]的[!UICONTROL項目優先順序]區域中的資料。 您可將其匯出為下列格式：</p> 
    <ul> 
     <li>PDF</li> 
     <li>[!DNL Excel]</li> 
     <li>[!UICONTROL Tab]分隔</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/preferences-portfolio-optimizer.png" alt="preferences_portfolio_optimizer.png"> </td> 
   <td>[!UICONTROL首選項]</td> 
   <td> <p>使用此表徵圖可修改[!UICONTROLPortfolio優化程式]列中顯示的項目欄位，或根據其狀態修改在[!UICONTROL優化程式]中顯示的項目。 </p> <p>提示：  
     <ul> 
      <li> <p>不是全部 [!DNL Workfront] 標準欄位可供新增至欄。 </p> </li> 
     </ul> 
     <ul> 
      <li> <p>您只能在產品組合中的任何專案中新增具有非零值的自訂欄位。</p> </li> 
     </ul> </p> </td> 
  </tr> 
 </tbody> 
</table>
