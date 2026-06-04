---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: 計算潛在風險成本
description: 專案的潛在風險成本會考慮專案風險的潛在成本及其發生的可能性。
author: Lisa
feature: Work Management
exl-id: f4dc1950-efd8-4936-83fd-1280ee465923
TQID: https://experienceleague.adobe.com/32kwPUhdtWhFeqQ34oReoU8xl2JlaWQeZlq7MI1jqtc
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2: id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 302
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

* 在Portfolio Optimizer中，當專案與Portfolio相關聯時，在「風險」欄中。\
  投資組合中所有專案的所有潛在風險成本加總，構成了Portfolio的風險。\
  如需Portfolio Optimizer的詳細資訊，請參閱文章[Portfolio Optimizer概觀](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md)。

如需有關在專案上建立風險的詳細資訊，請參閱文章[在專案上建立和編輯風險](../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md)

如需有關專案商業案例的詳細資訊，請參閱文章[為專案建立商業案例](../../../manage-work/projects/define-a-business-case/create-business-case.md)。
