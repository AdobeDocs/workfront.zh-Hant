---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: 計算淨值
description: 專案的淨值，是計算專案的收益並移除成本後，專案的總預期值。
author: Lisa
feature: Work Management
exl-id: 44e3f211-c816-4ee1-aafc-c40fc8732f1a
source-git-commit: 6afa65f921864403c10541d283ef717dce81aed7
workflow-type: tm+mt
source-wordcount: '397'
ht-degree: 1%

---

# 計算淨值

專案的淨值，是計算專案的收益並移除成本後，專案的總預期值。

## 專案淨值概觀

Adobe Workfront會使用下列公式計算專案的「淨值」：

```
Project Net Value = Planned Benefit - Budgeted Cost - Potential Risk Cost
```

下列欄位可能會影響專案的淨值：

* **計畫權益**：這是專案所有者完成業務案例的&#x200B;**專案資訊**&#x200B;區域時所指定的手動專案。\
  如需有關專案計畫權益的詳細資訊，請參閱文章[業務案例領域概觀](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md)中的[專案資訊](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md#project-info)區段。

* **預算成本**：這是您首次啟動專案時所預估的與專案相關的總成本。

  **預算成本**&#x200B;使用&#x200B;**預算勞力成本**&#x200B;值，該值是在業務案例的資源預算區域中計算的，並考慮到資源規劃工具中工作角色的預算時數以及每個工作角色的每小時成本費率。\
  預算成本會影響專案的&#x200B;**淨值**。 如需如何計算預算成本的詳細資訊，請參閱[計算預算成本](../../../manage-work/projects/project-finances/budgeted-cost.md)。

* **潛在風險成本**：這是與專案上任何風險相關的成本，如業務案例或專案的[風險]索引標籤中所定義。\
  如需有關計算專案潛在風險成本的詳細資訊，請參閱文章[計算潛在風險成本](../../../manage-work/projects/project-finances/potential-risk-cost.md)。

   

## 找出專案淨值

您可以在Workfront的下列區域中找到專案的淨值：

* 在業務案例的摘要區域中 \
  如需業務案例摘要區域的詳細資訊，請參閱文章[建立專案的業務案例](../../../manage-work/projects/define-a-business-case/create-business-case.md) [建立專案的業務案例](../../../manage-work/projects/define-a-business-case/create-business-case.md)中的「瞭解業務案例摘要」一節。

  ![](assets/net-value-on-business-case-summary-highlighted-350x444.png)

* 在Portfolio最佳化工具中（若專案與專案組合相關聯）

  >[!TIP]
  >
  >所有專案淨值的總計是投資組合的淨值。

  如需有關Portfolio最佳化程式的詳細資訊，請參閱[Portfolio最佳化程式概述](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md)。

* 在下列清單和報告的「專案淨值」欄位中：

   * 專案
   * 任務
   * 問題
   * 專案 (財務資料)

  如需有關建立報告的詳細資訊，請參閱文章[建立自訂報告](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)。
