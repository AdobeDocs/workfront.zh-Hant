---
content-type: release-notes
navigation-topic: product-releases-archive
title: 2017.2 Beta 1發行活動
description: 本頁說明2017.2 Beta 1版本預覽環境中所有可用的變更。 此頁面的功能已於2017年5月10日在預覽環境中推出。
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 99812ed3-a300-478e-973f-b957382d934b
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '1380'
ht-degree: 0%

---

# 2017.2 Beta 1發行活動

本頁說明2017.2 Beta 1版本預覽環境中所有可用的變更。 此頁面的功能已於2017年5月10日在預覽環境中推出。

>[!IMPORTANT]
>
>本頁所述的功能在生產環境使用之前可能會有所變更。

2017.2 Beta 1版本包含適用於Workfront管理員和其他使用者的增強功能：

管理員的&#x200B;**：**

* [還原檔案](#restore-documents)
* [新預覽橫幅及發行資訊](#new-preview-banner-with-release-information) 
* [API 7可用性](#api-7-availability)

所有使用者的&#x200B;**：**

* [訂閱任務和問題](#subscribe-to-tasks-and-issues)
* [資源排程改善](#resource-scheduling-improvements)
* [比較校樣](#compare-proofs)
* 使用者和專案的[新資源集區欄位](#new-field-for-resource-pools-for-users-and-projects)
* [已更新儀表板清單的外觀](#updated-look-and-feel-in-the-dashboard-list)
* [在Workfront中移除簽署功能](#removing-the-endorsements-functionality-in-workfront)
* [使用拖放功能重新排序任何清單中的欄（即將移除功能）](#reorder-columns-in-any-list-with-drag-and-drop-functionality-is-being-removed)

## 還原檔案 {#restore-documents}

Workfront管理員現在可以還原過去30天內刪除的個別檔案。 

在此變更之前，Workfront管理員只能還原專案、任務和問題（包括和已刪除的專案、任務或問題一起刪除的檔案）。

如需詳細資訊，請參閱[還原已刪除的專案](../../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md)。

## 含有發行資訊的新的預覽橫幅 {#new-preview-banner-with-release-information}

預覽沙箱環境頂端的藍色橫幅現在會顯示預覽環境的版本名稱和版本號碼。 按一下版本名稱會帶您前往說明網站文章，您可在此找到有關目前預覽版本的詳細資訊。 如需有關預覽沙箱環境的詳細資訊，請參閱[Adobe Workfront預覽沙箱環境](../../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md) 

## API 7可用性 {#api-7-availability}

API 7現已可用，並包含新的和更新的物件。

如需詳細資訊，請參閱[ API版本7](../../../../wf-api/api/new-api-version-7.md)的新增功能。

## 訂閱任務和問題 {#subscribe-to-tasks-and-issues}

Workfront會傳送有關您指派給或擁有之專案的通知。

從目前版本開始，如果您想追蹤未指派給您但可能影響您工作的專案，您可以訂閱它們。

您可以訂閱您至少有權檢視的問題和任務。 當您訂閱的問題或任務新增評論時，您將會收到有關該評論的電子郵件通知。

如需訂閱問題和工作的詳細資訊，請參閱[在Adobe Workfront中訂閱專案](../../../../workfront-basics/using-notifications/subscribe-to-items-in-workfront.md)

## 資源排程改善 {#resource-scheduling-improvements}

>[!NOTE]
>
>已棄用資源排程工具，並已從Workfront的23.1版本中移除。 如需有關使用工作負載平衡器排程資源的資訊，請參閱[工作負載平衡器概覽](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md)。

排程資源時，有以下改良功能可使用：

* [在單一檢視中檢視資源排程時間表上的更多專案](#view-more-items-on-the-resource-scheduling-timeline-in-a-single-view)
* [設定專案名稱以在排程時間表上的任務和問題上顯示](#configure-the-project-name-to-display-on-tasks-and-issues-on-the-scheduling-timeline)
* [設定是否在排程時間表上顯示父系任務](#configure-whether-parent-tasks-are-displayed-on-the-scheduling-timeline)
* [更輕鬆地展開或收合排程時間表上的所有任務和問題](#more-easily-expand-or-collapse-all-tasks-and-issues-on-the-scheduling-timeline)
* [捲動時，角色和使用者資訊會保留在排程時間表的最上方](#role-and-user-information-remains-at-the-top-of-the-scheduling-timeline-when-scrolling)

### 在單一檢視中檢視資源排程時間表上的更多專案 {#view-more-items-on-the-resource-scheduling-timeline-in-a-single-view}

現在當您為團隊或您擔任資源管理員的任何專案排程資源時，任務和問題在排程時間表上所佔用的垂直空間較少。 這可讓您在單一檢視中檢視更多工和問題。

如果您決定在排程時間表上顯示每個任務和問題的專案名稱，則會展開每個任務和問題的垂直空間，以減少在單一檢視中顯示的任務和問題。

如需排程資源的詳細資訊，請參閱  開始使用資源排程。

### 設定專案名稱以在排程時間表上的任務和問題上顯示 {#configure-the-project-name-to-display-on-tasks-and-issues-on-the-scheduling-timeline}

當您為團隊或您身為資源管理員的任何專案排程資源時，現在可以將專案名稱設定為顯示在排程時間表上的每個任務和問題上。 這可讓檢視排程時間表的使用者快速檢視任務或問題所在的專案名稱。

如需詳細資訊，請參閱「開始使用資源排程」。

### 設定是否在排程時間表上顯示父系任務 {#configure-whether-parent-tasks-are-displayed-on-the-scheduling-timeline}

當您為身為資源管理員的專案排程資源時，現在可以設定當專案的「摘要完成模式」選項設定為「手動」時，父系任務是否顯示在排程時間表上。

在此變更之前，當專案的「摘要完成模式」設定為「手動」時，父系任務一律會顯示在排程時間表上。 

當專案的「摘要完成模式」設定為「自動」時，父系任務無法顯示在排程時間表上。 此體驗未變更。

如需詳細資訊，請參閱「開始使用資源排程」。

### 更輕鬆地展開或收合排程時間表上的所有任務和問題 {#more-easily-expand-or-collapse-all-tasks-and-issues-on-the-scheduling-timeline}

有新連結可用，可讓您更輕鬆地摺疊排程時間表上的所有任務和問題。

如需詳細資訊，請參閱「開始使用資源排程」。

### 捲動時，角色和使用者資訊會保留在排程時間表的最上方 {#role-and-user-information-remains-at-the-top-of-the-scheduling-timeline-when-scrolling}

現在，當在排程時間表上向下捲動以檢視其他資訊時，角色名稱和使用者名稱保持在排程時間表上使用者和角色區域的頂端，使其更容易檢視任務與問題相關聯的使用者和角色。

在此變更之前，角色名稱和使用者名稱會捲動到目前檢視之外。

如需排程資源的詳細資訊，請參閱  開始使用資源排程。

## 比較校訂 {#compare-proofs}

您現在可以在任何單一檔案清單中比較兩個檔案校訂，例如在專案、任務、問題、投資組合的「檔案」標籤中，或在「全域導覽列」的主要「檔案」區域中。 

這兩個校訂會顯示在檢閱和核准工具中，您可以校訂每個檔案，同時在並排檢視中比較它們。

如需詳細資訊，請參閱[比較校樣](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/compare-proofs.md)。

## 使用者和專案之資源集區的新欄位 {#new-field-for-resource-pools-for-users-and-projects}

R1.5版本在「預覽」環境中引入「資源規劃」的新功能。 此功能可讓您建立新的資源集區，即使用者的集合。

現在您可以將這些資源集區與專案及使用者建立關聯。 您現在會在專案和使用者物件上看到名為「資源集區」的新欄位。

如需有關新的資源集區以及它們如何與專案和使用者關聯的詳細資訊，請參閱[資源集區概觀](../../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md)

## 已更新控制面板清單中的外觀 {#updated-look-and-feel-in-the-dashboard-list}

現在，檢視控制面板清單時，外觀和感覺更現代，而且可擴充。

此功能先前僅適用於已註冊提早存取的使用者。 預覽環境中的所有使用者現在都可以使用此功能。 2017.2版將提供給生產環境中的所有使用者。 

如需儀表板的詳細資訊，請參閱[建立儀表板](../../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md)。

## 移除Workfront中的簽署功能 {#removing-the-endorsements-functionality-in-workfront}

在評估更新串流中包含的功能時，我們發現簽署是一種低採用率和低使用率功能。 在2017.2中，從2017.2版開始，Workfront將移除以下與簽署相關的功能（此功能在預覽中不再提供）：

* 使用者設定檔區域中的「簽署」標籤；
* 簽署物件將從API總管中移除；如果您目前正在為物件「簽署」或「簽署共用」提取API報表，移除此物件後，呼叫將無效。

下列功能將繼續保留在網頁應用程式中：

* 此功能移除前由另一個使用者對使用者進行的簽署，將保留在簽署者的更新串流中。 

簽署不是可報告的物件，因此此物件的報告沒有任何變更。

## 使用拖放功能重新排序任何清單中的欄（即將移除功能） {#reorder-columns-in-any-list-with-drag-and-drop-functionality-is-being-removed}

在2017.2版的生產環境中，將欄從一個位置拖曳至另一個位置以變更任何清單中欄順序的功能，即將從「搶先存取」中移除，且任何使用者都無法再使用。 

如需有關此功能的詳細資訊，請參閱[修改欄寬和順序](../../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md)。
