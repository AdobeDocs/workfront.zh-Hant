---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: 「任務約束概述：盡可能遲」
description: 「盡可能晚」(ALAP)是「Adobe Workfront任務約束」，它使任務的完成時間盡可能接近項目結束。
author: Alina
feature: Work Management
exl-id: 475427d0-020b-4851-a614-c9931659e07d
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '368'
ht-degree: 0%

---

# 任務約束概覽：盡可能晚

「盡可能晚」(ALAP)是「Adobe Workfront任務約束」，它使任務的完成時間盡可能接近項目結束。

使用此約束可能導致重新計畫前置任務或從屬任務。

如需先前關係的詳細資訊，請參閱 [使用任務前置任務](../../../manage-work/tasks/use-prdcssrs/use-task-predecessors.md).

如果項目使用「從完成日期開始的計畫」計畫模式，並且任務起始日期的系統或組預設值為「基於項目計畫日期」，則「盡可能晚」為預設約束。

有關為新任務設定預設約束的位置的資訊，請參閱 [配置全系統任務和問題首選項](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

有關如何更新任務的任務約束的資訊，請參閱 [更新任務的任務約束](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Use the As Late As Possible Task Constraint</h2>
<p>(NOTE: replaced with new article linked above) </p>
<p>To update the Task Constraint to As Late As Possible:&nbsp;</p>
<ol>
<li value="1">Go to a task whose Task Constraint you want to update.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click&nbsp;<strong>Edit</strong>.</p> </li>
<li value="3"> <p>In the&nbsp;<strong>Overview</strong>&nbsp;section, expand the&nbsp;<strong>Task Constraint</strong>&nbsp;drop-down menu.</p> </li>
<li value="4"> <p>Select&nbsp;<strong>As Late As Possible</strong>.</p> </li>
<li value="5">Click <strong>Save Changes</strong>.&nbsp;</li>
</ol>
</div>
-->

## 最新可用時間與盡可能晚之間的差異

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;[! This section is duplicated in "Latest Available Time"] - inserted a snippet for both articles (Alina)) </p>
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
<p>(NOTE: this content was here before but it was wrong - according to this issue in Hub, per Dev, the correct functionality is in the snippet above: https://hub.workfront.com/task/6193c6910004bce9de07cda7757f3ce8/updates?email-source=subscribedCommunication) </p>
<p>The Latest&nbsp;Available Time constraint differs from the As Late&nbsp;As Possible constraint when the following criteria exist:</p>
<ul>
<li> The project is scheduled From Completion </li>
<li> Tasks in the project have a predecessor relationship </li>
<li> The predecessor task has a flexible task constraint </li>
</ul>
<p> In this situation: </p>
<ul>
<li> <p><strong>Latest Available Time:</strong> Using the Latest&nbsp;Available Time constraint on the successor task gives priority to flexible constraint of the predecessor.</p> <p>For example, Task A is a predecessor to Task B. Task B has the Latest&nbsp;Available Time constraint and Task A has the As Soon&nbsp;As Possible constraint. In this situation, the task is scheduled as close&nbsp;to the start&nbsp;of the project as possible.</p> </li>
<li> <p><strong>As Late As Possible:</strong> In this scenario, using the As Late&nbsp;As Possible constraint on the successor task gives the priority to the successor task.</p> <p>For example, Task A is a predecessor to Task B. Task B has the As Late&nbsp;As Possible&nbsp;constraint and Task A has the As Soon&nbsp;As Possible constraint. In this situation, the task is scheduled as close to the end&nbsp;of the project as possible.</p> </li>
</ul>
</div>
-->
