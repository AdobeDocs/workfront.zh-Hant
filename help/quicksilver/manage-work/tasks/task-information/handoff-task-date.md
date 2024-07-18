---
content-type: overview
product-area: projects
navigation-topic: task-information
title: 任務移交日期概觀
description: 「移交日期」是任務可供工作的日期。 這通常表示其前置任務已解決，且任務的受指派人可以開始處理它。
author: Alina
feature: Work Management
exl-id: caf2dbba-5311-418d-8c82-ddcc256f9926
source-git-commit: b774a74863bb35e3477a69ff11189c40a6d66437
workflow-type: tm+mt
source-wordcount: '723'
ht-degree: 2%

---

# 任務移交日期概觀

「移交日期」是任務可供工作的日期。 這通常表示其前置任務已解決，且任務的受指派人可以開始處理它。

>[!TIP]
>
>問題和專案的移交日期不存在。

## Adobe Workfront如何計算移交日期

>[!NOTE]
>
>只有當專案狀態等於以下狀態時，才會計算「移交日期」：
>
>* 保留
>* 目前
>* 完成
>* 廢棄
>

Workfront使用下列規則來計算任務的移交日期：

* **當任務具有未完成的前置任務**&#x200B;時：任務的移交日期為Null。
* **當任務具有完整的前置任務時**：移交日期與前置任務的實際完成日期相同。 如果前置任務有延遲，Workfront會使用下列公式計算後續任務的「移交日期」：

  `Successor Handoff Date = Predecessor Actual Completion Date + Lag`

  如需延遲時間的詳細資訊，請參閱[延遲型別概觀](../use-prdcssrs/lag-types.md)。

  如果後續任務有多個前置任務，則根據前置任務的最新「實際完成日期」計算「移交日期」。 例如，如果兩個前置任務的實際完成日期是2022年11月8日和2022年11月20日，則後續任務的移交日期為2022年11月20日。

  >[!NOTE]
  >
  >   根據實際完成日期計算後續任務的「移交日期」或前置任務無論是否強制執行，都相同。 如需強制前置任務的詳細資訊，請參閱[強制前置任務](../use-prdcssrs/enforced-predecessors.md)。


* **當任務沒有前置任務和**&#x200B;時：

   * **計劃開始日期在過去**：如果任務沒有強制的限制設定，則移交日期與專案的計劃開始日期相同。 若是任務有強制限制的情況，請參閱下方的「當任務有計畫日期的強制限制時」一節。
   * **計劃開始日期是未來日期（目前日期之後的任何日期）**：如果任務沒有強制限制設定，則移交日期與任務的計劃開始日期相同。 若是任務有強制限制的情況，請參閱下方的「當任務有計畫日期的強制限制時」一節。

>[!NOTE]
>
>當任務具有跨專案前置任務時，僅當出現以下任一情況時，才會重新計算後續任務的移交日期：
>
>* 您手動重新計算後置者專案的時間表。 您必須擁有專案的管理許可權才能重新計算時間表。
>* 後續專案的時間表會在夜間自動重新計算。
>
>如需重新計算專案時間表的相關資訊，請參閱[重新計算專案時間表](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md)。

* **當任務具有計畫日期的強制限制時**：移交日期會依限制型別以及任務是否具有實際開始日期而有所不同。\
  下列是任務的強制限制：

   * 必須開始時間
   * 必須完成時間
   * 開始時間不早於
   * 開始時間不晚於
   * 固定日期

  存在下列情況：

   * **當任務的限製為「必須開始於」或「開始時間不得早於**」時：如果任務限制日期是過去的時間，而且任務上沒有「實際開始日期」（任務尚未開始），則移交日期是任務開始作業時可能的最近日期。 如果任務已開始，則移交日期等於專案的開始日期。
   * **當任務的限製為「必須完成於」或「開始不得晚於**」時：如果任務限制日期是未來日期，而且任務沒有實際開始日期（任務尚未開始），則移交日期是任務的計劃開始日期。 如果任務上有「實際開始日期」，則「移交日期」為專案的開始日期。
   * **當任務具有固定日期的限制時**：移交日期是任務的計劃開始日期，無論任務是否有前置任務，也無論前置任務是否已完成。

<!--these are old descriptions, edited by Anna As. on August 25, 2023 in this issue - https://experience.adobe.com/#/@adobeinternalworkfront/so:hub-Hub/workfront/issue/64c0032500018fabd4fc484167eb10dc/updates
   * When the task has a constraint of Must Start On or Start No Earlier Than, the Handoff Date is the Constraint date, unless there is an Actual Start Date on the task. If there is an Actual Start Date on the task, the Handoff Date is the Actual Completion Date of the predecessor.
   * When the task has a constraint of Must Finish On or Start No Later Than, the Handoff Date is always the Actual Completion Date of the predecessor, regardless of whether there is an Actual Start Date on the task or not. 
   * When the task has a constraint of Fixed Dates, the Handoff Date is the Planned Start Date of the task, regardless of whether it has a predecessor or not and regardless of whether the predecessor is completed or not.

-->

## 尋找移交日期

您可以在任務報告或任務清單檢視中顯示任務的「移交日期」。\
如需建立報告的詳細資訊，請參閱[建立自訂報告](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)。
