---
content-type: overview
product-area: projects
navigation-topic: task-information
title: 「可以開始」任務的概述
description: 當任務準備好開始時，Adobe Workfront會在任務中新增「可開始」指標，以輕鬆識別您開始執行任務是否安全。 您可以在任務清單或報告的視圖中查看此指標。
author: Alina
feature: Work Management
exl-id: 158f8370-9717-4c61-99fa-e3b76a9e61cb
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '390'
ht-degree: 0%

---

# 任務的「可以開始」概述

當任務準備好開始時，Adobe Workfront會在任務中新增「可開始」指標，以輕鬆識別您開始執行任務是否安全。 您可以在任務清單或報告的視圖中查看此指標。

當任務準備就緒後，該任務的「可啟動」欄位將設定為True。

## Workfront如何將任務標示為「可開始」

Workfront會先檢查下列事項，然後才在「可開始」欄位中將任務標示為True:

* 如果任務具有父級，則它將檢查其設定為True的父級的「可啟動」值是否為Can Start。 如果父項的值為False，則所有子任務的值都將Can Start設定為False。 
* 它還檢查任務的前任及其父代的前任是否完成。 如果完成，則任務的「可啟動」值設定為True。 如果任務前置任務或其父任務的前置任務未完成，或狀態為「完成 — 待批」，則任務的「可啟動」值將設定為False。 

   有關任務前置任務的資訊，請參見 [任務前置任務概述](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

## 識別可開始任務的考量事項

* 如果任務與其前置任務之間的依賴關係類型為「啟動 — 啟動」，則前置任務必須在被視為解決前置關係且後續任務可以啟動之前啟動。 如需相依性類型的相關資訊，請參閱 [任務相關性類型概述](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).
* 如果任務具有跨項目前置任務，則前置任務的完成不會觸發「可以啟動」(Can Start)指標自動應用於後繼任務。 您必須手動重新計算後繼項目的時間表，或者，在後續任務顯示為可啟動任務之前，Workfront必須自動重新計算它。 有關重新計算項目時間表的詳細資訊，請參見 [重新計算項目時間表](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).

   如需跨專案前置項目的相關資訊，請參閱 [建立跨專案的前置項目](../../../manage-work/tasks/use-prdcssrs/cross-project-predecessors.md).
