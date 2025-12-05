---
product-area: projects
navigation-topic: plan-a-project
title: 計畫專案概述
description: 專案是Adobe Workfront中的大型工作專案。 您可以將專案劃分為較小工作專案的任務。 可以將任務指派給負責完成任務的使用者或團隊。 當所有使用者完成其任務時，專案也會變得完成。
author: Alina
feature: Work Management
recommendations: noDisplay, noCatalog
exl-id: 23372e16-3933-445d-977c-901f52299cb2
source-git-commit: fb57f04a4031eaf38f88c3a1b2542d64ee230a8c
workflow-type: tm+mt
source-wordcount: '1673'
ht-degree: 0%

---

# 計畫專案概述

<!--Audited: 12/2025-->

<!--
< see if you need to add something about approval settings, issue for ad-hoc happenings and how to work with documents??-->

<!--this article is linked to the ESM area in the UI; the ESM team on the Adobe side linked to this article for their -->

專案是Adobe Workfront中的大型工作專案。 您可以將專案劃分為較小工作專案的任務。 可以將任務指派給負責完成任務的使用者或團隊。 當所有使用者完成其任務時，專案也會變得完成。

除了在專案中計畫您的任務外，許多其他詳細資訊也會進入計畫專案。 從判斷經濟影響到考量資源可用性，有許多專案元素需要注意。

## 建立專案範圍

專案計畫是指明確決定完成專案必須完成的主要目標。

在專案的初始階段中，您可能尚未決定您是否應實際執行專案。 這樣可能不符合成本效益，或者您沒有資源。 在此規劃階段中，您可以在Workfront中建立專案，不需新增任何工作，並將其狀態設定為Planning。

或者，您可以提交專案請求，詢問您的Portfolio經理建立專案是否可行。 這可讓您提交專案的業務案例，以便估計完成專案所需的專案。 這樣會建立狀態為「已要求」的專案。

如需有關建立專案的詳細資訊，請參閱文章[建立專案](../../../manage-work/projects/create-projects/create-project.md)。

如需有關建立專案要求的資訊，請參閱[要求專案](/help/quicksilver/manage-work/projects/create-projects/request-project.md)。

在計畫專案之前，請先考慮下列問題：

* 哪些是強制性的目標，哪些是選擇性的？
* 您是否有足夠的時間達成所有目標或僅達成核心目標？
* 您是否有足夠的預算完成所有目標？

您可以使用專案的業務案例，定義目標並確保專案與組織的策略一致。

如需定義專案商業案例的詳細資訊，請參閱文章[建立專案的商業案例](../../../manage-work/projects/define-a-business-case/create-business-case.md)。

定義專案的整體範圍後，您可以決定是否要進行專案並開始進行計畫。

## 初步專案計畫

