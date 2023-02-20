---
product-area: projects
navigation-topic: plan-a-project
title: 確定項目中的工作細分結構
description: 為專案定義工作劃分結構(WBS)是一組最終概述專案計畫的活動。 WBS將項目的結果分成可管理的工作元素，這些工作元素可用於定義里程碑和組織工作分配。
author: Alina
feature: Work Management
exl-id: a76c468d-6373-4dab-93ff-a0b3734f368c
source-git-commit: fb538c6511514eedf81f4b9be452d5f87e3f7577
workflow-type: tm+mt
source-wordcount: '1738'
ht-degree: 1%

---

# 確定項目中的工作細分結構

為專案定義工作劃分結構(WBS)是一組最終概述專案計畫的活動。 WBS將項目的結果分成可管理的工作元素，這些工作元素可用於定義里程碑和組織工作分配。

您必須擁有具有「編輯」項目訪問權限的計畫許可證，才能建立項目的「工作劃分結構」。 視您在建置WBS時執行的活動數量，可能需要額外存取Adobe Workfront的其他區域。

建議您在對「工作劃分結構」進行變更時，將專案保持在「規劃」狀態，以避免通知觸發給專案團隊中的使用者。

## 定義項目交付項

項目的目的是向內部和外部利益攸關方提供切實的交付成果。 項目的交付項是您希望通過完成項目而實現的結果。 結果幾乎總是與至少一個交付項相關聯，而所有交付項都應與一個項目相關聯。

項目交付項可以是消費品、智慧產品（如報告）或服務。 例如，如果您的項目範圍是要建造房屋，則某些交付項可能包括：

* 建立架構計畫
* 完成管道
* 電工
* 澆築地基
* 框架工作
* 關閉房子的出售。

根據項目的規模和範圍，項目可以由多個交付件組成。

在確定交付項後，您可以開始將它們分解為任務。 任務是您為交付項目的整體結果而實現的輸出。 定義任務時，您會考慮下列參數：

* 完成所需的時間。
* 完成工作所需的預算。
* 完成工作所需的資源。
* 根據任務的邏輯時間表來排程資源。

在定義任務時，請確保不要為單個任務計畫太多的工作。 如果任務所需的工作時間超過40小時（通常是一週的工作時間），則您可能需要在子任務中劃分該工作量。 所有子任務的完成將完成主任務。

若要定義Workfront中的WBS結果和交付項目，建議您執行下列活動，以建立項目任務的分層視圖：

* 如果您尚未這麼做，請建立新專案。\
   如需建立專案的相關資訊，請參閱文章 [建立專案](../../../manage-work/projects/create-projects/create-project.md).

* 為完成每個結果和交付項所需的所有活動項建立任務。\
   如需建立工作的相關資訊，請參閱文章 [在專案中建立任務](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md) .

* 從您剛建立的任務中，識別哪些是主要結果，並將其與里程碑建立關聯。\
   如需建立里程碑工作的相關資訊，請參閱文章 [建立里程碑路徑](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md) 和 [將里程碑與任務關聯](../../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md).

* 將範圍過大的任務分解為子任務。 將它們與定義交付項的父級關聯。\
   如需建立子任務的相關資訊，請參閱文章 [建立子任務](../../../manage-work/tasks/create-tasks/create-subtasks.md).

* 識別子任務和里程碑之間的相依關係。\
   在依賴關係中，任務的開始取決於另一個任務或任務組的完成。\
   如需任務相依性的相關資訊，請參閱文章 [任務前置任務概述](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md) 和 [在任務清單上建立前置關係](../../../manage-work/tasks/use-prdcssrs/create-predecessors-on-task-list.md).

