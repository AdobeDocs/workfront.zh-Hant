---
content-type: release-notes
navigation-topic: product-releases-archive
title: 2018.1 Beta 3發行活動
description: 本頁說明2018.1 Beta 3版本預覽環境中最近可用的所有變更。 預覽環境已於2018年1月7日提供此功能。 它將在2018年初在生產環境中提供。
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 26bbc4a0-e5ed-4b5f-bfc2-f888362c1d22
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '1850'
ht-degree: 0%

---

# 2018.1 Beta 3發行活動

本頁說明2018.1 Beta 3版本預覽環境中最近可用的所有變更。 預覽環境已於2018年1月7日提供此功能。 它將在2018年初在生產環境中提供。

>[!IMPORTANT]
>
> 本頁所述的功能在生產環境使用之前可能會有所變更。

如需2018.1年度所有變更的清單，請參閱  [2018.1發行活動總覽](../../../../product-announcements/product-releases/quarterly-release-archive/2018.1-release-activity/2018-1-release-activity-overview.md)。

2018.1 Beta 3版本包含適用於Workfront管理員和其他使用者的增強功能：

管理員的&#x200B;****

* [群組管理員改善](#group-administrator-improvements)

**所有使用者**

* [HTML5校訂檢視器改善](#html5-proofing-viewer-improvements)
* Workfront中的[校訂改善](#proofing-improvements-within-workfront)
* [首頁區域改善](#home-area-improvements) 
* [敏捷改善](#agile-improvements)
* [甘特圖改善](#gantt-chart-improvements)
* [資源規劃工具改善](#resource-planner-improvements)

## 群組管理員改善 {#group-administrator-improvements}

* [已更新群組管理員的重設密碼UI](#reset-password-ui-updated-for-group-administrators)
* [群組管理員的存取層級設定選項](#access-level-setup-options-for-group-administrators)
* [建立群組的週期性時程表](#create-timesheet-profiles-for-groups)
* [以群組管理員身分復原使用者的已刪除專案](#recover-deleted-items-for-users-as-a-group-administrator)

### 重設群組管理員的密碼UI已更新 {#reset-password-ui-updated-for-group-administrators}

作為群組管理員，當您重設其他使用者的密碼時，系統會提示您輸入自己的密碼，然後才能變更他們的密碼。 UI已更新，以反映此功能。 在此變更之前，UI顯示需要Workfront管理員密碼。

如需其他使用者重設密碼的詳細資訊，請參閱[編輯使用者的設定檔](../../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)。

如需群組管理員的權能詳細資訊，請參閱[建立群組](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md)中的「群組管理員的權能」一節。

### 群組管理員的存取層級設定選項 {#access-level-setup-options-for-group-administrators}

身為Workfront管理員，您現在可以控制群組管理員是否能夠以其他使用者身分登入，或是否可以重設其他使用者的密碼。 我們已在存取層級中新增設定，以啟用或停用此存取。 在此變更之前，所有群組管理員都可以以其他使用者身分登入，並依預設重設其他使用者的密碼。 此變更僅影響「規劃者存取層級」。

如需設定使用者存取層級的詳細資訊，請參閱[授予使用者存取權](../../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md)。

如需群組管理員的權能詳細資訊，請參閱[建立群組](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md)中的「群組管理員的權能」一節。

### 建立群組的週期性時程表 {#create-timesheet-profiles-for-groups}

作為群組管理員，您現在可以為您管理的群組建立時間表設定檔，並將其與您管理的群組或這些群組的使用者建立關聯。 時程表設定檔可確保系統會自動為與其相關聯的使用者建立時程表。

在此變更之前，只有Workfront管理員可以建立時間表設定檔。

如需建立時間表設定檔的詳細資訊，請參閱[建立、編輯和指派時間表設定檔](../../../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md)。

如需群組管理員的權能詳細資訊，請參閱[建立群組](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md)中的「群組管理員的權能」一節。

### 以群組管理員身分復原使用者的已刪除專案 {#recover-deleted-items-for-users-as-a-group-administrator}

如果專案與您身為群組管理員的群組相關聯，您可以從資源回收筒復原專案或其任何已刪除的任務、問題或檔案。 在此變更之前，只有Workfront管理員可以從資源回收筒復原專案。

如需有關在Workfront中復原已刪除專案的詳細資訊，請參閱[還原已刪除的專案](../../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md)。

如需群組管理員的權能詳細資訊，請參閱[建立群組](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md)中的「群組管理員的權能」一節。 

## HTML5校訂檢視器改進  {#html5-proofing-viewer-improvements}

* [比較模式](#compare-mode)
* [篩選評論清單](#filter-the-comment-list)
* [輸入第一個字元後，就會搜尋註解清單](#comment-list-is-searched-after-the-first-character-is-entered)

### 比較模式 {#compare-mode}

您現在可以在HTML5校訂檢視器中使用比較模式來檢視靜態和視訊校訂。 

HTML5校訂檢視器中的比較模式與舊版校訂檢視器有下列差異：

* 啟動「比較」模式時，較新版本會移至右側，而您正在比較的版本會開啟於左側。

  之前，較新版本會移至左側，而您正在比較的版本會在右側開啟。

* 您可以直接從校訂檢視器中選擇要比較的校訂版本。 
* 進入同時導覽時，會維持目前縮放等級和校訂檢視器中的校訂位置。
* 使用同時導覽時新增重設選項。
* 結束比較模式時，您可以選擇要關閉的校樣。 

  舊版一律關閉。

* 各種外觀、感覺和易用性改進。

如需詳細資訊，請參閱[在校訂檢視器中比較校訂](../../../../workfront-proof/wp-work-proofsfiles/review-proofs-wpv/compare-proofs.md)。

### 篩選評論清單 {#filter-the-comment-list}

您現在可以在註解清單中篩選註解。 您可以依使用者、動作、未讀取內容等條件進行篩選。

### 輸入第一個字元後，就會搜尋註解清單 {#comment-list-is-searched-after-the-first-character-is-entered}

現在，當您搜尋註解清單時，會在您輸入第一個字元後自動篩選清單。

在此變更之前，您必須在搜尋欄位中輸入至少3個字元，才能篩選評論清單。

如需詳細資訊，請參閱中的。

## Workfront中的校訂改善 {#proofing-improvements-within-workfront}

* [將校樣從Workfront Proof連結至Workfront](#link-proofs-from-workfront-proof-to-workfront)
* [無法再從檔案中移除校訂](#can-no-longer-remove-a-proof-from-a-document)
* [產生和開啟校樣時更新外觀](#updated-look-and-feel-when-generating-and-opening-proofs)

### 從Workfront Proof連結校樣至Workfront {#link-proofs-from-workfront-proof-to-workfront}

您現在可以將已存在於Workfront Proof帳戶中的檔案校訂連結至Workfront。

在此變更之前，您無法存取Workfront中Workfront Proof已存在的校訂。 

如需詳細資訊，請參閱[從外部應用程式連結檔案](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md)中的[從外部應用程式連結檔案](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md)。

### 無法再從檔案移除校訂 {#can-no-longer-remove-a-proof-from-a-document}

您無法再從檔案移除校訂。 若要移除校訂，您必須刪除整個檔案。

此增強功能可減少使用者不小心刪除校訂檔案所有版本的風險。 

如需有關刪除檔案的資訊，請參閱[刪除校訂](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/remove-archiveg-proof.md)中的[刪除校訂](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/remove-archiveg-proof.md)。

### 產生和開啟校樣時更新外觀 {#updated-look-and-feel-when-generating-and-opening-proofs}

現在當校訂產生時，會有更新的動畫旋轉圖示。

## 主區域改善 {#home-area-improvements}

「首頁」區域已進行下列增強功能：

* [從主區域檢視校訂核准](#view-proof-approvals-from-the-home-area)
* [為首頁區域中的專案設定版面配置範本時，會顯示預設欄位](#default-fields-are-displayed-when-configuring-the-layout-template-for-items-in-the-home-area)

### 從首頁區域檢視校訂核准 {#view-proof-approvals-from-the-home-area}

除了標準核准外，您現在還可以在首頁區域檢視校訂核准。

之前，您可以檢視Workfront核准，但無法檢視校訂的核准。  

如需詳細資訊，請參閱[使用主區域](../../../../workfront-basics/using-home/using-the-home-area/use-the-home-area.md)。

### 為首頁區域中的專案設定版面配置範本時，會顯示預設欄位 {#default-fields-are-displayed-when-configuring-the-layout-template-for-items-in-the-home-area}

以前，預設欄位從版面配置範本中不可見。

如需詳細資訊，請參閱建立及管理版面配置範本。

## 敏捷功能改進 {#agile-improvements}

* [直接從任務或問題詳細資訊頁面將任務和問題新增到疊代](#add-tasks-and-issues-to-the-iteration-directly-from-the-task-or-issue-details-page)
* [包括敏捷團隊的Scrum待處理專案和劇本面板上的問題](#include-issues-on-the-scrum-backlog-and-story-board-for-an-agile-team)
* [套用群組和篩選器至敏捷團隊的待處理專案](#apply-groupings-and-filters-to-the-backlog-for-an-agile-team)
* [建立空白反複專案並稍後更新](#create-a-blank-iteration-and-update-it-later)
* [建立疊代時會預先填入「焦點」和「容量」欄位](#the-focus-and-capacity-fields-are-pre-populated-when-creating-an-iteration)

### 直接從任務或問題詳細資訊頁面將任務和問題新增到疊代 {#add-tasks-and-issues-to-the-iteration-directly-from-the-task-or-issue-details-page}

您現在可以直接從任務或問題，將目前指派給敏捷團隊的任務和問題新增到疊代。

之前，您只能從待處理專案將任務新增至反複專案。 

如需詳細資訊，請參閱[建立反複專案](../../../../agile/use-scrum-in-an-agile-team/iterations/create-an-iteration.md)中的[建立反複專案](../../../../agile/use-scrum-in-an-agile-team/iterations/create-an-iteration.md)。

### 包括敏捷團隊的Scrum待處理專案和故事板的問題 {#include-issues-on-the-scrum-backlog-and-story-board-for-an-agile-team}

使用Scrum敏捷方法時，問題現在預設會包含在敏捷團隊的待辦專案中（使用Kanban方法時，問題不會顯示在敏捷團隊的待辦專案中）。

在此變更之前，只能將任務新增到待處理專案。 如果您想要新增問題，必須先將問題轉換為任務，然後才能新增。

如需有關使用待處理專案問題的資訊，請參閱  [管理敏捷待處理專案](../../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md)。

### 將群組和篩選器套用至敏捷團隊的待處理專案 {#apply-groupings-and-filters-to-the-backlog-for-an-agile-team}

敏捷待處理專案現在提供分組和篩選選項，可讓您依分組組織待處理專案，以及篩選特定任務和問題。

在此變更之前，您可以將檢視套用至敏捷待辦專案。

如需詳細資訊，請參閱  [管理敏捷待處理專案](../../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md)，在  [管理敏捷待處理專案](../../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md)。

### 建立空白反複專案並於稍後更新 {#create-a-blank-iteration-and-update-it-later}

您不再需要在疊代中新增任務或問題才能建立它。 您可以建立空白反複專案，並在稍後新增任務和問題。

如需詳細資訊，請參閱[建立反複專案](../../../../agile/use-scrum-in-an-agile-team/iterations/create-an-iteration.md)。

### 建立疊代時會預先填入「焦點」和「容量」欄位 {#the-focus-and-capacity-fields-are-pre-populated-when-creating-an-iteration}

現在，建立反複專案時，「焦點」和「容量」欄位會預先填入您的團隊已建立的所有過去反複專案的平均值。 如果您的團隊尚未建立任何過去的反複專案，這些欄位會顯示為0。

之前，這些欄位一律設為0。

如需詳細資訊，請參閱[建立反複專案](../../../../agile/use-scrum-in-an-agile-team/iterations/create-an-iteration.md)。

## 甘特圖改進 {#gantt-chart-improvements}

* [啟用甘特圖中的編輯模式](#enable-edit-mode-in-the-gantt-chart)
* [編輯甘特圖時移除前置任務](#remove-predecessors-when-editing-the-gantt-chart)

### 啟用甘特圖中的編輯模式 {#enable-edit-mode-in-the-gantt-chart}

當您啟用甘特圖中的編輯模式時，您可以變更圖表內的資訊。 在此變更之前，您無法編輯甘特圖中的資訊。 您只能編輯工作清單上的工作資訊。

如需有關編輯甘特圖的詳細資訊，請參閱工作清單甘特圖](../../../../manage-work/gantt-chart/use-the-gantt-chart/update-info-task-list-gantt.md)中的[更新資訊。

### 編輯甘特圖時移除前置任務 {#remove-predecessors-when-editing-the-gantt-chart}

使用甘特圖的編輯模式，您現在可以移除專案甘特圖中任務之間的前置任務關係。 在此增強功能之前，您只能在任務清單或任務層級移除前置任務關係。

如需有關編輯甘特圖的詳細資訊，請參閱工作清單甘特圖](../../../../manage-work/gantt-chart/use-the-gantt-chart/update-info-task-list-gantt.md)中的[更新資訊。

## 資源規劃工具改善 {#resource-planner-improvements}

* [資源規劃工具中持續時間為零的預算](#budget-with-zero-duration-in-the-resource-planner)

* [在資源規劃工具中依成本顯示資料](#show-data-by-cost-in-the-resource-planner)

### 資源規劃工具中工期為零的預算 {#budget-with-zero-duration-in-the-resource-planner}

>[!NOTE]
>
>此功能已從預覽環境中移除，並將在18.1版本中發行。

您現在可以在資源規劃工具中，針對專案時間範圍之內或之外的任何日期來編列資源預算。 在此增強功能之前，您只能為專案時間範圍內的日期編列資源預算。

如需有關資源規劃工具中預算資源的詳細資訊，請參閱[資源規劃工具概觀](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md)中的「資源規劃工具中的預算資源」一節。

### 在資源規劃工具中依成本顯示資料 {#show-data-by-cost-in-the-resource-planner}

除了時數與FTE值之外，您現在還可以按成本在「資源規劃工具」中顯示資訊。 當您在「依專案檢視」或「依角色檢視」檢視中檢視成本時，可以在「資源規劃工具」中顯示成本。 當您在「依使用者檢視」檢視中檢視資源規劃工具時，無法顯示「成本」。

如需依小時、約當全職人數或成本值檢視資源規劃工具的相關資訊，請參閱[資源規劃工具導覽概觀](../../../../resource-mgmt/resource-planning/resource-planner-navigation.md)。
