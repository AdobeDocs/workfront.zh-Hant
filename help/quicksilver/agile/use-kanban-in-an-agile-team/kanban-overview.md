---
content-type: overview
product-area: agile-and-teams
navigation-topic: use-kanban-in-an-agile-team
title: 看板概述
description: 請查看本文，以更好地了解看板板的功能。
author: Lisa
feature: Agile
exl-id: d7daa6c1-dae2-4e5c-a765-6a6ebdfaa331
source-git-commit: a478e5355db33e076b321a6219442198901f3252
workflow-type: tm+mt
source-wordcount: '444'
ht-degree: 0%

---

# 看板概述

以下幾節可讓您更清楚了解 [!UICONTROL 看板] 董事會職能：

## [!UICONTROL 看板] 板佈局與功能

此 [!UICONTROL 看板] 展示板包含下列元素：

**積壓列**:顯示當前積壓的所有任務。 預設不會顯示此欄。 如需積壓工作的詳細資訊，包括如何在 [!UICONTROL 看板] 展示板，請參閱 [管理敏捷積壓](../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md).

**動態狀態**:根據文章所在的狀態列指示文章的進展情況。

如需詳細資訊，請參閱 [更新上的動態狀態 [!UICONTROL 看板] 展示板](../../agile/use-kanban-in-an-agile-team/update-the-status-of-stories.md).

您可以修改敏捷檢視，為專案自訂動態狀態，如區段所述 [[!UICONTROL 建立或自訂敏捷檢視]](../../reports-and-dashboards/reports/reporting-elements/views-overview.md#customizing-an-agile-view) in [檢視概觀，於 [!DNL Adobe Workfront]](../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

>[!NOTE]
>
>預設情況下，看板板上最多顯示50張卡，但您可以按一下 **[!UICONTROL 顯示更多]** 來顯示其他卡片。

## 子任務與動態之間的關係

如果文章包含子任務，則無法更新父文章本身的任何資訊（如點/小時或完成百分比）。 此外，您無法將故事 [!UICONTROL 看板] 展示板以更新其狀態。 相反，你對故事子任務所做的任何改變都反映在故事上。 所有子任務的合併動態點或小時決定父動態的點或小時。

例如，如果一個故事只有一個子任務值為4點，那麼故事本身也有4點。 如果將子任務點值更改為3，則父小節的點值將更改為3。 如果在同一篇文章上建立另一個子任務，並將該子任務的點值設定為4，則文章的點值將更改為7，以反映這兩個子任務的合併點值。

同樣的邏輯適用於第二層子任務（子任務的子任務）。 如果子任務具有一個或多個第二級子任務，則根據第二級子任務計算子任務。

## 支援的功能

使用看板板時，您可以執行以下操作：

* [將子任務新增至 [!UICONTROL 看板] 展示板](../../agile/use-kanban-in-an-agile-team/add-a-subtask-to-an-existing-story.md)
* [將現有任務或問題新增至 [!UICONTROL 看板] 展示板](../../agile/use-kanban-in-an-agile-team/add-existing-tasks-or-issues-to-the-kanban-board.md)
* [將使用者指派至 [!UICONTROL 看板] 展示板](../../agile/use-kanban-in-an-agile-team/assign-users-to-a-story.md)
* [從 [!UICONTROL 看板] 展示板](../../agile/use-kanban-in-an-agile-team/add-story-from-kanban-board.md)
* [從 [!UICONTROL 看板] 展示板](../../agile/use-kanban-in-an-agile-team/delete-story-from-kanban-board.md)
* [編輯動態資訊](../../agile/use-kanban-in-an-agile-team/edit-story-information.md)
* [依使用者篩選 [!UICONTROL 看板] 展示板](../../agile/use-kanban-in-an-agile-team/filter-by-user.md)
* [在 [!UICONTROL 看板] 展示板](../../agile/use-kanban-in-an-agile-team/work-in-progress-limit-on-the-kanban-board.md)
* [在 [!UICONTROL 看板] 展示板](../../agile/use-kanban-in-an-agile-team/reorder-stories-on-the-kanban-board.md)
* [更新上的動態狀態 [!UICONTROL 看板] 展示板](../../agile/use-kanban-in-an-agile-team/update-the-status-of-stories.md)
* [在 [!UICONTROL 看板] 展示板](../../agile/use-kanban-in-an-agile-team/use-flags-on-stories.md)
* [將積壓工作新增至 [!UICONTROL 看板] 展示板](../../agile/use-kanban-in-an-agile-team/view-the-backlog-on-the-kanban-board.md)
