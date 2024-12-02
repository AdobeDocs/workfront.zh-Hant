---
content-type: overview
product-area: projects
navigation-topic: task-duration
title: 期間型別概要：計算的指定
description: 「計算的任務指派」是一種期間型別，您可以在Adobe Workfront中為任務設定。 如需Workfront中期間型別的一般資訊，請參閱任務期間與期間型別概觀。
author: Alina
feature: Work Management
exl-id: 5f1f6109-5d54-4c3f-9aa5-dc6ce165a1cd
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '482'
ht-degree: 0%

---

# 期間型別概要：計算的指定

「計算的任務指派」是一種期間型別，您可以在Adobe Workfront中為任務設定。 如需Workfront中期間型別的一般資訊，請參閱[任務期間與期間型別概觀](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md)。

## 計算的工作分派期間型別概要

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: This Hub issue has a powerpoint that highlights information that is useful to users when using Calculated Assignment duration type. I don't think we can use the powerpoint, because it's old. I also don't know if the things they discuss are still relevant, since the PP is from 2015. I've closed the issue, but I'm putting a link here just in case the info is useful. https://hub.workfront.com/issue/5a9dd7d5007d02a8966014557c23cc89/updates)</p>
-->

* 當您使用計算的指派工期型別時，必須指定任務的工期與計畫時數。 Workfront接著將「計畫時數」的量除以「工期」中的時數，再除以指派給任務的資源數，以計算每個資源的配置百分比（計算工作分派）。 每個資源的配置百分比會平均有相同的值。 在此情況下，您無法修改每個資源的配置值。
* 您的Workfront或群組管理員可以將您系統或群組的預設「期間型別」設定為「計算指派」。 在此情況下，所有新任務都將以此期間型別建立。 如需有關將您的任務和問題偏好設定變更為系統層級或群組層級專案偏好設定一部分的資訊，請參閱[設定全系統的任務和問題偏好設定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md)。

  在此情況下，任務的預設值為1天期間，預設值為0小時計畫時數。 除非專案經理設定更精確的期間並以實際的估計填入計畫時數欄位，否則資源似乎配置不足。

在下列情況下，計算的指派是慣用的期間型別：

* 當指派具有活動視窗，但未完成其工作所分配的整個期間時。 例如，您被指派在週末之前將報告遞送給您的主管。 您有5天的工期，但您只需要10個小時即可草擬檔案。
* 當由於專案經理可以相互獨立地估計計畫持續時間和計畫投入量而將單一資源指派給任務時。

  您可以對相同結果使用「已計算的工作期間型別」，但專案經理必須輸入資源的百分比配置，才能影響已計算的「計畫時數」值。 這使得專案規劃更加困難和耗時。

每個資源的配置百分比計算如下：

```
Planned Hours / Duration / Number of Resources = Allocation Percentage for each resource
```

例如，在下面概述的案例中，每個任務的工期為3天。 專案經理手動輸入「持續時間」（3天或24小時）和「計畫時數」，因此會計算配置百分比（或指定百分比）：

![](assets/calcassign-350x80.png)

## 將任務的期間型別變更為計算的任務指派

如需有關變更任務期間型別的資訊，請參閱[更新任務的期間型別](../../../manage-work/tasks/taskdurtn/update-duration-type-of-task.md)。

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: replaced with new article linked above)</p>
-->

<!--
<ol data-mc-conditions="QuicksilverOrClassic.Draft mode">
<li value="1">Go to a task for which you want to change the Duration Type.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click <strong>Task Details</strong> in the left panel, then in the Overview area double click <strong>Duration Type</strong>. </p> </li>
<li value="3">Select <strong>Calculated Assignment</strong> from the drop-down menu.</li>
<li value="4">Click <strong>Save</strong> <strong>Changes</strong>.</li>
</ol>
-->
