---
content-type: overview
product-area: projects
navigation-topic: task-information
title: 任務計畫起始日期概覽
description: 任務的計畫起始日期是您作為任務建立者決定任務上的工作應開始的日期。 計畫任務日期會影響項目的日期和時間表。 有關項目計畫起始日期的資訊，請參閱項目計畫起始日期概覽。
author: Alina
feature: Work Management
exl-id: 2ac6327f-4a13-4fb8-ad8e-03d032221483
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '626'
ht-degree: 2%

---

# 任務計畫起始日期概覽

任務的計畫起始日期是您作為任務建立者決定任務上的工作應開始的日期。 計畫任務日期會影響項目的日期和時間表。 有關項目計畫起始日期的資訊，請參閱 [項目計劃開始日期概覽](../../../manage-work/projects/planning-a-project/project-planned-start-date.md).

## 任務的計畫起始日期

您可以指定任務的「計劃開始日期」，或根據特定標準讓Adobe Workfront自行計算。 

* [人工設定任務的計畫起始日期](#manually-set-the-planned-start-date-of-a-task)
* [如何計算任務的計畫起始日期](#how-the-planned-start-date-is-calculated-for-a-task)

### 人工設定任務的計畫起始日期 {#manually-set-the-planned-start-date-of-a-task}

設定任務的「計畫起始日期」取決於您分配給任務的任務約束類型。 

您可以在建立任務時手動設定計畫起始日期，如文章所述 [在專案中建立任務](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md).

在選擇以下任一任務約束時，您可以人工指定計畫起始日期： 

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>任務約束類型</strong> </p> </th> 
   <th> <p><strong>人工更改計畫完成日期的效果</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>必須開始時間</p> <p>開始時間不早於</p> <p>開始時間不晚於</p> </td> 
   <td> <p><span class="s1">為了保持持續時間不變，計畫完成日期將被調整。</span> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>固定日期</p> </td> 
   <td> <p>為了使計畫完成日期保持相同，會調整持續時間。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 如何計算任務的計畫起始日期 {#how-the-planned-start-date-is-calculated-for-a-task}

當系統自動計算任務時，以下內容可能會影響任務的計畫起始日期：

* 「設定」的「任務和問題」區域中的「開始日期」首選項設定

   您的Workfront或組管理員可以確定新任務是從與項目的計劃開始日期相同的日期開始，還是從您建立任務的日期開始。

   如需工作與問題偏好設定的相關資訊，請參閱 [配置全系統任務和問題首選項](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

* 任務限制

   有關「任務約束」的詳細資訊，請參閱文章 [任務約束概覽](../../../manage-work/tasks/task-constraints/task-constraint-overview.md)

* 任務前置關係

   有關任務前置任務的詳細資訊，請參閱文章 [任務前置任務概述](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

* 項目開始日期，從開始日期開始計畫項目時。
* 任務的主要受託人的計畫時間。

   當主要受託人在任務期間計畫了超時時，任務的計畫日期將相應調整 **考慮任務持續時間中的用戶超時** 已為 **用戶關閉時間** 欄位。 新項目將從「項目首選項」區域繼承此設定，但您可以在項目級別編輯此設定。

   例如，如果計畫在6月1日開始並在6月3日完成具有「盡快約束」的任務，而主要受託人在6月1日標籤為「超時」，則「計畫起始日期」將變為6月2日。

   如需 **用戶關閉時間** 首選項，請參閱文章  [配置系統範圍的項目首選項](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) 或 [編輯專案](../../../manage-work/projects/manage-projects/edit-projects.md).

自動設定後，計畫起始日期將根據以下計算確定： 

```
Planned Start Date = Planned Completion Date - Task Duration
```

例如，如果任務的完成日期為9月16日，持續時間為10天，則計畫起始日期為9月6日。

>[!NOTE]
>
> 項目的「更新類型」還必須設定為「自動且更改時」或「自動」，以便自動調整計畫小時數和持續時間。\
如需更新類型的詳細資訊，請參閱文章 [選擇項目更新類型](../../../manage-work/projects/manage-projects/select-project-update-type.md).
