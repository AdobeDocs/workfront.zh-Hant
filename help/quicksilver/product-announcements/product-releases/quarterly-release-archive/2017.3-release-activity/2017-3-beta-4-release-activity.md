---
content-type: release-notes
navigation-topic: product-releases-archive
title: 2017.3 Beta 4發行活動
description: 本頁說明2017.3 Beta 4版本預覽環境中最近可用的所有變更。 此頁面上的功能已在2017年9月25日當週的「預覽」環境中提供。 它將在2017年11月初的生產環境中提供。
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: d6bb889c-a057-453f-8f80-761cfb1ad4a1
source-git-commit: 6405c01c8b1d842a4175f9caa18a7ed31316a3a1
workflow-type: tm+mt
source-wordcount: '1676'
ht-degree: 0%

---

# 2017.3 Beta 4發行活動

本頁說明2017.3 Beta 4版本預覽環境中最近可用的所有變更。 此頁面上的功能已在2017年9月25日當週的「預覽」環境中提供。 它將在2017年11月初的生產環境中提供。

>[!IMPORTANT]
>
> 本頁所述的功能在生產環境使用之前可能會有所變更。

如需2017.3年度所有變更的清單，請參閱  [2017.3發行活動總覽](../../../../product-announcements/product-releases/quarterly-release-archive/2017.3-release-activity/2017-3-release-activity-overview.md)。

2017.3 Beta 4版本包含適用於Workfront管理員和其他使用者的增強功能：

管理員的&#x200B;**&#x200B;**

