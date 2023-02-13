---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: 「任務約束概述：完成時間不晚於'
description: 完成不晚於(FNLT)是任務約束，它將任務安排在指定日期之前完成。
author: Alina
feature: Work Management
exl-id: ea0e74fb-45a0-4466-b57d-294a9babb340
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '388'
ht-degree: 0%

---

# 任務約束概覽：完成時間不晚於

完成不晚於(FNLT)是任務約束，它將任務安排在指定日期之前完成。

## 不晚於約束的概覽

對任務使用「完成時間不晚於」(FNLT)約束時，請考慮以下事項：

* 當計畫項目為「開始日期」時，應使用此約束。 在此情況下，您可以對任務提供軟約束，然後強制其他從屬任務顯示為「風險」。
* 如果將FNLT約束與「從完成日期開始的計畫」項目一起使用，此約束將按盡可能晚的任務安排任務。
* 將具有FNET約束的任務移動或複製到另一個項目時，任務的約束或項目日期可能會根據約束日期以及項目的起始日期和完成日期而改變。 存在下列情況：

   * 排程從開始時：

      * 當任務的約束日期早於項目計畫起始日期時，任務約束將盡快更改為。
      * 當任務的約束日期晚於項目計畫完成日期時，項目計畫完成日期將更改以匹配任務的完成約束日期。

      * 排程完成時：

         * 當任務的約束日期晚於項目完成日期時，任務約束將變為盡可能晚。
         * 當任務的約束日期早於項目的計畫起始日期時，項目計畫起始日期將更改以匹配任務的起始約束日期。
      * 無論項目計畫如何，當任務的約束日期在項目的「開始」和「完成」日期內時，任務約束或項目日期均不會更改。

   有關移動任務的資訊，請參閱 [移動任務](../../../manage-work/tasks/manage-tasks/move-tasks.md). 有關複製任務的資訊，請參閱 [複製和複製任務](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md).

有關如何更新任務的任務約束的資訊，請參閱 [更新任務的任務約束](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Use the Finish No Later Than constraint</h2>
<p>To update the Task Constraint to Finish No Later Than:</p>
<ol>
<li value="1">Go to a task whose Task Constraint you want to update.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click <strong>Edit</strong>.</p> </li>
<li value="3">In the <strong>Overview</strong> section, expand the <strong>Task Constraint</strong> drop-down menu.</li>
<li value="4"> <p>Select <strong>Finish No Later Than</strong>.</p> <p> <img src="assets/fnlt-350x266.png" alt="FNLT.png" style="width: 350;height: 266;"> </p> </li>
<li value="5"> <p>Specify a <strong>Planned Completion Date</strong>.</p> <p>You must complete the task on and not later than this date. </p> </li>
<li value="6">Click <strong>Save Changes</strong>.</li>
</ol>
</div>
-->
