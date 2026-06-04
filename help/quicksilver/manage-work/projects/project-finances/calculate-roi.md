---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: 計算投資報酬率(ROI)
description: 投資報酬率(ROI)是Adobe Workfront的量度，可讓投資組合經理快速瞭解專案相對於專案原始計畫收益和預算成本的表現。
author: Lisa
feature: Work Management
exl-id: 1a3d16cb-8cb1-472e-8102-0ea8e0bc0edd
TQID: https://experienceleague.adobe.com/x7MGrAZbtlDd0oTePPgRdLQfUg8-M4GkkQdeWXUTyh4
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2:
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 348
ht-degree: 1%

---

# 計算投資報酬率(ROI)

投資報酬率(ROI)是Adobe Workfront的量度，可讓投資組合經理快速瞭解專案相對於專案原始計畫收益和預算成本的表現。

## 專案投資報酬率(ROI)概要

Workfront使用下列公式計算ROI：

```
Project ROI = [(Project Planned Benefit - Project Budgeted Cost) / Project Budgeted Cost] x 100
```

下列欄位會影響專案的ROI：

* **專案計畫權益**：這是專案所有者在完成業務案例的專案資訊區域時所指定的手動專案。 這是您身為專案所有者的預估值，您認為完成專案後，專案可能會受益。 這是特定數量的貨幣，且必須是正值。\
  如需有關專案計畫權益的詳細資訊，請參閱[為專案建立業務案例](../../../manage-work/projects/define-a-business-case/create-business-case.md)一文中的「專案資訊」一節。

* **專案預算成本**：這是您首次啟動專案時所預估的與專案相關的總成本。

  **預算成本**&#x200B;使用&#x200B;**預算勞力成本**&#x200B;值，該值是在業務案例的資源預算區域中計算的，並考慮到資源規劃工具中工作角色的預算時數以及每個工作角色的每小時成本費率。\
  如需詳細資訊，請參閱[計算預算成本](../../../manage-work/projects/project-finances/budgeted-cost.md)。

## 找到專案投資報酬率(ROI)

您可以在Workfront的下列區域中檢視專案的ROI值：

* 在Portfolio Optimizer中，如果專案與專案組合相關聯

  >[!NOTE]
  >
  >所有專案ROI值的總和即為產品組合的ROI。

  如需Portfolio Optimizer的相關資訊，請參閱文章[Portfolio Optimizer概觀](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md)。

* 在「專案ROI」欄位中的下列清單和報告中：

   * 專案
   * 任務
   * 問題
   * 專案 (財務資料)

  如需在Workfront中建立報表的詳細資訊，請參閱文章[建立自訂報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)。
