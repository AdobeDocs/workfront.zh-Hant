---
content-type: overview
product-area: projects
navigation-topic: task-information
title: 計畫時數概觀
description: 與任務、問題或專案相關的計畫時數代表指派的使用者完成任務、問題或專案所需的時間量。
author: Alina
feature: Work Management
exl-id: 0b86c760-691a-436e-9beb-31e9ac36440a
source-git-commit: 48efc796923079622ce4bc1c2bddb2429915c9a1
workflow-type: tm+mt
source-wordcount: '2815'
ht-degree: 0%

---

# 計畫時數概觀

<!-- Audited: 01/2024 -->

與任務、問題或專案相關的計畫時數代表指派的使用者完成任務、問題或專案所需的時間量。

## 關於Adobe Workfront中計畫時數的考量事項

* 計畫時數主要與Adobe Workfront中的工作專案（任務和問題）相關聯。 工作專案的計畫時數會統計至其專案的計畫時數。
* 依預設，Workfront會將任務和問題計畫時數平均分發給任務或問題期間的所有天。
* 將使用者和角色指派給任務和問題時，任務和問題的規劃時數會與使用者或角色指派建立關聯。
* 如果您想在Workfront中使用資源管理工具，必須定義任務和問題的計畫時數值。
* 您只能為某些期間型別修改任務的計畫時數值。

  如需更多有關修改任務中與任務期間型別相關的計畫時數的資訊，請參閱區段 [根據期間型別更新任務計畫時數](#update-task-planned-hours-based-on-duration-type) 本文章內容。

* 您可以隨時修改問題的計畫時數值。
* 您無法修改專案或父系任務的計畫時數值，因為它們是所有任務和子任務的所有計畫時數的計算總數。
* 使用資源管理工具管理使用者配置可能會變更任務、問題和專案的規劃時數，以及與工作專案關聯的指派的時數。

## 任務計畫時數與專案計畫時數的比較 {#planned-hours-on-tasks-vs-planned-hours-on-projects}

從任務累計至專案計畫時數的計畫時數。 問題中的計畫時數並不總是向上彙整到專案的計畫時數。

本節說明任務和專案計畫時數之間的差異。 它還說明您可以在何處檢視累計至專案的問題計畫時數。

### 任務的計畫時數 {#planned-hours-on-tasks}

任務的計畫時數表示任務實際工時估計可能花費的時間量。 依預設，Workfront會平均分配每個任務期間內每天的計畫時數總計。 計畫時數的每日金額會成為任務的每日分配。 如果將任務指派給多個資源，則預設會為每個資源分配相等的每日時數。

使用工作負載平衡器，您可以修改指派給任務之使用者的每日配置。 當任務期間型別為簡單時，這也可以更新任務的計畫時數。 如需詳細資訊，請參閱文章中的「管理使用者指派時更新任務計畫時數」一節 [在工作負載平衡器中管理使用者配置](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

當任務包含子任務時，父任務的計畫時數是任何子任務上所有計畫時數的總和。 您無法更新父系任務的計畫時數。

>[!NOTE]
>
>與計畫時數不同，父系任務的實際時數是直接在父系任務上記錄的時數。 它們不代表子系任務的實際時數總和。\
>如需實際時數的詳細資訊，請參閱 [檢視實際小時](../../../manage-work/tasks/task-information/actual-hours.md).

### 專案計畫時數 {#planned-hours-on-projects}

您無法編輯專案上的計畫時數金額。 專案計畫時數是專案所有任務之所有計畫時數的計算總和。

計畫時數的計算中是否包含問題，取決於您在專案中檢視計畫時數的位置。 您可以在專案的下列位置中檢視專案計畫時數：

* **「專案詳細資訊」區段和「編輯專案」方塊**：僅考慮專案上任務的計畫時數。 在專案詳細資訊區段或編輯專案方塊中檢視專案計畫時數總計時，未考慮專案上問題的計畫時數。

* **工作負載平衡器**：只有與工作負載平衡器中可見的任務相關的計畫時數會顯示在專案的工作負載平衡器中。 使用者每日分配可以在工作負載平衡器中變更專案每日計畫時數。
* **使用率區段**：在「使用率」區段中檢視專案計畫時數總數時，會考慮與指派給任務之使用者相關聯的計畫時數以及專案上的問題。
* **角色配置面板** 在任務清單中：此區域顯示指派給工作角色或與工作角色相關聯之使用者的任務與專案問題的計畫時數。 與未指派或指派給團隊的任務和問題相關的計畫時數未顯示在此區域中。 如需詳細資訊，請參閱 [在角色分配面板中檢視專案計畫時數](../../../manage-work/projects/planning-a-project/view-planed-hours-in-role-allocation-panel.md).

## 在任務期間中的計畫時數分佈

依預設，Workfront會平均分配計畫時數至任務的期間，並根據專案排程的可用性為任務的每一天分配相等的計畫時數。

例如，如果任務設定為下午4點開始，而排程在任務的第一天還剩一小時，Workfront會在任務的第一天放置一個計畫小時，然後將計畫小時的剩餘時間平均分配到任務期間中的其餘天。

>[!NOTE]
>
>每日計畫時數或每日配置是在任務期間每天的計畫時數配置。 如果任務有一個指派，則此數字代表每個指派的每日計畫時數。 如果任務有多個指派，則每個指派的每日計畫時數與任務的每日計畫時數不同。 對於具有多個指派的任務，Workfront中沒有每日計畫時數每個指派的視覺化表示法。

## 找到並瞭解計畫時數值

您可以在Workfront的各個區域找到計畫時數值。

顯示的計畫時數源自專案上的工作專案，或根據您檢視它們的區域和物件而計算的方式不同。

您可以在Workfront的下列區域中找到計畫時數：

* [專案、任務或問題的詳細資訊區段](#the-details-section-of-a-project-task-or-issue)
* [編輯任務或編輯問題方塊](#the-edit-task-or-edit-issue-box)
* [報告](#reports)
* [工作負載平衡器](#the-workload-balancer)
* [資源規劃工具](#the-resource-planner)
* [使用率報表](#the-utilization-report)
* [角色配置面板](#the-role-allocation-panel)

### 專案、任務或問題的詳細資訊區段 {#the-details-section-of-a-project-task-or-issue}

![詳細資訊區段的計畫時數](assets/planned-hours-on-details-for-project.png)

任務、問題或專案詳細資訊區段中的計畫時數是與專案相關的計畫時數總計。

如需有關專案計畫時數的詳細資訊，請參閱 [任務計畫時數與專案計畫時數的比較](#planned-hours-on-tasks-vs-planned-hours-on-projects) 一節。

### 編輯任務或編輯問題方塊 {#the-edit-task-or-edit-issue-box}

![編輯任務方塊](assets/planned-hours-on-edit-task-box-nwe.png)

任務或問題的編輯方塊中的計畫時數是相應專案的總計畫時數。

如需有關專案計畫時數的詳細資訊，請參閱 [任務計畫時數與專案計畫時數的比較](#planned-hours-on-tasks-vs-planned-hours-on-projects) 一節。

對於任務，您只能編輯特定期間型別的計畫時數。 如需詳細資訊，請參閱 [根據期間型別更新任務計畫時數](#update-task-planned-hours-based-on-duration-type) 一節。

您可以在「工作總攬」區域中檢視指派給任務或問題的每個使用者或工作角色的計畫時數個別分配。

### 報告 {#reports}

![報告上的計畫時數](assets/planned-hours-on-task-report.png)

您可以在專案、任務和問題報告中新增「計畫時數」欄位。

計畫時數欄預設包含在任務清單的標準檢視中。

任務、問題或專案報告中的計畫時數是指個別專案顯示在「詳細資訊」區段或編輯方塊中的總計畫時數。

如需建立報表的相關資訊，請參閱 [建立自訂報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

>[!NOTE]
>
>如果您建立專案（財務資料）報告並按日期將其分組，則計畫時數可能會根據專案上任務的時間表顯示專案的部分計畫時數。 依預設，Workfront會平均分配任務期間每天的計畫時數。 特定時間範圍的計畫時數符合Workfront在專案（財務資料）報表中為該時間範圍設定的相等分佈。

<!--
### The Scheduling areas  {#the-scheduling-areas}

![](assets/task-detail-expanded-in-scheduler-with-planned-hours-and-adjusted-daily-allocations-nwe-350x323.png)

The Planned Hours for tasks and issues display in the Scheduling areas in the Planned Hours field.

You can view the daily allocation of Planned Hours for each user assigned to a task or an issue in the Scheduling areas.

The daily hour amount represents one of the following:

* the default amount equally distributed by Workfront for each day of the Duration of the tasks or issues
* the adjusted daily allocation managed by resource managers.

  For information about adjusting daily allocations in the Scheduling tools, see [Manage user allocations in the Scheduling areas](../../../resource-mgmt/resource-scheduling/manage-allocations-scheduling-areas.md).
-->

### 工作負載平衡器 {#the-workload-balancer}

![工作負載平衡器中的計畫時數](assets/planned-hours-on-wb-expanded-with-pti-info.png)

任務、問題和專案的以下計畫時數顯示在任務、問題或專案名稱右側的工作負載平衡器：

* 對於任務和問題，顯示與其關聯的計畫時數。
* 對於專案，畫面上顯示的任務和問題的總計畫時數。

  >[!TIP]
  >
  >工作負載平衡器沒有顯示所有計畫時數的專案詳細資訊區域。

您可以在工作負載平衡器中檢視指派給任務或問題的每個使用者的每日規劃時數分配。

計畫時數的每日小時量代表下列其中一項： 

* Workfront在任務、問題或專案期間每天均分的預設金額
* 資源管理員管理的調整每日配置

  如需有關在工作負載平衡器調整每日分配資訊，請參閱 [在工作負載平衡器中管理使用者配置](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

### 資源規劃工具 {#the-resource-planner}

![資源規劃工具中的計畫時數](assets/planned-hours-on-all-objects-in-resource-planned-expanded.png)

資源規劃工具會顯示專案、任務和問題的計畫時數。

您可以在資源規劃工具的PLN欄中，檢視與工作專案相關聯之使用者與職務角色的每週計畫時數配置。

>[!TIP]
>
>工作負載平衡器中的每日配置調整會影響資源規劃工具中任務和問題的每週配置。

每個物件的計畫時數會依您套用至資源規劃工具的檢視而有所不同。 如需詳細資訊，請參閱 [資源規劃工具之專案與角色檢視中的時數、約當全職人數及成本資訊概要](../../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md).

任務和問題的每週計畫時數表示以下其中一項：

* Workfront平均分配任務或問題期間每天的預設每週金額
* 由資源管理員在工作負載平衡器管理的調整每週配置

  如需有關在工作負載平衡器調整每日分配資訊，請參閱 [在工作負載平衡器中管理使用者配置](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

專案、使用者和角色的每週金額會受與其相關之任務和問題的每週計畫時數金額影響。

### 使用率報表 {#the-utilization-report}

專案計畫時數是指與每個任務和問題上的工作分派相關聯的時數。

>[!IMPORTANT]
>
>請注意，「使用率」報表中的「計畫時數」與指派相關聯，而非與任務和問題本身相關聯。 使用率報告中的計畫時數並不總是與專案任務和問題的計畫時數相符。 但是，計畫時數不符合與任務和問題上的指派相關聯的時數。

您可以在「使用率」報表中檢視下列計畫時數型態：

* 專案上所有工作分派在包含專案之整體生命週期中的總計畫時數
* 指定日期範圍內所有指派的計畫時數總計（您可以指定個別周或月）。

  當使用工作負載平衡器調整使用者每日分配時數時，如果在使用率報告中選取的日期僅包含任務或問題的持續時間的一部分，則特定日期範圍的計畫時數可能會受到影響。 如需有關調整使用者每日配置的資訊，請參閱 [在工作負載平衡器中管理使用者配置](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

如需詳細資訊，請參閱 [檢視資源使用率資訊](../../../resource-mgmt/resource-utilization/view-utilization-information.md).

### 角色配置面板

「角色配置」面板中的規劃時數代表在專案總期間中，與指派給專案上任務或問題的每個工作角色相關的規劃時數。 數字與資源規劃工具中的角色「計畫時數」相符。

>[!TIP]
>
請注意，與使用者關聯的計畫時數不會顯示在角色配置面板中。

如需詳細資訊，請參閱 [在工作負載平衡器顯示專案和方案的角色分配](../../../scenario-planner/show-role-allocation-workload-balancer.md).

## 根據期間型別更新任務計畫時數 {#update-task-planned-hours-based-on-duration-type}

只有在任務具有特定期間型別時，您才能在編輯任務時更新任務的總計畫時數。

存在下列情況：

* 您只能在編輯任務時使用計算的指派或簡單期間型別來修改任務的計畫時數。

  如需有關「已計算的指定工期型別」的詳細資訊，請參閱 [期間型別概要：計算的指定](../../../manage-work/tasks/taskdurtn/calculated-assignment.md).

  如需有關簡單期間型別的詳細資訊，請參閱 [期間型別概觀：簡單](../../../manage-work/tasks/taskdurtn/simple-duration-type.md).

* 當您管理使用者對任務的分配時，只能針對簡單期間型別任務在工作負載平衡器中更新任務計畫時數。 如需有關在工作負載平衡器中管理使用者配置的資訊，請參閱 [在工作負載平衡器中管理使用者配置](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).
* 您無法修改工期型別為投入比導向或已計算的工作之任務的計畫時數。 在這些情況下，Workfront會根據任務的期間來決定計畫時數；但在這種情況下，計畫時數一律等於期間（以小時為單位），不受指派資源之百分比配置的影響。

  如需投入比導向期間型別的詳細資訊，請參閱 [期間型別概觀：投入比導向](../../../manage-work/tasks/taskdurtn/effort-driven.md).

  如需有關已計算的工作期間型別的詳細資訊，請參閱 [期間型別概觀：計算的工作量](../../../manage-work/tasks/taskdurtn/calculated-work.md).

## 管理使用者分派時更新任務計畫時數

當您手動更新任務的使用者或工作角色分配時，可以更新任務的計畫時數。 僅當任務的期間型別為簡單時，才可能進行此作業。

如需詳細資訊，請參閱 [期間型別概觀：簡單](../../../manage-work/tasks/taskdurtn/simple-duration-type.md).

您可以更新指派給任務的使用者和角色的整體配置，或在使用工作負載平衡器時更新使用者每日配置。

如需有關管理工作的整體使用者與工作角色配置的資訊，請參閱 [管理任務的使用者和角色分配時數](../../../manage-work/tasks/assign-tasks/manage-allocation-hours-on-tasks.md).

如需有關管理任務的每日分配的資訊，請參閱 [在工作負載平衡器中管理使用者配置](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

手動更新工作的使用者或工作角色配置時，會發生下列情況：

* 如果您未手動更新個別使用者或角色指派以觸發對任務計畫時數的變更，則當您在任務上新增、移除或取代指派時，計畫時數保持不變。 將新工作分派新增至任務時，個別配置會重新分配至所有工作分派者。
* 當您手動更新分配以觸發任務變更計畫時數時，計畫時數會在您從任務移除指派時減少。 當您取代指定任務時，它們會維持不變。
* 當您手動更新指派以觸發對任務計畫時數的變更並將指派新增至任務時，新指派預設為0時指派。 您必須手動更新其對任務的指派，這可能會影響計畫時數。
* 如果您未手動更新指派以觸發對任務計畫時數的變更，並且您移除任務的所有指派，則計畫時數將保持不變。
* 當您手動更新分配以觸發任務變更計畫時數並移除任務的所有指派時，計畫時數也會移除，且任務的計畫時數會變成0。

>[!NOTE]
>
例如，如果一項任務有10個計畫時數，而您有兩個受指派人，則預設會各分配5個小時。
>
* 如果您沒有使用工作負載平衡器更新個別使用者配置或每日配置，並且您從任務中移除任何或所有受指派人，任務計畫時數將保留10小時。
* 如果您分別手動將工作分派的指派變更為4和6小時，並且移除指派給6小時的使用者及其工作角色，則任務「計畫小時」將更新為4小時。 如果您也移除分配至4小時的使用者，但保留與已移除使用者相關聯的工作角色，則任務的規劃時數仍為4小時。 如果您移除最後一個分配至4小時的使用者及其工作角色，並且該任務仍然未指派，則任務計畫時數將變為0。

## 使用工作量自動更新任務計畫時數

當您使用工作量來估計完成任務所需的工作量時，任務的計畫時數會自動更新。 這僅適用於具有簡單期間型別的任務。

如需有關使用工作量來預估任務工作量的資訊，請參閱 [工作投入概觀](../../../manage-work/tasks/task-information/work-effort.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this issue has the explanation of how Planned Hours should work - from Vazgen and Anna: https://hub.workfront.com/issue/6217dced00730b7034c4b808339a35ce/</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Details of their comments: </p>
-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>Anna Asatryan</p>
<p>3/22/2022 At 3:16 PM</p>
<p>&nbsp;</p>
<p>to Mark Paul, Corrie Butler, Arman Simonyan, Gagik Khalatyan, Alina Wilson, Artur Sargsyan, Vazgen Babayan, Anna Asatryan</p>
<p>I have done some rough calculations on what the planned hours/revenues should look like Book.xlsx . And if we look, for example at the 2 users highlighted in one of the screenshots their planned hours look way off from what the calculation looks like in the spreadsheet (i.e. equally distributed allocation). When looking at the Workload balancer (the second screenshot), as an example for the user Yashas Mitta, I can see that the allocation has been modified. Obviously the utilization report calculates the allocations based on the modified contouring using the new work per day calculation. The project financial report uses the old, equal distribution of allocation along the full duration of the task. Hence. there is a difference when grouping per periods.</p>
<p>Vazgen Babayan</p>
<p>I believe we will need to prioritise syncing the project financial data report with the new work per day.</p>
<p>Alina Wilson</p>
<p>@Anna Asatryan , do you have a definition of what we should say in documentation (glossary, for example) for how the Planned Hours (or Planned Revenue) is calculated, keeping in mind that we don't document the concept of "workPerDay". We call them "daily allocations", for example, but let me know if that's accurate, too.</p>
<p>Vazgen Babayan</p>
<p>Last Thursday at 3:13 PM</p>
<p>I think an important note here is that regardless the calculation, even if the both views used the same formula, they will not display the same data, because the underlying data sources are different. The Financial Data report does not respect user-entered allocations in Workload Balancer at this moment. So there will be a clear discrepancy, as Anna showed in her message. My recommendation for communication will be to explain that the data sources are different so there can be a mismatch in data and that we will look into addressing that on our roadmap.</p>
<p>Alina Wilson</p>
<p>So far, I hear you guys say this (with my questions for confirmation/ comments in bold):</p>
<p>- the utilization report calculates the allocations based on the modified contouring using the new work per day calculation (so this is what we see in the Workload Balancer, right?)</p>
<p>- the project financial report uses the old, equal distribution of allocation along the full duration of the task (this is before the daily allocations for example were modified in the WB, right?)</p>
<p>I have these additional questions:</p>
<p>- what does the Project Details show? Which Planned Hours, for instance - because earlier, we had a question about this also. - which numbers?</p>
<p>- what does any Planned Hours/ Planned Revenue field that can be pulled in any other report (outside of Financial Data and Utilization reports) show? - which numbers?</p>
<p>- are there any other areas I am not thinking of that we need to document, @Corrie Butler</p>
<p>I will try to document all the possible areas where these display but please help. Thanks!</p>
<p>Vazgen Babayan</p>
<p>Last Saturday at 3:41 PM</p>
<ul>
<li> <p>Confirming the first two points </p> </li>
</ul>
<p>For the following questions</p>
<ul>
<li> <p>Project details show an aggregated sum of task planned hours. It doesn't have anything to do with the work per day because it always deals with total numbers for the whole duration of the Project/Task.</p> </li>
<li> <p>Same thing applies to the Planned Hours and Planned Revenue fields in reports - they show totals for the whole Project/Task duration and thus have no use of work per day.</p> </li>
<li> <p>Can't think of any other fields related to this right now.</p> </li>
<li> <p>In general, if I were to summarize the system behavior, it's as follows:</p> </li>
<li> <p>Every area that only deals with total numbers of Planned Hours / Planned Revenue, uses the numbers entered on the tasks. Those are Task / Project Details, reports exposing those fields.</p> </li>
<li> <p>Areas that deal with time-sensitive portions of Planned Hours / Planned Revenue, use work per day. Those are all Resource Management tools - Workload Balancer, Resource Planner, Utilization Report, importing projects via Scenario Planner.</p> </li>
<li> <p>All the areas in the second point support user-edited allocations made in Workload Balancer.</p> </li>
<li> <p>Scheduling area and Project Financial Data reports use the old version of the work per day, which doesn't respect user-edited allocations from Workload Balancer.</p> </li>
<li> <p>Scheduling will be removed this year, and we need to do work to move the Project Financial Data reports to the new work per day sometime after Q3.</p> </li>
</ul>
<p>Alina Wilson</p>
<p>@Vazgen Babayan , one clarifying question: when you say "Scheduling and Project Financial Data reports use the old version of the work per day, which doesn't respect user-edited allocations from WB" - you mean that those use the system default which spreads the allocations evenly, correct? Because you can edit (daily) allocations in Scheduling tools, but it doesn't use that, correct? It uses the default of the daily allocation that the system figures out when dividing the Planned Hours by the number of days in the Duration. Please let me know. And thanks!</p>
<p>Anna Asatryan</p>
<p>Yesterday at 11:42 AM</p>
<p>@Alina Wilson , that's correct, when saying "Scheduling and Project Financial Data reports use the old version of the work per day, which doesn't respect user-edited allocations from WB" Vazgen meant that it spreads the allocation evenly.</p>
<p>As for the scheduling, the allocation modification that's being done there isn't reflected anywhere else in the application other than in the Scheduling itself. That's probably one of the reasons it's being deprecated.</p>
</div>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <br> </p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: everything below is drafted because I replaced it with the table above)</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can find the Planned Hours information on tasks, issues, or projects in the following locations:</p>
-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>The Planned Hours in the Details  section  of a task, issue, or project are the total Planned Hours of the respective item. </p>
<p>Finding the Planned Hours in the Details  section  is identical for tasks, issues, and projects. </p> <note type="tip">
You cannot edit the Planned Hours of projects manually, as they are a calculation of all Planned Hours of all the tasks on the project.
</note>
<p>To locate the Planned Hours value on the Details  section  of a task: </p>
<ol>
<li value="1">Go to a task for which you want to review the Planned Hours.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click <strong>Task Details</strong> in the left panel. </p> </li>
<li value="3"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>Overview</strong> area and notice the Planned Hours value.</p> <p>This value represents the time it would take the user assigned to the task to complete it. </p> </li>
</ol>
</div>
-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h3> </h3>
<p>The Planned Hours in the Edit box of a task, issue, or project are the total Planned Hours of the respective item. </p>
<p>Finding the Planned Hours while editing a task or an issue is identical. </p> <note type="tip">
You cannot edit the Planned Hours of projects manually, as they are a calculation of all Planned Hours of all the tasks on the project.
</note>
<p>To locate the value of Planned Hours while editing a task:</p>
<ol>
<li value="1">Go to the task or issue you want to view Planned Hours for.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click <strong>Edit</strong>.</p> <p>The Planned Hours are located in the <strong>Overview</strong> section. </p> </li>
</ol>
</div>
-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>The Planned Hours column is included in the Standard view of a task list, by default. For issues and projects, you can add it to the view, when you are editing the view or when you build a report. </p>
<p>The Planned Hours in a task, issue, or project report are the total Planned Hours of the respective item as they display in the Details  section  or the Edit box of the items. </p>
<p>Adding the Planned Hours column to a project view is similar to building a view in a project report. </p>
<p>To show Planned Hours in a project report:</p>
<ol>
<li value="1"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>Main Menu</strong> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of Workfront, then click <strong>Reports</strong>. </p> </li>
<li value="2">Click <strong>New Report</strong>, then choose <strong>Project</strong> as your object.</li>
<li value="3">Click <strong>Add Column</strong>, and start typing <strong>Planned Hours</strong> when the <strong>Show in this column</strong> drop-down field is displayed. Select the field when it appears in the list.</li>
<li value="4"> <p>Click <strong>Save + Close</strong> to save the report. </p> <p>The Planned Hours column shows the total number of Planned Hours on each project. </p> </li>
</ol>
</div>
-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>Planned Hours in Resource Management tools</p> <note type="important">
When viewing Planned Hours in the Resource Management tools by a specific time frame, the daily allocations for each work item and the daily allocations for the resources assigned to the work items during that time frame can influence the daily Planned Hours of projects or work items.
</note>
<p>You can see the value of Planned Hours for your tasks, issues, or projects when using the following Resource Management tools:</p>
<ul>
<li> <p>Resource Planner</p> <p>For information about using the Resource Planner, see <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md" class="MCXref xref">Resource Planner overview</a>.</p> </li>
<li> <p>Utilization Report.</p> <p>For information about the utilization report, see <a href="../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md" class="MCXref xref">Overview of the Resource Utilization report</a>.</p> </li>
<li>
<div data-mc-conditions="QuicksilverOrClassic.Quicksilver">
<p>Workload Balancer or Scheduling areas in the following sections:</p>
<ul>
<li>Scheduling or Workload Balancer sections in the Resourcing area</li>
<li>Scheduling or Workload Balancer section at the project level</li>
<li>Schedule or Workload Balancer section at the team level</li>
</ul>
</div> <p>For information about scheduling resources, see <a href="../../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md" class="MCXref xref">Get started with Resource Scheduling</a>.</p> <p>For information about the Workload Balancer, see <a href="../../../resource-mgmt/workload-balancer/overview-workload-balancer.md" class="MCXref xref">Workload Balancer overview</a>. </p> </li>
<li> <p><b>Role Allocation panel</b> in the project  task list or  Workload Balancer: The Planned Hours for the tasks and the issues on the project that are assigned to a job role or a user associated with a job role are taken into account in this area. For more information, see <a href="../../../manage-work/projects/planning-a-project/view-planed-hours-in-role-allocation-panel.md" class="MCXref xref">View project Planned Hours in the Role Allocation panel</a>. </p> </li>
</ul>
</div>
-->
