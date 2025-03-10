---
content-type: overview;reference
product-area: reports and dashboards
navigation-topic: data connect
title: KPI查詢
description: 增強的Analytics查詢
author: Courtney
feature: Reports and Dashboards
recommendations: noDisplay, noCatalog
exl-id: 9ca5574d-7bc5-4d9d-9ed7-4d5fad6f7857
source-git-commit: 905aaaa5d300bc71058dd6ee2d568c8fc1229570
workflow-type: tm+mt
source-wordcount: '406'
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

建立連線後，您可以使用本文中的查詢來擷取及視覺化資料。

## 已完成專案

「已完成專案KPI」會顯示篩選期間內已完成多少專案，以及百分比自上一個時段以來如何增加或減少。

您也可以檢視上一個時段中完成的專案數目，以及上一個時段中的天數。

![個KPI專案已完成](assets/kpi-projects-completed-350x182.png)

### 查詢

```
WITH completedProjectsInRange as ( 
    SELECT 
        COUNT(t0.PROJECTID) as PROJECT_COUNT 
    FROM PROJECTS_CURRENT t0 
    WHERE t0.ACTUALCOMPLETIONDATE >= '2025-01-01' 
        AND t0.ACTUALCOMPLETIONDATE <= '2025-01-31' 
), completedProjectsPreviousRange as ( 
    SELECT 
        COUNT(t0.PROJECTID) as PROJECT_COUNT 
    FROM PROJECTS_CURRENT t0 
    WHERE t0.ACTUALCOMPLETIONDATE >= '2024-12-01' 
        AND t0.ACTUALCOMPLETIONDATE <= '2024-12-31' 
), rawChange as ( 
    SELECT 
        (a.PROJECT_COUNT - b.PROJECT_COUNT) as CHANGE_FROM_PREVIOUS_PERIOD 
    FROM completedProjectsInRange a, completedProjectsPreviousRange b 
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

「準時完成專案」KPI會顯示篩選期間內準時完成專案的百分比，以及自上一個時段以來該百分比如何增加或減少。

您也可以檢視上一個時段準時完成的專案百分比，以及上一個時段內的天數。

![個KPI專案已於時間](assets/kpi-projects-completed-on-time-350x180.png)完成

```
WITH completedProjectsInRange as ( 
    SELECT 
        COUNT(t0.PROJECTID) as PROJECT_COUNT 
    FROM PROJECTS_CURRENT t0 
    WHERE t0.ACTUALCOMPLETIONDATE >= '2025-01-01' 
        AND t0.ACTUALCOMPLETIONDATE <= '2025-01-31' 
), completedOntimeProjectsInRange as ( 
    SELECT 
        COUNT(t0.PROJECTID) as PROJECT_COUNT 
    FROM PROJECTS_CURRENT t0 
    WHERE t0.ACTUALCOMPLETIONDATE >= '2025-01-01' 
        AND t0.ACTUALCOMPLETIONDATE <= '2025-01-31' 
        AND t0.PROGRESSSTATUS = 'ON' 
), percentOntimeProjects as ( 
    SELECT 
        CASE 
            WHEN a.PROJECT_COUNT = 0 THEN 0 
            ELSE ROUND(b.PROJECT_COUNT/a.PROJECT_COUNT) * 100 
        END as ONTIMEPROJECTPERCENT 
    FROM completedProjectsInRange a, completedOntimeProjectsInRange b 
), completedProjectsPreviousRange as ( 
    SELECT 
        COUNT(t0.PROJECTID) as PROJECT_COUNT 
    FROM PROJECTS_CURRENT t0 
    WHERE t0.ACTUALCOMPLETIONDATE >= '2024-12-01' 
        AND t0.ACTUALCOMPLETIONDATE <= '2024-12-31' 
), completedOntimeProjectsPreviousRange as ( 
    SELECT 
        COUNT(t0.PROJECTID) as PROJECT_COUNT 
    FROM PROJECTS_CURRENT t0 
    WHERE t0.ACTUALCOMPLETIONDATE >= '2024-12-01' 
        AND t0.ACTUALCOMPLETIONDATE <= '2024-12-31' 
        AND t0.PROGRESSSTATUS = 'ON' 
), percentOntimeProjectsPreviousRange as ( 
    SELECT 
        CASE 
            WHEN a.PROJECT_COUNT = 0 THEN 0 
            ELSE ROUND(b.PROJECT_COUNT/a.PROJECT_COUNT) * 100 
        END as ONTIMEPROJECTPERCENT 
    FROM completedProjectsPreviousRange a, completedOntimeProjectsPreviousRange b 
), rawChange as ( 
    SELECT 
        (a.ONTIMEPROJECTPERCENT - b.ONTIMEPROJECTPERCENT) as CHANGE_FROM_PREVIOUS_PERIOD 
    FROM percentOntimeProjects a, percentOntimeProjectsPreviousRange b 
), percentChange as ( 
    SELECT  
        CASE 
            WHEN a.ONTIMEPROJECTPERCENT = b.ONTIMEPROJECTPERCENT THEN 0 
            WHEN b.ONTIMEPROJECTPERCENT > 0 THEN ((a.ONTIMEPROJECTPERCENT - b.ONTIMEPROJECTPERCENT) / b.ONTIMEPROJECTPERCENT * 100) 
        END AS PERCENT_CHANGE_FROM_PREVIOUS_PERIOD 
    FROM percentOntimeProjects a, percentOntimeProjectsPreviousRange b 
) 

