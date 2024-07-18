---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: 「任務限制總覽：開始時間不晚於」
description: 「開始時間不晚於(SNLT)」是「作業限制」，可排定在指定日期之前開始作業。
author: Alina
feature: Work Management
exl-id: 86139ce6-c6b1-4ac4-a5cb-fd4aa899a025
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '435'
ht-degree: 0%

---

# 任務限制總覽：開始時間不晚於

「開始時間不晚於(SNLT)」是「作業限制」，可排定在指定日期之前開始作業。

使用SNLT限制時，請考量下列事項：

* 從完成日期開始排程專案時，您應該使用開始時間不晚於限制。 在這種情況下，您可以在任務強制其他相依任務顯示為「有風險」之前提供軟性任務限制。
* 如果專案使用「從完成日期開始排程」的排程模式，且作業「開始日期」的系統或群組預設值為「今天」，則「開始時間不晚於」為預設限制。 如需有關設定新任務的預設條件約束的詳細資訊，請參閱[設定全系統的任務和問題偏好設定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md)。
* 當您將SNLT限制與「從開始日期開始排程」專案搭配使用時，Adobe Workfront會以儘快排程作業的方式排程作業。
* 當您將具有SNLT限制的任務移動或複製到另一個專案時，任務的限制或專案日期可能會根據限制日期以及專案的開始與完成日期而變更。 存在下列情況：

   * 從開始排程目的地專案時：

      * 當任務的限制日期早於專案計劃開始日期時，任務限制會變更為「儘快」。
      * 當任務的限制日期晚於專案計畫完成日期時，專案計畫完成日期會變更以符合任務的完成限制日期。

      * 當目標專案排程為從完成開始時：

         * 當任務的限制日期晚於「專案完成日期」時，任務限制會變更為「儘可能遲」。
         * 當任務的限制日期早於專案的「計劃開始日期」時，專案的「計劃開始日期」會變更以符合任務的開始限制日期。

      * 無論專案的排程為何，當任務的限制日期在專案的「開始」與「完成」日期內時，不會變更「任務限制」或專案日期。

  如需關於移動任務的資訊，請參閱[移動任務](../../../manage-work/tasks/manage-tasks/move-tasks.md)。

  如需複製工作的相關資訊，請參閱[複製和複製工作](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md)。

如需有關如何更新任務之任務限制的資訊，請參閱[更新任務的任務限制](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md)。

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Use the Start No Later Than Task Constraint</h2>
<p>(NOTE: replaced with new article linked above) </p>
<p>To update the Task Constraint to Start No Later Than:</p>
<ol>
<li value="1">Go to a task whose Task Constraint you want to update.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click <strong>Edit</strong>.</p> </li>
<li value="3">In the <strong>Overview</strong> section, expand the <strong>Task Constraint</strong> drop-down menu.</li>
<li value="4"> <p>Select <strong>Start No Later Than</strong>.</p> </li>
<li value="5"> <p>Specify a <strong>Planned Start Date</strong>.</p> <p>This is the date by which the task must start, and not later than this date.</p> </li>
<li value="6">Click <strong>Save Changes</strong>.<br></li>
</ol>
</div>
-->
