---
content-type: overview
product-area: agile-and-teams
navigation-topic: use-kanban-in-an-agile-team
title: 看板總覽
description: 請檢閱本文，以更加瞭解Kanban展示板的運作方式。
author: Jenny
feature: Agile
exl-id: d7daa6c1-dae2-4e5c-a765-6a6ebdfaa331
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '486'
ht-degree: 0%

---

# Kanban總覽

<!-- Audited: 01/2024 -->

下列章節可讓您更瞭解[!UICONTROL Kanban]展示板的運作方式。

如需K[!UICONTROL anban]方法的說明，請參閱[建立敏捷團隊](/help/quicksilver/agile/get-started-with-agile-in-workfront/create-an-agile-team.md)。

如果您有興趣從敏捷團隊[!UICONTROL Kanban]展示板移轉至[!DNL Workfront] [!UICONTROL 展示板]，請參閱[將敏捷團隊[!UICONTROL Kanban]展示板移轉至 [!DNL Workfront] 展示板](/help/quicksilver/agile/use-boards-agile-planning-tools/migrate-kanban-cards-to-boards.md)。

## [!UICONTROL Kanban]展示板配置與功能

[!UICONTROL Kanban]面板由下列元素組成：

**待處理專案欄**：顯示目前待處理專案上的所有工作。 預設不會顯示此欄。 如需有關待處理專案的詳細資訊，包括如何在[!UICONTROL Kanban]展示板上顯示，請參閱[管理敏捷待處理專案](../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md)。

**內文狀態**：表示內文如何根據內文所在的狀態列進行進度。

如需詳細資訊，請參閱[在[!UICONTROL Kanban]面板](../../agile/use-kanban-in-an-agile-team/update-the-status-of-stories.md)上更新內文的狀態。

您可以修改敏捷檢視，以自訂專案的內文狀態，如[[!UICONTROL 在]](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md#create-or-customize-an-agile-view)中建立或編輯檢視中的[建立或自訂敏捷檢視 [!DNL Adobe Workfront]](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md)一節所述。

>[!NOTE]
>
>Kanban板上預設會顯示最多50張卡片，但您可以按一下「**[!UICONTROL 顯示更多]**」來顯示其他卡片。

## 子任務和劇本之間的關係

如果內文包含子任務，您就無法更新上層內文本身的任何資訊（例如點/小時或完成百分比）。 此外，您無法跨[!UICONTROL Kanban]面板移動內文以更新其狀態。 反之，您對內文子工作所做的任何變更都會反映在內文上。 所有子工作的合併內文點或時數會決定父內文的點或時數。

例如，如果內文只有一個子作業被指定為4點，則內文本身也有4點。 如果將子任務點值變更為3，父內文的點值就會變更為3。 如果您在相同內文上建立另一個子任務，並將該子任務的點值設為4，則內文的點值會變更為7，以反映兩個子任務的組合點值。

此邏輯同樣適用於第二層子任務（子任務的子任務）。 如果子任務有一或多個第二層子任務，則會根據第二層子任務計運算元任務。

## 支援的功能

使用Kanban展示板時，您可以執行下列動作：

* [將子任務新增至[!UICONTROL Kanban]展示板上的現有劇本](../../agile/use-kanban-in-an-agile-team/add-a-subtask-to-an-existing-story.md)
* [將現有任務或問題新增到[!UICONTROL Kanban]面板](../../agile/use-kanban-in-an-agile-team/add-existing-tasks-or-issues-to-the-kanban-board.md)
* [將使用者指派給[!UICONTROL Kanban]展示板上的劇本](../../agile/use-kanban-in-an-agile-team/assign-users-to-a-story.md)
* [從[!UICONTROL Kanban]面板新增劇本和問題](../../agile/use-kanban-in-an-agile-team/add-story-from-kanban-board.md)
* [從[!UICONTROL Kanban]展示板刪除劇本或問題](../../agile/use-kanban-in-an-agile-team/delete-story-from-kanban-board.md)
* [編輯劇本資訊](../../agile/use-kanban-in-an-agile-team/edit-story-information.md)
* [在[!UICONTROL Kanban]展示板上依使用者篩選](../../agile/use-kanban-in-an-agile-team/filter-by-user.md)
* [管理[!UICONTROL Kanban]展示板上的進行中工作(WIP)限制](../../agile/use-kanban-in-an-agile-team/work-in-progress-limit-on-the-kanban-board.md)
* [重新排序[!UICONTROL Kanban]展示板上的劇本](../../agile/use-kanban-in-an-agile-team/reorder-stories-on-the-kanban-board.md)
* [更新[!UICONTROL Kanban]展示板上內文的狀態](../../agile/use-kanban-in-an-agile-team/update-the-status-of-stories.md)
* [在[!UICONTROL Kanban]展示板上的劇本上使用旗標](../../agile/use-kanban-in-an-agile-team/use-flags-on-stories.md)
* [將待處理專案新增至[!UICONTROL Kanban]面板](../../agile/use-kanban-in-an-agile-team/view-the-backlog-on-the-kanban-board.md)