* 確定是否在項目的生命週期中的任何時間點需要批准和審核。 建立核准程式以滿足此需求。\
   如需核准的相關資訊，請參閱文章 [建立工作項的審批流程](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

## 估計工作計畫和計畫約束

建立項目的基本里程碑和任務結構後，您可以通過定義任務約束和持續時間來估計完成整個項目所需的時間。

請考量下列事項：

* 任務約束定義了在何時必須開始或結束任務。

   有關定義任務約束的資訊，請參閱文章 [任務約束概覽](../../../manage-work/tasks/task-constraints/task-constraint-overview.md).

* 任務的持續時間是完成任務的可用時間範圍。 預估持續時間時，您可能需要輸入值，以考慮延遲的可能性。 如果過去已完成類似的專案，您可能很清楚應在何處設定此值。

   由於持續時間是估計值，因此請務必設定樂觀的時間值，以考慮可能影響任務的因素，如天氣、停電、供應商困難或其他不可預見的事件。 此外，請務必考慮是否存在任何關聯的前置任務或依存任務，以及它們如何對工作施加約束並影響任務完成。

   根據任務的「持續時間類型」，您可以在項目的生命週期期間修改任務的持續時間，但這也會影響項目的時間軸。 有關任務持續時間的資訊，請參閱文章 [任務持續時間和持續時間類型概覽](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md) .

## 指派任務

在定義了每個任務的持續時間和限制後，您可以確定誰擁有完成工作所需的時間和技能。 您可以在Workfront中將任務指派給下列實體：

* 使用者\
   只能將具有計畫員或工作人員訪問權限級別的用戶分配給任務。 雖然您可以將任務指派給「請求者」和「審閱者」，但它們無法完成。 因此，我們不建議指派任務。

   如需存取層級及其如何定義使用者可對Workfront物件執行的相關資訊，請參閱 [存取層級概觀](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

* 職務角色
* 團隊

如需指派工作的相關資訊，請參閱 [指派任務](../../../manage-work/tasks/assign-tasks/assign-tasks-1.md) 區段。

## 管理資源

Workfront中的「資源管理」可讓您判斷是否有足夠的員工來完成專案。 將使用者新增至專案時，Workfront會顯示每位使用者的使用率。 資源管理器可以查看在項目的時間範圍內將人員分配給其他項目的總小時數。

>[!NOTE]
>
>只要項目的狀態為「計畫」，則分配給用戶的任務就不會顯示在其任務清單中。

在會計年度或季度之初，您可能希望在不了解特定工作劃分結構的情況下，在多個項目中以更高的級別管理您的資源。\
有關規劃更高級別資源使用的資訊，請參閱文章 [開始使用資源規劃](../../../resource-mgmt/resource-planning/get-started-resource-planning.md).

在構建一個項目的「工作劃分結構」並確保將每個任務分配給正確的資源時，您可以為需要完成的工作安排資源。\
如需排程資源的相關資訊，請參閱 [工作負載平衡器](../../../resource-mgmt/workload-balancer/workload-balancer.md) 區段。

## 估計項目財務

Workfront將計算每項任務的計畫成本和項目的總成本。 任務的計畫成本包括任務的所有費用，以及分配給任務的員工或職責的成本。 任務、角色和員工的每小時費率在建立任務、角色和用戶期間分配。

有關項目財務的資訊，請參閱 [項目財務](../../../manage-work/projects/project-finances/project-finances-overview.md) .

## 確定項目的批准點

在Workfront中建立核准流程，可以建立專案的審核點，以監控進度和潛在問題區域。 通過審批流程，項目所有者可以識別哪些任務延遲和提前，查看更改了任務狀態的清單的審核跟蹤，並查看問題的歷史記錄，包括問題如何解決和何時結束。 在審核項目後，項目所有者可以確定需要採取哪些步驟並在必要時更新項目計畫。

如需核准的相關資訊，請參閱文章 [建立工作項的審批流程](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md)

## 檢視您的WBS

若要了解專案的WBS，請檢視下列任務元素：

* 任務序列和時間表（計劃開始和完成日期以及任務持續時間）
* 前置相依性
* 子關係和父關係
* 指派

完成WBS後，您就可以在專案層級的任務清單或報表中加以檢視。

* [在任務清單中查看WBS](#view-the-wbs-in-a-task-list)
* [在任務報表中檢視WBS](#view-the-wbs-in-a-task-report)

### 在任務清單中查看WBS {#view-the-wbs-in-a-task-list}

您可以在項目級別查看任務清單。

1. 前往您要查看「工作劃分結構」的專案。
1. 選取 **工作** 標籤。
1. （選用）選取 **無** 在 **分組** 下拉式功能表。

   「工作劃分結構」不會顯示WBS中任務的縮排。

1. 從 **檢視** 下拉式功能表，然後選取 **工作劃分** 檢視。

   「工作劃分」結構會顯示在所選檢視的第二欄中。

   ![](assets/wbs-view-on-task-list-nwe-350x87.png)

### 在任務報表中檢視WBS {#view-the-wbs-in-a-task-report}

您可以執行下列任一操作，以建立任務報表並顯示任務的WBS:

* 將現有的「工作劃分結構」檢視套用至報表。
* 新增「工作劃分結構」欄至任何自訂報表。

>[!TIP]
>
>建議您新增專案群組，以清楚說明工作屬於哪些專案。 任務的縮排不會顯示在任務報告中。

如需建立報表的相關資訊，請參閱文章 [建立自訂報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

## 將專案的WBS儲存為範本

如果您處理的其他專案會遵循您剛建立的WBS，則可能會將專案儲存為範本。 範本可節省建立未來相關專案的時間和精力。

如果您的組織沒有任何週轉，請考慮等到完成使用者指派以儲存範本後再進行。 無論項目何時另存為模板，都可以在將模板附加到新項目期間刪除用戶分配或特定任務。

下列「工作劃分結構」的元素可儲存在範本中，以供日後與其他專案搭配使用：

* 前置依賴項
* 分配（包括項目責任人、發起人和資源管理器）
* 核准程序
* 任務約束
* 文件
* 開支及其他財務資料
* 目標
* 小時類型
* 請求佇列結構
* 提醒通知
* 風險
* 收費率
* 共用資訊
* 自訂表單

如需將專案儲存為範本的相關資訊，請參閱文章 [從專案建立範本](../../../manage-work/projects/create-and-manage-templates/create-template-from-project.md) .
