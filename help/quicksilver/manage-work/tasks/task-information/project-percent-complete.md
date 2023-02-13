---
content-type: overview
product-area: projects
navigation-topic: task-information
title: 專案完成百分比概觀
description: 項目的「完成百分比」值是根據項目中的「計畫持續時間」或「計畫小時數」來計算的。 您的Adobe Workfront管理員或群組管理員會定義在「專案偏好設定」區域中設定資訊時，在計算系統完成百分比時要考慮哪個值。 有關配置項目首選項的資訊，請參閱配置全系統項目首選項。
author: Alina
feature: Work Management
exl-id: d2395569-9fe5-42e7-a392-cff49eb519d9
source-git-commit: 31533bd7ee1890a8343d32770d623d5d9a6007d2
workflow-type: tm+mt
source-wordcount: '783'
ht-degree: 0%

---

# 專案完成百分比概觀

項目的「完成百分比」值是根據項目中任務的「持續時間」或「計畫小時數」計算的。 您的Adobe Workfront管理員或群組管理員會定義在「專案偏好設定」區域中設定資訊時，在計算系統完成百分比時要考慮哪個值。

如需設定專案偏好設定的相關資訊，請參閱 [配置系統範圍的項目首選項](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

父任務的「完成百分比」基於其每個子任務的「持續時間」或「計畫小時數」。

同樣，項目的「完成百分比」也基於項目中每個主要任務的持續時間或計畫小時數。

主要任務是父任務和沒有子任務的獨立任務。

>[!TIP]
>
>主要任務在項目計畫中不會縮進。

## Workfront如何計算完成百分比

* [更新任務的完成百分比](#update-the-percent-complete-on-a-task)
* [Workfront如何計算父任務的完成百分比](#how-workfront-calculates-percent-complete-on-a-parent-task)
* [Workfront如何計算專案的完成百分比](#how-workfront-calculates-percent-complete-on-a-project)

### 更新任務的完成百分比 {#update-the-percent-complete-on-a-task}

您可以手動修改任務的完成百分比。 這不是計算。

Workfront使用個別任務的完成百分比來計算其父任務的完成百分比或專案的完成百分比。

有關更新任務完成百分比的資訊，請參閱 [查看和更新任務的完成百分比](../../../manage-work/projects/updating-work-in-a-project/view-update-percent-complete-for-tasks.md).

### Workfront如何計算父任務的完成百分比 {#how-workfront-calculates-percent-complete-on-a-parent-task}

根據您的Workfront或組管理員在系統或組級別的「項目首選項」中選擇的項目，父任務的完成百分比將根據任務的持續時間或計畫小時計算。

請考量下列情況：

* 如果系統根據計畫小時計算完成百分比，則父任務完成百分比將使用以下公式計算：

   `Parent Task Percent Complete = (((Task 1 Planned Hours * Task 1 Percent Complete) + (Task 2 Planned Hours * Task 2 Percent Complete))/Total Planned Hours of Parent)*100`

   父代的「總計畫小時數」表示每個子代的所有「計畫小時數」的總和。

   ![](assets/project-with-tasks-percent-complete-planned-hours-calculation.png)

* 如果系統根據「持續時間」計算完成百分比，則父任務完成百分比將使用以下公式計算：

   `Parent Task Percent Complete = (((Task 1 Duration * Task 1 Percent Complete) + (Task 2 Duration * Task 2 Percent Complete))/ Total Duration of Parent)*100`

   ![](assets/project-with-tasks-percent-complete-duration-calculation.png)

   >[!IMPORTANT]
   >
   >父任務的總持續時間是子任務的所有持續時間的總計。 例如，父項任務（具有兩個子項，各自的持續時間為1天和2天）的總持續時間為3天，即使兩個子項可以在同一天開始也是如此。


### Workfront如何計算專案的完成百分比 {#how-workfront-calculates-percent-complete-on-a-project}

根據您的Workfront或組管理員在系統或組級別的「項目首選項」中選擇的項目完成百分比，將根據項目上主要任務的「持續時間」或「計畫小時數」計算項目完成百分比。

* 如果系統根據計畫小時計算完成百分比，則使用以下公式計算項目完成百分比：

   `Project Percent Complete =(((Task 1 Planned Hours * Task 1 Percent Complete) + (Task 2 Planned Hours * Task 2 Percent Complete))/Total Planned Hours of the Project)*100`

   項目的「總計計畫時數」是項目上所有主要任務的「計畫時數」的總和。

   ![](assets/project-with-tasks-percent-complete-planned-hours-calculation.png)

   >[!NOTE]
   >
   >任務1或任務2隻能是父任務或獨立任務。 此計算中不使用子任務的「計畫小時數」和「完成百分比」。

* 如果系統根據持續時間計算完成百分比，則使用以下公式計算項目完成百分比：

   `Project Percent Complete = (((Task 1 Duration * Task 1 Percent Complete) + (Task 2 Duration * Task 2 Percent Complete))/Duration of the Project)*100`

   >[!IMPORTANT]
   >
   >「專案持續時間」是顯示完成百分比之主要任務的所有持續時間總計。 例如，如果項目的獨立任務的持續時間為2天，父任務的持續時間為5天，並且已完成了工作，則該項目的總持續時間為7天，即使這兩個任務可以在同一天開始。

   ![](assets/project-with-tasks-percent-complete-duration-calculation.png)

   >[!NOTE]
   >
   >任務1或任務2隻能是父任務或獨立任務。 此計算中不使用子任務的持續時間和完成百分比。

## 使用持續時間的專案完成百分比範例

使用任務的持續時間來計算項目完成百分比時，請考慮以下示例：

![](assets/project-with-tasks-percent-complete-duration-calculation.png)

以下資訊用於計算專案的完成百分比

* 獨立任務完成百分比（任務1 - 20%）
* 父任務完成百分比（任務2 - 25%）
* 任務1的持續時間（5天）
* 任務2的持續時間（2天）
* 專案持續時間（7天）


要使用持續時間計算項目完成百分比，請執行以下操作：

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