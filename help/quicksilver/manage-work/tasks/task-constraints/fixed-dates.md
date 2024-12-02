---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: 任務限制總覽：固定日期
description: 當您想要指定任務的確切開始日期和結束日期時，可以使用固定日期任務限制。 如需有關任務限制的詳細資訊，請參閱任務限制總覽。
author: Alina
feature: Work Management
exl-id: 084f54a6-e757-405c-b388-5d5f61608e71
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '437'
ht-degree: 0%

---

# 任務限制總覽：固定日期

當您想要指定任務的確切開始日期和結束日期時，可以使用固定日期任務限制。 如需有關任務限制的詳細資訊，請參閱[任務限制總覽](../../../manage-work/tasks/task-constraints/task-constraint-overview.md)。

## 固定日期限制的總覽

使用「固定日期」限制時，請考量下列事項：

* 當您選取「固定日期(FIXT)」任務限制時，必須指定任務的計劃開始日期與計畫完成日期。 在這種情況下，會忽略任務的前置任務關係。
* 使用FIXT限制時，任務的期間欄位不可編輯。 期間的計算方式為任務的計劃開始日期與計畫完成日期之間的差異。
* 如果任務的「工期型別」是「投入比導向」，則任務上的受指派人數也會影響任務的「工期」。
* 當您將具有FIXT限制的任務移動或複製到另一個專案時，任務的限制或專案日期可能會根據限制日期以及專案的開始與完成日期而變更。 存在下列情況：

   * 從開始排程目的地專案時：

      * 當任務的任何限制日期早於專案開始日期時，任務限制會變成「儘快」。
      * 當任務的任何或兩個限制日期晚於專案的計畫完成日期時，專案計畫完成日期會變更以符合任務的完成限制日期。

   * 當目標專案排程為從完成開始時：

      * 當任務的任何限制日期晚於專案完成日期時，任務限制會變更為儘可能晚的。
      * 當任務的任何或兩個限制日期早於專案的計劃開始日期時，專案計劃開始日期會變更以符合任務的開始限制日期。

   * 無論專案排程為何，當任務的限制日期在專案的「開始日期」與「完成日期」內時，不會變更「任務限制」或專案日期。

  如需關於移動任務的資訊，請參閱[移動任務](../../../manage-work/tasks/manage-tasks/move-tasks.md)。 如需複製工作的相關資訊，請參閱[複製和複製工作](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md)。

如需有關如何更新任務之任務限制的資訊，請參閱[更新任務的任務限制](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md)。

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
