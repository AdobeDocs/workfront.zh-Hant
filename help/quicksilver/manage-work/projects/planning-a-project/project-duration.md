---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: 專案期間概觀
description: Adobe Workfront會考量最早任務的「開始日期」與最近任務的「完成日期」來計算專案的「期間」，並計算兩個日期之間的天數。
author: Alina
feature: Work Management
exl-id: b558eaad-669b-4079-b61a-07df227edfa2
source-git-commit: bbd64e9deed1b89d720272508b3562c354578704
workflow-type: tm+mt
source-wordcount: '253'
ht-degree: 0%

---

# 專案期間概觀

Adobe Workfront會考量最早任務的「開始日期」與最近任務的「完成日期」來計算專案的「期間」，並計算兩個日期之間的天數。

## 專案期間

專案期間的計算公式如下：

```
Project Duration = Completion Date of the latest task - Start Date of the earliest task
```

>[!NOTE]
>
>專案的問題期間不會影響專案期間。

專案期間會根據與專案關聯的排程或指派給任務的使用者，計算兩個任務日期之間的天數。 如需Workfront使用哪個排程來計算持續時間的詳細資訊，請參閱[排程總覽](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/schedules-overview.md)。

## 專案期間型別

「專案持續時間」有兩種型別，以及Workfront計算時所用的公式：

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Check these formulas? Should they be divided by the hours per day?!) </p>
-->

* **計畫期間**： 

  ```
  Project Planned Duration = Planned Completion Date of the latest task - Planned Start Date of the earliest task / Typical hour per day
  ```

* **實際持續時間**： 

  ```
  Project Actual Duration = Actual Completion Date of the latest task - Actual Start Date of the earliest task / Typical hour per day
  ```

## 找到專案持續時間

您可以在Workfront的下列區域中找到專案計畫和實際持續時間：

* 。在專案詳細資訊區域，在總覽區段。

  如需有關專案概述子標籤的詳細資訊，請參閱文章[專案概述區域中的管理資訊](../../../manage-work/projects/manage-projects/understand-project-overview-area.md)。

* 在專案報表中，加入報表中的「期間」或「實際期間」欄位。

  如需有關建立報告的詳細資訊，請參閱文章[建立自訂報告](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)。
