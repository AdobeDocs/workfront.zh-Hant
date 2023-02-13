---
content-type: overview
product-area: projects
keywords: 重複，重發，重發
navigation-topic: manage-tasks
title: 循環任務概述
description: 循環任務概述
author: Alina
feature: Work Management
exl-id: 9ddb75bf-1c7b-4f4b-b80b-a9512192920d
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '615'
ht-degree: 3%

---

# 循環任務概述

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: DO NOT DO NOT EDIT OR CHANGE!!! linked to the NWE UI, this is not linked to classic - direct links:</p>
<p>https://one.workfront.com/s/csh?context=2288&pubname=workfront-classic</p>
<p>https://one.workfront.com/s/csh?context=2288&pubname=the-new-workfront-experience >> this)</p>
</div>
-->

您可以為必須在單一專案中重複的活動建立週期性工作。

本文概述有關建立和編輯循環任務的資訊和考量事項。

如需如何在Adobe Workfront中建立循環工作的詳細資訊，請參閱 [建立循環任務](../../../manage-work/tasks/create-tasks/create-recurring-tasks.md).

## 循環任務概述和考量事項

您可以選擇建立循環任務，以指示項目生命週期中可重複的工作。

例如，在IT項目期間，可能需要定期備份軟體。 為此活動建立循環任務可縮短設定多個單獨任務所需的時間。

在Workfront中建立週期性任務時，請考量下列事項：

* 無法將循環任務添加到模板。
* 不能向現有任務添加重複頻率。
* 循環任務顯示為子任務或子項，主要事件以父任務的形式顯示。
* 不能將批准附加到父循環任務。
* Workfront會將您為父項週期更新的大部分欄位建立給子項任務時傳輸。 建立子任務時，以下欄位不會轉移到這些任務：

   * 子任務的「任務約束」(Task Constraint)自動更改為：

      * 從「開始日期」開始計畫的項目的「必須開始」。
      * 從完成日期開始計畫的項目必須完成。
   * 附加到父項的文檔不會轉移到子項。


* 在您指出該任務重複執行後，父任務上將發生以下更改：

   * 父任務的「持續時間」欄位將更名為「每次發生的持續時間」。 對於子任務，它仍為持續時間。
   * 在父任務上禁用狀態，並在子任務上自動將其設定為New。 完成所有子項後，父項任務會自動完成，狀態將更新為「完成」。
   * 唯一可用於循環任務的持續時間類型是：

      * 簡單
      * 投入比導向

## 編輯循環任務的考量事項

您對循環任務父級所做的某些更改可能不會更新所有現有的循環。 顯示進度或已單獨更新的子任務在更新父任務時不會更新。 Workfront認為任務顯示在下列情況下的進度：

* 狀態已更新，任務不再是新任務
* 任務完成百分比高於零
* 該任務具有前置關係

下表說明對父觸發器所做的更改是否更新了未單獨編輯或顯示進度的子觸發器：

| 父任務上更新的欄位 | 向未編輯的子項或子項進行更新，且未記錄任何進度 |
|---|---|
| 週期頻率* | ✔ |
| 指派&#42;&#42; | ✔ |
| 名稱 | ✔ |
| 說明 | ✔ |
| 優先順序 | ✔ |
| 期間 | ✔ |
| 計畫小時 | ✔ |
| 成本類型 | ✔ |
| 收入類型 | ✔ |
| 資源平準 | ✔ |
| 平準延遲 | ✔ |
| 任務約束 | 不更新子項 |
| 附加或移除自訂Forms | 不更新子項 |
| 持續時間類型 | 不更新子項 |
| 自訂表單資訊 | 不更新子項 |

{style=&quot;table-layout:auto&quot;}

&#42; 更新父任務的「重複頻率」時，存在以下情況：

* 如果更改現有父任務的「重複頻率」，則如果現有子任務未顯示任何進度，並且您未手動更新它們，則會刪除現有子任務並替換為遵循新重複頻率的新子任務。
* 如果更改現有父任務的「重複頻率」，則不會刪除顯示進度的子任務。 此時，這些工作會視為與週期分開。

&#42;&#42; 在父任務上分配的分配將應用於週期中的所有子任務。 對父任務上的分配所做的任何更改都將覆蓋子任務上的任何單個分配。 如果任務顯示進度，則分配不會更改。

 
