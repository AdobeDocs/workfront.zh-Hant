---
content-type: overview
product-area: projects
navigation-topic: task-duration
title: '''持續時間類型概觀：計算分配'
description: 「計算分配」是可為Adobe Workfront中的任務設定的「持續時間類型」。 有關Workfront中「持續時間類型」的一般資訊，請參閱「任務持續時間和持續時間類型概述」。
author: Alina
feature: Work Management
exl-id: 5f1f6109-5d54-4c3f-9aa5-dc6ce165a1cd
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '478'
ht-degree: 0%

---

# 持續時間類型概觀：計算分配

「計算分配」是可為Adobe Workfront中的任務設定的「持續時間類型」。 如需Workfront中持續時間類型的一般資訊，請參閱 [任務持續時間和持續時間類型概覽](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

## 計算分配持續時間類型概覽

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: This Hub issue has a powerpoint that highlights information that is useful to users when using Calculated Assignment duration type. I don't think we can use the powerpoint, because it's old. I also don't know if the things they discuss are still relevant, since the PP is from 2015. I've closed the issue, but I'm putting a link here just in case the info is useful. https://hub.workfront.com/issue/5a9dd7d5007d02a8966014557c23cc89/updates)</p>
-->

* 使用「計算分配持續時間類型」時，必須同時指定任務的持續時間和計畫小時數。 然後，Workfront將「計畫小時數」除以「持續時間」中的小時數，再除以分配給任務的資源數，以計算每個資源的分配百分比（計算分配）。 每個資源的分配百分比將具有相同的值。 在此情況下，您無法修改每個資源的分配值。
* 您的Workfront或群組管理員可將系統或群組的預設持續時間類型設定為計算指派。 在這種情況下，將使用此持續時間類型建立所有新任務。 有關在系統級或組級項目首選項中更改任務和發出首選項的資訊，請參閱 [配置全系統任務和問題首選項](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

   在這種情況下，任務的預設持續時間為一天，預設時間為0小時計畫小時。 除非項目經理設定更精確的持續時間並以實際的估計值填入「計畫時數」欄位，否則資源似乎分配不足。

在以下情況下，「計算分配」是首選的「持續時間類型」：

* 當分配具有活動窗口，但未佔用分配的完成其工作的整個持續時間時。 例如，您被指派在當周結束時將報表傳送給您的主管。 您有5天的時間，但只需10小時就能起草文檔。
* 將單個資源分配給任務時，因為項目經理可以獨立估計計畫的持續時間和計畫工作量。

   您可以對相同結果使用計算的工作期間類型，但項目經理必須為資源輸入百分比分配，以便影響計畫小時數的計算值。 這使得項目規劃更加困難和費時。

每個資源的分配百分比計算如下：

```
Planned Hours / Duration / Number of Resources = Allocation Percentage for each resource
```

例如，在下面概述的方案中，每個任務的持續時間為3天。 項目經理人工輸入「持續時間」（3天或24小時）和「計畫小時數」，因此，系統會計算分配百分比（或分配百分比）:

![](assets/calcassign-350x80.png)

## 將任務的持續時間類型更改為計算分配

有關更改任務的「持續時間類型」的資訊，請參閱 [更新任務的持續時間類型](../../../manage-work/tasks/taskdurtn/update-duration-type-of-task.md).

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
