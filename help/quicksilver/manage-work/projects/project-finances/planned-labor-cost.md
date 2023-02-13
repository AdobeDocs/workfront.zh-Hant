---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: 計算計畫人工成本
description: 在您計畫項目上的工作時，Adobe Workfront會根據分配給此工作的職責和用戶的「每小時成本」值計算這些職責和用戶的計畫人工成本。
author: Alina
feature: Work Management
exl-id: af053e9a-09dc-4b4d-8ed4-f681ed611a59
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '309'
ht-degree: 0%

---

# 計算計畫人工成本

在您計畫項目上的工作時，Adobe Workfront會根據分配給此工作的職責和用戶的「每小時成本」值計算這些職責和用戶的計畫人工成本。

項目的計畫人工成本是與任務職責相關的成本或分配用於完成項目工作的用戶與每個職責或用戶完成該工作的計畫小時數（計畫小時數）之間的計算。

## 計畫人工成本概覽

此 **計畫人工成本** 通過添加項目上所有任務的所有計畫人工成本來計算項目的成本。

>[!TIP]
>
>沒有與問題或項目本身相關的計畫人工成本。

Workfront使用以下公式計算項目的計畫人工成本：

```
Project Planned Labor Cost= SUM(Tasks Planned Labor Cost)
```

任務計畫人工成本根據以下項目計算：

* 任務上的資源數及其分配給任務的個別分配
* 任務的成本類型。

任務計畫人工成本使用以下公式計算：

```
Task Planned Cost = Planned Hours x User or Job Role Cost Per Hour
```

有關Workfront如何根據任務分配和成本類型計算任務的計畫人工成本的詳細資訊，請參閱文章中的「修改單個任務的成本類型」部分 [追蹤成本](../../../manage-work/projects/project-finances/track-costs.md).

## 查找計畫人工成本

您可以在Workfront的以下區域找到項目的計畫人工成本：

* 專案報表
* 專案清單
* 一個基線報表，您可在其中追蹤一段時間
* 透過API

如需建立報表和使用Workfront API的相關資訊，請參閱下列文章：

* [建立自訂報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)
* [API 基本概念](../../../wf-api/general/api-basics.md)
