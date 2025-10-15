---
product-area: projects
navigation-topic: plan-a-project
title: 決定專案中的工作分解結構
description: 定義專案的工作劃分結構(WBS)是一組最終概述專案計畫的活動。 WBS會將專案結果劃分為可管理的工作元素，這些工作元素可用於定義里程碑和組織工作指派。
author: Alina
feature: Work Management
exl-id: a76c468d-6373-4dab-93ff-a0b3734f368c
source-git-commit: 5bc7a1c00b72cfc07270cafee5bf753989b48d33
workflow-type: tm+mt
source-wordcount: '1750'
ht-degree: 1%

---

# 決定專案中的工作分解結構

定義專案的工作劃分結構(WBS)是一組最終概述專案計畫的活動。 WBS會將專案結果劃分為可管理的工作元素，這些工作元素可用於定義里程碑和組織工作指派。

您必須擁有具有「編輯專案」存取權的計畫授權，才能建置專案的工作劃分結構。 視您在建立WBS時執行的活動數量而定，可能需要額外存取Adobe Workfront的其他區域。

建議您在變更「工作分解結構」時，讓專案保持在「計畫」狀態，以避免向「專案團隊」的使用者觸發通知。

## 定義專案交付專案

專案的目的是為內部和外部利害關係人提供具體的交付專案。 專案交付專案是指您想透過完成專案而達成的結果。 結果幾乎總是與至少一個交付專案相關聯，並且所有交付專案都應與專案相關聯。

專案交付專案可以是消費品、智慧輸出（例如報告）或服務。 例如，如果您的專案範圍是建置房屋，則某些交付專案可能包括：

* 建立架構計畫
* 正在完成管道
* 電氣工時
* 打地基
* 框架工作
* 關閉房屋的出售。

根據其大小和範圍，專案可以由多個交付專案組成。

識別交付專案後，您就可以開始將其細分為任務。 任務是指為了提供專案的整體結果而實現的輸出。 定義任務時，您會考量下列引數：

* 完成所需的時間。
* 完成工作所需的預算。
* 完成工作所需的資源。
* 根據任務的邏輯時間表排程資源。

定義任務時，請確保不要為一個單獨的任務計畫太多工作。 如果任務需要的工作超過40小時（典型的一週工作），則您可能需要細分子任務中的該工作量。 完成所有子任務後，主任務即告完成。

若要在Workfront中定義WBS結果和交付專案，建議您執行下列活動以建立專案任務的階層檢視：

* 如果您尚未這麼做，請建立新專案。\
  如需有關建立專案的資訊，請參閱文章[建立專案](../../../manage-work/projects/create-projects/create-project.md)。

* 針對完成每個結果和交付專案所需的所有行動專案建立任務。\
  如需有關建立任務的資訊，請參閱文章[在專案中建立任務](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md) 。

* 從您剛建立的任務中，找出哪些是主要結果，並將其與里程碑建立關聯。\
  如需有關建立里程碑任務的資訊，請參閱文章[建立里程碑路徑](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md)以及[將里程碑與任務建立關聯](../../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md)。

* 將範圍過大的任務劃分為子任務。 將它們與定義交付專案的父項建立關聯。\
  如需有關建立子工作的資訊，請參閱文章[建立子工作](../../../manage-work/tasks/create-tasks/create-subtasks.md)。

* 識別子任務之間和里程碑之間的相依性關係。\
  在相依關係中，任務的開始取決於另一個任務或任務群組的完成。\
  如需有關任務相依性的資訊，請參閱文章[任務前置任務概觀](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md)和[在任務清單上建立前置任務關係](../../../manage-work/tasks/use-prdcssrs/create-predecessors-on-task-list.md)。

* 決定專案存留期中的任何時間點，是否需要核准和審查。 建立核准流程以滿足此需求。\
  如需核准的相關資訊，請參閱文章[建立工作專案的核准流程](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md)。

## 預估工作排程與排程限制

一旦您建立了專案的基本里程碑和任務結構，您就可以藉由定義任務限制和持續時間來估計完成整個專案所需的時間。

請考量下列事項：

* 任務限制定義任務工作必須開始或結束的時間。

  如需定義任務限制的相關資訊，請參閱文章[任務限制總覽](../../../manage-work/tasks/task-constraints/task-constraint-overview.md)。

* 任務的期間是完成任務可用的時間範圍。 在預估「持續時間」時，您可能想要輸入考慮延遲可能性的值。 如果類似的專案在過去曾經完成，您對於設定此值的位置可能有一個不錯的想法。

  由於持續時間是預估值，請務必設定樂觀的時間值，以考慮可能影響工作的因素，例如天氣、停電、供應商困難或其他無法預見的事件。 此外，請務必考慮是否有任何相關的前置任務或相依性任務，以及這些任務如何對工作施加限制並影響任務完成。

  根據任務的期間型別，您可以在專案存留期中修改任務的期間，但這也會影響專案的時間表。 如需有關任務持續時間的資訊，請參閱文章[任務持續時間和持續時間型別概觀](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md) 。

## 指派任務

定義每個任務的工期與限制後，您可以決定誰有時間與技能完成工作。 您可以在Workfront中指派任務給下列實體：