SELECT 
    a.ONTIMEPROJECTPERCENT, 
    b.ONTIMEPROJECTPERCENT as PREVIOUS_ONTIMEPROJECTPERCENT, 
    c.CHANGE_FROM_PREVIOUS_PERIOD, 
    d.PERCENT_CHANGE_FROM_PREVIOUS_PERIOD 
FROM percentOntimeProjects a, percentOntimeProjectsPreviousRange b, rawChange c, 
percentChange d
```

## 平均 專案期間

平均 專案期間KPI會顯示實際結束日期在篩選期間內之專案的平均完成時間量（以天、周或年為單位），以及百分比自上一個期間以來如何增加或減少。

您也可以檢視前一個時段內具有實際結束日期的專案平均完成時間量，以及前一個時段內的天數。

>[!NOTE]
>
>這僅計入已完成專案的持續時間。


![KPI平均專案期間](assets/kpi-avg.-project-duration-350x168.png)

```
WITH averageProjectDurationInRange as ( 
    SELECT 
        AVG(t0.ACTUALDURATIONMINUTES) as AVERAGE_PROJECT_DURATION 
    FROM PROJECTS_CURRENT t0 
    WHERE t0.ACTUALCOMPLETIONDATE >= '2025-01-01' 
        AND t0.ACTUALCOMPLETIONDATE <= '2025-01-31' 
), averageProjectPreviousRange as ( 
    SELECT AVG (t0. ACTUALDURATIONMINUTES) as AVERAGE_PROJECT_DURATION FROM PROJECTS_CURRENT t0 
    WHERE t0.ACTUALCOMPLETIONDATE >= '2024-12-01' 
        AND t0.ACTUALCOMPLETIONDATE <= '2024-12-31' 
), rawChange as ( 
    SELECT ((a.AVERAGE_PROJECT_DURATION - b.AVERAGE_PROJECT_DURATION) / 480) as CHANGE_FROM_PREVIOUS_PERIOD FROM averageProjectDurationInRange a, averageProjectPreviousRange b 
), percentChange as ( 
    SELECT  
        CASE 
            WHEN a.AVERAGE_PROJECT_DURATION = b.AVERAGE_PROJECT_DURATION THEN 0 
            WHEN b.AVERAGE_PROJECT_DURATION > 0 THEN ((a.AVERAGE_PROJECT_DURATION - b.AVERAGE_PROJECT_DURATION)  / b.AVERAGE_PROJECT_DURATION) * 100 
        END AS PERCENT_CHANGE_FROM_PREVIOUS_PERIOD 
        FROM averageProjectDurationInRange a, averageProjectPreviousRange b 
) 
 
SELECT 
    a.AVERAGE_PROJECT_DURATION, 
    b.AVERAGE_PROJECT_DURATION as PREVIOUS_AVERAGE_PROJECT_DURATION, 
    c.CHANGE_FROM_PREVIOUS_PERIOD, 
    d.PERCENT_CHANGE_FROM_PREVIOUS_PERIOD 
