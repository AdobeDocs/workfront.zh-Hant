---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: 任務限制總覽：儘快
description: 「儘快」是一種任務限制，可讓任務的開始時間儘可能接近專案開始。
author: Alina
feature: Work Management
exl-id: 9cb232fe-bc74-4433-afac-88be69514c88
TQID: https://experienceleague.adobe.com/7hhcYNT9BVO7Epe--D-UprRexh-32kHtIlOGYohwpto
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40cid: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: b91c0848-76c4-4da4-8b81-3aade0518dd0id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 392
ht-degree: 0%

---

# 任務限制總覽：儘快

「儘快」是一種任務限制，可讓任務的開始時間儘可能接近專案開始。

## 使用「儘快」限制的注意事項

* 如果專案使用從開始日期起排程的排程模式，且新任務的系統預設開始日期設定為「根據專案計畫日期」，則「儘快」為預設限制。

* 如果專案使用「從開始日期開始排程」的排程模式，且新作業的系統或群組預設「開始日期」設定為「今天」，則預設的「作業限制」為「開始時間不得早於」。

  如需有關設定新任務的預設條件約束的詳細資訊，請參閱[設定全系統的任務和問題偏好設定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md)。

如需有關如何更新任務之任務限制的資訊，請參閱[更新任務的任務限制](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md)。

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

## 最早可用時間與儘快可用時間之間的差異

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: [! This section is duplicated in "Earliest Available Time"]) </p>
-->

當以下所有條件存在時，「最早可用時間」限制與「儘快」限制會有所不同：

* 專案已排定從完成日程。
* 專案中的任務具有前置任務關係。
* 前置任務具有彈性任務限制。

在此情況下：

* **最早可用時間：**&#x200B;在後續任務上使用最早可用時間限制，會優先處理前置任務的彈性限制。

  例如，假設任務A是任務B的前置任務。任務B具有「最早可用時間」限制，而任務A具有「儘可能晚到」限制。 在此情況下，任務會排程在儘可能接近專案完成的時間。

* **儘快：**&#x200B;在此案例中，使用後續任務的「儘快」限制會將優先權給予後續任務。

  例如，假設任務A是任務B的前置任務。任務B具有「儘快」限制，而任務A具有「儘快」限制。 在此情況下，任務會排程儘可能接近專案開始。
