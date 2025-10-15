---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: 任務限制總覽：儘可能遲
description: 儘可能延遲(ALAP)是Adobe Workfront任務限制，可將任務的完成時間儘可能置於專案結尾處。
author: Alina
feature: Work Management
exl-id: 475427d0-020b-4851-a614-c9931659e07d
source-git-commit: 7427706f6ce6cad3370b91269c1b4e7a10ed09f9
workflow-type: tm+mt
source-wordcount: '370'
ht-degree: 0%

---

# 任務限制總覽：儘可能遲

儘可能延遲(ALAP)是Adobe Workfront任務限制，可將任務的完成時間儘可能置於專案結尾處。

使用此限制可能會導致前置任務或相依任務被重新排程。

如需前置任務關係的詳細資訊，請參閱[使用前置任務：文章索引](../../../manage-work/tasks/use-prdcssrs/use-task-predecessors.md)。

如果專案使用的排程模式是「從完成日期開始排程」，且作業「開始日期」的系統或群組預設值為「根據專案計畫日期」，則「儘可能延遲」為預設限制。

如需有關設定新任務的預設條件約束的詳細資訊，請參閱[設定全系統的任務和問題偏好設定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md)。

如需有關如何更新任務之任務限制的資訊，請參閱[更新任務的任務限制](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md)。

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Use the As Late As Possible Task Constraint</h2>
<p>(NOTE: replaced with new article linked above) </p>
<p>To update the Task Constraint to As Late As Possible: </p>
<ol>
<li value="1">Go to a task whose Task Constraint you want to update.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click <strong>Edit</strong>.</p> </li>
<li value="3"> <p>In the <strong>Overview</strong> section, expand the <strong>Task Constraint</strong> drop-down menu.</p> </li>
<li value="4"> <p>Select <strong>As Late As Possible</strong>.</p> </li>
<li value="5">Click <strong>Save Changes</strong>. </li>
</ol>
</div>
-->

## 最新可用時間和儘可能晚可用時間之間的差異

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: [! This section is duplicated in "Latest Available Time"] - inserted a snippet for both articles (Alina)) </p>
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
<li> <p><strong>Latest Available Time:</strong> Using the Latest Available Time constraint on the successor task gives priority to flexible constraint of the predecessor.</p> <p>For example, Task A is a predecessor to Task B. Task B has the Latest Available Time constraint and Task A has the As Soon As Possible constraint. In this situation, the task is scheduled as close to the start of the project as possible.</p> </li>
<li> <p><strong>As Late As Possible:</strong> In this scenario, using the As Late As Possible constraint on the successor task gives the priority to the successor task.</p> <p>For example, Task A is a predecessor to Task B. Task B has the As Late As Possible constraint and Task A has the As Soon As Possible constraint. In this situation, the task is scheduled as close to the end of the project as possible.</p> </li>
</ul>
</div>
-->
