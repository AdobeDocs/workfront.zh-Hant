---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: 計算潛在風險成本
description: 專案的潛在風險成本會考慮專案風險的潛在成本及其發生的可能性。
author: Lisa
feature: Work Management
exl-id: f4dc1950-efd8-4936-83fd-1280ee465923
source-git-commit: 6afa65f921864403c10541d283ef717dce81aed7
workflow-type: tm+mt
source-wordcount: '302'
ht-degree: 0%

---

# 計算潛在風險成本

專案的潛在風險成本會考慮專案風險的潛在成本及其發生的可能性。

## 專案潛在風險成本概要

Adobe Workfront使用下列公式計算專案的潛在風險成本：

```
Potential Risk Cost =SUM(Potential Risk Costs * Risk Probability)
```

複查專案的潛在風險成本時，請考量下列事項：

* 專案的計畫風險成本與潛在風險成本相同。
* 潛在風險成本未併入專案的計畫成本中。 而是用來決定其淨值。

## 找出專案的潛在風險成本

您可以在Workfront的下列區域中找到專案的風險及其潛在成本：

* 在專案的「風險」標籤中。
* 在業務案例摘要中。\
  如需有關專案商業案例的詳細資訊，請參閱文章[為專案建立商業案例](../../../manage-work/projects/define-a-business-case/create-business-case.md)。
* 在專案報告中，當您新增計畫風險成本欄位至報告欄位時。\
  如需在Workfront中建立報表的詳細資訊，請參閱文章[建立自訂報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)。

* 在Portfolio最佳化工具中，當專案與Portfolio相關聯時，在「風險」欄中。\
  投資組合中所有專案的所有潛在風險成本總和會加總至Portfolio的風險。\
  如需有關Portfolio最佳化程式的詳細資訊，請參閱文章[Portfolio最佳化程式概述](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md)。

如需有關在專案上建立風險的詳細資訊，請參閱文章[在專案上建立和編輯風險](../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md)

如需有關專案商業案例的詳細資訊，請參閱文章[為專案建立商業案例](../../../manage-work/projects/define-a-business-case/create-business-case.md)。
