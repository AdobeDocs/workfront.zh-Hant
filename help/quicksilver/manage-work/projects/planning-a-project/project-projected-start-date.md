---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: 項目預計起始日期概覽
description: 「預計起始日期」是根據項目上第一個任務的「預計起始日期」即時的項目開始日期。
author: Alina
feature: Work Management
exl-id: 6277e6cf-0a73-4ba8-a3fd-c0da473dc5d4
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '428'
ht-degree: 0%

---

# 項目預計起始日期概覽

## 項目和任務的預計起始日期概覽

「預計起始日期」是根據項目上第一個任務的「預計起始日期」即時的項目開始日期。 

在首次計畫項目時，任務和項目的計畫起始日期和預計起始日期是相同的。 由於可能發生延遲或任務可能提前完成，預計起始日期可能與計畫起始日期不同。 

項目上第一個任務的預計起始日期中的更改將觸發項目預計起始日期中的更改。 

## 修改任務的預計起始日期

項目或任務的預計起始日期是Adobe Workfront完成的計算，無法人工修改。 

以下事件可以觸發任務的「預計開始日期」中的修改：

* 開始處理任務時，任務的實際起始日期將變為其預計起始日期。
* 如果任務的計畫起始日期通過，則預計起始日期將移至將來，指明任務可以開始的最早日期。\
   Workfront在計算任務的最早可用日期時，會考慮任務的計畫小時數，以及分配給任務的項目或用戶的計畫。 
* 滯後的前置任務會影響其從屬任務的「預計起始日期」。 從屬任務的「預計起始日期」根據前置任務關係的「相依類型」和前置任務的「預計日期」移動。 

如果其中任何任務是項目上的第一個任務，則項目的預計起始日期將更改為與此任務的預計起始日期匹配。 

## 查找項目或任務的預計起始日期

您可以在Workfront的以下區域找到項目或任務的預計開始日期：

* 您可以將其新增至專案或任務報表或檢視。

   如需建立報表的詳細資訊，請參閱文章 [建立自訂報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

* 在項目的「項目詳細資訊」部分或任務的「任務詳細資訊」部分。
