---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: 專案期間概觀
description: Adobe Workfront會考量最早任務的「開始日期」與最近任務的「完成日期」來計算專案的「期間」，並計算兩個日期之間的天數。
author: Alina
feature: Work Management
exl-id: b558eaad-669b-4079-b61a-07df227edfa2
TQID: https://experienceleague.adobe.com/1j0nj2W5f7FtgIk46G3ePFA-zwt7VAyV9fQWKm2kZJ4
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40cid: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: ce22a157-dd2c-405f-b740-c2f204bb4c1aid: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 254
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

* . 在專案詳細資訊區域，在總覽區段。

  如需有關專案概述子標籤的詳細資訊，請參閱文章[專案概述區域中的管理資訊](../../../manage-work/projects/manage-projects/understand-project-overview-area.md)。

* 在專案報表中，加入報表中的「期間」或「實際期間」欄位。

  如需有關建立報告的詳細資訊，請參閱文章[建立自訂報告](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)。
