---
content-type: overview
product-area: projects
navigation-topic: task-duration
title: '''持續時間類型概觀：計算工作」'
description: 計算工作是持續時間類型，您可以在Adobe Workfront中為任務設定。 有關Workfront中「持續時間類型」的一般資訊，請參閱「任務持續時間和持續時間類型概述」。
author: Alina
feature: Work Management
exl-id: f521c2f5-8d58-44c0-af18-6940ad0950ea
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '541'
ht-degree: 1%

---

# 持續時間類型概觀：計算工作

計算工作是持續時間類型，您可以在Adobe Workfront中為任務設定。 如需Workfront中持續時間類型的一般資訊，請參閱 [任務持續時間和持續時間類型概覽](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

## 計算的工作期間類型概覽

計算工作確定完成任務所需的工作量（計畫小時數）。 當分配給任務的資源在整個任務期間被分配時，建議您使用計算的工作期間類型。

您的Workfront或群組管理員可將系統或群組的預設持續時間類型設定為計算工作。 在這種情況下，將使用此持續時間類型建立所有新任務。 有關在系統級或組級項目首選項中更改任務和發出首選項的資訊，請參閱 [配置全系統任務和問題首選項](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

在將資源添加到任務時，項目經理可以看到計畫工作量的增加。 為了說明問題，一個包含三個資源的1小時計畫會議代表總共需要3個小時的工作時間，一個包含10個資源的1小時計畫會議代表需要10小時的工作時間。 這假設每個資源都分配給具有100%分配的任務。

## 複查使用計算的工作期間類型時計算所需工作的公式

在任務上使用「計算的工作持續時間類型」時，Workfront會使用以下兩個公式計算每個任務的工作量。 公式會因每個資源分配給任務的時間百分比以及分配給每個任務的資源數量而異：

* 簡化公式：假設您已為任務分配了一個資源，並且這些資源在任務可用時間的100%內分配給任務，則每個任務的「需要工作」值將使用以下公式計算：

```
Work Required (Planned Hours) = (Duration of the task in hours) x (The number of resources assigned to the task)
```

* 複雜公式：如果您使用各種分配來分配每個資源，則公式會將這些分配納入並考慮這些變化：

```
Work Required (Planned Hours) = SUM[(Duration of the task in hours) x (Percent allocated towards tasks for each resource)]
```

## 查看添加或從任務中刪除資源的效果

向具有「計算的工作持續時間」類型的任務添加或刪除受分配者時，可以手動編輯「持續時間」。 當任務中添加或刪除受分配者時，「計畫小時數」將發生更改。

在以下示例中，「設定」的「項目首選項」中的「每個工作日的典型小時數」設定為8。 每個任務的持續時間為1天。 隨著受分配人數的更改，計畫小時數會根據給定任務的受分配人數而改變：

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>受分配人數（每100%分配）</strong> </p> </th> 
   <th> <p><strong>期間</strong> </p> </th> 
   <th> <p><strong>計畫小時</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>1</p> </td> 
   <td> <p>1天</p> </td> 
   <td> <p>8 小時</p> <p>（1天x每個工作日8小時x 1受託人= 8計畫小時）</p> </td> 
  </tr> 
  <tr> 
   <td> <p>2</p> </td> 
   <td> <p>1天</p> </td> 
   <td> <p>16小時</p> <p>（1天x每工作日8小時x 2受分配者= 16計畫小時）</p> </td> 
  </tr> 
  <tr> 
   <td> <p>3</p> </td> 
   <td> <p>1天</p> </td> 
   <td> <p>24 小時</p> <p>（1天x每個工作日8小時x 3個受分配者= 24個計畫小時）</p> </td> 
  </tr> 
 </tbody> 
</table>

在這種情況下，每個受託人將100%分配給「計算的工作」任務。

![](assets/calcwork-350x71.png)

## 將任務的持續時間類型更改為計算工作

有關更改任務的「持續時間類型」的資訊，請參閱 [更新任務的持續時間類型](../../../manage-work/tasks/taskdurtn/update-duration-type-of-task.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: replaced with new article linked above)</p>
-->

<!--
<ol data-mc-conditions="QuicksilverOrClassic.Draft mode">
<li value="1">Go to a task for which you want to change the Duration Type.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click <strong>Task Details</strong> in the left panel, then in the Overview area double click <strong>Duration Type</strong>. </p> </li>
<li value="3">Select <strong>Calculated Work</strong> from the drop-down menu.</li>
<li value="4">Click <strong>Save</strong> <strong>Changes</strong>.</li>
</ol>
-->
