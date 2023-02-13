---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: 「任務約束概述：最新可用時間'
description: 「最新可用時間」(LAT)是Adobe Workfront中的「任務限制」類型。
author: Alina
feature: Work Management
exl-id: acf55004-9424-4e24-9ff5-90f6fd7f72a6
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '334'
ht-degree: 0%

---

# 任務約束概覽：最新可用時間

「最新可用時間」(LAT)是Adobe Workfront中的「任務限制」類型。

## 使用最新可用時間任務約束

在考慮項目中的前置項 — 後繼項關係後，如果要安排從最新可用時間開始的任務，則可以使用LAT約束。

此約束與「盡快」不同，因為它不會強制重新安排前置任務或後置任務。 相反，它只會影響與其關聯的任務的時間表，根據其與其他任務的關係將其設定為最新的可用時間。

有關如何更新任務的任務約束的資訊，請參閱 [更新任務的任務約束](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>To update the Task Constraint to Latest Available Time:</p>
<p>(NOTE:&nbsp;replaced with new article linked above)&nbsp;</p>
<ol>
<li value="1">Go to a task whose Task Constraint you want to update.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click <strong>Edit</strong>.</p> </li>
<li value="3">In the <strong>Overview</strong> section, expand the <strong>Task Constraint</strong> drop-down menu.</li>
<li value="4"> <p>Select <strong>Latest Available Time</strong>.</p> </li>
<li value="5">Click <strong>Save Changes</strong>.</li>
</ol>
</div>
-->

## 最新可用時間與盡可能晚之間的差異

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: [! This section is duplicated in "As Late As Possible"] - inserted snippet in both (Alina)) </p>
-->

當存在以下條件時，「最新可用時間」約束與「盡可能晚」約束不同：

* 專案排程從開始日期開始
* 項目中的任務具有前置關係
* 後續任務具有靈活的任務約束

在這種情況下：

* **最新可用時間：** 在前置任務上使用「最新可用時間」約束將優先順序設定為後置任務的靈活約束。

   **範例：** 例如，任務A是任務B的前身。任務A具有最新的可用時間約束，任務B具有盡快的約束。 在此情況下，任務A將排程得盡可能靠近項目開始。

   ![](assets/latest-available-time-task-constraint-in-task-list-350x116.png)

* **盡可能晚：** 在此情況下，對前置任務使用盡可能晚的約束將優先順序分配給前置任務。

   **範例：** 例如，任務A是任務B的前身。任務A具有盡可能晚的約束，任務B具有盡可能快的約束。 在此情況下，任務A將排程得盡可能接近專案結尾。

   ![](assets/as-late-as-possible-task-constraint-in-task-list-350x104.png)

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE:&nbsp;this content was here before but it was wrong - according to this issue in Hub, per Dev, the correct functionality is in the snippet above: https://hub.workfront.com/task/6193c6910004bce9de07cda7757f3ce8/updates?email-source=subscribedCommunication) </p>
<p>The Latest Available Time constraint differs from the As Late As Possible constraint when the following criteria exist:</p>
<ul>
<li> The project is scheduled From Completion </li>
<li> Tasks in the project have a predecessor relationship </li>
<li> The predecessor task has a flexible task constraint </li>
</ul>
<p> In this situation: </p>
<ul>
<li> <p><strong>Latest Available Time:</strong> Using the Latest Available Time constraint on the successor task gives priority to flexible constraint of the predecessor.</p> <p>For example, Task A is a predecessor to Task B. Task B has the Latest Available Time constraint and Task A has the As Soon As Possible constraint. In this situation, Task B is scheduled as close to the start of the project as possible.</p> </li>
<li> <p><strong>As Late As Possible:</strong> In this scenario, using the As Late As Possible constraint on the successor task gives the priority to the successor task.</p> <p>For example, Task A is a predecessor to Task B. Task B has the As Late As Possible constraint and Task A has the As Soon As Possible constraint. In this situation, Task B is scheduled as close to the end of the project as possible.</p> </li>
</ul>
</div>
-->
