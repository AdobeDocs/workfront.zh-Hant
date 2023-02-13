---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: 「任務約束概述：必須完成」
description: 您可以使用「必須完成(MFO)任務約束」將任務安排為在特定日期結束。
author: Alina
feature: Work Management
exl-id: 9e546a0f-7f7a-4f1c-9d9d-aa3cea377fdf
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '395'
ht-degree: 0%

---

# 任務約束概覽：必須完成

您可以使用「必須完成(MFO)任務約束」將任務安排為在特定日期結束。

「必須完成」(Must Finish On)約束計畫任務，以在您在 **計畫完成日期** 欄位。

>[!TIP]
>
>人工更新任務的計畫完成日期將任務的約束更改為必須完成。

## 必須完成任務約束的概述

在計畫具有「必須完成」約束的任務時，請考慮以下事項：

* 前置關係不會強制重新計畫任務。 Adobe Workfront實際上忽視了前身關係。
* 任務顯示為 **風險** 如果前任們開始落後或遲到。

* 將具有MFO約束的任務移動或複製到另一個項目時，任務的約束或項目日期可能會根據約束日期以及項目的起始日期和完成日期而改變。 存在下列情況：

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
<h2>Use the Must Finish On Task Constraint</h2>
<p>To update the Task Constraint to Must Finish On:</p>
<ol>
<li value="1">Go to a task whose Task Constraint you want to update.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click <strong>Edit</strong>.</p> </li>
<li value="3">In the <strong>Overview</strong> section, expand the <strong>Task Constraint</strong> drop-down menu.</li>
<li value="4"> <p>Select <strong>Must Finish On</strong>.</p> </li>
<li value="5"> <p>Specify a <strong>Planned Completion Date</strong>.</p> <p>The task must complete by this date, and no later than this date. </p> </li>
<li value="6">Click <strong>Save Changes</strong>. </li>
</ol>
</div>
-->
