---
content-type: overview
product-area: projects
navigation-topic: task-duration
title: 期間型別概觀：簡單
description: 簡易期間型別是一種期間型別，您可以在Adobe Workfront中為任務設定。
author: Alina
feature: Work Management
exl-id: 9bb472db-1448-467e-93ca-611453e1c00a
source-git-commit: 0792651822fd85cb3bfbb754aaf949c4fc4038a1
workflow-type: tm+mt
source-wordcount: '322'
ht-degree: 0%

---

# 期間型別概觀：簡單

<!-- Audited: 5/2025 -->

簡易期間型別是一種期間型別，您可以在Adobe Workfront中為任務設定。 如需Workfront中期間型別的詳細資訊，請參閱[任務期間與期間型別概觀](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md)。

## 簡單期間型別概觀

您的Workfront或群組管理員可以將系統或群組的預設期間型別設定為「簡單」。 在此情況下，所有新任務都將以此持續時間型別建立。

如需有關將您的任務和問題偏好設定變更為系統層級或群組層級專案偏好設定一部分的資訊，請參閱[設定全系統的任務和問題偏好設定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md)。

當任務具有簡單期間型別時，會發生下列情況：

* 專案經理可以修改任務的期間和計畫時數，在修改這些時數應在受指派人之間的分配方式時。

  如需相關資訊，請參閱[使用簡單期間型別](../../../manage-work/tasks/taskdurtn/update-planned-hours-duration-for-simple-duration-task.md)更新任務的計畫時數與期間。

  >[!IMPORTANT]
  >
  >當您第一次建立任務並指派給它簡易期間型別，但未指定期間時，Workfront會根據您為任務指定的計畫時數金額計算任務的期間。 如果您手動修改簡單期間任務的期間，Workfront會停止比對計畫時數與期間，因為它假設您要手動定義它們。
  >
  >Workfront會使用下列公式計算未手動修改工期的工作工期：
  >
  > `Task Duration = Task Planned Hours / Typical hours per work day`
  >
  >您的Workfront管理員會在您執行個體設定的專案偏好設定區域中定義`Typical hours per work day`。

* 配置百分比已隱藏，但配置時數可供編輯。
* 所有新客戶的系統層級「期間型別」皆設為「簡單」。

## 將任務的期間型別變更為簡單

如需有關變更任務期間型別的資訊，請參閱[更新任務的期間型別](../../../manage-work/tasks/taskdurtn/update-duration-type-of-task.md)。

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: replaced with new article linked above)</p>
-->

<!--
<ol data-mc-conditions="QuicksilverOrClassic.Draft mode">
<li value="1">Go to a task for which you want to change the Duration Type.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click <strong>Task Details</strong> in the left panel, then in the Overview area double click <strong>Duration Type</strong>. </p> </li>
<li value="3"> <p>Select <strong>Simple</strong> from the drop-down menu.</p> </li>
<li value="4">Click <strong>Save</strong> <strong>Changes</strong><strong>.</strong></li>
</ol>
-->
