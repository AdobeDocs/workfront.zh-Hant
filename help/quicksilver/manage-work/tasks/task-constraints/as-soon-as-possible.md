---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: 「任務約束概述：盡快'
description: 「盡快」是任務約束，使任務的開始時間盡可能接近項目的開始。
author: Alina
feature: Work Management
exl-id: 9cb232fe-bc74-4433-afac-88be69514c88
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '391'
ht-degree: 0%

---

# 任務約束概覽：盡快

「盡快」是任務約束，使任務的開始時間盡可能接近項目的開始。

## 盡快使用約束的考量事項

* 如果項目使用從起始日期開始的計畫模式，並且新任務的系統預設起始日期設定為基於項目計畫日期，則「盡快」是預設約束。

* 如果項目使用從開始日期開始的計畫模式，並且系統或組將新任務的預設起始日期設定為今天，則預設任務約束為不早於開始。

   有關為新任務設定預設約束的位置的資訊，請參閱 [配置全系統任務和問題首選項](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

有關如何更新任務的任務約束的資訊，請參閱 [更新任務的任務約束](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: replaced with new article linked above) </p>
<p>To update the Task Constraint to As Soon As Possible: </p>
<ol>
<li value="1">Go to a task whose Task Constraint you want to update.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click <strong>Edit</strong>.</p> </li>
<li value="3"> <p>In the <strong>Overview</strong> section, expand the <strong>Task Constraint</strong> drop-down menu.</p> </li>
<li value="4"> <p>Select <strong>As Soon As Possible</strong>.</p> </li>
<li value="5">Click <strong>Save Changes</strong>. </li>
</ol>
</div>
-->

## 最早可用時間與盡快之間的差異

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: [! This section is duplicated in "Earliest Available Time"])&nbsp;</p>
-->

當存在以下所有條件時，「最早可用時間」約束與「盡快」約束不同：

* 已排程專案完成。
* 項目中的任務具有前置關係。
* 前置任務具有靈活的任務約束。

在這種情況下：

* **最早可用時間：** 對後繼任務使用最早可用時間約束將優先順序置於前置任務的靈活約束。

   例如，假設任務A是任務B的前身。任務B具有最早可用時間約束，任務A具有盡可能晚的約束。 在這種情況下，將盡可能在項目完成前安排任務。

* **盡快：** 在此情況下，對後續任務使用盡快約束將優先順序分配給後續任務。

   例如，假設任務A是任務B的前身。任務B具有盡可能快的約束，任務A具有盡可能晚的約束。 在此情況下，會盡可能將任務安排在接近項目開始的位置。
