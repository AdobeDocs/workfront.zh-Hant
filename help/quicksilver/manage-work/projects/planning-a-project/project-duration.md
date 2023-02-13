---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: 專案期間概觀
description: Adobe Workfront會考慮最早任務的開始日期和最新任務的完成日期，計算項目的持續時間，並計算兩個日期之間的天數。
author: Alina
feature: Work Management
exl-id: b558eaad-669b-4079-b61a-07df227edfa2
source-git-commit: bbd64e9deed1b89d720272508b3562c354578704
workflow-type: tm+mt
source-wordcount: '253'
ht-degree: 2%

---

# 專案期間概觀

Adobe Workfront會考慮最早任務的開始日期和最新任務的完成日期，計算項目的持續時間，並計算兩個日期之間的天數。

## 專案持續時間

項目的持續時間按以下公式計算：

```
Project Duration = Completion Date of the latest task - Start Date of the earliest task
```

>[!NOTE]
>
>專案問題的持續時間不會影響專案的持續時間。

項目持續時間根據與項目關聯的計畫或分配給任務的用戶計算兩個任務日期之間的天數。 如需Workfront用來計算持續時間的排程相關資訊，請參閱 [排程概觀](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/schedules-overview.md).

## 專案期間類型

「專案持續時間」有兩種類型，而Workfront計算公式有兩種：

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Check these formulas? Should they be divided by the hours per day?!) </p>
-->

* **計畫持續時間**: 

   ```
   Project Planned Duration = Planned Completion Date of the latest task - Planned Start Date of the earliest task / Typical hour per day
   ```

* **實際期間**: 

   ```
   Project Actual Duration = Actual Completion Date of the latest task - Actual Start Date of the earliest task / Typical hour per day
   ```

## 找出專案持續時間

您可以在以下區域找到項目計畫期間和實際持續時間：Workfront

* .在「專案詳細資料」區域的「概述」區段中。

   如需專案的「概述」子標籤的詳細資訊，請參閱文章 [在項目概覽區域中管理資訊](../../../manage-work/projects/manage-projects/understand-project-overview-area.md).

* 在「專案」報表中，在報表中加入「持續時間」或「實際持續時間」欄位。

   如需建立報表的詳細資訊，請參閱文章 [建立自訂報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
