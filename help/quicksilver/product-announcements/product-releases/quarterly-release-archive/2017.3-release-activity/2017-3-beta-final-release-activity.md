---
content-type: release-notes
navigation-topic: product-releases-archive
title: 2017.3 Beta最終發行活動
description: 本頁說明2017.3 Beta最終版本預覽環境中最近可用的所有變更。 此頁面的功能已於2017年9月12日在預覽環境中推出。 它將在2017年11月初的生產環境中提供。
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 880828f4-3908-4ef0-ab1f-774f8dee72b6
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '3821'
ht-degree: 0%

---

# 2017.3 Beta最終發行活動

本頁說明2017.3 Beta最終版本預覽環境中最近可用的所有變更。 此頁面的功能已於2017年9月12日在預覽環境中推出。 它將在2017年11月初的生產環境中提供。

>[!IMPORTANT]
>
> 本頁所述的功能在生產環境使用之前可能會有所變更。

如需2017.3年度所有變更的清單，請參閱  [2017.3發行活動總覽](../../../../product-announcements/product-releases/quarterly-release-archive/2017.3-release-activity/2017-3-release-activity-overview.md)。

2017.3 Beta最終版本包含適用於Workfront管理員和其他使用者的增強功能：

管理員的&#x200B;**&#x200B;**