FROM averageProjectDurationInRange a, averageProjectPreviousRange b, rawChange c, 
percentChange d
```

## 每專案平均任務數

「每專案平均任務數」KPI會顯示篩選期間內指派給專案的平均任務數，以及自上一個時段以來百分比增加或減少的方式。

您也可以檢視上一個時段內指派給專案的平均任務數，以及上一個時段內的天數。

每個專案的![KPI平均任務數](assets/kpi-average-tasks-per-project-350x179.png)

```
WITH tasksPerProjectInRange as ( 
    SELECT 
        COUNT(t0.TASKID) as TASK_COUNT 
    FROM TASKS_CURRENT t0 
        LEFT JOIN PROJECTS_CURRENT t1 ON t1.PROJECTID = t0.PROJECTID 
    WHERE 
        ( 
            t1.PLANNEDSTARTDATE >= '2025-01-01' 
            AND t1.PLANNEDSTARTDATE <= '2025-01-31' 
        ) 
        OR ( 
            t1.PLANNEDCOMPLETIONDATE >= '2025-01-01' 
            AND t1. PLANNEDCOMPLETIONDATE <= '2025-01-31' 
        ) 
        OR ( 
            t1.PLANNEDSTARTDATE <= '2025-01-01' 
            AND t1. PLANNEDCOMPLETIONDATE >= '2025-01-31' 
        ) 
    GROUP BY t0.PROJECTID 
), averageTasksPerProjectInRange as ( 
    SELECT AVG(TASK_COUNT) AS AVERAGE_TASK_COUNT FROM tasksPerProjectInRange 
), tasksPerProjectInPreviousRange as ( 
    SELECT 
        COUNT(t0.TASKID) as TASK_COUNT 
    FROM TASKS_CURRENT t0 
        LEFT JOIN PROJECTS_CURRENT t1 ON t1.PROJECTID = t0.PROJECTID 
    WHERE 
        ( 
            t1.PLANNEDSTARTDATE >= '2024-12-01' 
            AND t1.PLANNEDSTARTDATE <= '2024-12-31' 
        ) 
        OR ( 
            t1.PLANNEDCOMPLETIONDATE >= '2024-12-01' 
            AND t1. PLANNEDCOMPLETIONDATE <= '2024-12-31' 
        ) 
        OR ( 
            t1.PLANNEDSTARTDATE <= '2024-12-01' 
            AND t1. PLANNEDCOMPLETIONDATE >= '2024-12-31' 
        ) 
    GROUP BY t0.PROJECTID 
), averageTasksPerProjectInPreviousRange as ( 
    SELECT 
        AVG(TASK_COUNT) AS AVERAGE_TASK_COUNT 
        FROM tasksPerProjectInPreviousRange 
), rawChange as ( 
    SELECT 
        (a.AVERAGE_TASK_COUNT - b.AVERAGE_TASK_COUNT) as CHANGE_FROM_PREVIOUS_PERIOD 
    FROM averageTasksPerProjectInRange a, averageTasksPerProjectInPreviousRange b 
), percentChange as ( 
    SELECT 
        CASE 
            WHEN a.AVERAGE_TASK_COUNT = b.AVERAGE_TASK_COUNT THEN 0 
            WHEN b.AVERAGE_TASK_COUNT > 0 THEN ((a.AVERAGE_TASK_COUNT - b.AVERAGE_TASK_COUNT) / b.AVERAGE_TASK_COUNT) * 100  
        END as PERCENT_CHANGE_FROM_PREVIOUS_PERIOD 
    FROM averageTasksPerProjectInRange a, averageTasksPerProjectInPreviousRange b 
) 
 
SELECT 
    a.AVERAGE_TASK_COUNT, 
    b.AVERAGE_TASK_COUNT as PREVIOUS_AVERAGE_TASK_COUNT, 
    c.CHANGE_FROM_PREVIOUS_PERIOD, 
    d.PERCENT_CHANGE_FROM_PREVIOUS_PERIOD 
FROM averageTasksPerProjectInRange a, averageTasksPerProjectInPreviousRange b, rawChange c, percentChange d
```

## 疑難排解

* **沒有結果**：如果您的查詢未傳回任何結果，請檢查以確定是否正確複製雙引號和單引號。