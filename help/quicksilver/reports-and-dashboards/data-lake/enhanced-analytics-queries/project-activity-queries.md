---
content-type: overview;reference
product-area: reports and dashboards
navigation-topic: data connect
title: 專案活動查詢
description: 增強的Analytics查詢
author: Courtney
feature: Reports and Dashboards
recommendations: noDisplay, noCatalog
exl-id: b7155160-4537-4919-bebf-72056b181bb6
source-git-commit: da5c7197b3826855bae5dd3d3bf2ba9d07d7f188
workflow-type: tm+mt
source-wordcount: '178'
ht-degree: 0%

---

# 專案活動查詢

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

## 專案使用者的登入事件

顯示指派給專案在指定日期登入的人員數量。

```
WITH userlogins as ( 
    SELECT 
        userid, 
        lastlogindate 
    FROM ( 
        SELECT 
            userid, 
            lastlogindate, 
            lag(lastlogindate, 1, '1990-01-01') OVER (PARTITION BY userid ORDER BY begin_effective_timestamp) as previous_login 
        FROM users_event 
    ) 
    WHERE lastlogindate != previous_login 
) 
 
SELECT 
    tds.projectid, 
    ads.calendardate, 
    count(1) 
FROM assignments_daily_history ads 
    INNER JOIN tasks_daily_history tds ON ads.taskid = tds.taskid AND tds.calendardate = ads.calendardate 
    INNER JOIN userlogins ul ON ads.assignedtoid = ul.userid and TO_DATE(ul.lastlogindate) = ads.calendardate 
GROUP BY tds.projectid, ads.calendardate
```

### 專案使用者的登入事件：深入研究

```
WITH userlogins as ( 
    SELECT 
        userid, 
        lastlogindate 
    FROM ( 
        SELECT 
            userid, 
            lastlogindate, 
            lag(lastlogindate, 1, '1990-01-01') OVER (PARTITION BY userid ORDER BY begin_effective_timestamp) as previous_login 
        FROM users_event 
    ) 
    WHERE lastlogindate != previous_login 
) 

SELECT 
    tds.projectid, 
    ul.userid, 
    ads.calendardate, 
    count(1) 
FROM assignments_daily_history ads 
INNER JOIN tasks_daily_history tds ON ads.taskid = tds.taskid AND tds.calendardate = ads.calendardate 
INNER JOIN userlogins ul ON ads.assignedtoid = ul.userid AND TO_DATE(ul.lastlogindate) = ads.calendardate 
group by tds.projectid, ul.userid, ads.calendardate
 
```

## 專案使用者的任務狀態變更事件

顯示在指定日期變更專案之任務狀態的人數。

```
WITH task_status_changes as (  
    SELECT 
        taskid, 
        status, 
        begin_effective_timestamp  
    FROM (  
        SELECT 
            taskid, 
            status, 
            begin_effective_timestamp, 
            lag(status, 1, 'NOSTATUS') OVER (PARTITION BY taskid ORDER BY begin_effective_timestamp) as previous_status 
        FROM tasks_event 
        WHERE status != 'CPL' 
    )  
    WHERE status != previous_status  
)  
 
SELECT 
    tds.projectid, 
    count(tds.status), 
    ads.calendardate 
FROM assignments_daily_history ads 
    INNER JOIN tasks_daily_history tds ON ads.taskid = tds.taskid AND tds.calendardate = ads.calendardate 
    INNER JOIN task_status_changes tsc ON tsc.taskid = ads.taskid AND tsc.taskid = tds.taskid and TO_DATE(tsc.begin_effective_timestamp) = tds.calendardate 
GROUP BY tds.projectid, ads.calendardate
```

### 專案使用者的任務狀態變更事件：深入研究

```
WITH task_status_changes as (  
    SELECT 
        taskid, 
        status, 
        lastupdatedbyid, 
        begin_effective_timestamp  
    FROM (  
        SELECT 
            taskid, 
            status, 
            begin_effective_timestamp, 
            lastupdatedbyid, 
            lag(status, 1, 'NOSTATUS') OVER (PARTITION BY taskid ORDER BY begin_effective_timestamp) as previous_status  
        FROM tasks_event  
        WHERE status != 'CPL'  
    )  
    WHERE status != previous_status  
)  
 
SELECT 
    tds.projectid, 
    tsc.lastupdatedbyid, 
    count(tsc.status), 
    ads.calendardate 
FROM assignments_daily_history ads 
    INNER JOIN tasks_daily_history tds ON ads.taskid = tds.taskid AND tds.calendardate = ads.calendardate 
    INNER JOIN task_status_changes tsc ON tsc.taskid = ads.taskid AND tsc.taskid = tds.taskid AND TO_DATE(tsc.begin_effective_timestamp) = tds.calendardate 
GROUP BY tds.projectid, tsc.lastupdatedbyid, ads.calendardate
```

## 專案使用者的任務完成事件

顯示在指定日期完成專案任務的人員數量。

```
WITH task_status_changes as (  
    SELECT 
        taskid, 
        status, 
        begin_effective_timestamp  
    FROM (  
        SELECT 
            taskid, 
            status, 
            begin_effective_timestamp, 
            lag(status, 1, 'NOSTATUS') OVER (PARTITION BY taskid ORDER BY begin_effective_timestamp) as previous_status  
        FROM tasks_event  
        WHERE status = 'CPL'  
    )  
    WHERE status != previous_status  
) 
 
SELECT 
    tds.projectid, 
    count(tds.status), 
    ads.calendardate 
FROM assignments_daily_history ads 
    INNER JOIN tasks_daily_history tds ON ads.taskid = tds.taskid and tds.calendardate = ads.calendardate 
    INNER JOIN task_status_changes tsc ON tsc.taskid = ads.taskid and tsc.taskid = tds.taskid and TO_DATE(tsc.begin_effective_timestamp) = tds.calendardate 
GROUP BY tds.projectid, ads.calendardate
```

### 專案使用者的任務完成事件：深入研究

```
WITH task_status_changes as (  
    SELECT 
        taskid, 
        status, 
        lastupdatedbyid, 
        begin_effective_timestamp  
    FROM (  
        SELECT 
            taskid, 
            status, 
            begin_effective_timestamp, 
            lastupdatedbyid, 
            lag(status, 1, 'NOSTATUS') OVER (PARTITION BY taskid ORDER BY begin_effective_timestamp) as previous_status  
        FROM tasks_event  
        WHERE status = 'CPL'  
    )  
    WHERE status != previous_status  
)  
 
SELECT 
    tds.projectid, 
    tsc.lastupdatedbyid, 
    count(tsc.status), 
    ads.calendardate 
FROM assignments_daily_history ads 
    INNER JOIN tasks_daily_history tds ON ads.taskid = tds.taskid AND tds.calendardate = ads.calendardate 
    INNER JOIN task_status_changes tsc ON tsc.taskid = ads.taskid AND tsc.taskid = tds.taskid AND TO_DATE(tsc.begin_effective_timestamp) = tds.calendardate 
GROUP BY tds.projectid, tsc.lastupdatedbyid, ads.calendardate
```
