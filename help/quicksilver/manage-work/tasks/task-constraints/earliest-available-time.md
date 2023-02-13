---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: 「任務約束概述：最早可用時間'
description: 最早可用時間是任務約束，它將任務安排為在考慮任何前置關係後，從最早可用時間開始。
author: Alina
feature: Work Management
exl-id: 9c01e4bd-c6ca-4540-a0f1-ecdd44df84e0
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '299'
ht-degree: 0%

---

# 任務約束概覽：最早可用時間

最早可用時間是任務約束，它將任務安排為在考慮任何前置關係後，從最早可用時間開始。

有關如何更新任務的任務約束的資訊，請參閱 [更新任務的任務約束](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: replaced with new article linked above) </p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">To update the Task Constraint to Earliest Available Time:</p>
-->

<!--
   <li value="1" data-mc-conditions="QuicksilverOrClassic.Draft mode">Go to a task whose constraint you want to modify. </li>
   -->

<!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <strong>Edit Task</strong>.</p>
   -->

<!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click <strong>Edit</strong>.</p>
   -->

<!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">In the <strong>Overview</strong> section, expand the <strong>Task Constraint</strong> drop-down menu.</p>
   -->

<!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Select <strong>Earliest Available Time</strong>.</p>
   -->

<!--
   <li value="5" data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <strong>Save Changes</strong>.</li>
   -->

## 最早可用時間與盡快之間的差異

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: [! This section is duplicated in "Earliest Available Time"])</p>
-->

當存在以下所有條件時，「最早可用時間」約束與「盡快」約束不同：

* 已排程專案自完成
* 項目中的任務具有前置關係
* 前置任務具有靈活的任務約束

在這種情況下：

* **最早可用時間：** 對後繼任務使用最早可用時間約束將優先順序置於前置任務的靈活約束。

   **範例：** 任務A是任務B的前身。任務B具有最早可用時間約束，任務A具有盡可能晚的約束。 在此情況下，任務B將排定得盡可能接近項目完成。

   ![任務的日期接近項目完成日期時的最早可用時間約束](assets/earliest-available-constraint-dates-closer-to-project-completion-350x137.png)

* **盡快：** 在此情況下，對後續任務使用盡快約束將優先順序分配給後續任務。

   **範例：**  任務A是任務B的前身。任務B具有盡快的約束，任務A具有盡快的約束。 在此情況下，任務B將排程得盡可能接近項目開始。

   ![任務的日期接近項目的「開始日期」時，盡快約束](assets/as-soon-as-possible-dates-closer-to-project-start-350x126.png)
