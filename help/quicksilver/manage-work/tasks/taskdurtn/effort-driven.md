---
content-type: overview
product-area: projects
navigation-topic: task-duration
title: 期間型別概觀：投入比導向
description: 投入比導向是持續時間型別，您可以在Adobe Workfront中為任務設定。 如需Workfront中期間型別的一般資訊，請參閱任務期間與期間型別概觀。
author: Alina
feature: Work Management
exl-id: 3c8534f7-02d0-4404-a37b-0ef6360e8efc
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '862'
ht-degree: 1%

---

# 期間型別概觀：投入比導向

投入比導向是持續時間型別，您可以在Adobe Workfront中為任務設定。 如需Workfront中期間型別的一般資訊，請參閱[任務期間與期間型別概觀](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md)。

## 投入比導向期間型別概觀

您的Workfront或群組管理員可以將系統或群組的預設「期間型別」設定為「投入比導向」。 在此情況下，所有新任務都將以此期間型別建立。 如需有關將您的任務和問題偏好設定變更為系統層級或群組層級專案偏好設定一部分的資訊，請參閱[設定全系統的任務和問題偏好設定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md)。

在此案例中，除非您作為專案經理花時間考慮該任務是否實際為投入比導向任務，否則可能會任意縮短專案計畫。

使用投入比導向：

* 根據任務可用的資源數決定計畫期間。 期間等於計畫時數。 計畫期間等於計畫時數除以受指派人數。

  套用至任務的工作量層級會決定分工與「工期」。

* 在指派多個資源時，追蹤在任務上所花費的總時數。

  當新增資源時，任務的計畫期間會減少。 （「多手能輕而易舉」的原則說明了此「工期型別」對任務計畫工期的影響。）

以下各節提供有關Workfront如何計算付出導向任務的計畫期間以及新增資源對具有此期間型別的任務的影響的更多詳細資訊。

## 投入比導向期間型別公式的概要

「工期型態」為「投入比導向」之任務的「計畫工期」計算公式取決於指派給該任務的每個資源的配置百分比。 在投入比導向任務的情況下，Workfront會計算任務的計畫時數，並且一律與任務的期間相同：

```
Planned Hours (in hours) = Duration (in days)
```

您可以手動調整任務的工期。

Workfront假設每天有8個工作小時。 您的Workfront或群組管理員使用「設定」中「專案偏好設定」內的「每工作日一般小時數」設定，來定義每工作日小時數。 如需有關將您的任務和問題偏好設定變更為系統層級專案偏好設定一部分的詳細資訊，請參閱[設定系統範圍的任務和問題偏好設定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md)。

>[!TIP]
>
>Workfront會考量指派給任務的每個資源的排程，以決定任務每個資源的配置百分比。 如需有關建立排程並指派給使用者的資訊，請參閱[建立排程](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)。

請考量下列情況：

* [資源100%配置給工作](#resources-are-allocated-100-to-the-task)
* [資源會以各種時間百分比分配給任務](#resources-are-allocated-for-various-percentages-of-time-to-the-task)

### 資源100%配置給任務 {#resources-are-allocated-100-to-the-task}

此公式假設所有資源皆為100%配置給作業。

```
Planned Duration = (Planned Hours / Number of Resources) / 8
```

此計算假設正常工作日的時數為8。 方程式包含此值，因此計畫期間會以天為單位顯示。

### 資源會以各種時間百分比分配給任務 {#resources-are-allocated-for-various-percentages-of-time-to-the-task}

因為每個指定的資源都可以有唯一的配置層次，所以實際公式會將這些配置值列入考量：

```
Planned Duration = (Planned Hours / SUM(Percent allocation for each resource for the task)) / 8
```

此計算假設正常工作日的時數為8。 方程式包含此值，因此計畫期間會以天為單位顯示。

## 將更多資源新增至任務的影響

將受指派者新增或移除至具有投入比導向期間型別、期間和計畫時數的任務時，未變更。 但計畫期間不會變更。

在下列範例中，系統設定中的專案偏好設定中，每工作日一般時數設定為8。 由於持續時間為3天，因此計畫時數設定為24 （3天x 8小時每工作日= 24計畫時數）。

>[!NOTE]
>
>使用固定日期任務限制時，當您新增或移除受指派人時，計畫期間保持相同，而是調整期間和計畫時數。 使用固定日期以外的任何任務限制時，會調整計畫持續時間。

下表說明計畫期間如何隨著將資源新增至任務而改變：

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> </th> 
   <th> <p><strong>受指派人數（每100%配置）</strong> </p> </th> 
   <th> <p><strong>期間</strong> </p> </th> 
   <th> <p><strong>規劃時數</strong> </p> </th> 
   <th><strong>規劃期間</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> </td> 
   <td> <p>1</p> </td> 
   <td> <p>3天</p> </td> 
   <td> <p>24 小時</p> <p>（3天x每個工作日8小時= 24計畫小時）</p> </td> 
   <td> <p>3天</p> <p>（24計畫時數/ 1受指派人= 3天）</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> <p>2</p> </td> 
   <td> <p>3天</p> </td> 
   <td> <p>24 小時</p> <p>（3天x每個工作日8小時= 24計畫小時）</p> </td> 
   <td> <p>1.5天</p> <p>（24個計畫時數/ 2個受指派人= 12小時或1.5天）</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> <p>3</p> </td> 
   <td> <p>3天</p> </td> 
   <td> <p>24 小時</p> <p>（3天x每個工作日8小時= 24計畫小時）</p> </td> 
   <td> <p>1天</p> <p>（24個計畫時數/ 3個受指派人= 8小時或1天）</p> </td> 
  </tr> 
 </tbody> 
</table>

## 將任務的期間型別變更為投入比導向

如需有關變更任務期間型別的資訊，請參閱[更新任務的期間型別](../../../manage-work/tasks/taskdurtn/update-duration-type-of-task.md)。

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
