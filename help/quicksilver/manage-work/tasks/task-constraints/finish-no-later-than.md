---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: 任務限制總覽：完成時間不晚於
description: 「完成時間不晚於(FNLT)」是「作業限制」，可排定在您指定日期之前完成的工作。
author: Alina
feature: Work Management
exl-id: ea0e74fb-45a0-4466-b57d-294a9babb340
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '388'
ht-degree: 0%

---

# 任務限制總覽：完成時間不晚於

「完成時間不晚於(FNLT)」是「作業限制」，可排定在您指定日期之前完成的工作。

## 完成時間概覽不晚於限制

為任務使用「完成時間不晚於(FNLT)」限制時，請考量下列事項：

* 當專案是從「開始日期」排程時，您應使用此限制。 在這種情況下，您可以在任務強制其他相依任務顯示為「有風險」之前提供軟性任務限制。
* 當您使用FNLT限制與「排程自完成日期」專案時，此限制會將作業排程為儘可能晚的任務。
* 當您將具有FNET限制的任務移動或複製到另一個專案時，任務的限制或專案日期可能會根據限制日期以及專案的開始與完成日期而變更。 存在下列情況：

   * 從開始排程目的地專案時：

      * 當任務的限制日期早於專案計劃開始日期時，任務限制會變更為「儘快」。
      * 當任務的限制日期晚於專案計畫完成日期時，專案計畫完成日期會變更以符合任務的完成限制日期。

      * 當目標專案排程為從完成開始時：

         * 當任務的限制日期晚於「專案完成日期」時，任務限制會變更為「儘可能遲」。
         * 當任務的限制日期早於專案的「計劃開始日期」時，專案的「計劃開始日期」會變更以符合任務的開始限制日期。

      * 無論專案的排程為何，當任務的限制日期在專案的「開始」與「完成」日期內時，不會變更「任務限制」或專案日期。

  如需關於移動任務的資訊，請參閱[移動任務](../../../manage-work/tasks/manage-tasks/move-tasks.md)。 如需複製工作的相關資訊，請參閱[複製和複製工作](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md)。

如需有關如何更新任務之任務限制的資訊，請參閱[更新任務的任務限制](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md)。

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