* [在核准設定區域中重新呼叫要求的新設定](#new-configuration-for-recalling-requests-in-the-approval-settings-area)
* [設定預設校訂角色](#configure-default-proof-roles)

**所有使用者**

* [主區域（已更新我的工作區域）](#home-area-updated-my-work-area)

* [已更新配置範本以支援主區域](#updated-layout-template-to-support-the-home-area)

* 適用於敏捷的[Kanban](#kanban-for-agile)
* [包含敏捷團隊的Scrum待處理專案上的問題](#include-issues-on-the-scrum-backlog-for-an-agile-team)
* [在Scrum敏捷故事板上包含問題](#include-issues-on-the-scrum-agile-story-board)
* [套用群組和篩選器至敏捷團隊的待處理專案](#apply-groupings-and-filters-to-the-backlog-for-an-agile-team)
* [在預覽環境中傳回增強的@Tagging功能](#enhanced-tagging-functionality-returns-in-the-preview-environment)
* 更新資料流中的[篩選器系統更新現在跨物件持續存在](#filter-system-updates-in-the-update-stream-is-now-persistent-across-objects)
* [在使用情況報告中視覺化資料](#visualize-data-in-the-utilization-report)
* [使用報告效能改善](#utilization-report-performance-improvement)
* [檔案增強功能：精簡的介面](#document-enhancements-streamlined-interface)
* Workfront中的[校訂增強功能](#proofing-enhancements-within-workfront)
* Workfront Proof和Workfront中的[校訂增強功能](#proofing-enhancements-within-both-workfront-proof-and-workfront)
* 更新及電子郵件的[ RTF格式](#rich-text-formatting-for-updates-and-emails)
* [新甘特圖重新設計](#new-gantt-chart-redesign)
* [內建報告包含更新的說明](#built-in-reports-contain-updated-descriptions)
* [在匯出的報告、清單和儀表板中標示品牌](#branding-in-exported-reports-lists-and-dashboards)
* [複製任務和移動任務或問題時的改進](#improvements-when-copying-tasks-and-moving-tasks-or-issues)
* [資源預算時數報告的新群組：配置日期](#new-grouping-for-resource-budgeted-hour-reports-allocation-date)
* [資源規劃工具改善](#resource-planner-improvements)
* [行動裝置改良](#mobile-improvements)
* [Workfront與Slack](#workfront-integration-with-slack)整合
* [Outlook 365改良](#outlook-365-improvements)
* [API變更](#api-changes)

## 主區域（已更新我的工作區域） {#home-area-updated-my-work-area}

>[!NOTE]
>
>17.3版本不會將此功能發佈到生產環境；在2018年初之前，此功能將保留在「預覽」中。

新的「首頁」區域為目前在「我的工作」區域中可用的相同資料提供替代的增強型檢視。 「首頁」區域比「我的工作」區域提供下列優點：

* 更精簡且更直覺的介面
* 增強效能

以下功能在「我的工作」區域中可用，但尚未在「首頁」區域中實作：

* 檢視您的個人行事曆
* 更新RTF格式的任務和問題
* 核准校樣
* 檢視您提交核准的工作清單
* 在專案上建立臨時問題
* 僅檢視那些已委派給您的核准

如需有關使用新主區域的詳細資訊，請參閱[使用主區域](../../../../workfront-basics/using-home/using-the-home-area/use-the-home-area.md)。

## 更新版面範本以支援首頁區域 {#updated-layout-template-to-support-the-home-area}

>[!NOTE]
>
>17.3版本不會將此功能發佈到生產環境；在2018年初之前，此功能將保留在「預覽」中。

身為Workfront管理員，您可以設定指派給您的組織的使用者配置範本，以決定該使用者是否可以存取「首頁」區域。 未指派版面配置範本的使用者一律可以存取「首頁」區域。

如需詳細資訊，請參閱建立和管理版面範本中的「自訂首頁」。

## 適用於敏捷的Kanban  {#kanban-for-agile}

除了已支援的Scrum敏捷方法之外，敏捷團隊現在可以在Workfront中使用Kanban方法。

Workfront中的Scrum和Kanban敏捷方法有以下差異：

**在Workfront中使用看板的好處**

* 在Kanban敏捷故事板上顯示待處理專案。

  如需詳細資訊，請參閱中的。

* 設定待處理專案上的專案，以便在其他專案移至等同於完成的狀態時，自動新增到看板敏捷故事板中。

  如需詳細資訊，請參閱[設定Kanban](../../../../agile/get-started-with-agile-in-workfront/configure-kanban.md)中的[設定要自動從待處理專案新增的劇本](../../../../agile/get-started-with-agile-in-workfront/configure-kanban.md#configur5)。

* 設定要在Kanban敏捷故事板上顯示的進行中工作(WIP)限制。

  如需詳細資訊，請參閱[設定看板](../../../../agile/get-started-with-agile-in-workfront/configure-kanban.md)中的[設定進行中的工作(WIP)限制](../../../../agile/get-started-with-agile-in-workfront/configure-kanban.md#configur4)。

**在Workfront中使用Scrum的好處**

* 將一組內文新增到敏捷疊代，並為該疊代建立內文板。
* 在Scrum故事板上加入問題。
* 包括敏捷團隊待處理專案上的問題。

  如需詳細資訊，請參閱[設定Scrum](../../../../agile/get-started-with-agile-in-workfront/configure-scrum.md)中的[設定將工作專案新增至疊代](../../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configur5)時如何套用日期。

* 子任務可以顯示在Scrum故事板上。
* 檢視待執行工作圖表，以檢視反複專案期間內文的進度。

  如需詳細資訊，請參閱[敏捷待執行工作圖表總覽](../../../../agile/use-scrum-in-an-agile-team/burndown/burndown-chart-overview.md)。

如需有關啟用和設定敏捷團隊看板的詳細資訊，請參閱[建立敏捷團隊](../../../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md)中的[決定敏捷方法](../../../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md#deciding)。

## 包括敏捷團隊的Scrum待辦專案上的問題 {#include-issues-on-the-scrum-backlog-for-an-agile-team}

>[!NOTE]
>
>此功能已於2017年11月14日從生產環境中移除。 我們計畫於2018年初將其重新引入預覽環境，其中包含增強型設計和提升穩定性。 它將在2018.1版本的生產環境中可用。

您現在可以在使用Scrum敏捷方法時將問題包含在敏捷團隊的待辦專案中（使用Kanban方法時，問題未顯示在敏捷團隊的待辦專案中）。 現有的Scrum敏捷團隊必須啟用此功能才能納入問題。 在2017.3版之後建立的Scrum敏捷團隊的待辦專案中會自動包含問題。

在此變更之前，只能將任務新增到待處理專案。 如果您想要新增問題，必須先將問題轉換為任務，然後才能新增。

由於您現在可存取的不僅是待處理專案上的任務，因此先前在待處理專案上可用的任何自訂任務檢視都會複製並新增到待處理專案中，作為自訂待處理專案檢視。

如需有關使用待處理專案問題的資訊，請參閱  [管理敏捷待處理專案](../../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md)。

如需啟用問題以供敏捷Scrum團隊待處理專案使用的相關資訊，請參閱  [&#128279;](../../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configur5)設定在[設定Scrum](../../../../agile/get-started-with-agile-in-workfront/configure-scrum.md)中將工作專案新增到疊代時如何套用日期。

## 在Scrum敏捷故事板上包含問題 {#include-issues-on-the-scrum-agile-story-board}

>[!NOTE]
>
>此功能已於2017年11月14日從生產環境中移除。 我們計畫於2018年初將其重新引入預覽環境，其中包含增強型設計和提升穩定性。 它將在2018.1版本的生產環境中可用。

現在當您使用Scrum敏捷方法時，可以在故事板上加入問題。

如需詳細資訊，請參閱[設定Scrum](../../../../agile/get-started-with-agile-in-workfront/configure-scrum.md)中的[設定敏捷故事板上的狀態列](../../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configur2)。

## 將群組和篩選器套用至敏捷團隊的待處理專案 {#apply-groupings-and-filters-to-the-backlog-for-an-agile-team}

>[!NOTE]
>
>此功能已於2017年11月14日從生產環境中移除。 我們計畫於2018年初將其重新引入預覽環境，其中包含增強型設計和提升穩定性。 它將在2018.1版本的生產環境中可用。

敏捷待處理專案現在提供分組和篩選選項，可讓您依分組組織待處理專案，以及篩選特定任務和問題。

在此變更之前，您可以將檢視套用至敏捷待辦專案。

如需詳細資訊，請參閱  [管理敏捷待處理專案](../../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md)，在  [管理敏捷待處理專案](../../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md)。

## 更新和電子郵件的RTF格式 {#rich-text-formatting-for-updates-and-emails}

>[!NOTE]
>
>您在預覽環境中進行的格式變更可能會回覆成未格式化的狀態。

現在，您可以格式化對Workfront物件所做的註解和更新，以強調重要資訊。 

使用RTF工具，您可以將格式屬性套用至文字、建立專案符號和編號清單，以及將超連結新增至其他資源。

套用至更新串流中評論的格式也會顯示在更新電子郵件通知中。 若要進一步瞭解如何格式化您的註解，請參閱[更新工作](../../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md)。

## 預覽環境中傳回增強的@Tagging功能 {#enhanced-tagging-functionality-returns-in-the-preview-environment}

您可以再次使用@符號，在「預覽」環境中所有物件的「更新流」中標籤其他使用者。 在過去@tagging會將標籤使用者的名字和姓氏放在更新流中。 現在，增強的@tagging功能只會顯示使用者的名字。 若要進一步瞭解如何在更新中標籤使用者，請參閱[在更新中標籤其他人](../../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md)。

## 更新流中的篩選器系統更新現在跨物件持續存在 {#filter-system-updates-in-the-update-stream-is-now-persistent-across-objects}

「篩選系統更新」選項現在持續存在於整個Workfront網站的物件中。 這可讓您隱藏系統更新，並只檢視一個物件上「更新流」中的使用者註解，而且當您瀏覽至其他物件時，該設定會保留。

在此變更之前，您必須在瀏覽Workfront網站時選擇篩除每個物件的系統更新。

如需詳細資訊，請參閱[更新工作](../../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md)。

## 在使用情況報告中以視覺效果呈現資料 {#visualize-data-in-the-utilization-report}

 您現在可以在圖表檢視中檢視使用率資訊。 

如需詳細資訊，請參閱[資源使用狀況報告簡介](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md)中的[資源使用狀況報告簡介](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md)。

## 使用率報表效能改善 {#utilization-report-performance-improvement}

>[!NOTE]
>
>此功能在Beta最終發行後的修補程式中發行。

現在，當執行「使用率」報告時，系統會提示您在執行報告之前套用篩選器。 此變更可確保儘快在「使用率」報告中產生最相關的資訊。

如需有關執行使用率報告的詳細資訊，請參閱[資源使用率報告概覽](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md)中的[資源使用率報告概覽](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md)。

## 檔案增強功能：精簡的介面 {#document-enhancements-streamlined-interface}

向Workfront新增檔案的使用者體驗現在更簡化且更直覺。 現在，您可以從檔案系統上傳檔案、要求檔案，或從協力廠商應用程式(例如Google或Dropbox)連結檔案，全都透過簡單的下拉式選單完成。 

以前，您可以透過啟動「新增檔案」對話方塊使用這些選項。 

如需詳細資訊，請參閱下列資訊：

* [從您的檔案系統新增檔案至Adobe Workfront](../../../../documents/adding-documents-to-workfront/add-documents-from-file-system.md)
* [要求檔案](../../../../documents/adding-documents-to-workfront/request-a-document.md)
* [從外部應用程式連結檔案](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md) 

>[!NOTE]
>
>進行此變更後，從剪貼簿貼上影像或檔案的選項將不再可用。

## Workfront中的校訂增強功能 {#proofing-enhancements-within-workfront}

* [改善的使用者體驗和其他功能](#improved-user-experience-and-additional-functionality)
* [直接從校訂檢視器共用](#share-directly-from-the-proofing-viewer)
* [設定預設校訂角色](#configure-default-proof-roles)

### 改善的使用者體驗和其他功能 {#improved-user-experience-and-additional-functionality}

除了在Workfront中建立校訂時改善的使用者體驗外，現在還提供以下附加功能：

* 將多個影像合併為單一校訂。
* 多個解析度的校訂網站（多個解析度可作為個別校訂建立，或可合併至單一校訂中）。
* 在上傳過程中編輯檔案名稱。
* 在校樣建立表單中包含自訂欄位。
* 新增自訂訊息到校訂電子郵件通知。
* 其他校訂設定 
* 校樣URL時的即時錯誤驗證（之前，您必須等待幾分鐘才會顯示錯誤）

如需詳細資訊，請參閱。

>[!NOTE]
>
> 使用自動化工作流程建立新校訂時，不支援使用拖放功能將使用者從一個階段移動至另一個階段。 請改為從一個步驟中移除使用者，然後將他們新增到另一個步驟。

*2018.1版將重新引入使用拖放功能將使用者從一個步驟移至另一個步驟的選項。*

### 直接從校訂檢視器共用 {#share-directly-from-the-proofing-viewer}

現在，您可以直接從校訂檢視器與特定Workfront使用者共用。

>[!NOTE]
>
>此功能僅適用於新校訂（2017.3版之後建立的校訂），且僅適用於與Workfront Proof Premium帳戶整合的Workfront執行個體。

在此變更之前，您只能透過建立連結，然後與使用者共用該連結來共用。 

如需詳細資訊，請參閱[在Adobe Workfront中共用校訂](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md)中的[在Adobe Workfront中共用校訂](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md)。

### 設定預設校訂角色 {#configure-default-proof-roles}

您現在可以設定預設校訂角色，新使用者和訪客使用者必須在Workfront系統中新校訂。 

這是與校訂共用校訂時，在校訂上指派使用者的預設角色。 

## Workfront Proof和Workfront中的校訂增強功能 {#proofing-enhancements-within-both-workfront-proof-and-workfront}

* [在HTML5視訊校訂檢視器中重新啟動並略過（鍵盤快速鍵）](#restart-and-skip-in-html5-video-proofing-viewer-keyboard-shortcuts)
* [HTML5校訂檢視器更新](#html5-proofing-viewer-updates)

### 在HTML5視訊校訂檢視器中重新啟動並跳過（鍵盤快速鍵） {#restart-and-skip-in-html5-video-proofing-viewer-keyboard-shortcuts}

現在，視訊的HTML5校訂檢視器內有鍵盤快速鍵，可讓您從視訊的開頭重新啟動視訊，並跳至視訊的結尾。

如需有關可用鍵盤快速鍵的詳細資訊，請參閱[Workfront Proof校訂檢視器中的鍵盤快速鍵](../../../../workfront-proof/wp-work-proofsfiles/review-proofs-wpv/keyboard-shortcuts.md)。

### HTML5校訂檢視器更新 {#html5-proofing-viewer-updates}

HTML5檢視器現在支援靜態校樣。

在此變更之前，HTML5檢視器僅支援視訊校樣。 

校樣靜態內容時，HTML檢視器包含下列新功能：

* 在單一檢視中時，在多個頁面上加上標籤進行單一註解

  這之前只有在連續檢視或Magazine檢視中才可行

* 透過校訂縮圖導覽校訂

   * 輕鬆識別正在稽核的校樣部分。 這點很重要，尤其是當使用者使用格式較大的校樣和較長的網頁，或在任何時候  需要更大的縮放等級才能檢視詳細資訊。
   * 變更縮放等級
   * 平移內容

* 在測量工具中指定自訂值
* 在Workfront Proof的校樣檢視器中對校樣內的文字加上註解時，您可以包含用於指示文字應該加粗顯示、斜體顯示和底線的選項。

HTML5檢視器尚未支援現有Flash檢視器目前提供的所有功能。 下列功能目前無法使用，但將納入未來版本：

* 多媒體檔案支援
* 比較模式（視訊和靜態）
* 篩選評論（視訊和靜態）
* 檢閱檔案中的超連結（靜態）
* 翻譯（視訊與靜態）
* 顯示目前處理校訂之使用者的存在狀態指標
* 共用校樣

如需有關在HTML5檢視器中校訂靜態校訂的詳細資訊，請參閱。

身為Workfront Proof中的Workfront管理員，您可以決定組織中的使用者是否擁有視訊校訂的新HTML5校訂檢視器的存取權。

## 新的甘特圖重新設計 {#new-gantt-chart-redesign}

新的甘特圖包含下列改善專案：

* 新圖示和標籤
* 放大和縮小特定時間範圍的新選項
* 圖表清單部分中的較小工作儲存格
* 重新設計設定、列印及切換至預計日期的選項。

如需有關在甘特圖設定選項的詳細資訊，請參閱[設定資訊在甘特圖上的顯示方式](../../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md)。 

## 內建報表包含更新的說明 {#built-in-reports-contain-updated-descriptions}

我們已更新Workfront中系統報表的說明，以包含報表型別和所含欄位的相關資訊。  

在此變更之前，我們大部分的內建報表都沒有說明，或是說明非常有限。

如需內建報表的詳細資訊，請參閱[使用Adobe Workfront內建報表](../../../../reports-and-dashboards/reports/using-built-in-reports/use-workfront-built-in-reports.md)。

## 匯出的報告、清單和儀表板中的品牌 {#branding-in-exported-reports-lists-and-dashboards}

>[!NOTE]
>
>此功能目前無法用於預覽環境中的所有叢集。

如果您在Workfront中運用品牌，則您在全域導覽列中使用的標誌現在包含在您從Workfront匯出的.pdf檔案中。

下列.pdf檔案將會在匯出的檔案中包含您組織的標誌：

* 匯出的清單
* 匯出和傳遞的報表
* 列印的報告面板

如需有關從Workfront匯出資料的詳細資訊，請參閱[匯出資料](../../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md)。

## 改進複製任務和移動任務或問題時的功能 {#improvements-when-copying-tasks-and-moving-tasks-or-issues}

我們已改善您複製任務或移動任務或問題的方式，讓您更輕鬆地為已複製或已移動的任務或問題選擇父級。 例如，在複製任務時選取父項時，您現在可以看到任務階層及其父項 — 子項關係，以及在具有大量任務的專案中搜尋父項。

在此變更之前，**選取父項**&#x200B;步驟中沒有搜尋欄位，而且任務清單中看不到任務的階層。

如需複製工作的詳細資訊，請參閱[複製和複製工作](../../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md)。

如需關於移動問題的詳細資訊，請參閱[移動問題](../../../../manage-work/issues/manage-issues/move-issues.md)。

## 在核准設定區域中重新呼叫請求的新組態 {#new-configuration-for-recalling-requests-in-the-approval-settings-area}

我們已在系統層級的「核准設定」區域引入新設定，可讓Workfront管理員決定是否應允許使用者召回第一個狀態為未決核准的問題或請求。 如果允許召回，則問題會被刪除；如果不允許召回，則當問題的第一個狀態為未決核準時，使用者無法看到召回按鈕。

在此變更之前，始終允許召回問題。 撤回核準時，核准被完全略過，將問題置於其第一個狀態，不附加核准。

如需核准設定的詳細資訊，請參閱[設定全域核准設定](../../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md)。 

>[!NOTE]
>
>此功能發行時，此選項預設為停用。 依預設，所有組織都會啟用目前回溯問題。 當此功能發行時，Workfront管理員必須手動啟用此設定，以保持功能在Workfront中的原樣。

## 資源預算時數報表的新群組：配置日期 {#new-grouping-for-resource-budgeted-hour-reports-allocation-date}

我們新增了在您建置資源預算時數報告時按「配置日期」將結果分組的功能。

在此變更之前，您可以在報表檢視中顯示「配置日期」，並在篩選中使用它，但您無法在分組中使用此欄位。

如需配置日期的詳細資訊，請參閱[Adobe Workfront術語表](../../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md)。

如需建立報告的詳細資訊，請參閱[建立自訂報告](../../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)。

## 資源規劃工具改善 {#resource-planner-improvements}

* [資源規劃工具：依FTE顯示資料](#resource-planner-show-data-by-fte)
* [資源規劃工具：依周和季顯示資料](#resource-planner-show-data-by-week-and-quarter)
* [資源規劃工具：依使用者檢視](#resource-planner-view-by-user)
* [資源規劃工具：拖放專案以建立優先順序](#resource-planner-drag-and-drop-projects-to-establish-priority)
* [資源規劃工具：將資源規劃工具中的資料匯出至Excel](#resource-planner-export-the-data-in-the-resource-planner-to-excel)

### 資源規劃工具：依FTE顯示資料 {#resource-planner-show-data-by-fte}

您現在可以在「資源規劃工具」中按FTE顯示資源的配置與可用性。 在此變更之前，您只能以小時顯示值。

如需有關使用資源規劃工具的詳細資訊，請參閱[資源規劃工具概觀](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md)。

### 資源規劃工具：按周和季度顯示資料 {#resource-planner-show-data-by-week-and-quarter}

您現在可以變更資源規劃工具的時間範圍間隔，以按周或季度檢視。 在此變更之前，您可以檢視資源的配置與可用性，並僅依月份編列預算。

如需有關使用資源規劃工具的詳細資訊，請參閱[資源規劃工具概觀](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md)。

### 資源規劃工具：依使用者檢視 {#resource-planner-view-by-user}

您現在可以在「資源規劃工具」中顯示資訊，先依使用者，然後依專案、角色及任務來進行。 您還可以顯示計畫和可用時數之間的差異，或使用者的FTE。 在此變更之前，您可以依專案和角色在資源規劃工具中顯示資訊。

如需有關使用資源規劃工具的詳細資訊，請參閱[資源規劃工具概觀](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md)。

### 資源規劃工具：拖放專案以建立優先順序 {#resource-planner-drag-and-drop-projects-to-establish-priority}

您現在可以依照所需的優先順序拖放專案。 在此變更之前，您只能透過手動指派數字來建立專案的優先順序。

如需有關使用資源規劃工具的詳細資訊，請參閱[資源規劃工具概觀](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md)。

### 資源規劃工具：將資源規劃工具中的資料匯出至Excel {#resource-planner-export-the-data-in-the-resource-planner-to-excel}

您現在可以將資源規劃工具中的資訊匯出至Excel檔案。

如需有關使用資源規劃工具的詳細資訊，請參閱[資源規劃工具概觀](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md)。

## 行動裝置改良 {#mobile-improvements}

我們已新增存取您的專案並從Workfront行動應用程式管理專案的功能。 您現在可以使用Workfront行動應用程式進行以下操作：

* 存取您的專案清單
* 存取專案中的任務和子任務清單
* 存取專案的問題清單
* 在專案上記錄新問題

您可以在更新Workfront行動應用程式時安裝此功能。 此更新將於2017年11月在Apple和Android行動商店推出。

## Workfront與Slack整合 {#workfront-integration-with-slack}

>[!NOTE]
>
>Slack整合目前無法使用。 2017年11月，它將可用於您的生產環境。

我們正在啟動Workfront與Slack之間的新整合。 如果貴組織已將Slack用於通訊，您現在可以將其與Workfront整合，並執行常見的Workfront動作，而不會將您的通訊管道留在Slack中。 您現在可以從Slack帳戶執行下列動作：

* 在Workfront中搜尋專案
* 存取您的工作和核准清單
* 建立任務
* 建立問題
* 從與您共用的連結訂閱該專案的任何專案
* 從與您共用的連結指派任務和問題給他們
* 核准您的工作
* 存取「我的最愛」和「最近使用的專案」清單

如需有關從Slack存取Workfront的詳細資訊，請參閱[將Workfront與Slack搭配使用。](https://support.workfront.com/hc/en-us/sections/115000458033)

## Outlook 365改良 {#outlook-365-improvements}

我們已對的Workfront增益集進行下列改進  Outlook 365：

* 在Workfront中新增任務或問題至專案：您現在可以使用Outlook 365增益集將電子郵件轉換成Workfront中的任務或問題。 在此程式中，您可以指定要新增任務或問題的專案，以及受指派人和到期日。 在此增強功能之前，您只能提交要求至要求佇列，或從Outlook 365將個人工作新增至您的[處理中]清單。 
* 在轉換為任務、問題或請求的原始電子郵件中保留Workfront物件的連結：當您從Outlook 365轉換電子郵件至任務、問題或請求時，Outlook 365會保留從原始電子郵件中轉換至任務或問題的連結。 在此變更之前，Outlook中不會指出電子郵件是否已轉換為任務或提交為請求。 

  如需有關將電子郵件從Outlook 365轉換為任務或問題的詳細資訊，請參閱[將Outlook電子郵件新增至專案做為任務或問題](../../../../workfront-integrations-and-apps/using-workfront-with-outlook/add-outlook-email-to-project-as-task-or-issue.md)。

## API變更 {#api-changes}

* [API 8現已可用](#api-8-now-available)
* [已移除且已棄用的API版本](#removed-and-deprecated-versions-of-the-api)
* [2017.3 Beta最終發行活動](#updated-message-format-for-event-subscriptions)
* [無法傳遞訊息的事件訂閱重試](#event-subscription-retries-for-undeliverable-messages)

### API 8現已推出 {#api-8-now-available}

Workfront API第8版現已可用，可為您的Workfront整合提供最新和更新的資源。

如需Workfront API變更清單，請參閱[API版本8](../../../../wf-api/api/new-api-version-8-updates.md)的更新。

### 已移除和已棄用的API版本 {#removed-and-deprecated-versions-of-the-api}

### 更新活動訂閱的訊息格式

為了提供您整合的更多實用資訊(包括Workfront事件訂閱API)，我們已包含與支援資源關聯的舊值和新值，以變更這些資源的傳出訊息格式。 為避免失敗，您使用Workfront事件訂閱API的任何整合都必須更新為新格式，如[事件訂閱API](../../../../wf-api/general/event-subs-api.md)所述。

### 無法傳遞訊息的事件訂閱重試 {#event-subscription-retries-for-undeliverable-messages}

Workfront事件訂閱架構現在提供機制，可處理無法傳送至客戶端點的事件觸發傳出訊息。 為確保訊息持續傳遞，客戶應確保正確設定任何使用事件訂閱傳出訊息的端點。 如需詳細資訊，請參閱[事件訂閱重試](../../../../wf-api/api/event-sub-retries.md)。
