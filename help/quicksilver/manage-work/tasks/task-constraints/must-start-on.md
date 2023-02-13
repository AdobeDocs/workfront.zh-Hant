---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: 「任務約束概述：必須開始」
description: 使用「必須開始(MSO)任務約束」可以計畫任務在特定日期完全開始。
author: Alina
feature: Work Management
exl-id: 09062d46-2b80-4758-946e-d6dec0f7a7c0
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '395'
ht-degree: 0%

---

# 任務約束概覽：必須開始

使用「必須開始(MSO)任務約束」可以計畫任務在特定日期完全開始。

「必須開始」約束計畫任務，以便在您在 **計劃開始日期** 欄位。

>[!TIP]
>
>人工更新任務的計畫起始日期將任務的約束更改為「必須開始」。

## 必須從任務約束開始的概覽

在計畫具有「必須開始」約束的任務時，請考慮以下事項：

* 前置關係不強制此任務重新計畫。 Workfront實際上忽略了任務中具有此約束的任何前置關係。
* 任務顯示 **風險** 如果前任們開始落後或遲來。

* 將具有MSO約束的任務移動或複製到另一個項目時，任務的約束或項目日期可能會根據約束日期和項目的起始日期和完成日期而改變。 存在下列情況：

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
<h2>Use the Must Start On Task Constraint</h2>
<p>(NOTE: replaced with new article linked above) </p>
<p>To update the Task Constraint to Must Start On:</p>
<ol>
<li value="1">Go to a task whose Task Constraint you want to update.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click <strong>Edit</strong>.</p> </li>
<li value="3">In the <strong>Overview</strong> section, expand the <strong>Task Constraint</strong> drop-down menu.</li>
<li value="4"> <p>Select <strong>Must Start On</strong>.</p> </li>
<li value="5"> <p>Specify a <strong>Planned Start Date</strong>.</p> <p>The task must start by this date, and no later than this date.</p> </li>
<li value="6">Click <strong>Save Changes</strong>. </li>
</ol>
</div>
-->
