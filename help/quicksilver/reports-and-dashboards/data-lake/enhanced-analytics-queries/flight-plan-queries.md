---
content-type: overview;reference
product-area: reports and dashboards
navigation-topic: data connect
title: 小眾測試版計畫查詢
description: 增強的Analytics查詢
author: Courtney
feature: Reports and Dashboards
recommendations: noDisplay, noCatalog
exl-id: afa58d44-fd5c-48ee-aeb8-58888aaacb28
source-git-commit: da5c7197b3826855bae5dd3d3bf2ba9d07d7f188
workflow-type: tm+mt
source-wordcount: '99'
ht-degree: 1%

---

# 小眾測試版計畫查詢

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

## 專案計畫時數調整（日期範圍內）

```
WITH VALID_PROJECTS AS ( 
    SELECT 
        projectid, 
        plannedstartdate as projectplannedstartdate, 
        plannedcompletiondate as projectplannedcompletiondate, 
        actualstartdate as projectactualstartdate, 
        actualcompletiondate as projectactualcompletiondate, 
        condition as projectcondition, 
        name as projectname, 
        status, 
        groupid, 
        conditiontype, 
        calendardate as snapshotdate 
    FROM PROJECTS_DAILY_HISTORY 
    WHERE nvl(trim(deleted),'-1') != '1' 
        AND ( 
            to_date(actualcompletiondate) > '2021-01-01' 
            OR actualcompletiondate is NULL 
        ) 
), VALID_CUSTOMENUMS AS ( 
    SELECT 
        distinct valueasstring, 
        groupid, 
        enumclass, 
        equateswith, 
        label, 
        calendardate 
    FROM CUSTOMENUMS_DAILY_HISTORY 
), VALID_TASKS AS ( 
    SELECT 
        projectid, 
        taskid, 
        plannedminutes, 
        planneddurationminutes, 
        completedminutes, 
        completedplannedminutes, 
        completedplanneddurationminutes, 
        taskcompleted, 
        numberofchildren, 
        snapshotdate, 
        CASE 
            WHEN actualcompletiondate is not NULL or percentcomplete = '100' or status='CPL' THEN 0 
            ELSE plannedminutes - completedplannedminutes 
        END as remainingminutes, 
        CASE 
            WHEN actualcompletiondate is not NULL or percentcomplete = '100' or status='CPL' THEN 0 
            ELSE planneddurationminutes - completedplanneddurationminutes 
        END as remainingdurationminutes 
    FROM ( 
        SELECT 
            a.projectid,a.taskid, 
            a.actualcompletiondate, 
            a.percentcomplete, 
            a.numberofchildren, 
            a.plannedminutes, 
            a.planneddurationminutes, 
            a.completedminutes, 
            a.completedplannedminutes, 
            a.completedplanneddurationminutes, 
            a.snapshotdate, 
            a.status, 
            CASE 
                WHEN a.actualcompletiondate is not NULL or a.percentcomplete = '100' or a.status='CPL' THEN 1 
                ELSE 0 
            END as taskcompleted 
        FROM ( 
            SELECT 
                distinct 
                    t.projectid,t.taskid, 
                    t.actualcompletiondate, 
                    t.percentcomplete, 
                    t.numberofchildren, 
                    t.workrequired as plannedminutes, 
                    t.plannedDurationMinutes as planneddurationminutes, 
                    t.actualwork as completedminutes, 
                    round((t.workrequired * t.percentcomplete)/100) as completedplannedminutes, 
                    round((t.plannedDurationMinutes * t.percentcomplete)/100) as completedplanneddurationminutes, 
                    t.groupid, 
                    t.status, 
                    t.calendardate as snapshotdate  
            FROM TASKS_DAILY_HISTORY t  
            WHERE nvl(trim(t.deleted),'-1') != '1' 
        ) a 
        INNER JOIN valid_projects v ON (a.projectid = v.projectid AND a.snapshotdate = v.snapshotdate) 
    ) 
), VALID_ISSUES AS ( 
    SELECT 
        projectid, 
        optaskid, 
        plannedminutes, 
        planneddurationminutes, 
        completedminutes, 
        completedplannedminutes, 
        completedplanneddurationminutes, 
        issueresolved, 
        calendardate as snapshotdate, 
        CASE 
            WHEN actualcompletiondate is not NULL or percentcomplete = '100' or equateswith='CLS' or (equateswith='CLS' and status='CLS') THEN 0 
            ELSE plannedminutes - completedplannedminutes 
        END as remainingminutes, 
        CASE  
            WHEN actualcompletiondate is not NULL or percentcomplete = '100' or equateswith='CLS' or (equateswith='CLS' and status='CLS') THEN 0 
            ELSE planneddurationminutes - completedplanneddurationminutes END as remainingdurationminutes 
    FROM ( 
        SELECT 
            projectid, 
            optaskid, 
            actualcompletiondate, 
            equateswith, 
            plannedminutes, 
            planneddurationminutes, 
            percentcomplete, 
            completedminutes, 
            status, 
            CASE 
                WHEN actualcompletiondate is not NULL or percentcomplete = '100' or equateswith = 'CLS' or (equateswith='CLS' and status='CLS') THEN 1 
                ELSE 0 
            END as issueresolved, 
            round((plannedminutes * percentcomplete)/100) as completedplannedminutes, 
            round((planneddurationminutes * percentcomplete)/100) as completedplanneddurationminutes, 
            calendardate 
        FROM ( 
            SELECT 
                a.projectid, 
                a.optaskid, 
                a.actualcompletiondate, 
                ce.equateswith, 
                a.plannedminutes, 
                a.planneddurationminutes, 
                a.completedminutes, 
                a.calendardate, 
                a.status, 
                CASE 
                    WHEN a.percentcomplete is not null THEN a.percentcomplete 
                    WHEN a.actualcompletiondate is not NULL or a.percentcomplete = '100' or ce.equateswith='CLS' or (ce.equateswith='CLS' and a.status='CLS') THEN 100 
                    ELSE 0 
                END as percentcomplete 
            FROM ( 
                SELECT 
                    distinct t.projectid, 
                    t.optaskid, 
                    t.actualcompletiondate, 
                    t.workrequired as plannedminutes, 
                    t.planneddurationminutes as planneddurationminutes, 
                    t.actualworkrequired as completedminutes, 
                    t.calendardate as calendardate, 
                    t.percentcomplete, 
                    t.status, 
                FROM OPTASKS_DAILY_HISTORY t 
                WHERE nvl(trim(t.deleted),'-1') != '1' 
                    AND t.optasktype in ('ISU','BUG') 
            ) a 
            INNER JOIN VALID_PROJECTS v ON (a.projectid=v.projectid AND a.calendardate = v.snapshotdate)  
            LEFT JOIN VALID_CUSTOMENUMS ce ON (ce.valueasstring = a.status AND ce.groupid = v.groupid AND a.projectid = v.projectid AND ce.enumclass='STATUS_OPTASK' AND a.calendardate = ce.calendardate) 
        ) 
    ) 
), AGGREGATE_TASKS AS ( 
    SELECT 
        projectid, 
        snapshotdate, 
        SUM(CASE WHEN numberofchildren=0 THEN plannedminutes ELSE 0 END) as plannedminutes, 
        SUM(CASE WHEN numberofchildren=0 THEN planneddurationminutes ELSE 0 END) as planneddurationminutes, 
        SUM(CASE WHEN numberofchildren=0 THEN completedminutes ELSE 0 END) as completedminutes, 
        SUM(CASE WHEN numberofchildren=0 THEN completedplannedminutes ELSE 0 END) as completedplannedminutes, 
        SUM(CASE WHEN numberofchildren=0 THEN completedplanneddurationminutes ELSE 0 END) as completedplanneddurationminutes, 
        SUM(CASE WHEN numberofchildren=0 THEN remainingminutes ELSE 0 END) as remainingminutes, 
        SUM(CASE WHEN numberofchildren=0 THEN remainingdurationminutes ELSE 0 END) as remainingdurationminutes, 
        count(CASE WHEN numberofchildren=0 THEN taskid ELSE NULL END) as totaltaskcount, 
        SUM(CASE WHEN numberofchildren=0 THEN taskcompleted ELSE 0 END) as totalcompletedtaskcount 
    FROM valid_tasks 
    GROUP BY projectid, snapshotdate 
), AGGREGATE_ISSUES AS ( 
    SELECT 
        projectid, 
        snapshotdate, 
        SUM(plannedminutes) as issueplannedminutes, 
        SUM(planneddurationminutes) as issueplanneddurationminutes, 
        SUM(completedminutes) as issuecompletedminutes, 
        SUM(completedplannedminutes) as issuecompletedplannedminutes, 
        SUM(completedplanneddurationminutes) as issuecompletedplanneddurationminutes, 
        SUM(remainingminutes) as issueremainingminutes, 
        SUM(remainingdurationminutes) as issueremainingdurationminutes, 
        count(optaskid) as totalissuecount, 
        SUM(issueresolved) as totalresolvedissue 
    FROM valid_issues 
    GROUP BY projectid, snapshotdate 
) 
     
SELECT 
    p.projectid as projectguid, 
    p.projectname, 
    p.projectplannedstartdate as projectplannedstartdate, 
    p.projectplannedcompletiondate as projectplannedcompletiondate, 
    p.projectactualstartdate as projectactualstartdate, 
    p.projectactualcompletiondate as projectactualcompletiondate, 
    p.projectcondition as projectcond, 
    coalesce(t.plannedminutes, 0) as plannedminutes, 
    coalesce(t.planneddurationminutes, 0) as planneddurationminutes, 
    coalesce(t.completedminutes, 0) as completedminutes, 
    coalesce(t.completedplannedminutes, 0) as completedplannedminutes, 
    coalesce(t.completedplanneddurationminutes,0) as completedplanneddurationminutes, 
    coalesce(t.remainingminutes,0) as remainingminutes, 
    coalesce(t.remainingdurationminutes, 0) as remainingdurationminutes, 
    coalesce(cast(t.totaltaskcount as Integer),0) - coalesce(cast(pt.totaltaskcount as Integer),0) as taskaddeddaily, 
    coalesce(cast(t.totalcompletedtaskcount as Integer),0) - coalesce(cast(pt.totalcompletedtaskcount as Integer),0) as taskcompleteddaily, 
    coalesce(t.plannedminutes,0) - coalesce(pt.plannedminutes,0) as plannedminutesdaily, 
    coalesce(t.planneddurationminutes,0) - coalesce(pt.planneddurationminutes,0) as planneddurationminutesdaily, 
    coalesce(t.completedminutes,0) - coalesce(pt.completedminutes,0) as completedminutesdaily, 
    coalesce(t.completedplannedminutes,0) - coalesce(pt.completedplannedminutes,0) as completedplannedminutesdaily, 
    coalesce(t.completedplanneddurationminutes,0) - coalesce(pt.completedplanneddurationminutes,0) as completedplanneddurationminutesdaily, 
    CASE 
        WHEN ce.equateswith='CPL' THEN TRUE 
        WHEN ce.equateswith is NULL and p.status='CPL' THEN TRUE 
        ELSE FALSE 
    END as iscompleted, 
    coalesce(cast(t.totaltaskcount as Integer),0) as totaltaskcount, 
    coalesce(cast(t.totalcompletedtaskcount as Integer),0) as totalcompletedtaskcount, 
    coalesce(i.issueplannedminutes, 0) as issueplannedminutes, 
    coalesce(i.issueplanneddurationminutes, 0) as issueplanneddurationminutes, 
    coalesce(i.issuecompletedminutes, 0) as issuecompletedminutes, 
    coalesce(i.issuecompletedplannedminutes, 0) as issuecompletedplannedminutes, 
    coalesce(i.issuecompletedplanneddurationminutes,0) as issuecompletedplanneddurationminutes, 
    coalesce(i.issueremainingminutes,0) as issueremainingminutes, 
    coalesce(i.issueremainingdurationminutes, 0) as issueremainingdurationpminutes, 
    coalesce(cast(i.totalissuecount as Integer),0) - coalesce(cast(pi.totalissuecount as Integer),0) as issueaddeddaily, 
    coalesce(cast(i.totalresolvedissue as Integer),0) - coalesce(cast(pi.totalresolvedissue as Integer),0) as issueresolveddaily, 
    coalesce(i.issueplannedminutes,0) - coalesce(pi.issueplannedminutes,0) as issueplannedminutesdaily, 
    coalesce(i.issueplanneddurationminutes,0) - coalesce(pi.issueplanneddurationminutes,0) as issueplanneddurationminutesdaily, 
    coalesce(i.issuecompletedminutes,0) - coalesce(pi.issuecompletedminutes,0) as issuecompletedminutesdaily, 
    coalesce(i.issuecompletedplannedminutes,0) - coalesce(pi.issuecompletedplannedminutes,0) as issuecompletedplannedminutesdaily, 
    coalesce(i.issuecompletedplanneddurationminutes,0) - coalesce(pi.issuecompletedplanneddurationminutes,0) as issuecompletedplanneddurationminutesdaily, 
    coalesce(cast(i.totalissuecount as Integer),0) as totalissuecount, 
    coalesce(cast(i.totalresolvedissue as Integer),0) as totalresolvedissue, 
    convert_timezone('UTC',current_timestamp)::timestamp_ntz as dl_load_ts, 
    ce2.equateswith as conditionequateswith, 
    ce2.label as conditionlabel, 
    p.status as status, 
    ce.equateswith as statusequateswith, 
    ce.label as statuslabel, 
    split_part(p.status, ':', 2) as statuspending, 
    p.conditiontype as projectconditiontype, 
    CASE  
        WHEN p.conditiontype = 'PG' THEN 'PROGRESS STATUS' 
        WHEN p.conditiontype = 'MN' THEN 'MANUAL' 
    END as projectconditiontypename 
FROM valid_projects p 
    LEFT JOIN ( 
        SELECT 
            customenumid, 
            enumclass, 
            calendardate, 
            label, 
            equateswith 
        FROM CUSTOMENUMS_DAILY_HISTORY) ce ON (ce.enumclass = 'STATUS_PROJ' AND p.status = ce.label AND ce.calendardate = p.snapshotdate) 
    LEFT JOIN aggregate_tasks t ON (p.snapshotdate = t.snapshotdate AND t.projectid = p.projectid) 
    LEFT JOIN aggregate_issues i ON (p.snapshotdate = i.snapshotdate AND i.projectid = p.projectid) 
    LEFT JOIN aggregate_tasks pt ON (p.snapshotdate = dateadd(days,1,pt.snapshotdate) AND p.projectid = pt.projectid) 
    LEFT JOIN aggregate_issues pi ON (p.snapshotdate = dateadd(days,1,pi.snapshotdate) AND p.projectid = pi.projectid) 
    LEFT JOIN ( 
        SELECT 
            customenumid, 
            enumclass, 
            calendardate, 
            label, 
            equateswith 
        FROM CUSTOMENUMS_DAILY_HISTORY) ce2 ON (ce2.enumclass = 'CONDITION_PROJ' AND p.projectcondition = ce2.label AND ce2.calendardate = p.snapshotdate)
```