* [定義專案的開始和完成日期](#define-the-start-and-completion-date-of-the-project)
* [定義專案排程](#define-the-project-schedule)
* [管理規劃專案所需的其他資訊](#manage-additional-information-needed-for-planning-the-project)

### 定義專案的開始和完成日期 {#define-the-start-and-completion-date-of-the-project}

當您計畫專案時，首先必須決定的事項之一是時間表：決定專案何時可以開始，以及專案必須完成的時間。

決定是否設定完成專案的截止日期，或者您是否應該設定起點並從那裡開始工作。

您可以從「開始日期」排程專案，或從「完成日期」排程專案。 您可在最初建立專案時設定此屬性，並可隨時透過編輯專案來變更此屬性。

如需詳細資訊，請參閱[編輯專案](/help/quicksilver/manage-work/projects/manage-projects/edit-projects.md)。

### 定義專案排程 {#define-the-project-schedule}

您必須決定排程，並將其與專案相關聯，並與負責完成專案任務的使用者相關聯。

排程會定義使用者可在專案上工作的時間。

請考慮在排程上定義下列專案：

* 假日
* 休假
* 一天或一週內可用於工作的小時數

瞭解使用者何時可以工作對於瞭解專案上任務的進度很重要。

您可以在Workfront執行個體中建立多個排程，並套用將用於所有專案的預設排程。 您也可以建立其他自訂排程，以將其與不同的個人建立關聯。

如需有關排程的詳細資訊，請參閱文章[建立排程](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)。

## 建立專案時間表

在您決定專案的主要目標，並決定專案值得追求之後，您應該計算每個目標的時間表。 每個目標都可以成為您專案中的一項任務。

這有助於排定目標的優先順序，並據此規劃您的工作分解結構。 工作分解結構會定義專案的時間表。\
如需有關在專案上建立任務的詳細資訊，請參閱本文中的[定義任務](#define-tasks)一節。

建立專案的時間表時，請考量下列事項：

* 將較大的目標劃分為子系任務，並定義其開始和完成日期。
* 將任務指派給個人或團隊，讓您知道誰負責完成任務。 您可以將任務指派給工作角色，但只有在專案的初始計畫階段中，當您不確定可以將誰指派給任務時。 啟動專案後，最好使用使用者或團隊指派取代工作角色。
* 決定您的目標是否與其他目標相依。

  您可以將這些相依性設定為前置任務。

  例如，您可能有要建公寓樓的專案。 您的其中一個目標包括水管工程，另一個目標是打好基礎。 您的其中一項水管工程是連線主要城市水線，這必須在奠基前完成。 不過，大部分其他管道工作要等到奠基後才可完成。 在此情況下，您應考慮使用前置任務，以瞭解一個目標在其先決條件完成後何時可以開始。

  當您使用父系任務來組織目標時，您可以為每個主要目標建立一個任務，並在進入將主要目標分解為個別任務的階段時新增子任務。 這樣可使屬於目標一部分的任務在專案內保持井然有序。

  如需有關前置任務的詳細資訊，請參閱[前置任務概觀](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md)。

* 考量專案最重要的目標，並將其標幟為里程碑任務。

  我們建議使用父系任務作為里程碑。

  如需有關使用里程碑工作的詳細資訊，請參閱[建立里程碑路徑](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md)。

* 為每個目標定義時間表。 如果您使用父系任務，則每個子系任務都必須有定義的「開始日期」和「完成日期」。 同一專案中任務的最早「開始日期」與任務的最晚「完成日期」之間的時間會產生專案時間表。

## 定義任務 {#define-tasks}

當您定義專案目標及與其相關的任務時，就是建立專案時間表。

您可以透過下列方式在專案上建立任務：

* 當您內聯編輯專案上的任務清單時，手動將任務新增到專案。
* 使用具有已定義範本任務的範本，並將其新增到您的專案。

  「範本任務」成為「專案任務」。

  如需有關建立任務的詳細資訊，請參閱文章[在專案中建立任務](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md)。

定義任務時，請考量下列事項：

* 定義每項工作的時間表。 這會在每個任務的期間欄位中擷取。

  如需有關工作持續時間的資訊，請參閱文章[工作持續時間和持續期間型別概觀](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md)。

* 定義工作之間的父子關係。
* 定義任務之間的前置任務關係。
* 將里程碑路徑與專案建立關聯，並將里程碑與其個別任務建立關聯。

  如需有關使用里程碑工作的詳細資訊，請參閱文章[建立里程碑路徑](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md)。

* 定義完成每項工作所需的工作量。 這是在每個任務的計畫時數欄位中擷取的。

  如需計畫時數的詳細資訊，請參閱文章[計畫時數概觀](../../../manage-work/tasks/task-information/planned-hours.md)。

* 將每個任務指派給負責完成任務的使用者或團隊。
* 檢查您指派給任務之使用者的可用性。 確保他們能夠自由工作且不會過度分配，以便完成指派的任務。 如果使用者過度分配或他們的排程有休假，請考慮下列其中一項：

   * 減少每個任務的計畫時數。
   * 新增更多使用者至任務，以確保任務可在為其分配的時間內完成。
   * 將任務重新指派給沒有其他限制的使用者。\
     如需計畫專案資源的詳細資訊，請參閱文章[資源計畫：文章索引](../../../resource-mgmt/resource-planning/resource-planning-overview.md)。\
     如需排程資源以完成專案工作的詳細資訊，請參閱[工作負載平衡器總覽](../../../resource-mgmt/workload-balancer/overview-workload-balancer.md)。

## 管理規劃專案所需的其他資訊 {#manage-additional-information-needed-for-planning-the-project}

規劃專案時，必須先設定其他資訊，才能開始處理專案。

請考慮提出下列問題：

* 是否有法規要求您保留事件與程式的記錄？ 如果是，您需要追蹤哪些專案？

  Workfront可讓您記錄編輯、範圍變更、狀態變更和動作，以便遵守特定於您行業的法規。\
  如需定義要在Workfront中追蹤哪些更新的詳細資訊，請參閱文章[系統追蹤的更新](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/system-tracked-update-feeds.md)。

* 是否有任何您需要追蹤的資訊在Workfront中沒有儲存該資訊的欄位？

  如果有的話，請為可儲存此資訊的專案或任務建立自訂Forms 。

  如需有關建立自訂表單的詳細資訊，請參閱文章[建立自訂表單](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)。

* 您是否需要記錄流程，並使用屬於日常工作或決定專案解決方案的資產？ 如果是，請建立儲存檔案的系統。

  如需詳細資訊，請參閱[檔案：文章索引](/help/quicksilver/documents/documents-overview.md)。

* 專案工作能夠繼續之前，是否有任何必須授與的核准檢查點？ 如果是，請針對您建置專案時可以使用的專案或任務建立核准流程，並清查哪些檔案或校訂必須核准，才能繼續工作。

  如需核准的詳細資訊，請參閱下列文章：

   * [建立工作專案的核准程式](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md)
   * [檢閱和核准工作](/help/quicksilver/review-and-approve-work/review-and-approve-work.md)
   * [整合檔案核准的可用功能](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/asset-review-and-approval.md)
