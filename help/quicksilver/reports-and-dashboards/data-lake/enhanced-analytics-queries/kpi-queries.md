---
content-type: overview;reference
product-area: reports and dashboards
navigation-topic: data connect
title: KPI查詢
description: 增強的Analytics查詢
author: Courtney
feature: Reports and Dashboards
recommendations: noDisplay, noCatalog
hide: true
hidefromtoc: true
source-git-commit: eccecaece64b78aa19444407b182ea80b2115a63
workflow-type: tm+mt
source-wordcount: '385'
ht-degree: 2%

---


# KPI查詢

您可以使用本文中的查詢來建立類似於Enhanced Analytics中的資料視覺效果。

>[!IMPORTANT]
>
>查詢會產生類似於「增強型Analytics」中所顯示的結果，但可能不會完全相符。


## 先決條件

開始之前，您必須

1. 與您的Business Intelligence (BI)工具建立連線：
   1. [建立Snowflake的讀取器帳戶或連線](/help/quicksilver/reports-and-dashboards/data-lake/create-a-reader-account.md)
   1. [建立與Workfront資料連線的連線](/help/quicksilver/reports-and-dashboards/data-lake/share-data-externally.md)

建立連線後，您可以使用本檔案中的查詢來擷取及視覺化資料。

## 已完成專案

「已完成專案KPI」會顯示篩選期間內已完成多少專案，以及百分比自上一個時段以來如何增加或減少。 在這些數字下方，您可以看到上一個時段完成的專案數目，以及上一個時段中的天數。

![個KPI專案已完成](assets/kpi-projects-completed-350x182.png)

### 查詢

```
WITH completedProjectsInRange as ( 
SELECT COUNT(t0.PROJECTID) as PROJECT_COUNT FROM PROJECTS_CURRENT t0 
WHERE t0.ACTUALCOMPLETIONDATE >= '2025-01-01' 
AND t0.ACTUALCOMPLETIONDATE <= '2025-01-31' 
), completedProjectsPreviousRange as ( 
SELECT COUNT(t0.PROJECTID) as PROJECT_COUNT FROM PROJECTS_CURRENT t0 
WHERE t0.ACTUALCOMPLETIONDATE >= '2024-12-01' 
AND t0.ACTUALCOMPLETIONDATE <= '2024-12-31' 
), rawChange as ( 
SELECT (a.PROJECT_COUNT - b.PROJECT_COUNT) as CHANGE_FROM_PREVIOUS_PERIOD FROM completedProjectsInRange a, completedProjectsPreviousRange b 
), percentChange as ( 
SELECT  
CASE 
WHEN a.PROJECT_COUNT = b.PROJECT_COUNT THEN 0.00 
WHEN b.PROJECT_COUNT > 0 THEN ((a.PROJECT_COUNT - b.PROJECT_COUNT) / b.PROJECT_COUNT * 100) 
END AS PERCENT_CHANGE_FROM_PREVIOUS_PERIOD 
FROM completedProjectsInRange a, completedProjectsPreviousRange b 
) 
SELECT 
a.PROJECT_COUNT, 
b.PROJECT_COUNT as PREVIOUS_PROJECT_COUNT, 
c.CHANGE_FROM_PREVIOUS_PERIOD, 
d.PERCENT_CHANGE_FROM_PREVIOUS_PERIOD 
FROM completedProjectsInRange a, completedProjectsPreviousRange b, rawChange c, 
percentChange d
```

## 已準時完成專案

「準時完成專案」KPI會顯示篩選期間內準時完成專案的百分比，以及自上一個時段以來該百分比如何增加或減少。 在這些數字下方，您可以看到上一個時段準時完成的專案百分比，以及上一個時段中的天數。

![個KPI專案已於時間](assets/kpi-projects-completed-on-time-350x180.png)完成

## 平均 專案期間

平均 專案期間KPI會顯示實際結束日期在篩選期間內之專案的平均完成時間量（以天、周或年為單位），以及百分比自上一個期間以來如何增加或減少。 在這些數字底下，您可以看到具有前一個時段中實際結束日期之專案的平均完成時間量，以及前一個時段中的天數。

![KPI平均專案期間](assets/kpi-avg.-project-duration-350x168.png)

## 每專案平均任務數

「每專案平均任務數」KPI會顯示篩選期間內指派給專案的平均任務數，以及自上一個時段以來百分比增加或減少的方式。 在這些數字下方，您可以看到在前一個時段內指派給專案的平均任務數，以及前一個時段內的天數。

每個專案的![KPI平均任務數](assets/kpi-average-tasks-per-project-350x179.png)