* [在設定區域中新增資源管理喜好設定區域](#new-resource-management-preferences-area-in-the-setup-area)

**所有使用者**

* [重複的工作](#duplicate-tasks)
* 在排程資源時[自動執行指派](#automate-assignments-when-scheduling-resources)
* 在排程資源時[修改多項工作的指派](#modify-assignments-for-multiple-tasks-when-scheduling-resources)
* [套用FTE分配至資源規劃工具](#apply-fte-distribution-to-the-resource-planner)
* 使用者設定的[工作角色區段包含FTE可用性的百分比](#job-role-section-for-user-settings-includes-percentage-of-fte-availability)
* [儲存並管理專案使用報告中的篩選器](#save-and-manage-filters-in-the-utilization-report-on-a-project)
* 使用率報告中[其他篩選選項](#additional-filtering-options-in-the-utilization-report)
* [依方案或Portfolio檢視使用率報告](#view-the-utilization-report-by-program-or-portfolio)
* [在專案與任務報告中顯示原始問題資訊](#show-original-issue-information-in-project-and-task-reports)
* 更新資料流中的[篩選器系統更新現在跨物件持續存在](#filter-system-updates-in-the-update-stream-is-now-persistent-across-objects)
* [報告Workfront中的作用中校訂階段](#report-on-active-proof-stages-within-workfront)
* [指派自訂Workfront Proof許可權設定檔給Workfront中的使用者](#assign-custom-workfront-proof-permission-profiles-to-users-within-workfront)
* [時數資源已新增到事件訂閱](#hour-resource-added-to-event-subscriptions)

## 複製任務 {#duplicate-tasks}

您現在可以快速複製專案中的一項任務或一組任務。 這個動作會建立與原始任務相同的任務。 復製程式中沒有其他選項可讓您對新建立的任務進行任何變更。  

在此變更之前，您可以將任務複製到新專案或現有專案，並在複製時修改部分資訊。

的  有關複製任務的詳細資訊，請參閱[複製和複製任務](../../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md)。

## 排程資源時自動化指派 {#automate-assignments-when-scheduling-resources}

>[!NOTE]
>
>已棄用資源排程工具，並已從Workfront的23.1版本中移除。 如需有關使用工作負載平衡器排程資源的資訊，請參閱[工作負載平衡器概覽](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md)。

您現在可以允許Workfront在排程多個專案的資源時（從「排程」標籤），或排程單一專案的資源時（從「人員配置」標籤），自動建議未指派的任務和問題的指派。

Workfront會分析所有可用使用者的目前工作指派，並為任何尚未指派的任務或問題建議智慧型邏輯指派。 您可以在最後確定指派之前修改任何提議或現有的指派。

如需詳細資訊，請參閱「在排程區域中手動指派未指派的任務和問題」。

## 在排程資源時修改多重作業的指派 {#modify-assignments-for-multiple-tasks-when-scheduling-resources}

在排程資源時（從「排程」標籤或「人員配置」標籤），大量指派、交換或取消指派使用者時，您現在可以修改在一或多個專案中所指定之特定作業（包括所有子作業與相關問題）的指派。

在此變更之前，您只能在整個專案中修改任務和問題的指派（您不能在專案中指定特定任務）。

如需詳細資訊，請參閱「在排程區域中手動指派未指派的任務和問題」。

## 套用FTE分配至資源規劃工具 {#apply-fte-distribution-to-the-resource-planner}

>[!NOTE]
>
>此功能目前無法用於所有叢集的預覽。

當使用者有多個角色時，您現在可以根據每個角色的FTE可用性百分比，顯示使用者每個角色的正確可用時數。

例如，如果使用者的排程指出他們在一個月內可工作100小時，且他們主要角色的FTE可用性百分比為75%，而他們其他角色的FTE可用性百分比為25%，則資源規劃工具將列出主要角色下具有75可用時數的使用者，而其他角色下具有25可用時數的使用者。

在此變更之前，在「資源規劃工具」中顯示的使用者名稱僅針對「主要角色」，而且根據使用者的排程（100小時），使用者的完整可用性僅與「主要角色」相關聯。 只有當使用者被指派給該角色中的任務，且使用者在其他角色中的可用時數為零時，才會在「資源規劃工具」中顯示該使用者的其他角色。

如需有關如何為資源規劃工具中的使用者和角色計算可用時數和可用FTE的詳細資訊，請參閱[計算資源規劃工具中使用者和角色的時數和可用FTE的概觀](../../../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md)。

## 使用者設定值的工作角色區段包含FTE可用性的百分比 {#job-role-section-for-user-settings-includes-percentage-of-fte-availability}

>[!NOTE]
>
>此功能目前無法用於所有叢集的預覽。

現在，當更新使用者設定檔時，您可以新增其他工作角色到使用者，並定義分配給每個工作角色的FTE百分比。

在此變更之前，您無法將特定數量的FTE配置給任何與使用者相關聯的工作角色。

如需有關更新使用者工作角色的FTE可用性百分比的詳細資訊，請參閱[編輯使用者的設定檔](../../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)或[設定我的設定](../../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md)。

## 在設定區域中新增資源管理喜好設定區域 {#new-resource-management-preferences-area-in-the-setup-area}

您現在可以在安裝程式中找到稱為資源管理的新區域。 在此區域中，我們引進了設定，可讓您指定如何在資源規劃工具中計算使用者可用性。 您可以使用下列方法計算此值：

* 手動：除了使用者的個別FTE之外，還會使用系統的「預設排程」來決定使用者在「資源規劃工具」中的可用時數。 使用者的排程會被忽略。
* 自動：使用者的排程是用來決定使用者在資源規劃工具中的可用時數。 FTE可用性是根據使用者的排程和預設排程來計算。 使用者FTE的值會被忽略。 

如需有關為系統設定資源管理偏好設定的詳細資訊，請參閱[設定資源管理偏好設定](../../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md)。

## 儲存並管理專案使用報告中的篩選器 {#save-and-manage-filters-in-the-utilization-report-on-a-project}

現在，您可以儲存在「使用率」報告中建立的篩選器。 此外，您可以重新命名已儲存的篩選器、複製已儲存的篩選器、刪除已儲存的篩選器或修改已儲存的篩選器。

以前，每次篩選「使用率」報告時，都必須指定個別的篩選選項。

如需有關在[使用率]報告中儲存和管理篩選器的詳細資訊，請參閱[資源使用率報告簡介](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md)中的[資源使用率報告簡介](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md)。

## 使用率報表中的其他篩選選項 {#additional-filtering-options-in-the-utilization-report}

現在，執行「使用率」報告時，除了先前可用的「任務」、「問題」和「Portfolio」欄位外，建立篩選時，還會使用「角色」、「方案」和「專案」的新篩選欄位。

在此變更之前，您只能透過新增篩選規則來依投資組合、計畫和專案篩選。

如需詳細資訊，請參閱[資源使用狀況報告簡介](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md)中的[資源使用狀況報告簡介](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md)。

## 依方案或Portfolio檢視使用率報表 {#view-the-utilization-report-by-program-or-portfolio}

您現在可以依方案或投資組合檢視使用情況報告。 這可讓您在單一使用率報表中檢視多個專案的資訊。

為了協助這項變更，「使用率」索引標籤現在可在Workfront的報告區域以及個別專案中使用。

在此變更之前，只能在專案中存取「使用報告」 。

如需詳細資訊，請參閱  [資源使用率報告概觀](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md)。 

## 在專案和任務報告中顯示原始問題資訊 {#show-original-issue-information-in-project-and-task-reports}

>[!NOTE]
>
>此功能目前無法用於所有叢集的預覽。

對於透過轉換問題所建立的專案和任務，您現在可以在專案或任務報告中找到有關原始問題的下列資訊：

* 原始問題輸入日期
* 原始問題名稱
* 原始問題建立者ID

透過以文字模式建立自訂檢視，此資訊可以顯示在任務或專案報告或清單中。

在此變更之前，您無法報告此資訊。

如需有關建立自訂文字模式檢視以擷取原始問題資訊的詳細資訊，請參閱[檢視：在任務或專案清單上顯示原始問題資訊](../../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-display-original-issue-info-task-project-list.md)。

## 更新流中的篩選器系統更新現在跨物件持續存在 {#filter-system-updates-in-the-update-stream-is-now-persistent-across-objects}

>[!NOTE]
>
>此功能未透過Beta 4發行至預覽環境。 它將在10月上半月的預覽中提供。

「篩選系統更新」選項現在持續存在於整個Workfront網站的物件中。 這可讓您隱藏系統更新，並只檢視一個物件上「更新流」中的使用者註解，而且當您瀏覽至其他物件時，該設定會保留。

在此變更之前，您必須在瀏覽Workfront網站時選擇篩除每個物件的系統更新。

如需詳細資訊，請參閱[更新工作](../../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md)。

## Workfront中主動校訂階段的報告 {#report-on-active-proof-stages-within-workfront}

在Workfront中建立檔案版本報告時，現在有一個名為「主動校訂階段」的欄。 此欄可讓您檢視報告中每個檔案版本上目前有效的校訂階段。 階段的名稱會顯示在「主動校訂階段」欄中。 如果檔案版本上目前沒有作用中的階段，欄為空白。

如需檢視與報表中可用欄位的詳細資訊，請參閱[Adobe Workfront術語辭彙表](../../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md)。

## 在Workfront中指派自訂Workfront Proof許可權設定檔給使用者 {#assign-custom-workfront-proof-permission-profiles-to-users-within-workfront}

現在當您在Workfront中啟用使用者的校訂功能時，可以指派自訂Workfront Proof許可權設定檔。 

在此變更之前，只有下列許可權設定檔可用：監督員、管理員、管理員。

## 時數資源已新增到事件訂閱 {#hour-resource-added-to-event-subscriptions}

使用新的時數資源，您現在可以建立事件訂閱，讓您的計費應用程式與Workfront保持同步。

若要深入瞭解事件訂閱，請參閱[事件訂閱API](../../../../wf-api/general/event-subs-api.md)。
