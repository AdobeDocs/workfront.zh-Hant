---
content-type: release-notes
navigation-topic: product-releases-archive
title: 2018.2 Beta 5發行活動
description: 本頁說明2018.2 Beta 5版本預覽環境中最近可用的所有變更。 此功能將於2018年6月1日在預覽環境中提供。 Beta 5發行的校訂增強功能將於6月4日星期一在預覽環境中提供。 它將在2018年7月的生產環境中提供。
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 0a8602aa-34c8-44d0-a102-9497d106f806
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '3158'
ht-degree: 1%

---

# 2018.2 Beta 5發行活動

本頁說明2018.2 Beta 5版本預覽環境中最近可用的所有變更。 此功能將於2018年6月1日在預覽環境中提供。 Beta 5發行的校訂增強功能將於6月4日星期一在預覽環境中提供。 它將在2018年7月的生產環境中提供。

>[!IMPORTANT]
>
> 本頁所述的功能在生產環境使用之前可能會有所變更。

如需2018.2年度所有變更的清單，請參閱  [2018.2發行活動總覽](../../../../product-announcements/product-releases/quarterly-release-archive/2018.2-release-activity/2018-2-release-activity-overview.md)。

2018.2 Beta 5版本包含Workfront管理員和其他使用者的增強功能：

管理員的&#x200B;**&#x200B;**

