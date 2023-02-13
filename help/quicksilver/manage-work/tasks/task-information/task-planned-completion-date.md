---
content-type: overview
product-area: projects
navigation-topic: task-information
title: 任務計畫完成日期概覽
description: 任務的計畫完成日期是任務設定為完成的日期。
author: Alina
feature: Work Management
exl-id: b0522db5-9c68-4b1a-82c8-5a9e613eb2ff
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '775'
ht-degree: 1%

---

# 任務計畫完成日期概覽

任務的計畫完成日期是任務設定為完成的日期。

您可以指定任務的「計畫完成日期」，也可以保留給Adobe Workfront，以根據特定標準計算。 

項目上任務的計畫完成日期決定從起始日期開始計畫項目時項目的計畫完成日期。 有關項目計畫完成日期的詳細資訊，請參閱 [設定項目計畫完成日期](../../../manage-work/projects/planning-a-project/project-planned-completion-date.md).

>[!NOTE]
>
>任務的計畫完成日期與任務的提交日期或任務的預計完成日期不同，方法如下：
>
>* 「提交日期」是指分配給任務的人員手動估計完成任務的日期。 如需詳細資訊，請參閱下列文章：
   * [提交日期概述](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md)
   * [提交日期與計畫完成日期之間的交互](../../../manage-work/projects/updating-work-in-a-project/interactions-between-commit-and-planned-completion-dates.md).
* 預計完成日期是Workfront計算的日期，它考慮任務延遲、任務或其前置任務的時間表，以及確定實際完成任務時的實際使用日期的其他因素。 如需詳細資訊，請參閱 [項目、任務和問題的預計完成日期概覽](../../../manage-work/projects/planning-a-project/project-projected-completion-date.md).
>


## 人工設定任務的計畫完成日期

您必須具有任務的「編輯」訪問權限和「管理」權限，才能更新任務的「計畫完成日期」。

設定任務的計畫完成日期取決於分配給任務的任務約束類型。 

您可以在Workfront的以下區域人工設定計畫完成日期：

* 在「編輯任務」框中，建立或編輯任務時。 如需詳細資訊，請參閱 [編輯任務](../../../manage-work/tasks/manage-tasks/edit-tasks.md).
* 在「任務詳細資訊」區域中。 如需詳細資訊，請參閱 [在「任務詳細資訊概覽」區域中管理任務資訊](../../../manage-work/tasks/manage-tasks/task-information-in-overview.md).
* 如果查看任務時顯示了計畫完成日期，則在「首頁」區域。 如需詳細資訊，請參閱 [在「首頁」區域更新或編輯工作項](../../../workfront-basics/using-home/using-the-home-area/update-and-edit-work-item-home.md).
* 在任務標題中。 如需詳細資訊，請參閱 [新物件標題](../../../workfront-basics/the-new-workfront-experience/new-object-headers.md).
* 在「計畫完成日期」欄位顯示在視圖中的任務清單或報表中。

   如需詳細資訊，請參閱 [編輯清單中的任務](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md).

在選擇以下任何任務約束時，您可以人工指定計畫完成日期： 

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
   <td> <p>必須完成時間</p> <p>完成時間不晚於</p> <p>完成時間不早於</p> </td> 
   <td> <p><span class="s1">為了保持「持續時間」相同，計畫起始日期將被調整。</span> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>固定日期</p> </td> 
   <td> <p>為了使計畫起始日期保持相同，會調整「持續時間」。</p> </td> 
  </tr> 
 </tbody> 
</table>

## Workfront如何自動計算任務的計畫完成日期

當系統自動計算任務時，以下內容會影響任務的計畫完成日期：

* 任務限制

   有關「任務約束」的詳細資訊，請參閱文章 [任務約束概覽](../../../manage-work/tasks/task-constraints/task-constraint-overview.md).

* 任務前置關係

   有關任務前置任務的詳細資訊，請參閱文章 [任務前置任務概述](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

* 項目完成日期，從完成日期開始計畫項目時。
* 任務的主要受託人的計畫時間。

   當主要受託人在任務期間計畫了超時時，任務的計畫日期將相應調整 **考慮任務持續時間中的用戶超時** 已為 **用戶關閉時間** 欄位。 新項目將從「項目首選項」區域繼承此設定，但您可以在項目級別編輯此設定。

   例如，如果計畫在6月1日開始並在6月3日完成具有「盡快約束」的任務，而主要受託人在6月2日標籤為「暫停」，則任務「計畫完成日期」將變為6月4日。

   如需 **用戶關閉時間** 首選項，請參閱文章 [配置系統範圍的項目首選項](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) 或 [編輯專案](../../../manage-work/projects/manage-projects/edit-projects.md).

* 與「批准設定」關聯的時間量（如果任務與批准相關聯）。 如需詳細資訊，請參閱 [配置全局批准設定](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md).

自動設定後，計畫完成日期將根據以下計算確定： 

```
Planned Completion Date = Planned Start Date + Duration
```

例如，如果任務的起始日期為9月16日，持續時間為10天，則計畫完成日期為9月26日。

>[!NOTE]
 項目的「更新類型」必須設定為「自動」和「更改時」或「自動」，以便自動調整「計畫小時數」和「持續時間」。\
如需更新類型的詳細資訊，請參閱文章 [選擇項目更新類型](../../../manage-work/projects/manage-projects/select-project-update-type.md).
