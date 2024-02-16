---
content-type: release-notes
navigation-topic: product-releases-archive
title: 2018.1 Beta 4發行活動
description: 本頁說明2018.1 Beta 4版本預覽環境中最近可用的所有變更。 預覽環境已於2018年1月24日提供此功能。 它將在2018年3月的生產環境中提供。
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 8e016f12-bc72-475c-a8cc-38ded4351f88
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '2435'
ht-degree: 0%

---

# 2018.1 Beta 4發行活動

本頁說明2018.1 Beta 4版本預覽環境中最近可用的所有變更。 預覽環境已於2018年1月24日提供此功能。 它將在2018年3月的生產環境中提供。

>[!IMPORTANT]
>
> 本頁所述的功能在生產環境使用之前可能會有所變更。

如需2018.1年度所有變更的清單，請參閱  [2018.1版本活動概覽](../../../../product-announcements/product-releases/quarterly-release-archive/2018.1-release-activity/2018-1-release-activity-overview.md).

2018.1 Beta 4版本包含適用於Workfront管理員和其他使用者的增強功能：

**適用於管理員**

* [由群組管理員管理的排程](#schedules-managed-by-group-administrators)

**適用於所有使用者**

* [Workfront中的校訂改善](#proofing-improvements-within-workfront)
* [在Workfront中建立校訂 — 改善使用者體驗和其他功能](#proof-creation-in-workfront-proof-improved-user-experience-and-additional-functionality)
* [Workfront和Workfront Proof中的校訂改善](#proofing-improvements-within-workfront-and-workfront-proof)
* [透過Workfront Proof中的Basecamp整合更新外觀](#updated-look-and-feel-with-basecamp-integration-in-workfront-proof)
* [從剪貼簿將影像貼到Workfront](#paste-images-to-workfront-from-the-clipboard)
* [改善使用率報告](#utilization-report-improvements)
* [從Workfront移除資源預算時數物件](#remove-the-resource-budgeted-hour-object-from-workfront)
* [報告使用情況統計資料](#report-usage-statistics)
* [甘特圖更新](#gantt-chart-updates)
* [全新Portfolio最佳化工具](#new-portfolio-optimizer)
* [資源規劃工具中的預算日期調整選項](#budget-date-adjustment-option-in-the-resource-planner)
* [資源排程：根據群組成員資格限制指定給使用者](#resource-scheduling-restrict-assignments-to-users-based-on-group-membership)
* [資源排程：允許指定給使用者，無論角色為何](#resource-scheduling-allow-assignments-to-users-regardless-of-role)
* [Emoji支援](#emoji-support)

## Workfront中的校訂改善 {#proofing-improvements-within-workfront}

Workfront中的檔案清單已進行下列改進： 

* [從檔案清單檢視校訂進度](#view-proof-progress-from-the-document-list)
* [從檔案清單檢視列印摘要的新選項](#new-option-to-view-the-print-summary-from-the-document-list)
* [更新從檔案清單產生或開啟校訂的外觀](#updated-look-and-feel-for-generating-or-opening-the-proof-from-the-document-list)
* [從檔案清單上的檔案中移除的各種連結](#various-links-removed-from-documents-on-the-document-list)
* [檢視組合校訂的檔案名稱](#view-file-names-on-combined-proofs)
* [從檔案清單檢視校訂的目前使用中階段](#view-the-current-active-stage-of-a-proof-from-the-document-list)

### 從檔案清單檢視校訂進度 {#view-proof-progress-from-the-document-list}

現在檢視檔案清單時，所有校訂的校訂進度指示器都會顯示。 （包括已傳送、已開啟、已提出的評論和決定。）

在此變更之前，您必須在檔案清單中選取校訂，以在右側面板中檢視校訂進度。 

如需詳細資訊，請參閱 [校訂進度和狀態概觀](../../../../review-and-approve-work/proofing/proofing-overview/view-progress-status-proof.md).

### 從檔案清單檢視列印摘要的新選項 {#new-option-to-view-the-print-summary-from-the-document-list}

您現在可以直接從檔案清單中檢視校樣的列印摘要。

在此變更之前，您只能從校訂檢視器檢視列印摘要。 

如需有關從檔案清單檢視列印摘要的詳細資訊，請參閱 [在Adobe Workfront中列印校訂摘要](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/print-proof-summary-in-wf.md).

### 更新從檔案清單產生或開啟校訂的外觀 {#updated-look-and-feel-for-generating-or-opening-the-proof-from-the-document-list}

現在，將滑鼠懸停在檔案清單中的檔案時，產生校樣或開啟校樣的選項已更新。 這些選項現在更顯眼且顯示為按鈕。

在此變更之前，這些選項可用作檔名稱下方的連結。

如需詳細資訊，請參閱下列章節：

* 。
* 中的。

### 從檔案清單上的檔案中移除的各種連結 {#various-links-removed-from-documents-on-the-document-list}

下列動作不再可作為檔案清單內個別檔案的連結：

* 產生證據
* 證明
* 詳细資料
* 共用
* 簽出/簽入

下列動作現在可作為檔案清單中檔案的按鈕使用：

* 未完成的校訂（產生校訂後即可使用） 
* 產生校訂（尚未產生校訂時可用）

下列動作現在可在開啟校樣或產生校樣按鈕旁的下拉式選單中使用：

* 校訂詳細資訊
* 文件詳細資訊
* 列印摘要

如需詳細資訊，請參閱下列章節：

* 。
* 中的。

### 檢視組合校訂的檔案名稱 {#view-file-names-on-combined-proofs}

您現在可以檢視組成合併校訂的個別檔案名稱。 在檔案清單中選取校訂時，此資訊會顯示在「詳細資訊」標籤中。

如需詳細資訊，請參閱檢視合併校訂中包含的所有檔案。 

### 從檔案清單檢視校訂的目前使用中階段 {#view-the-current-active-stage-of-a-proof-from-the-document-list}

現在，在檔案清單中選取校訂時，目前的作用中階段會顯示在詳細資訊標籤的右欄。 

如需詳細資訊，請參閱 [檢視校訂上的使用中階段](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/view-active-stages-proof.md).  

## 在Workfront中建立校訂 — 改善使用者體驗和其他功能 {#proof-creation-in-workfront-proof-improved-user-experience-and-additional-functionality}

除了在Workfront Proof中建立校訂時改善的使用者體驗外，現在還提供以下附加功能：

* 將多個影像合併為單一校訂。
* 多個解析度的校訂網站（多個解析度可作為個別校訂建立，或可合併至單一校訂中）。
* 在上傳過程中編輯檔案名稱。
* 在校樣建立表單中包含自訂欄位。
* 新增自訂訊息到校訂電子郵件通知。
* 其他校訂設定 
* 校樣URL時的即時錯誤驗證（之前，您必須等待幾分鐘才會顯示錯誤）

>[!NOTE]
>
>這個在Workfront Proof中的新校訂建立頁面現在符合在Workfront中建立校訂時最近提供的校訂建立頁面。 

如需詳細資訊，請參閱  [在Workfront Proof中產生校訂](../../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).

## Workfront和Workfront Proof中的校訂改善 {#proofing-improvements-within-workfront-and-workfront-proof}

將檔案新增至Workfront和Workfront校訂時，適用下列變更：

* [檢閱校樣時調整評論清單大小](#resize-the-comment-list-when-reviewing-proofs)
* [檢閱靜態校樣時超連結為作用中](#hyperlinks-are-active-when-reviewing-static-proofs)
* [新增校訂時的改進](#improvements-when-adding-proofs)

### 檢閱校樣時調整評論清單大小 {#resize-the-comment-list-when-reviewing-proofs}

現在您可以在校訂檢視器中檢閱校訂時調整註解清單的大小。

如需詳細資訊，請參閱中的。

### 檢閱靜態校樣時超連結為作用中 {#hyperlinks-are-active-when-reviewing-static-proofs}

在校訂檢視器中檢閱靜態校訂時，超連結現在處於活動狀態。 按一下超連結以前往連結的頁面。

任何包含文字的檔案型別(例如PDF、DOC等)都支援此功能。 不支援影像檔案。

### 新增校訂時的改進 {#improvements-when-adding-proofs}

新增要校訂的檔案時，可使用下列增強功能。 

* 收件者清單中的資訊現在以3欄檢視提供，讓資訊更容易檢視和修改。 

  以前，資訊會以單欄檢視顯示，在需要變更時需要進行更多點按。 

  如需詳細資訊，請參閱中的。

* 使用自動化工作流程時，將一或多個收件者從一個工作流程階段拖曳至另一個工作流程階段。 您可以直接拖曳到舞台，或是拖曳到圖表上的舞台（位於頁面頂端）。

  如需詳細資訊，請參閱中的。

* 即使捲動，工作流程圖表仍會顯示在頁面頂端。 依照預設，圖表會摺疊；展開圖表可檢視完整圖表。

  如需詳細資訊，請參閱中的。

* 將範本新增到校訂中的自動化工作流程時，會顯示載入動畫，表示正在載入範本。

  如需詳細資訊，請參閱中的。

* 以下設定已從「校訂設定」區段移至「新校訂」頁面上的「工作流程」區段：

   * 主要決策者
   * 只需要一個決定

## 透過Workfront Proof中的Basecamp整合更新外觀 {#updated-look-and-feel-with-basecamp-integration-in-workfront-proof}

Basecamp與Workfront Proof整合的外觀與操作方式現已更新。 功能保持不變。

## 從剪貼簿將影像貼到Workfront {#paste-images-to-workfront-from-the-clipboard}

您現在可以從系統剪貼簿貼上影像，將影像檔案新增至Workfront。

從剪貼簿貼上的功能已在舊版中從Workfront移除；此版本正在重新推出這項功能。 新方法更精簡且更直覺。

如需詳細資訊，請參閱 [從剪貼簿貼上影像](../../../../documents/managing-documents/paste-image-clipboard.md). 

## 改善使用率報告 {#utilization-report-improvements}

「使用率」報表包含下列改善專案：

* 在專案的「使用率」報表中檢視收入

  可讓您檢視預算收入、計畫收入、實際收入、預算差異和計畫差異。

* 比較收入與計畫成本與實際成本

  可讓您檢視計畫或實際成本以及計畫收入。 也會顯示利潤(%) （利潤的計算方式為收入 — 成本/收入）。

* 收入會在檢檢視表時顯示。
* 捲動時標題保持可見。

  現在，捲動使用率報告中的資訊時，使用率報告頂部的標題一律可見，可讓您更輕鬆地瞭解報告中的資料。

  先前，「使用率」報表頂端的標題在捲動時不會顯示。

* 個別專案的使用情況報告會自動載入

  檢視專案的「使用率」報表時，報表會自動載入。

  在此變更之前，您必須在報表執行前按一下「執行」 。

* 提升效能

如需「使用率」報表的詳細資訊，請參閱 [資源使用率報表概要](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

## 從Workfront移除資源預算時數物件 {#remove-the-resource-budgeted-hour-object-from-workfront}

為了解決效能問題，已暫時從Workfront移除資源預算時數欄位。

提醒一下，資源預算時數是您為資源規劃工具中的資源或專案預算的時數。 目前，您無法在網頁應用程式中或透過API在此欄位上報告。 當效能問題解決後，該欄位將在未來版本中恢復。

如需有關資源規劃工具中預算時數的詳細資訊，請參閱 [資源規劃工具概觀](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md). 

## 報告使用情況統計資料 {#report-usage-statistics}

您現在可以在報表清單中顯示Workfront報表的下列使用情形資訊：

* 最後檢視者
* 上次檢視日期
* 最後 10 個檢視者
* 本月/季/年的檢視次數
* 檢視上個月/季/年
* 所有檢視

在此更新之前，您在報表上可看到的使用資訊有所限制。

如需有關報告使用情況的詳細資訊，請參閱 [檢視報表使用情形](../../../../reports-and-dashboards/reports/report-usage/view-report-usage.md)

## 由群組管理員管理的排程 {#schedules-managed-by-group-administrators}

身為群組管理員，您可以建立及編輯與所管理群組及其子群組相關聯的排程。 在此變更之前，只有Workfront管理員可以建立和編輯排程。

如需管理排程的詳細資訊，請參閱 [建立排程](../../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)

## 甘特圖更新 {#gantt-chart-updates}

甘特圖現在可供編輯。 您可以使用甘特圖對您的任務進行下列更新：

* 建立前置任務關係
* 編輯任務工期
* 更新任務完成百分比
* 套用資源平準

在此變更之前，您只能移除甘特圖中的前置任務關係，而且只能編輯工作清單中的工作。

如需甘特圖的詳細資訊，請參閱 [更新工作清單甘特圖中的資訊](../../../../manage-work/gantt-chart/use-the-gantt-chart/update-info-task-list-gantt.md)

## 全新Portfolio最佳化工具 {#new-portfolio-optimizer}

Workfront的Portfolio最佳化工具區域現在已更新為全新的外觀。 功能未變更。

如需有關Portfolio最佳化程式的詳細資訊，請參閱 [Portfolio最佳化工具概觀](../../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md)

## 資源規劃工具中的預算日期調整選項 {#budget-date-adjustment-option-in-the-resource-planner}

我們新增了一個選項，可讓您快速檢視時間範圍，而不會產生預算衝突。 當您檢視沒有預算衝突的時間範圍發生時，可以手動將預算時數移至這些時間。 這也會調整時數的預算日期。 在此更新之前，無法一眼檢視專案的預算衝突。

如需有關「資源規劃工具」中調整預算日期的更多資訊，請參閱 [資源規劃工具概觀](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md)

## 資源排程：根據群組成員資格限制指定給使用者 {#resource-scheduling-restrict-assignments-to-users-based-on-group-membership}

>[!NOTE]
>
>已棄用資源排程工具，並已從Workfront的23.1版本中移除。 如需有關使用工作負載平衡器排程資源的資訊，請參閱 [工作負載平衡器概覽](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

在「排程」區域中進行使用者指派時（如「手動指派排程區域中的未指派任務和問題」中所述），您現在可以設定Workfront，將任務和問題的指派限製為僅限屬於在任務或問題源自的專案上定義的群組成員的使用者。 

這適用於以下列方式指定任務：

* 將使用者指派給特定角色的所有任務和問題時，如「在排程區域中手動指派未指派的任務和問題」中所述。

  在此變更之前，任務或問題可始終指派給任何使用者，而不論該使用者的群組成員資格為何。 

* 與其他使用者交換指派時，如「在排程區域中手動指派未指派的任務和問題」中所述。

  在此變更之前，任務或問題可始終指派給任何使用者，而不論該使用者的群組成員資格為何。 

* 從排程時間表手動指派任務或問題時，如「在排程區域中手動指派未指派的任務和問題」中所述。

  在此變更之前，任務或問題可始終指派給任何使用者，而不論該使用者的群組成員資格為何。 

* 當允許Workfront自動指派使用者時，如「在排程區域中手動指派未指派的任務和問題」所述。

  在此變更之前，無論群組成員資格為何，Workfront都會將任務和問題指派給使用者。

如需設定此選項的詳細資訊，請參閱「開始使用資源排程」。

## 資源排程：允許指定給使用者，無論角色為何 {#resource-scheduling-allow-assignments-to-users-regardless-of-role}

在「排程」區域中進行使用者指派時（如「手動指派排程區域中的未指派任務和問題」中所述），您現在可以設定Workfront以允許將任務和問題指派給任何使用者，無論該使用者的使用者設定檔中是否定義了符合指派給他們的任務或問題的角色指派的角色。

這適用於以下列方式指定任務：

* 將使用者指派給特定角色的所有任務和問題時，如「在排程區域中手動指派未指派的任務和問題」中的「在排程區域中手動指派未指派的任務和問題」所述。

  在此變更之前，您指派之使用者的主要角色必須與「選取角色」欄位中已定義的角色相符。

* 與其他使用者交換指派時，如「在排程區域中手動指派未指派的任務和問題」中所述。

  在此變更之前，您指派之使用者的主要角色必須與「選取角色」欄位中已定義的角色相符。

* 從排程時間表手動指派任務或問題時，如「在排程區域中手動指派未指派的任務和問題」中所述。

  在此變更之前，排程時間表上只會顯示其角色符合您指派之任務或問題的使用者。

>[!NOTE]
>
>在允許Workfront自動指派使用者時，這不適用，如手動指派排程區域中未指派的任務和問題中所述。 當自動指派使用者時，只能將任務和問題指派給具有相符角色的使用者。

如需設定此選項的詳細資訊，請參閱「開始使用資源排程」。

## Emoji支援 {#emoji-support}

現在，您可以插入emoji來設定您在Workfront中註釋和更新的基調。 在「更新」標籤上新增至評論的任何表情符號，也會顯示在更新電子郵件通知中。 

如需詳細資訊，請參閱 [更新工作](../../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
