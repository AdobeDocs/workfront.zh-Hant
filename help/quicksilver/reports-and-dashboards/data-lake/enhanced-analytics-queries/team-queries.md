---
content-type: overview;reference
product-area: reports and dashboards
navigation-topic: data connect
title: 依團隊查詢的活動
description: 增強的Analytics查詢
author: Courtney
feature: Reports and Dashboards
recommendations: noDisplay, noCatalog
exl-id: 6f07e52b-b813-4b3a-9333-0c9300e051ca
source-git-commit: da5c7197b3826855bae5dd3d3bf2ba9d07d7f188
workflow-type: tm+mt
source-wordcount: '172'
ht-degree: 0%

---

# 依團隊查詢的活動

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

## 主團隊的使用者登入事件 

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
    uc.hometeamid, 
    TO_DATE(ul.lastlogindate), 
    count(*) 
FROM users_current uc 
    INNER JOIN userlogins ul ON uc.userid = ul.userid 
WHERE hometeamid is not null 
GROUP BY uc.hometeamid, TO_DATE(ul.lastlogindate) 
```

### 主團隊的使用者登入事件：深入研究

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
    uc.hometeamid, 
    uc.userid, 
    TO_DATE(ul.lastlogindate), 
    count(*) 
FROM users_current uc 
    INNER JOIN userlogins ul ON uc.userid = ul.userid 
WHERE hometeamid is not null 
GROUP BY uc.hometeamid, uc.userid, TO_DATE(ul.lastlogindate)
```

## 團隊使用者的登入事件

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
    tmc.teamid, 
    TO_DATE(ul.lastlogindate), 
    count(*) 
FROM teammembers_current tmc 
    inner join teams_current tc on tc.teamid = tmc.teamid and tc.teamtype != 'PROJECT' 
    inner join userlogins ul on tmc.userid = ul.userid 
WHERE tmc.teamid is not null 
GROUP BY tmc.teamid, TO_DATE(ul.lastlogindate)
```

### 團隊使用者的登入事件：深入研究

```
WITH userlogins as ( 
    SELECT userid, lastlogindate 
    FROM ( 
        SELECT userid, lastlogindate, lag(lastlogindate, 1, '1990-01-01') OVER (PARTITION BY userid  ORDER BY begin_effective_timestamp) as previous_login 
        FROM users_event 
    ) 
    WHERE lastlogindate != previous_login 
) 
 
SELECT tmc.teamid, tmc.userid, TO_DATE(ul.lastlogindate), count(*) 
FROM teammembers_current tmc 
    INNER JOIN teams_current tc ON tc.teamid = tmc.teamid AND tc.teamtype != 'PROJECT' 
    INNER JOIN userlogins ul ON tmc.userid = ul.userid 
WHERE tmc.teamid is not null 
GROUP BY tmc.teamid, tmc.userid, TO_DATE(ul.lastlogindate)
```



## 主團隊使用者的任務狀態變更事件 

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
    uc.hometeamid, 
    TO_DATE(tsc.begin_effective_timestamp), 
    count(tsc.taskid) as task_status_updates 
FROM users_current uc 
    INNER JOIN assignments_current ac ON uc.userid = ac.assignedtoid 
    INNER JOIN task_status_changes tsc ON ac.taskid = tsc.taskid 
WHERE hometeamid is not null 
GROUP BY uc.hometeamid,  TO_DATE(tsc.begin_effective_timestamp)
```

### 主團隊使用者的任務狀態變更事件：深入研究

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
    uc.hometeamid, 
    uc.userid, 
    TO_DATE(tsc.begin_effective_timestamp), 
    count(tsc.taskid) as task_status_updates 
FROM users_current uc 
    INNER JOIN assignments_current ac ON uc.userid = ac.assignedtoid 
    INNER JOIN task_status_changes tsc ON ac.taskid = tsc.taskid 
WHERE hometeamid is not null 
GROUP BY uc.hometeamid, uc.userid, TO_DATE(tsc.begin_effective_timestamp)
```

## 團隊使用者的任務狀態變更事件

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

SELECT tmc.teamid,  TO_DATE(tsc.begin_effective_timestamp), count(tsc.taskid) as task_status_updates  
FROM teammembers_current tmc 
    INNER JOIN teams_current tc ON tc.teamid = tmc.teamid AND tc.teamtype != 'PROJECT' 
    INNER JOIN assignments_current ac ON tmc.userid = ac.assignedtoid  
    INNER JOIN task_status_changes tsc ON ac.taskid = tsc.taskid  
WHERE tmc.teamid is not null  
GROUP BY tmc.teamid,  TO_DATE(tsc.begin_effective_timestamp) 
```

