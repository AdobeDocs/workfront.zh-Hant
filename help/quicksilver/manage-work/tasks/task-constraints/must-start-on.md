---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: 「任務限制總覽：必須開始於」
description: 使用「必須開始於(MSO)任務限制」將任務排程為完全在特定日期開始。
author: Alina
feature: Work Management
exl-id: 09062d46-2b80-4758-946e-d6dec0f7a7c0
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '395'
ht-degree: 0%

---

# 任務限制總覽：必須開始於

使用「必須開始於(MSO)任務限制」將任務排程為完全在特定日期開始。

「必須開始於」限制排程任務，使其完全依照您在&#x200B;**規劃開始日期**&#x200B;欄位中指定的時間和日期開始。

>[!TIP]
>
>手動更新任務的計劃開始日期會將任務的限制變更為必須開始於。

## 「必須開始於任務限制」的概觀

排程具有「必須開始於」限制的任務時，請考量下列事項：

* 前置任務關係不會強制此任務重新排程。 Workfront基本上會忽略具有此限制之任務的任何前置任務關係。
* 如果前置任務開始落後或延遲，則任務確實顯示&#x200B;**有風險**。

* 當您將具有MSO限制的任務移動或複製到另一個專案時，任務的限制或專案日期可能會根據限制日期以及專案的開始和完成日期而變更。 存在下列情況：

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
