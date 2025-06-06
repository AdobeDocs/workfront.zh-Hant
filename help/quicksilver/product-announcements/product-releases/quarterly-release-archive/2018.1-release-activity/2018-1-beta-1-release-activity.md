---
content-type: release-notes
navigation-topic: product-releases-archive
title: 2018.1 Beta 1發行活動
description: 本頁說明2018.1 Beta 1版本預覽環境中最近可用的所有變更。 此頁面的功能已於2017年12月1日在預覽環境中推出。 它將於2018年3月在生產環境中提供。
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: efcc2217-ab69-4ac4-8e9a-f811eba77d49
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '1065'
ht-degree: 0%

---

# 2018.1 Beta 1發行活動

本頁說明2018.1 Beta 1版本預覽環境中最近可用的所有變更。 此頁面的功能已於2017年12月1日在預覽環境中推出。 它將於2018年3月在生產環境中提供。

>[!IMPORTANT]
>
> 本頁所述的功能在生產環境使用之前可能會有所變更。

如需2018.1年度所有變更的清單，請參閱  [2018.1發行活動總覽](../../../../product-announcements/product-releases/quarterly-release-archive/2018.1-release-activity/2018-1-release-activity-overview.md)。

2018.1 Beta 1版本包含適用於Workfront管理員和其他使用者的增強功能：

管理員的&#x200B;**&#x200B;**

* [已更新配置範本以支援主區域](#updated-layout-template-to-support-the-home-area)
* [停用從Workfront傳送的校訂電子郵件通知](#disable-proofing-email-notifications-sent-from-workfront)
* [新增至事件訂閱的新資源](#new-resources-added-to-event-subscriptions)

**所有使用者**

* [主區域（已更新我的工作區域）](#home-area-updated-my-work-area)
* [在業務案例與更新的業務案例摘要下顯示資源規劃工具資料](#display-resource-planner-data-under-the-business-case-and-updated-business-case-summary)
* [在資源規劃工具中顯示計畫時數配置的百分比](#display-the-percentage-of-planned-hour-allocation-in-the-resource-planner)
* [「自動與變更時」及「僅變更」更新型別會在更新任務的同時觸發父物件的更新](#the-automatic-and-on-change-and-change-only-update-types-trigger-updates-to-the-parent-objects-at-the-same-time-as-tasks-are-updated)
* [甘特圖中可用的時間表快照](#timeline-snapshot-available-in-the-gantt-chart)

## 主區域（已更新我的工作區域） {#home-area-updated-my-work-area}

新的「首頁」區域為目前在「我的工作」區域中可用的相同資料提供替代的增強型檢視。 「首頁」區域比「我的工作」區域提供下列優點：

* 更精簡且更直覺的介面
* 增強效能
* 更新RTF格式的任務和問題

## 更新版面範本以支援首頁區域 {#updated-layout-template-to-support-the-home-area}

身為Workfront管理員，您可以設定指派給您的組織的使用者配置範本，以決定該使用者是否可以存取「首頁」區域。 未指派版面配置範本的使用者一律可以存取「首頁」區域。

如需詳細資訊，請參閱「建立及管理版面範本」。

## 停用從Workfront傳送的校訂電子郵件通知 {#disable-proofing-email-notifications-sent-from-workfront}

您現在可以設定在對校訂進行評論時，Workfront執行個體中的使用者是否收到來自Workfront的電子郵件通知。

以前，當對校訂進行評論時，校訂電子郵件一律從Workfront傳送。 如果Workfront Proof中也啟用了通知，則會導致使用者收到重複通知。 

對於現有的Workfront客戶，Workfront預設會設定為在校訂上發表評論時傳送電子郵件。

如需如何在Workfront中停用校樣的電子郵件通知，以便校樣電子郵件僅從Workfront Proof傳送的詳細資訊，請參閱。  

## 在業務案例和更新的業務案例摘要下方顯示資源規劃工具資料 {#display-resource-planner-data-under-the-business-case-and-updated-business-case-summary}

「資源預算」區域現在可用於專案的業務案例。 在此區域中，您可以檢視資源規劃工具中資源的估計預算時數以及與其相關的預算勞力成本。

業務案例的資源估計區域已重新命名為舊版資源估計。

作為此變更的一部分，業務案例摘要現在包含以資源估計和資源預算為基礎的財務資訊。

在此變更之前，您無法在專案的業務案例中看到資源規劃工具資訊。 您只能看到在舊版資源集區的Capacity Planner中指定的資源估計資訊。

如需建立業務案例的詳細資訊，請參閱[為專案建立業務案例](../../../../manage-work/projects/define-a-business-case/create-business-case.md)。

## 在資源規劃工具中顯示計畫時數配置的百分比 {#display-the-percentage-of-planned-hour-allocation-in-the-resource-planner}

「資源規劃工具」的「使用者檢視」現在包含新欄位，可讓您檢視使用者和職務角色的「計畫時數分配」，以總可用時數的百分比表示。

在此變更之前，您只能在單獨的欄中檢視使用者和工作角色的規劃與可用時數總計。

如需「計畫時數配置百分比」欄的詳細資訊，請參閱[資源規劃工具概觀](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md)中的「檢視可用時數與計畫時數或約當全職人數之間的差異」一節。

## 「自動與變更時」及「僅變更」更新型別會在更新任務的同時觸發父物件的更新 {#the-automatic-and-on-change-and-change-only-update-types-trigger-updates-to-the-parent-objects-at-the-same-time-as-tasks-are-updated}

我們已變更當專案中的較低層級物件更新時，父系任務和專案更新的方式。 父物件更新的時間由專案上的「更新型別」欄位決定。 您可以從下列更新型別中選取：

* 自動與專案變更時
* 僅限變更
* 僅限自動
* 僅限手動

現在，當您選取「自動與變更時」或「僅變更」更新型別時，您套用至個別任務的變更也會立即套用至父任務和專案。

在此變更之前，您必須重新整理頁面，以確保專案的父物件和時間表也會更新。

如需有關專案更新型別的詳細資訊，請參閱[選取專案更新型別](../../../../manage-work/projects/manage-projects/select-project-update-type.md)。

## 甘特圖中可用的時間表快照 {#timeline-snapshot-available-in-the-gantt-chart}

您現在可以使用甘特圖中的新時間表快照，快速捲動至專案期限中的特定點。

當您在檢視任務或專案清單時，為甘特圖選取較精細的時間範圍時，水準卷軸會顯示在甘特圖的底部。 按一下卷軸可讓您在快照中檢視專案的整個時間表。 您可以按一下甘特圖快照內的任何位置，以導覽至專案期限中的特定點。

在此變更之前，您必須水準捲動整個甘特圖以尋找特定時間點，或者您必須縮小粒度檢視。

如需有關資訊如何顯示在甘特圖中的詳細資訊，請參閱[設定資訊在甘特圖上的顯示方式](../../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md)。

## 新增至事件訂閱的新資源 {#new-resources-added-to-event-subscriptions}

現在您可以為下列資源建立事件訂閱：

* **費用：**&#x200B;在新增或修改費用時通知您。
* **工作分派：**&#x200B;當使用者、工作角色或團隊的任務或問題新增或修改工作分派時，通知您。
* **時程表：**&#x200B;在時程表提交、拒絕或核準時通知您。

若要深入瞭解事件訂閱，請參閱[事件訂閱API](../../../../wf-api/general/event-subs-api.md)。