### 團隊使用者的任務狀態變更事件：深入研究

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
    tmc.teamid, 
    tmc.userid, 
    TO_DATE(tsc.begin_effective_timestamp), 
    count(tsc.taskid) as task_status_updates  
FROM teammembers_current tmc 
    inner join teams_current tc ON tc.teamid = tmc.teamid AND tc.teamtype != 'PROJECT' 
    inner join assignments_current ac ON tmc.userid = ac.assignedtoid  
    inner join task_status_changes tsc ON ac.taskid = tsc.taskid  
WHERE tmc.teamid is not null  
GROUP BY tmc.teamid, tmc.userid, TO_DATE(tsc.begin_effective_timestamp) 
```

## 主團隊的使用者任務完成事件

```
WITH task_status_done as ( 
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
        FROM tasks_event te 
        WHERE status = 'CPL' 
    ) 
    WHERE status != previous_status 
), task_percentage_done as ( 
    SELECT 
        taskid, 
        percentcomplete, 
        begin_effective_timestamp 
    FROM ( 
        SELECT 
            taskid, 
            percentcomplete, 
            begin_effective_timestamp, 
            lag(percentcomplete, 1, '0') OVER (PARTITION BY taskid ORDER BY begin_effective_timestamp) as previous_percent_complete 
        FROM tasks_event 
        WHERE TO_NUMBER(percentcomplete) = 100 
    ) 
    WHERE percentcomplete != previous_percent_complete 
), task_completion_date_exists as ( 
    SELECT 
        taskid, 
        actualcompletiondate 
    FROM tasks_event 
    WHERE actualcompletiondate is not null 
) 
 
SELECT 
    uc.hometeamid, 
    TO_DATE(tasks_done.task_completion_date), 
    count(tasks_done.taskid) as task_completed 
FROM users_current uc 
    INNER JOIN assignments_current ac ON uc.userid = ac.assignedtoid  
    INNER JOIN ( 
        SELECT distinct taskid, task_completion_date 
        FROM ( 
            SELECT taskid, TO_DATE(begin_effective_timestamp) as task_completion_date 
            FROM task_status_done 
            UNION  
            SELECT taskid, TO_DATE(begin_effective_timestamp) as task_completion_date 
            FROM task_percentage_done 
            UNION 
            SELECT taskid, TO_DATE(actualcompletiondate) as task_completion_date 
            FROM task_completion_date_exists 
        )  
    ) tasks_done ON ac.taskid = tasks_done.taskid 
WHERE uc.hometeamid is not null 
GROUP BY uc.hometeamid, TO_DATE(tasks_done.task_completion_date)
```

### 主團隊的使用者任務完成事件：深入研究

```
WITH task_status_done as ( 
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
        FROM tasks_event te 
        WHERE status = 'CPL' 
    ) 
    WHERE status != previous_status 
), task_percentage_done as ( 
    SELECT 
        taskid, 
        percentcomplete, 
        begin_effective_timestamp 
    FROM ( 
        SELECT 
            taskid, 
            percentcomplete, 
            begin_effective_timestamp, 
            lag(percentcomplete, 1, '0') OVER (PARTITION BY taskid ORDER BY begin_effective_timestamp) as previous_percent_complete 
        FROM tasks_event 
        WHERE TO_NUMBER(percentcomplete) = 100 
    ) 
    WHERE percentcomplete != previous_percent_complete 
), task_completion_date_exists as ( 
    SELECT 
        taskid, 
        actualcompletiondate 
    FROM tasks_event 
    WHERE actualcompletiondate is not null 
) 
 
SELECT 
    uc.hometeamid, 
    uc.userid, 
    TO_DATE(tasks_done.task_completion_date), 
    count(tasks_done.taskid) as task_completed 
FROM users_current uc 
    INNER JOIN assignments_current ac ON uc.userid = ac.assignedtoid  
    INNER JOIN ( 
        SELECT distinct taskid, task_completion_date 
        FROM ( 
            SELECT taskid, TO_DATE(begin_effective_timestamp) as task_completion_date 
            FROM task_status_done 
            UNION  
            SELECT taskid, TO_DATE(begin_effective_timestamp) as task_completion_date 
            FROM task_percentage_done 
            UNION 
            SELECT taskid, TO_DATE(actualcompletiondate) as task_completion_date 
            FROM task_completion_date_exists 
        ) 
    ) tasks_done ON ac.taskid = tasks_done.taskid 
