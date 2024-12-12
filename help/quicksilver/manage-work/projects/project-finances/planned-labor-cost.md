---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: 計算計畫勞力成本
description: 當您計畫專案上的工作時，Adobe Workfront會根據角色與使用者的每小時成本值，計算指派給此工作的角色與使用者的計畫勞力成本。
author: Lisa
feature: Work Management
exl-id: af053e9a-09dc-4b4d-8ed4-f681ed611a59
source-git-commit: 6afa65f921864403c10541d283ef717dce81aed7
workflow-type: tm+mt
source-wordcount: '309'
ht-degree: 0%

---

# 計算計畫勞力成本

當您計畫專案上的工作時，Adobe Workfront會根據角色與使用者的每小時成本值，計算指派給此工作的角色與使用者的計畫勞力成本。

專案的計畫勞力成本是與工作角色或指派完成專案工作的使用者相關聯的成本，與可能要求每個角色或使用者完成該工作的計畫時數金額（計畫時數）之間的計算。

## 計畫勞力成本概要

專案的&#x200B;**計畫勞力成本**&#x200B;的計算方式為加入專案上所有任務的所有計畫勞力成本。

>[!TIP]
>
>沒有與問題或與專案本身相關的計畫勞力成本。

Workfront會使用下列公式計算專案的計畫勞力成本：

```
Project Planned Labor Cost= SUM(Tasks Planned Labor Cost)
```

作業計畫勞力成本是根據下列專案計算：

* 任務上的資源數目及其配置給任務的個別資源
* 任務的成本型別。

作業計畫勞力成本使用下列公式計算：

```
Task Planned Cost = Planned Hours x User or Job Role Cost Per Hour
```

如需有關Workfront如何根據任務指派和成本型別計算任務計畫勞力成本的詳細資訊，請參閱文章[追蹤成本](../../../manage-work/projects/project-finances/track-costs.md)中的「修改個別任務的成本型別」一節。

## 找出計畫勞力成本

您可以在Workfront的下列區域中找到專案的計畫勞力成本：

* 專案報告
* 專案清單
* 您可以長期追蹤的基準線報告
* 透過API

如需建立報表和使用Workfront API的詳細資訊，請參閱下列文章：

* [建立自訂報告](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)
* [API 基本概念](../../../wf-api/general/api-basics.md)