* 使用者\
  只有具有供需規劃員或工作者存取層級的使用者才能指派至任務。 雖然您可以將工作指派給請求者和檢閱者，但他們無法完成這些工作。 因此，我們不建議指派工作給對方。

  如需存取層級的相關資訊，以及存取層級如何定義使用者可以對Workfront物件執行的動作，請參閱[存取層級概觀](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md)。

* 職務角色
* 團隊

如需指派工作的相關資訊，請參閱[指派工作](../../../manage-work/tasks/assign-tasks/assign-tasks-1.md)區段中的文章。

## 管理資源

Workfront中的資源管理可讓您確定是否有足夠的員工完成專案。 將使用者新增至專案時，Workfront會顯示每個使用者的使用率。 資源管理員可檢視在專案的時間範圍內，將人員指派給其他專案的總時數。

>[!NOTE]
>
>只要專案具有Planning狀態，指派給使用者的任務就不會出現在他們的任務清單中。

在會計年度或季度開始時，您可能想要跨多個專案在更高的層次管理資源，而不需要瞭解特定的「工作細分結構」。\
如需在更高層級規劃資源使用的相關資訊，請參閱文章[開始使用資源規劃](../../../resource-mgmt/resource-planning/get-started-resource-planning.md)。

當您在建立專案的「工作分解結構」前後關聯中管理資源，並確保每個任務都指派給正確的資源時，您就可以排定資源以進行需要完成的工作。\
如需有關排程資源的資訊，請參閱[工作負載平衡器：文章索引](../../../resource-mgmt/workload-balancer/workload-balancer.md)區段中的文章。

## 預估專案財務

Workfront將計算每個任務的計畫成本以及專案的整體成本。 任務的計畫成本包括任務的所有費用以及指派給任務的員工或角色的成本。 在任務、角色和使用者建立期間指派任務、角色和員工的小時費率。

如需有關專案財務的資訊，請參閱[專案財務：文章索引](../../../manage-work/projects/project-finances/project-finances-overview.md)一節。

## 決定專案的核准點

透過在Workfront中建立核准流程，您可以建立專案的稽核點，以監控進度和潛在問題區域。 透過核准程式，「專案擁有者」可以辨別哪些任務為延遲或提前，檢視列出變更任務狀態者的稽核軌跡，並檢視問題歷史記錄，包括問題的解決方式及關閉時間。 檢閱專案時，專案所有者可決定要採取的步驟，並視需要更新專案計畫。

如需核准的相關資訊，請參閱文章[建立工作專案的核准流程](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md)

## 檢視您的WBS

若要瞭解專案的WBS，您想要檢視下列任務元素：

* 任務序列和時間表（計劃開始和完成日期以及任務期間）
* 前置任務相依性
* 子系和父系關係
* 指派

完成WBS之後，您即可在專案層級的工作清單或報表中檢視它。

* [檢視工作清單中的WBS](#view-the-wbs-in-a-task-list)
* [在任務報告中檢視WBS](#view-the-wbs-in-a-task-report)

### 檢視工作清單中的WBS {#view-the-wbs-in-a-task-list}

您可以在專案層級檢視工作清單。

1. 前往您要檢視其工作分解結構的專案。
1. 選取&#x200B;**工作**&#x200B;標籤。
1. （選擇性）在&#x200B;**群組**&#x200B;下拉式功能表中選取&#x200B;**無**。

   工作分解結構不會顯示WBS中任務的縮排。

1. 從&#x200B;**檢視**&#x200B;下拉式功能表，選取&#x200B;**工作劃分**&#x200B;檢視。

   「工作劃分」結構會顯示在所選檢視的第二欄。

   ![工作清單中的工作分解結構](assets/work-breakdown-structure.png)

### 在任務報告中檢視WBS {#view-the-wbs-in-a-task-report}

您可以執行下列其中一項作業，建置作業報告並顯示作業的WBS：

* 將現有的工作劃分結構檢視套用至報表。
* 將「工作分解結構」欄新增至任何自訂報表。

>[!TIP]
>
>我們建議新增專案分組，以更清楚說明任務屬於哪些專案。 任務的縮排不會顯示在任務報告中。

如需有關建立報表的資訊，請參閱文章[建立自訂報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)。

## 將專案的WBS儲存為範本

如果您處理其他專案，而這些專案遵循的工作排程與剛剛建立的WBS類似，您可能想要將專案儲存為範本。 建立未來相關專案時，範本可節省時間和精力。

如果貴組織的人員流失率很低，請考慮等到指定使用者之後再儲存範本。 無論專案何時儲存為範本，將範本附加到新專案期間都可以移除使用者指派或特定任務。

工作分解結構的下列元素可以儲存在範本中，以供日後與其他專案搭配使用：

* 前置任務相依性
* 工作分派（包括專案所有者、贊助者和資源管理員）
* 核准程序
* 任務限制
* 文件
* 費用與其他財務資訊
* 目標
* 小時類型
* 請求佇列結構
* 提醒通知
* 風險
* 計費費率
* 共用資訊
* 自訂表單

如需有關將專案儲存為範本的資訊，請參閱文章[從專案建立範本](../../../manage-work/projects/create-and-manage-templates/create-template-from-project.md) 。
