---
content-type: overview
product-area: projects
navigation-topic: task-information
title: 專案完成百分比總覽
description: 專案的完成百分比值是根據專案中任務的規劃期間或規劃時數來計算。 您的Adobe Workfront管理員或群組管理員會定義在系統中計算完成百分比時，在「專案偏好設定」區域中設定資訊時要考慮的值。 如需有關設定專案偏好設定的資訊，請參閱設定系統範圍的專案偏好設定。
author: Alina
feature: Work Management
exl-id: d2395569-9fe5-42e7-a392-cff49eb519d9
source-git-commit: 816fd70642ffb7b24095602ce160421aa947e2a6
workflow-type: tm+mt
source-wordcount: '778'
ht-degree: 0%

---

# 專案完成百分比總覽

<!-- Audited 01/2024 -->

專案的完成百分比值是根據專案中任務的期間或計畫時數而計算的。 您的Adobe Workfront管理員或群組管理員會定義在系統中計算完成百分比時，在「專案偏好設定」區域中設定資訊時要考慮的值。

如需有關設定專案偏好設定的資訊，請參閱[設定全系統的專案偏好設定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)。

父系任務的完成百分比取決於其每個子任務的期間或計畫時數。

同樣地，專案的完成百分比是根據專案中每個主要任務的持續時間或計畫時數。

主要任務是父系任務及沒有子系的獨立任務。

>[!TIP]
>
>主要任務未在專案計畫中縮排。

## Workfront計算完成百分比的方式

### 更新任務的完成百分比 {#update-the-percent-complete-on-a-task}

您可以手動修改任務的完成百分比。 這不是計算。

Workfront使用個別任務的完成百分比來計算其上層任務的完成百分比或專案的完成百分比。

如需更新任務完成百分比的資訊，請參閱[檢視並更新任務的完成百分比](../../../manage-work/projects/updating-work-in-a-project/view-update-percent-complete-for-tasks.md)。

### Workfront如何計算父系任務的完成百分比 {#how-workfront-calculates-percent-complete-on-a-parent-task}

根據您的Workfront或群組管理員在系統或群組層級的「專案偏好設定」中所選取的專案，系統會根據任務的期間或計畫時數計算父任務的完成百分比。

請考量下列情況：

* 如果系統根據計畫時數計算完成百分比，則父級任務完成百分比會使用下列公式計算：

  `Parent Task Percent Complete = (((Task 1 Planned Hours * Task 1 Percent Complete) + (Task 2 Planned Hours * Task 2 Percent Complete))/Total Planned Hours of Parent)*100`

  父系的計畫時數總計表示每個子系的所有計畫時數總和。

  ![](assets/project-with-tasks-percent-complete-planned-hours-calculation.png)

* 如果系統根據「工期」計算完成百分比，則使用下列公式計算父級任務完成百分比：

  `Parent Task Percent Complete = (((Task 1 Duration * Task 1 Percent Complete) + (Task 2 Duration * Task 2 Percent Complete))/ Total Duration of Parent)*100`

  ![](assets/project-with-tasks-percent-complete-duration-calculation.png)

  >[!IMPORTANT]
  >
  >「父系任務的總持續時間」是子系任務的所有持續時間的總計。 例如，如果父系任務有兩個子系且各自的「持續時間」為1天和2天，則其「總持續時間」為3天，即使兩個子系可以在同一天開始。


### Workfront計算專案完成百分比的方式 {#how-workfront-calculates-percent-complete-on-a-project}

根據您的Workfront或群組管理員在系統或群組層級的「專案偏好設定」中所選取的專案，專案的完成百分比會根據專案上主要任務的期間或計畫時數計算。

* 如果系統根據計畫時數計算完成百分比，則專案完成百分比會使用下列公式計算：

  `Project Percent Complete =(((Task 1 Planned Hours * Task 1 Percent Complete) + (Task 2 Planned Hours * Task 2 Percent Complete))/Total Planned Hours of the Project)*100`

  專案的總計畫時數是專案上所有主要任務的計畫時數總和。

  ![](assets/project-with-tasks-percent-complete-planned-hours-calculation.png)

  >[!NOTE]
  >
  >任務1或任務2隻能是父系任務或獨立任務。 此計算中未使用子系任務的計畫時數和完成百分比。

* 如果系統根據「持續時間」計算完成百分比，則使用下列公式計算專案完成百分比：

  `Project Percent Complete = (((Task 1 Duration * Task 1 Percent Complete) + (Task 2 Duration * Task 2 Percent Complete))/Duration of the Project)*100`

  >[!IMPORTANT]
  >
  >專案期間是顯示完成百分比之主要任務的所有期間總數。 例如，如果專案具有持續時間為2天的獨立任務，以及持續時間為5天的父任務，且已完成其工作，則專案的總持續時間為7天，即使這兩個任務可以在同一天開始。

  ![](assets/project-with-tasks-percent-complete-duration-calculation.png)

  >[!NOTE]
  >
  >任務1或任務2隻能是父系任務或獨立任務。 此計算中不會使用子系任務的持續期間和完成百分比。

## 使用期間的專案完成百分比範例

使用任務的期間來計算專案完成百分比時，請考慮以下範例：

![](assets/project-with-tasks-percent-complete-duration-calculation.png)

下列資訊可用來計算專案的完成百分比

* 獨立任務的完成百分比（任務1 - 20%）
* 父系任務的完成百分比（任務2 - 25%）
* 任務1的期間（5天）
* 任務2的期間（2天）
* 專案期間（7天）


若要使用「持續時間」計算專案的完成百分比：

`Project Percent Complete = (((Task 1 Duration * Task 1 Percent Complete) + (Task 2 Duration * Task 2 Percent Complete))/Duration of the Project)*100`

或

`(((5*0.2)+(2*0.25))/7)*100= 21.43%`


<!--drafted, this was the old example:

When using the Planned Duration of the tasks to calculate the percent complete of a project, consider the following example:

percent_complete_on_project_example.png

Only the parent task (Task 1) and the standalone task (Task 8) are used to calculate the percent complete of the project.

The secondary parents of Task 1 are used to calculate the percent complete of the main parent (Task 1).

To calculate the percent complete of the main parent (Task 1), first calculate the percent complete of its secondary parents:

Task 5 Percent Complete = ((14 * 0.75 + 12 * 0.25)/(12 + 14))*100 = 51.92%

Task 2 Percent Complete = ((5 * 0.7 + 2 * 0.5)/(5 + 2))*100 = 64.29 %

Then, to calculate the percent complete of the main parent (Task 1), use the following formula:

Task 1 Percent Complete =((56 * 0.5192 + 7 * 0.6429)/63)*100 = 53.29%

To calculate the percent complete of the project, you will need to have the following numbers ready:

Task 1 Duration (63 hours) and Percent Complete (53.29%)
Task 8 Duration (100 hours) and Percent Complete (4%)
Now, to calculate the percent complete of the project, use the following formula:

Project Percent Complete =((100 * 0.04 + 63 * 0.5329))/163)*100 = 23.05%
-->