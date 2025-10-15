---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: 任務限制總覽：最新可用時間
description: 最新可用時間(LAT)是Adobe Workfront中的任務限制型別。
author: Alina
feature: Work Management
exl-id: acf55004-9424-4e24-9ff5-90f6fd7f72a6
source-git-commit: 7427706f6ce6cad3370b91269c1b4e7a10ed09f9
workflow-type: tm+mt
source-wordcount: '334'
ht-degree: 0%

---

# 任務限制總覽：最新可用時間

最新可用時間(LAT)是Adobe Workfront中的任務限制型別。

## 使用最新可用時間任務限制

當您想要在專案中考慮前置任務 — 後續任務關係後，在最新的可用時間開始排程任務時，可以使用LAT限制。

此限制與「儘快」不同，因為它不會強制重新排程前置任務或後續任務。 相反地，它只會影響與其相關聯之任務的排程，根據其與其他任務的關係將其設定為最新的可用時間。

如需有關如何更新任務之任務限制的資訊，請參閱[更新任務的任務限制](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md)。

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>To update the Task Constraint to Latest Available Time:</p>
<p>(NOTE: replaced with new article linked above) </p>
<ol>
<li value="1">Go to a task whose Task Constraint you want to update.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click <strong>Edit</strong>.</p> </li>
<li value="3">In the <strong>Overview</strong> section, expand the <strong>Task Constraint</strong> drop-down menu.</li>
<li value="4"> <p>Select <strong>Latest Available Time</strong>.</p> </li>
<li value="5">Click <strong>Save Changes</strong>.</li>
</ol>
</div>
-->

## 最新可用時間和儘可能晚可用時間之間的差異

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: [! This section is duplicated in "As Late As Possible"] - inserted snippet in both (Alina)) </p>
-->

當存在下列條件時，「最新可用時間」限制與「儘可能晚到」限制不同：

* 從開始日期排程專案
* 專案中的任務具有前置任務關係
* 後續任務具有彈性任務限制

在此情況下：

* **最新可用時間：**&#x200B;在前置任務上使用最新可用時間限制，會優先處理後置任務的彈性限制。

  **範例：**&#x200B;例如，任務A是任務B的前置任務。任務A具有最新的可用時間限制，而任務B具有「儘快」限制。 在此情況下，任務A會儘可能安排在接近專案開始的時間。

  ![](assets/latest-available-time-task-constraint-in-task-list-350x116.png)

* **儘可能遲：**&#x200B;在此案例中，在前置任務上使用儘可能晚限制會將優先順序給予前置任務。

  **範例：**&#x200B;例如，任務A是任務B的前置任務。任務A具有儘可能晚的限制，而任務B具有儘可能早的限制。 在此情況下，任務A會排程儘可能接近專案結尾。

  ![](assets/as-late-as-possible-task-constraint-in-task-list-350x104.png)

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: this content was here before but it was wrong - according to this issue in Hub, per Dev, the correct functionality is in the snippet above: https://hub.workfront.com/task/6193c6910004bce9de07cda7757f3ce8/updates?email-source=subscribedCommunication) </p>
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
