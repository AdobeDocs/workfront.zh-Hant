---
content-type: overview
product-area: projects
navigation-topic: task-information
title: 任務計畫完成日期概要
description: 任務的計畫完成日期是任務設定為完成的日期。
author: Alina
feature: Work Management
exl-id: b0522db5-9c68-4b1a-82c8-5a9e613eb2ff
TQID: https://experienceleague.adobe.com/wzIsNsuGQcxPO78TcEzCz8juaIeUp7MNbjIMG7-5e8w
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40cid: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87effid: b91c0848-76c4-4da4-8b81-3aade0518dd0id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 789
ht-degree: 1%

---

# 任務計畫完成日期總覽

任務的計畫完成日期是任務設定為完成的日期。

您可以指定任務的規劃完成日期，也可以留給Adobe Workfront根據特定條件進行計算。

專案上任務的計畫完成日期決定專案從開始日期排程時的計畫完成日期。 如需有關專案計畫完成日期的詳細資訊，請參閱[設定專案計畫完成日期](../../../manage-work/projects/planning-a-project/project-planned-completion-date.md)。

>[!NOTE]
>
>任務的計畫完成日期與任務的認可日期或任務的預計完成日期有下列不同：
>
>* 「認可日期」是指指派給任務之人員手動估計其將完成任務的日期。 如需詳細資訊，請參閱下列文章：
>
>   * [認可日期總覽](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md)
>   * 認可日期與計畫完成日期之間的[互動](../../../manage-work/projects/updating-work-in-a-project/interactions-between-commit-and-planned-completion-dates.md)。
>
>* 「預計完成日期」是Workfront計算的日期，會考慮任務延遲、任務或其前置任務的時間表以及其他因素，以決定任務可實際完成的實際日期。 如需詳細資訊，請參閱[專案、任務和問題的預計完成日期總覽](../../../manage-work/projects/planning-a-project/project-projected-completion-date.md)。
>

## 手動設定任務的計畫完成日期

您必須具有任務的「編輯」存取權及任務的「管理」許可權，才能更新任務的規劃完成日期。

設定任務的「計畫完成日期」取決於您指派給任務的「任務限制」型別。

您可以在Workfront的下列區域中手動設定「規劃完成日期」：

* 在「編輯任務」方塊中，建立或編輯任務時。 如需詳細資訊，請參閱[編輯工作](../../../manage-work/tasks/manage-tasks/edit-tasks.md)。
* 在「工作詳細資訊」區域中。 如需相關資訊，請參閱[在任務詳細資訊總覽區域](../../../manage-work/tasks/manage-tasks/task-information-in-overview.md)中管理任務資訊。
* 如果在摘要面板中檢視任務時顯示規劃完成日期，則位於首頁區域。 如需詳細資訊，請參閱[更新或編輯首頁區域的工作專案](../../../workfront-basics/using-home/using-the-home-area/update-and-edit-work-item-home.md)。
* 在任務標題中。 如需詳細資訊，請參閱[新物件標頭](../../../workfront-basics/the-new-workfront-experience/new-object-headers.md)。
* 在檢視中顯示「規劃完成日期」欄位時，於任務清單或報告中。

  如需詳細資訊，請參閱[編輯清單中的工作](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md)。

當您選取下列任一「任務限制」時，可以手動指定「計畫完成日期」：

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
   <td> <p>必須完成時間</p> <p>完成時間不晚於</p> <p>完成時間不早於</p> </td> 
   <td> <p><span class="s1">已調整計劃開始日期以保持持續期間不變。</span> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>固定日期</p> </td> 
   <td> <p>持續時間會調整以保持計劃開始日期相同。</p> </td> 
  </tr> 
 </tbody> 
</table>

## Workfront如何自動計算任務的規劃完成日期

當系統自動計算時，下列專案會影響任務的「計畫完成日期」：

* 任務限制

  如需有關任務限制的詳細資訊，請參閱文章[任務限制總覽](../../../manage-work/tasks/task-constraints/task-constraint-overview.md)。

* 任務前置任務關係

  如需有關前置任務的詳細資訊，請參閱文章[前置任務概觀](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md)。

* 專案完成日期，專案排定自完成日期開始的時間。
* 任務之主要受指派人的休假排程。

  當主要受指派人在任務持續期間已排程休假時，則當&#x200B;**使用者休假**&#x200B;欄位中選取了&#x200B;**在任務持續期間中考慮使用者休假**&#x200B;設定時，任務的計畫日期會據此調整。 新專案會從「專案偏好設定」區域繼承此設定，但您可以在專案層級編輯此設定。

  例如，如果一項限製為「儘快」的任務排程在6月1日開始並在6月3日完成，而主要受指派人將6月2日標示為「休假」，則任務計畫完成日期會變成6月4日。

  如需&#x200B;**使用者休假**&#x200B;偏好設定的相關資訊，請參閱文章[設定全系統的專案偏好設定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)或[編輯專案](../../../manage-work/projects/manage-projects/edit-projects.md)。

* 如果任務與核准相關聯，則為與核准設定相關聯的時間量。 如需詳細資訊，請參閱[設定全域核准設定](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md)。

自動設定時，「計畫完成日期」會根據下列計算方式決定：

```
Planned Completion Date = Planned Start Date + Duration
```

例如，如果您的任務開始日期為9月16日且期間為10天，則計畫完成日期為9月26日。

>[!NOTE]
>
> 專案的更新型別必須設定為自動與變更時或自動，才能自動調整計畫時數與期間。\
>如需有關更新型別的詳細資訊，請參閱文章[選取專案更新型別](../../../manage-work/projects/manage-projects/select-project-update-type.md)。
