---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: 「任務約束概述：固定日期
description: 如果想要確定任務的確切開始日期和結束日期，可以使用「固定日期」任務約束。 有關任務約束的詳細資訊，請參閱任務約束概覽。
author: Alina
feature: Work Management
exl-id: 084f54a6-e757-405c-b388-5d5f61608e71
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '437'
ht-degree: 0%

---

# 任務約束概覽：固定日期

如果想要確定任務的確切開始日期和結束日期，可以使用「固定日期」任務約束。 有關任務約束的詳細資訊，請參閱 [任務約束概覽](../../../manage-work/tasks/task-constraints/task-constraint-overview.md).

## 固定日期限制概覽

使用「固定日期」限制時，請考量下列事項：

* 選擇「固定日期(FIXT)」任務約束時，必須指定任務的「計畫起始日期」和「計畫完成日期」。 在這種情況下，會忽略任務的前置關係。
* 使用FIXT約束時，任務的「持續時間」欄位不可編輯。 持續時間的計算方式為任務的計畫起始日期和計畫完成日期之間的差異。
* 如果任務的「持續時間類型」為「工作驅動」，則任務上的受分配者數也會影響任務的「持續時間」。
* 將具有FIXT約束的任務移動或複製到另一個項目時，任務的約束或項目日期可能會根據約束日期以及項目的起始日期和完成日期而改變。 存在下列情況：

   * 排程從開始時：

      * 如果任務的任何約束日期早於項目起始日期，則任務約束將盡快更改為「」。
      * 當任務的任何或兩個約束日期晚於項目的計畫完成日期時，項目計畫完成日期將更改以匹配任務的完成約束日期。
   * 排程完成時：

      * 當任務的任何約束日期晚於項目完成日期時，任務約束將更改為盡可能晚。
      * 如果任務的任何或兩個約束日期早於項目的計畫起始日期，則項目計畫起始日期將更改以匹配任務的起始約束日期。
   * 無論項目計畫如何，當任務的約束日期在項目的「開始」和「完成」日期內時，「任務約束」或項目日期均不會更改。

   有關移動任務的資訊，請參閱 [移動任務](../../../manage-work/tasks/manage-tasks/move-tasks.md). 有關複製任務的資訊，請參閱 [複製和複製任務](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md).

有關如何更新任務的任務約束的資訊，請參閱 [更新任務的任務約束](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Use the Fixed Dates Task Constraint</h2>
<p>(NOTE:&nbsp;replaced with new article linked above) </p>
<p>To update the Task Constraint to Finish No Later Than:</p>
<ol>
<li value="1">Go to a task whose Task Constraint you want to update.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click <strong>Edit</strong>.</p> </li>
<li value="3">In the <strong>Overview</strong> section, expand the <strong>Task Constraint</strong> drop-down menu.</li>
<li value="4"> <p>Select <strong>Fixed Dates</strong>.</p> </li>
<li value="5"> <p>Specify a <strong>Planned Start Date</strong>.</p> <p>The task must start on this date. </p> </li>
<li value="6"> <p>Specify a <strong>Planned Completion Date</strong>.</p> <p>The task must complete on this date. </p> </li>
<li value="7">Click <strong>Save Changes</strong>.</li>
</ol>
</div>
-->
