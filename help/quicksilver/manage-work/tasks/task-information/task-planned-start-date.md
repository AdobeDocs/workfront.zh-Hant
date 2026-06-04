---
content-type: overview
product-area: projects
navigation-topic: task-information
title: 任務計劃開始日期總覽
description: 任務的計劃開始日期是您作為任務建立者決定開始任務工作的日期。 計畫任務日期會影響專案的日期和時間表。 如需專案計劃開始日期的相關資訊，請參閱專案計劃開始日期概觀。
author: Alina
feature: Work Management
exl-id: 2ac6327f-4a13-4fb8-ad8e-03d032221483
TQID: https://experienceleague.adobe.com/5VM6UTgVLYBRMGtwWXQ6LbXqwQiYI1EuIPl7GbQSAwk
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: b91c0848-76c4-4da4-8b81-3aade0518dd0
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 619
ht-degree: 2%

---

# 任務計劃開始日期總覽

<!-- Audited: 6/2025 -->

任務的計劃開始日期是您作為任務建立者決定開始任務工作的日期。 計畫任務日期會影響專案的日期和時間表。 如需專案計劃開始日期的相關資訊，請參閱[專案計劃開始日期概觀](../../../manage-work/projects/planning-a-project/project-planned-start-date.md)。

## 任務的計劃開始日期

您可以指定任務的計劃開始日期，也可以留給Adobe Workfront根據特定條件進行計算。

* [手動設定任務的計劃開始日期](#manually-set-the-planned-start-date-of-a-task)
* [如何計算任務的計劃開始日期](#how-the-planned-start-date-is-calculated-for-a-task)

### 手動設定任務的計劃開始日期 {#manually-set-the-planned-start-date-of-a-task}

設定任務的計劃開始日期取決於您指派給任務的任務限制型別。

建立任務時，您可以手動設定計劃開始日期。 如需詳細資訊，請參閱[在專案中建立任務](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md)。

當您選取下列任一「任務限制」時，可以手動指定「計劃開始日期」：

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>任務限制型別</strong> </p> </th> 
   <th> <p><strong>手動變更計畫完成日期的效果</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>必須開始時間</p> <p>開始時間不早於</p> <p>開始時間不晚於</p> </td> 
   <td> <p><span class="s1">已調整計畫完成日期以保持持續期間。</span> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>固定日期</p> </td> 
   <td> <p>持續時間會調整以保持計畫完成日期相同。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 如何計算任務的計劃開始日期 {#how-the-planned-start-date-is-calculated-for-a-task}

當系統自動計算時，下列專案會影響任務的「計劃開始日期」：

* 在設定的任務和問題區域中的開始日期偏好設定設定

  您的Workfront或群組管理員可決定新任務的開始日期是和專案的計劃開始日期相同，還是您建立任務的日期。

  有關任務和問題偏好設定的資訊，請參閱[設定全系統的任務和問題偏好設定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md)。

* 任務限制

  如需任務限制的詳細資訊，請參閱[任務限制總覽](../../../manage-work/tasks/task-constraints/task-constraint-overview.md)。

* 任務前置任務關係

  如需有關前置任務的詳細資訊，請參閱[前置任務概觀](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md)。

* 專案開始日期，從開始日期開始排程專案時。
* 任務的主要受指派人的休假排程。

  當主要受指派人在任務持續期間已排定休假時，則當「使用者休假」欄位中選取了考慮使用者在任務持續期間的休假設定時，任務的計畫日期會據此調整。 新專案會從「專案偏好設定」區域繼承此設定，但您可以在專案層級編輯此設定。

  例如，如果一項限製為「儘快」的任務排程在6月1日開始並在6月3日完成，而主要受指派人已在6月1日標示為休假，則任務的「計劃開始日期」會變成6月2日。

  如需使用者休假偏好設定的相關資訊，請參閱[設定全系統的專案偏好設定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)或[編輯專案](../../../manage-work/projects/manage-projects/edit-projects.md)。

自動設定時，「計劃開始日期」會根據下列計算方式決定：

```
Planned Start Date = Planned Completion Date - Task Duration
```

例如，如果您的任務完成日期為9月16日且持續時間為10天，則計劃開始日期為9月6日。

>[!NOTE]
>
> 專案的更新型別也必須設為自動與變更時或自動，才能自動調整計畫時數與期間。\
>如需有關更新型別的詳細資訊，請參閱[選取專案更新型別](../../../manage-work/projects/manage-projects/select-project-update-type.md)。
