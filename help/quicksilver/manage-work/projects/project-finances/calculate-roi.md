---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: 計算投資回報(ROI)
description: 投資回報(ROI)是Adobe Workfront指標，使投資組合經理能夠根據項目的原始計畫效益和預算成本快速查看項目的執行情況。
author: Alina
feature: Work Management
exl-id: 1a3d16cb-8cb1-472e-8102-0ea8e0bc0edd
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '348'
ht-degree: 0%

---

# 計算投資回報(ROI)

投資回報(ROI)是Adobe Workfront指標，使投資組合經理能夠根據項目的原始計畫效益和預算成本快速查看項目的執行情況。

## 項目投資回報(ROI)概述

Workfront使用下列公式計算ROI:

```
Project ROI = [(Project Planned Benefit - Project Budgeted Cost) / Project Budgeted Cost] x 100
```

以下欄位會影響專案的ROI:

* **項目計畫收益**:這是在完成業務案例的「項目資訊」區域時由項目所有者指定的手動輸入。 這是您作為專案擁有者所認為，如果您完成專案，可能會是專案的好處。 這是特定貨幣量，且必須為正值。\
   有關項目計畫效益的詳細資訊，請參閱文章中的「項目資訊」部分 [為項目建立業務案例](../../../manage-work/projects/define-a-business-case/create-business-case.md).

* **項目預算成本**：這是初次啟動專案時預估的與專案相關的總成本。

   此 **預算成本** 使用 **預算人工成本** 在「業務案例」的「資源預算」區域中計算的值，它考慮了資源計畫員中任務職責的預算小時數以及每個任務職責的「每小時成本」費率。\
   如需詳細資訊，請參閱 [計算預算成本](../../../manage-work/projects/project-finances/budgeted-cost.md).

## 找到項目投資回報(ROI)

您可以在Workfront的下列區域中檢視專案的ROI值：

* 在Portfolio優化程式中，如果項目與產品組合關聯

   >[!NOTE]
   >
   >所有項目ROI值的總計是產品組合的ROI。

   如需Portfolio優化程式的相關資訊，請參閱文章 [Portfolio優化程式概述](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md).

* 在項目ROI欄位中，以下清單和報告： 

   * 專案
   * 任務
   * 問題
   * 項目（財務資料）
   如需在Workfront中建立報表的詳細資訊，請參閱文章 [建立自訂報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
