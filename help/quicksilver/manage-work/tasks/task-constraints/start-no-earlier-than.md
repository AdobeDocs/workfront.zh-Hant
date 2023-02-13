---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: 「任務約束概述：開始時間不早於'
description: 使用「開始日期早於(SNET)任務約束」將任務安排在指定日期之後開始。
author: Alina
feature: Work Management
exl-id: 857859fb-87ee-4397-b292-239ed9dc8281
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '491'
ht-degree: 0%

---

# 任務約束概覽：開始時間不早於

使用「開始日期早於(SNET)任務約束」將任務安排在指定日期之後開始。

## 開始時間早於任務約束的概覽

使用「開始時間早於任務」約束時，請考慮以下事項：

* 從開始日期開始排程專案時，您應使用「開始時間早於」限制。 在此情況下，您可以對任務提供軟約束，然後強制其他從屬任務顯示為「風險」。
* 如果項目計畫為「開始日期」，並且新任務的系統或組預設起始日期設定為「今天」，則「開始日期不早於」是預設約束。 有關為任務配置預設值的資訊，請參閱 [配置全系統任務和問題首選項](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

* 如果計畫項目起始日期，並且新任務的系統預設起始日期設定為基於項目計畫日期，則新任務的預設約束是「盡快」。
* 如果計畫項目「自完成日期」項目，並且新任務的系統預設起始日期設定為「今天」，則「起始日期不早於」約束將計畫該任務，因為它將作為「盡可能晚」任務。
* 將具有SNET約束的任務移動或複製到另一個項目時，任務的約束或項目日期可能會根據約束日期以及項目的起始日期和完成日期而改變。 存在下列情況：

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
<h2>Use the Start No Earlier Than Task Constraint</h2>
<p>(NOTE:&nbsp;replaced with new article linked above)&nbsp;</p>
<p>To update the Task Constraint to Start No Later Than:</p>
<ol>
<li value="1">Go to a task whose Task Constraint you want to update.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click <strong>Edit</strong>.</p> </li>
<li value="3">In the <strong>Overview</strong> section, expand the <strong>Task Constraint</strong> drop-down menu.</li>
<li value="4"> <p>Select <strong>Start No Earlier Than</strong>.</p> </li>
<li value="5"> <p>Specify a <strong>Planned Start Date</strong>.</p> <p>This is the date by which the task must start, and not earlier than this date. </p> </li>
<li value="6">Click <strong>Save Changes</strong>.</li>
</ol>
</div>
-->
