---
content-type: overview
product-area: projects
navigation-topic: task-information
title: 任務的「可以開始」總覽
description: 當任務準備開始時，Adobe Workfront會在任務中新增可以開始指標，讓您輕鬆識別開始處理任務是否安全。 您可以在任務清單或報告的檢視中檢視此指標。
author: Alina
feature: Work Management
exl-id: 158f8370-9717-4c61-99fa-e3b76a9e61cb
source-git-commit: 7427706f6ce6cad3370b91269c1b4e7a10ed09f9
workflow-type: tm+mt
source-wordcount: '431'
ht-degree: 0%

---

# 任務的「可以開始」總覽

當任務準備開始時，Adobe Workfront會在任務中新增可以開始指標，讓您輕鬆識別開始處理任務是否安全。 您可以在任務清單或報告的檢視中檢視此指標。

當任務已準備好進行時，任務上的「可以開始」欄位會設定為True。

## Workfront如何將任務標示為「可以開始」

Workfront會在「可以開始」欄位將任務標籤為「True」之前，檢查下列專案：

* 如果任務有父系，其父系的「可以開始」值是否設定為True。 如果父系的值是False，則所有子工作的值也會設定為False。
* 任務的前置任務及其父項的前置任務是否完整。 如果任務完成，任務的「可以開始」值會設為True。 如果任一任務前置任務或其父項的前置任務未完成，或狀態為「完成 — 未決核准」，則任務的「可以開始」值會設為False。
* 工作相依性型別是「開始 — 開始」或「開始 — 完成」。 如果相依性型別為「開始 — 開始」或「開始 — 完成」，則相依性任務在前置任務進行中後（或在前置任務完成百分比大於1%後），會將「可以開始」旗標設定為「真」。

  如需前置任務的相關資訊，請參閱[前置任務概觀](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md)。

## 識別準備開始之任務的相關考量事項

* 如果任務與其前置任務之間的「相依性型別」是「開始 — 開始」，則前置任務必須先開始，前置任務關係才會被視為已解決，而後續任務才能開始。 如需相依性型別的相關資訊，請參閱[工作相依性型別的概觀](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md)。
* 如果任務具有跨專案前置任務，前置任務的完成不會觸發可開始指示器自動套用至前置任務。 您必須手動重新計算後續任務專案的時間表，或者Workfront必須先自動重新計算，後續任務才會顯示為「可以開始」任務。 如需重新計算專案時間表的相關資訊，請參閱[重新計算專案時間表](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md)。

  如需跨專案前置任務的相關資訊，請參閱[建立跨專案前置任務](../../../manage-work/tasks/use-prdcssrs/cross-project-predecessors.md)。
