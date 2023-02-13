---
content-type: overview
product-area: projects
navigation-topic: task-duration
title: '''持續時間類型概觀：努力驅動」'
description: 「工作驅動」是持續時間類型，您可在Adobe Workfront中為任務設定。 有關Workfront中「持續時間類型」的一般資訊，請參閱「任務持續時間和持續時間類型概述」。
author: Alina
feature: Work Management
exl-id: 3c8534f7-02d0-4404-a37b-0ef6360e8efc
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '821'
ht-degree: 1%

---

# 持續時間類型概觀：工作驅動

「工作驅動」是持續時間類型，您可在Adobe Workfront中為任務設定。 如需Workfront中持續時間類型的一般資訊，請參閱 [任務持續時間和持續時間類型概覽](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

## 工作驅動持續時間類型概觀

Workfront或群組管理員可將系統或群組的預設「持續時間類型」設為「工作驅動」。 在這種情況下，將使用此持續時間類型建立所有新任務。 有關在系統級或組級項目首選項中更改任務和發出首選項的資訊，請參閱 [配置全系統任務和問題首選項](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

在此情況下，存在任意縮短項目計畫的風險，除非您作為項目經理花時間考慮該任務是否實際為「工作驅動」任務。

使用「努力驅動」：

* 根據可用於處理任務的資源數確定計畫持續時間。 持續時間等於計畫小時數。 計畫持續時間等於計畫小時數除以受分配者數。

   應用於任務的工作量將決定分工和持續時間。

* 在分配多個資源時，跟蹤任務的總逗留時間。

   添加資源後，任務的「計畫持續時間」將減少。 （「多手輕工」的原則說明了此持續時間類型對任務的計畫持續時間的影響。）

以下各節提供了更詳細的資訊，說明Workfront如何計算「工作驅動」任務的「計畫持續時間」，以及添加資源對具有此「持續時間類型」的任務的影響。

## 工作驅動的持續時間類型公式概覽

計算「工作驅動的持續時間類型」任務的「計畫持續時間」的公式取決於分配給任務的每個資源的分配百分比。 在「工作驅動」任務中，Workfront會計算任務的「計畫小時數」，它們始終與任務的「持續時間」相同：

```
Planned Hours (in hours) = Duration (in days)
```

您可以手動調整任務的持續時間。

Workfront假設一天有8個工作小時。 您的Workfront或群組管理員會在「設定」的「專案偏好設定」中，使用「每日一般小時數」設定來定義每個工作日的小時數。 有關在系統級項目首選項中更改任務和問題首選項的詳細資訊，請參閱 [配置全系統任務和問題首選項](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

>[!TIP]
>
>Workfront會考慮指派給任務的每個資源的排程，以決定該任務的每個資源的分配百分比。 有關建立和為用戶分配調度的資訊，請參閱 [建立排程](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

請考量下列情況：

* [資源將100%分配給任務](#resources-are-allocated-100-to-the-task)
* [資源按任務的不同時間百分比分配](#resources-are-allocated-for-various-percentages-of-time-to-the-task)

### 資源將100%分配給任務 {#resources-are-allocated-100-to-the-task}

此公式假設所有資源均分配給任務。

```
Planned Duration = (Planned Hours / Number of Resources) / 8
```

此計算假設正常工作日的小時數為8。 方程式包含此值，以便以天為單位顯示「計畫持續時間」。

### 資源按任務的不同時間百分比分配 {#resources-are-allocated-for-various-percentages-of-time-to-the-task}

由於每個分配的資源都可以具有唯一的分配級別，因此實際公式將以下分配值納入考慮：

```
Planned Duration = (Planned Hours / SUM(Percent allocation for each resource for the task)) / 8
```

此計算假設正常工作日的小時數為8。 方程式包含此值，以便以天為單位顯示「計畫持續時間」。

## 向任務添加更多資源的效果

向具有「工作驅動的持續時間類型」、「持續時間」和「計畫小時數」的任務添加或刪除受分配者時，不會更改。 不過，「計畫持續時間」確實會變更。

在以下示例中，系統設定中的「項目首選項」中的「每工作日典型小時數」設定為8。 由於持續時間為3天，因此「計畫小時數」設定為24（3天x每工作日8小時= 24計畫小時數）。

>[!NOTE]
>
>使用「固定日期任務約束」時，添加或刪除分配時，「計畫持續時間」保持不變，而是調整「持續時間」和「計畫小時數」。 使用固定日期以外的任何任務約束時，將調整計畫持續時間。

下表說明了計畫持續時間隨著向任務添加資源而如何改變：

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> </th> 
   <th> <p><strong>受分配人數（每100%分配）</strong> </p> </th> 
   <th> <p><strong>期間</strong> </p> </th> 
   <th> <p><strong>計畫小時</strong> </p> </th> 
   <th><strong>計畫持續時間</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> </td> 
   <td> <p>1</p> </td> 
   <td> <p>3天</p> </td> 
   <td> <p>24 小時</p> <p>（3天x每工作日8小時= 24計畫小時）</p> </td> 
   <td> <p>3天</p> <p>（24計畫小時數/1受託人= 3天）</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> <p>2</p> </td> 
   <td> <p>3天</p> </td> 
   <td> <p>24 小時</p> <p>（3天x每工作日8小時= 24計畫小時）</p> </td> 
   <td> <p>1.5天</p> <p>（24計畫小時數/2個受分配者= 12小時，或1.5天）</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> <p>3</p> </td> 
   <td> <p>3天</p> </td> 
   <td> <p>24 小時</p> <p>（3天x每工作日8小時= 24計畫小時）</p> </td> 
   <td> <p>1天</p> <p>（24個計畫小時/ 3個受分配者= 8小時或1天）</p> </td> 
  </tr> 
 </tbody> 
</table>

## 將任務的「持續時間類型」更改為「工作驅動」

有關更改任務的「持續時間類型」的資訊，請參閱 [更新任務的持續時間類型](../../../manage-work/tasks/taskdurtn/update-duration-type-of-task.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: replaced with new article linked above)</p>
-->

<!--
<ol data-mc-conditions="QuicksilverOrClassic.Draft mode">
<li value="1">Go to a task for which you want to change the Duration Type.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click <strong>Task Details</strong> in the left panel, then in the Overview area click <strong>Duration Type</strong>. </p> </li>
<li value="3"> <p>Select <strong>Effort Driven</strong> from the drop-down menu.</p> </li>
<li value="4">Click <strong>Save</strong><strong>Changes</strong>.</li>
</ol>
-->