* [檢視使用者觸發的變更及稽核記錄](#view-user-triggered-changes-with-audit-logs)
* [以群組管理員身分檢視授權資訊](#view-license-information-as-a-group-administrator)

**所有使用者**

* [首頁區域中的行事曆檢視](#calendar-view-in-the-home-area)
* 首頁[&#128279;](#additional-updates-to-the-work-list-left-panel-in-home)中工作清單（左側面板）的其他更新
* [設定自動資源排程的工作角色限制](#configure-job-role-limits-for-automated-resource-scheduling)
* 資源規劃工具中的[專案和角色檢視改善](#project-and-role-view-improvements-in-the-resource-planner)
* [調整專案清單的欄寬](#resize-column-widths-for-project-lists)
* 新專案清單的[圖示支援](#icon-support-for-the-new-project-lists)
* [在檔案檢視中新增「大型縮圖」欄位](#add-large-thumbnail-field-in-document-views)
* [增加Excel匯出限制](#increase-excel-export-limit)
* 專案清單的[快速篩選](#quick-filters-for-project-lists)
* 專案與任務報告中的[參考問題集合](#reference-issue-collections-in-project-and-task-reports)
* 在Workfront中新增檔案版本時，[新增更強大的版本功能表](#new-more-robust-version-menu-when-adding-new-document-versions-in-workfront)
* Android Beta行動應用程式中的[行動裝置改良](#mobile-improvements-in-the-android-beta-mobile-app)
* [校訂檢視器增強功能(Workfront和Workfront Proof)](#proofing-viewer-enhancements-workfront-and-workfront-proof)
* Workfront中的[校訂增強功能](#proofing-enhancements-in-workfront)
* [Workfront Proof中的校訂增強功能](#proofing-enhancements-in-workfront-proof)

## 首頁區域中的行事曆檢視 {#calendar-view-in-the-home-area}

現在您可以使用Workfront首頁行事曆檢視來管理您的個人工作任務和排程。 「首頁行事曆」檢視可讓您進行下列工作：

* 設定您自己的排程，以完成指派給您的Workfront任務
* 快速檢視即將到期或逾期的工作
* 檢視您一週的總分配時數
* 更新指派給您的任務

如果您使用Outlook中的行事曆，可以整合行事曆，以在[首頁行事曆]檢視中顯示Outlook事件。

## 首頁工作清單（左側面板）的其他更新 {#additional-updates-to-the-work-list-left-panel-in-home}

「首頁」區域的「工作清單」現在提供下列增強功能：

* 「篩選」下拉式&#39;a5&#39;5c能表的「已完成」選項旁現在會以括弧顯示已完成專案的數目。

  以前，已完成專案的數量不會顯示在篩選功能表中。 

* 系統會顯示前2週完成的專案。

  以前會顯示過去3個月的已完成專案。

  如需有關檢視首頁區域已完成工作的資訊，請參閱文章[首頁區域工作清單顯示專案](../../../../workfront-basics/using-home/using-the-home-area/display-items-in-home-work-list.md)首頁區域工作清單顯示專案[首頁區域工作清單](../../../../workfront-basics/using-home/using-the-home-area/display-items-in-home-work-list.md)。

* 新增持續時間欄位和指派欄位，以在首頁區域中選擇專案時顯示。

  以前，指派欄位預設可用；但是，如果刪除，則無法重新新增。 「持續時間」欄位先前無法新增。

  如需有關新增欄位至首頁區域的資訊，請參閱建立及管理版面配置範本。

如需有關使用主區域的詳細資訊，請參閱[使用主區域](../../../../workfront-basics/using-home/using-the-home-area/use-the-home-area.md)。

## 使用稽核記錄檢視使用者觸發的變更 {#view-user-triggered-changes-with-audit-logs}

我們已為Workfront管理員建立下列稽核記錄，以追蹤使用者觸發的變更：

* 使用者稽核記錄
* 存取層級稽核記錄
* 群組稽核記錄
* 登入嘗試稽核記錄

之前，無法追蹤系統內的變更。

如需詳細資訊，請參閱[檢視和匯出稽核記錄](../../../../administration-and-setup/add-users/create-and-manage-users/view-and-export-audit-logs.md)。

## 以群組管理員身分檢視授權資訊 {#view-license-information-as-a-group-administrator}

我們已建立唯讀授權頁面，讓群組管理員檢視他們所管理之群組的授權計數。

在此變更之前，群組管理員無法檢視授權資訊。

如需詳細資訊，請參閱[群組管理員](../../../../administration-and-setup/manage-groups/group-roles/group-administrators.md)。

## 設定自動資源排程的工作角色限制 {#configure-job-role-limits-for-automated-resource-scheduling}

>[!NOTE]
>
>已棄用資源排程工具，並已從Workfront的23.1版本中移除。 如需有關使用工作負載平衡器排程資源的資訊，請參閱[工作負載平衡器概覽](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md)。

在自動資源排程設定中，您現在可以將限制指派給工作角色。 這可讓您以相同的角色控制被指派工作的資源數量。

之前，您無法指定可將工作指派給某個工作角色中的幾個使用者。

如需詳細資訊，請參閱「在排程區域中手動指派未指派的任務和問題」。

## 資源規劃工具中的專案和角色檢視改善 {#project-and-role-view-improvements-in-the-resource-planner}

資源規劃工具的「專案」和「角色」檢視現在包含下列改進：

* 改善篩選條件，可從整個資料庫擷取資訊，而非僅擷取畫面上的資訊。
* 全熒幕模式。
* 現在效能更快、效率更高。

   * 可顯示的專案、角色和使用者數的新限制。
   * 延遲載入，可加快專案和角色的載入速度。

* 直接從資源規劃工具快速存取專案和使用者。
* 「專案檢視」中更快速的拖放功能，可排定專案的優先順序。

在這些改進之前，您報告資源規劃工具載入緩慢，並且您注意到顯示的資料中出現不一致。 透過這些改善功能，這些應該現已淘汰。

如需相關資訊，以及瞭解資源規劃工具的新限制，請參閱[資源規劃工具顯示限制](../../../../resource-mgmt/resource-planning/resource-planner-display-limitations.md)

<!--
<p dir="ltr" data-mc-conditions="QuicksilverOrClassic.Draft mode">To participate in our current beta program and give us feedback on the functionality of the Resource Planner, see <a href="../../../../product-announcements/betas/resource-planner-performance-beta.md" class="MCXref xref" xrefformat="{para}">Resource Planner performance beta </a></p>
-->

## 調整專案清單的欄寬 {#resize-column-widths-for-project-lists}

由於我們一直在努力改善清單的功能，因此暫時停用了調整下列專案清單中欄寬大小的功能：

* 我擁有的專案
* 我參與的專案
* 所有專案

在此版本中，我們現在可以再次調整所有專案清單的欄大小。

我們對此功能新增了額外的改善。

現在，當您拖曳欄的右邊框以調整其大小時，右邊的相鄰欄會保持其大小，使清單變寬，而不是同時被修改。 您也可以將欄的框線拖曳到相鄰欄的框線右側。

在此改進之前，調整大小欄右側的相鄰欄會按比例調整大小，以適合熒幕，而且您無法將欄的邊框拖曳過相鄰欄的右邊框。  

如需有關重新排序清單中資料行大小的資訊，請參閱[修改資料行寬度和順序](../../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md)。

若要參與我們目前的清單改進測試計畫，請參閱[新清單研究。](https://experienceleaguecommunities.adobe.com/t5/workfront/ct-p/workfront) （需要登入）

## 新專案清單的圖示支援 {#icon-support-for-the-new-project-lists}

由於我們一直在努力改善清單的功能，因此暫時停用了顯示下列專案清單中狀態圖示的功能：

* 我擁有的專案
* 我參與的專案
* 所有專案

在此版本中，專案的專案清單或專案清單中的其他物件可以再次顯示狀態圖示。

如需關於使用清單的資訊，請參閱[開始使用Adobe Workfront中的清單](../../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md)。

## 在檔案檢視中新增「大型縮圖」欄位 {#add-large-thumbnail-field-in-document-views}

我們將新增「大型縮圖」欄位至清單或報表中的檔案檢視。 在檔案檢視中選取時，此欄位會在清單或報告中顯示檔案的400畫素寬縮圖。

在此變更之前，您只能將「縮圖」欄位新增到檔案檢視，這會顯示檔案的33至66畫素寬縮圖。

如需有關清單與報表中欄位的資訊，請參閱[Adobe Workfront術語辭彙表](../../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md)。

## 增加Excel匯出限制 {#increase-excel-export-limit}

我們已提高您可以在Excel檔案中匯出多少列的限制。 您現在可以匯出下列內容：

* Excel .xls檔案中的65,000列
* Excel .xlsx檔案中的100,000列

從Workfront匯出下列專案時，將套用新限制：

* 來自網頁介面的清單或報告
* 使用API的清單或報告
* 排程和傳遞的報表

在此改善之前，您只能在任何Excel檔案中匯出50,000列。

如需有關從Workfront匯出資料的資訊，請參閱[匯出資料](../../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md)。

## 專案清單的快速篩選 {#quick-filters-for-project-lists}

您現在可以將快速篩選套用至清單。

快速篩選的用途是協助您直接導覽至大型清單中您認為重要的專案，讓您能夠快速檢閱、更新或與他人共用。

目前，快速篩選僅適用於以下子標籤中的專案清單：

* 我參與的專案
* 我擁有的專案
* 所有專案

如需快速篩選的詳細資訊，請參閱[開始使用Adobe Workfront](../../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md)中的清單中的「將快速篩選套用至清單」一節。

## 專案與任務報告中的參考問題集合 {#reference-issue-collections-in-project-and-task-reports}

您現在可以在專案或任務檢視及篩選中參考問題的集合。 您只能在建立報表時使用文字模式才能執行此操作。

在此改善之前，您只能在專案檢視或篩選中參考一組任務。

如需如何在報表中參考集合的相關資訊，請參閱[報表中的參考集合](../../../../reports-and-dashboards/reports/text-mode/reference-collections-report.md)。

如需有關使用文字模式的資訊，請參閱  [文字模式的常見使用概述](../../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md)。

>[!NOTE]
>
>在以下影片中，問題集合的範例文字模式不正確。 報表[&#128279;](../../../../reports-and-dashboards/reports/text-mode/reference-collections-report.md)中的參考集合中有正確的範例文字模式。

## 在Workfront中新增檔案版本時，新增更強大的版本選單 {#new-more-robust-version-menu-when-adding-new-document-versions-in-workfront}

現在，在Workfront中將新版本新增到檔案時，「新版本」選單會包含其他選項，而且現在在可新增新版本的Workfront區域間會保持一致。

您可以從Workfront的下列區域新增檔案版本：

* 從「檔案」標籤中的「更多」下拉式功能表。
* 從檔案詳細資訊頁面上的「檔案動作」功能表。
* 從檔案詳細資訊頁面上的「所有版本」索引標籤。

在此變更之前，只有「檔案」標籤中的「更多」下拉式選單包含新增新版本的所有選項。

「新版本」功能表中提供下列選項，供您新增新版本的所有區域使用：

* 校樣
* 僅文件
* 連結選項(來自Dropbox、來自Google Drive等)
* 從剪貼簿貼上（這是新增版本時的新選項）

如需詳細資訊，請參閱[從您的檔案系統新增檔案至Adobe Workfront](../../../../documents/adding-documents-to-workfront/add-documents-from-file-system.md)一文中的[從您的檔案系統新增檔案至Adobe Workfront](../../../../documents/adding-documents-to-workfront/add-documents-from-file-system.md)。

## Android Beta行動應用程式中的行動裝置改良 {#mobile-improvements-in-the-android-beta-mobile-app}

在此版本發佈後不久，行動應用程式的Android Beta版本將會提供下列改善功能：

* 撥動動作

  您可以透過在Workfront行動應用程式中滑動各種物件來執行活動，例如自願執行任務、完成任務、將通知標示為已檢視或新增、傳送文字或致電聯絡人。

  此功能已改善下列區域：

   * 我的工作和首頁
   * 通知
   * 連絡人
   * 核准

* 檢視專案的「詳細資訊」標籤時的新外觀

  在行動應用程式的Android Beta版本中檢視專案時，介面已變更，使其更易於編輯、完成或附加檔案。

* 記錄時間的新體驗

  記錄時間比以往更快速、更輕鬆，記錄時間按鈕更易於存取，而記錄時數介面更簡化。

在此版本中，這些改良功能僅適用於Workfront行動應用程式的Android Beta版本。 目前無法供iOS使用。

如需如何註冊成為測試版以及下載Android Beta版本的Workfront行動應用程式的詳細資訊，請參閱。

## 校訂檢視器增強功能(Workfront和Workfront Proof) {#proofing-viewer-enhancements-workfront-and-workfront-proof}

* [已更新列印摘要頁面](#updated-print-summary-page)
* [直接從校訂檢視器將使用者新增到校訂](#add-users-to-a-proof-directly-from-the-proofing-viewer)
* [在校訂檢視器中顯示所有標籤工具](#display-all-markup-tools-in-the-proofing-viewer)
* [在校訂檢視器中設定預設排序選項](#configure-default-sorting-options-in-the-proofing-viewer)
* [在案頭校訂檢視器中檢視Workfront檔案核准](#view-workfront-document-approvals-in-the-desktop-proofing-viewer)
* [設定在案頭校訂檢視器中開啟新標籤和視窗的連結](#configure-links-that-open-new-tabs-and-windows-to-open-within-the-desktop-proofing-viewer)
* 校訂檢視器中的[顯示狀態指標](#presence-indicator-in-the-proofing-viewer)
* [篩選註解以在案頭校訂檢視器中顯示互動式URL校訂的單一頁面](#filter-comments-to-display-a-single-page-for-interactive-url-proofs-in-the-desktop-proofing-viewer)
* [靜態與視訊內容的案頭校訂檢視器](#desktop-proofing-viewer-for-static-and-video-content)
* [新增自訂裝置至您的系統](#add-custom-devices-to-your-system)

### 已更新列印摘要頁面 {#updated-print-summary-page}

「列印摘要」頁面已更新，具有新的外觀和風格，並改善功能。

如需詳細資訊，請參閱[在Adobe Workfront中列印校訂摘要](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/print-proof-summary-in-wf.md)。

### 直接從校訂檢視器將使用者新增到校訂 {#add-users-to-a-proof-directly-from-the-proofing-viewer}

現在，您可以直接從「網頁校訂檢視器」和「案頭校訂檢視器」將使用者新增到校訂中。 

之前，您無法將個別使用者新增到校樣中。 您只能複製公開URL或內嵌程式碼。

如需詳細資訊，請參閱文章中的[新增使用者以共用校訂](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/share-a-proof-in-proofing-viewer.md#sharing-with-individual-users)  [從校訂檢視器共用校訂](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/share-a-proof-in-proofing-viewer.md)。

### 在校訂檢視器中顯示所有標籤工具 {#display-all-markup-tools-in-the-proofing-viewer}

您現在可以將標示工具設定為隨時顯示，而不是在必須開啟的功能表中顯示。 如此可讓您更快速地切換工具。 以這種方式設定時，標籤工具會水準地顯示在網頁校訂檢視器和案頭校訂檢視器的頂端。

以前，標籤工具只能在下拉式選單中使用。

如需有關設定此標籤設定的詳細資訊，請參閱[設定校訂檢視器設定](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/configure-proofing-viewer-settings.md)。

如需在檢閱校樣時使用標籤選項的詳細資訊，請參閱文章中的。

### 在校訂檢視器中設定預設排序選項 {#configure-default-sorting-options-in-the-proofing-viewer}

現在，當您變更校訂中評論清單的排序選項時，該選項會在您下次在網頁校訂檢視器或案頭校訂檢視器中開啟任何校訂時成為預設排序選項。 

如需詳細資訊，請參閱文章中的。

### 在案頭校訂檢視器中檢視Workfront檔案核准 {#view-workfront-document-approvals-in-the-desktop-proofing-viewer}

現在，您可以在案頭校訂檢視器中做出Workfront檔案核准決定。

之前，只有網頁校訂檢視器可讓您作出Workfront檔案核准決定。 

如需詳細資訊，請參閱  [在文章的校訂檢視器中對校訂做出決定](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md)  [在校訂檢視器中對校訂做出決定](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md)。

### 設定在案頭校訂檢視器中開啟新標籤和視窗的連結 {#configure-links-that-open-new-tabs-and-windows-to-open-within-the-desktop-proofing-viewer}

在案頭校訂檢視器中校訂互動式內容時，您現在可以設定在新標籤或新視窗中開啟的連結，以便在案頭校訂檢視器中開啟，以便您可以繼續校訂。

在舊版校訂檢視器中，在新標籤或新視窗中開啟的連結無法在校訂檢視器中檢閱。

如需詳細資訊，請參閱[設定校訂檢視器設定](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/configure-proofing-viewer-settings.md)。

### 校訂檢視器中的顯示狀態指示器 {#presence-indicator-in-the-proofing-viewer}

現在，當在網路校訂檢視器或案頭校訂檢視器中檢視校訂時，您可以檢視目前檢視校訂的每個使用者的頭像都顯示在校訂檢視器的右上角。

如需詳細資訊，請參閱[與多位檢閱者同時檢閱校訂](../../../../workfront-proof/wp-work-proofsfiles/review-proofs-wpv/review-proof-with-multiple-reviewers.md)。

### 篩選註解以在案頭校訂檢視器中顯示互動式URL校訂的單一頁面 {#filter-comments-to-display-a-single-page-for-interactive-url-proofs-in-the-desktop-proofing-viewer}

在案頭校訂檢視器中檢閱互動式校訂中的URL時，您現在可以篩選註解，以顯示僅於目前頁面上所做的註解。 

在此變更之前，此選項僅適用於靜態校樣。

如需詳細資訊，請參閱文章中的。

### 靜態與視訊內容的案頭校訂檢視器 {#desktop-proofing-viewer-for-static-and-video-content}

案頭校訂檢視器現在支援靜態和視訊內容。

先前僅支援互動式內容。

如需有關設定要在案頭校訂檢視器中開啟的靜態與視訊校訂的資訊，請參閱[設定校訂檢視器設定](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/configure-proofing-viewer-settings.md)。

如需案頭校訂檢視器的詳細資訊，請參閱[在案頭校訂檢視器中檢閱校訂。](https://support.workfront.com/hc/en-us/sections/360000686434)

### 新增自訂裝置至您的系統 {#add-custom-devices-to-your-system}

您現在可以新增任何自訂裝置到您的系統，讓使用者檢閱互動式內容並模擬其在案頭校訂檢視器中檢閱校訂時特定裝置上的顯示方式。

在此變更之前，使用者只能從標準、預先設定的裝置清單中進行選擇。

如需關於新增自訂裝置的資訊，請參閱中的

如需有關使用者在檢閱互動式內容時如何選取裝置的資訊，請參閱[在校訂檢視器中變更互動式校訂解析度](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/view-interactive-content-as-it-appears-in-device.md)。

## Workfront中的校訂增強功能 {#proofing-enhancements-in-workfront}

* [直接從Workfront共用校訂連結](#share-the-proof-link-directly-from-workfront)
* [報告Workfront中的其他校訂資料](#report-on-additional-proofing-data-in-workfront)
* [在Workfront中檢視校訂核准的歷史資料](#view-historical-data-for-proof-approvals-in-workfront)

### 直接從Workfront共用校訂連結 {#share-the-proof-link-directly-from-workfront}

現在您可以在Workfront中產生校訂連結，並直接從Workfront共用。 或者，您可以複製URL並使用替代方法將其散佈。

在此變更之前，您只能在Workfront中複製校樣連結，並使用替代方法進行分發。

如需詳細資訊，請參閱文章[在Adobe Workfront中共用校訂](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md)中的[在Adobe Workfront中共用校訂](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md)。

>[!NOTE]
>
>目前可用的內嵌連結將在未來版本中移除。 您仍可透過Workfront API存取內嵌連結。

### 報告Workfront中的其他校訂資料 {#report-on-additional-proofing-data-in-workfront}

在包含檔案版本物件的報告中（例如檔案版本報告和校訂核准報告），現在有多個欄位可供您檢視其他校訂資訊。

* 校訂期限

  顯示校訂截止日期的一週中的某天、日期、一天中的時間和年份。

* 校訂決策

  顯示校訂的決策狀態（待定、需要變更或已核准）。

* 校樣名稱

  顯示校訂名稱。

* 校樣頁面

  顯示校訂中包含的頁數。

* 校訂進度

  顯示校訂的進度狀態（已傳送、已開啟、已評論、已作出決定）。

如需這些欄位的詳細資訊，請參閱  [Adobe Workfront術語辭彙表](../../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md)。

### 在Workfront中檢視校訂核准的歷史資料 {#view-historical-data-for-proof-approvals-in-workfront}

在校訂核准報告中，您可以新增欄位，讓您檢視不再有效的校訂的校訂核准決定。 若要這麼做，請將「核准者決定」欄位新增至您的報表。

在此變更前，在對校訂做出決定後，該決定無法再顯示在Workfront報告中。

如需詳細資訊，請參閱  [Adobe Workfront術語辭彙表](../../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md)。

## Workfront Proof中的校訂增強功能 {#proofing-enhancements-in-workfront-proof}

* [直接從校訂檢視器(Workfront Proof)建立新版本的校訂](#create-a-new-version-of-a-proof-directly-from-the-proofing-viewer-workfront-proof)
* [校訂檢視器和案頭校訂檢視器(Workfront Proof)中的新校訂詳細資訊連結](#new-proof-details-link-in-the-proofing-viewer-and-desktop-proofing-viewer-workfront-proof)

### 直接從校訂檢視器(Workfront Proof)建立新版本的校訂 {#create-a-new-version-of-a-proof-directly-from-the-proofing-viewer-workfront-proof}

在Workfront Proof中校訂時，您現在可以直接從新的校訂檢視器和案頭校訂檢視器建立新版本的校訂。

以前，此選項只能在舊版Flash Viewer中使用。

如需詳細資訊，請參閱文章中的[在Workfront Proof中複製校樣](../../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/copy-proofs.md)  [在Workfront Proof中複製校樣](../../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/copy-proofs.md)。

### 校訂檢視器和案頭校訂檢視器(Workfront Proof)中的新校訂詳細資訊連結 {#new-proof-details-link-in-the-proofing-viewer-and-desktop-proofing-viewer-workfront-proof}

在校訂檢視器中檢視校訂時，Workfront Proof使用者現在可以快速前往Workfront Proof中的校訂詳細資訊頁面。

如需詳細資訊，請參閱「檢視校訂詳細資訊」。