WHERE uc.hometeamid is not null 
GROUP BY uc.hometeamid, uc.userid, TO_DATE(tasks_done.task_completion_date) 
```

## 團隊使用者的任務完成事件

```
WITH task_status_done as ( 
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
        FROM tasks_event te 
        WHERE status = 'CPL' 
    ) 
    WHERE status != previous_status 
), task_percentage_done as ( 
    SELECT 
        taskid, 
        percentcomplete, 
        begin_effective_timestamp 
    FROM ( 
        SELECT 
            taskid, 
            percentcomplete, 
            begin_effective_timestamp, 
            lag(percentcomplete, 1, '0') OVER (PARTITION BY taskid ORDER BY begin_effective_timestamp) as previous_percent_complete 
        FROM tasks_event 
        WHERE TO_NUMBER(percentcomplete) = 100 
    ) 
    WHERE percentcomplete != previous_percent_complete 
), task_completion_date_exists as ( 
    SELECT 
        taskid, 
        actualcompletiondate 
    FROM tasks_event 
    WHERE actualcompletiondate is not null 
) 
 
SELECT 
    tmc.teamid, 
    TO_DATE(tasks_done.task_completion_date), 
    count(tasks_done.taskid) as task_completed 
FROM teammembers_current tmc 
    INNER JOIN teams_current tc ON tc.teamid = tmc.teamid and tc.teamtype != 'PROJECT' 
    INNER JOIN assignments_current ac ON tmc.userid = ac.assignedtoid  
    INNER JOIN ( 
        SELECT distinct taskid, task_completion_date 
        FROM ( 
            SELECT taskid, TO_DATE(begin_effective_timestamp) as task_completion_date 
            FROM task_status_done 
            UNION  
            SELECT taskid, TO_DATE(begin_effective_timestamp) as task_completion_date 
            FROM task_percentage_done 
            UNION 
            SELECT taskid, TO_DATE(actualcompletiondate) as task_completion_date 
            FROM task_completion_date_exists 
        )  
    ) tasks_done ON ac.taskid = tasks_done.taskid 
WHERE tmc.teamid is not null 
GROUP BY tmc.teamid, TO_DATE(tasks_done.task_completion_date) 
```

### 團隊使用者的任務完成事件：深入研究

```
WITH task_status_done as ( 
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
        FROM tasks_event te 
        WHERE status = 'CPL' 
    ) 
    WHERE status != previous_status 
), task_percentage_done as ( 
    SELECT 
        taskid, 
        percentcomplete, 
        begin_effective_timestamp 
    FROM ( 
        SELECT 
            taskid, 
            percentcomplete, 
            begin_effective_timestamp, 
            lag(percentcomplete, 1, '0') OVER (PARTITION BY taskid ORDER BY begin_effective_timestamp) as previous_percent_complete 
        FROM tasks_event 
        WHERE TO_NUMBER(percentcomplete) = 100 
    ) 
    WHERE percentcomplete != previous_percent_complete 
), task_completion_date_exists as ( 
    SELECT taskid, actualcompletiondate 
    FROM tasks_event 
    WHERE actualcompletiondate is not null 
) 
 
SELECT 
    tmc.teamid, 
    tmc.userid, 
    TO_DATE(tasks_done.task_completion_date), 
    count(tasks_done.taskid) as task_completed 
FROM teammembers_current tmc 
    INNER JOIN teams_current tc ON tc.teamid = tmc.teamid AND tc.teamtype != 'PROJECT' 
    INNER JOIN assignments_current ac ON tmc.userid = ac.assignedtoid  
    INNER JOIN ( 
        SELECT distinct taskid, task_completion_date 
        FROM ( 
            SELECT taskid, TO_DATE(begin_effective_timestamp) as task_completion_date 
            FROM task_status_done 
            UNION  
            SELECT taskid, TO_DATE(begin_effective_timestamp) as task_completion_date 
            FROM task_percentage_done 
            UNION 
            SELECT taskid, TO_DATE(actualcompletiondate) as task_completion_date 
            FROM task_completion_date_exists 
        )  
    ) tasks_done ON ac.taskid = tasks_done.taskid 
WHERE tmc.teamid is not null 
GROUP BY tmc.teamid, tmc.userid, TO_DATE(tasks_done.task_completion_date) 
```
