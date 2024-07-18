---
content-type: release-notes
navigation-topic: product-releases-archive
title: 2018.3 Beta 5發行活動
description: 本頁說明2018.3 Beta 5版本預覽環境中最近可用的所有變更。 此功能將於2018年9月21日在預覽環境中提供。 它將於2018年11月在生產環境中提供。
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: f208b566-2529-4c4d-aa66-0c8756e55a5a
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '2147'
ht-degree: 0%

---

# 2018.3 Beta 5發行活動

本頁說明2018.3 Beta 5版本預覽環境中最近可用的所有變更。 此功能將於2018年9月21日在預覽環境中提供。 它將於2018年11月在生產環境中提供。

如需2018.3年所有變更的清單，請參閱  [2018.3發行活動總覽](../../../../product-announcements/product-releases/quarterly-release-archive/2018.3-release-activity/2018-3-release-activity-overview.md)。

2018.3 Beta 5版本包含適用於所有使用者的增強功能：

* [追蹤您已在主區域提交的核准](#track-approvals-you-ve-submitted-in-the-home-area)
* [取代Workfront中的Flash工具](#replacement-of-flash-based-tools-in-workfront)
* [允許工作授權使用者存取專案的排程子標籤](#allowing-work-license-users-to-access-the-scheduling-subtab-of-a-project)
* [資源規劃工具中的已改良篩選器](#improved-filters-in-the-resource-planner)
* [在資源規劃工具中檢視實際時數](#view-actual-hours-in-the-resource-planner)
* 業務案例匯出中的[資源規劃工具資料](#resource-planner-data-in-the-business-case-export)
* [啟用公司層級收費率覆寫](#enable-company-level-billing-rate-override)
* [簡化角色型核准](#simplified-role-based-approvals)
* [使用率報告：從新資源預算區域填入預算時數](#utilization-report-populates-budgeted-hours-from-new-resource-budgeting-area)
* [使用率報告：檢視專案上按使用者的預算時數](#utilization-report-view-budgeted-hours-by-user-on-a-project)
* 校訂檢視器中不再支援[SWF檔案](#swf-files-no-longer-supported-in-the-proofing-viewer)
* 在校訂檢視器的註解清單中更快速地存取[動作](#actions-more-quickly-accessible-in-the-comment-list-in-the-proofing-viewer)
* [校訂檢視器中的校訂共用改善](#proof-sharing-improvement-in-the-proofing-viewer)
* 校訂檢視器中的[註解清單增強功能](#comments-list-enhancements-in-the-proofing-viewer)
* [在校訂檢視器中縮放和平移視訊校訂](#zoom-and-pan-video-proofs-in-the-proofing-viewer)
* 校訂檢視器中的[較亮背景](#lighter-background-in-the-proofing-viewer)
* [當在校訂檢視器中編輯評論時，能有更好的可見度](#better-visibility-when-a-comment-has-been-edited-in-the-proofing-viewer)
* [在校訂檢視器的註解清單中檢視與動作關聯的註解數](#view-the-number-of-comments-associated-with-an-action-in-the-comment-list-in-the-proofing-viewer)
* [將使用者新增到校訂檢視器中的校訂時指定階段](#specify-the-stage-when-adding-users-to-a-proof-in-the-proofing-viewer)
* [從互動式或靜態網站校訂開啟關聯的網站](#opening-the-associated-website-from-an-interactive-or-static-website-proof)
* [列印摘要增強功能](#print-summary-enhancements)
* [改善的校訂載入時間](#improved-proof-loading-time)
* [Workfront行動應用程式中更新標籤的新外觀](#new-look-and-feel-of-the-updates-tab-in-the-workfront-mobile-app)

## 追蹤您已在首頁區域中提交的核准 {#track-approvals-you-ve-submitted-in-the-home-area}

您現在可以使用「首頁」區域與您提交給其他使用者的核准互動。

從首頁，您可以：

* 撤回核准
* 提醒使用者核准
* 將使用者新增至檔案核准
* 檢視校訂核准

  以前，您只能在「我的工作」區域與已提交的核准互動。 

如需詳細資訊，請參閱[管理核准](../../../../review-and-approve-work/manage-approvals/manage-approvals.md)。 

## 取代Workfront中的Flash型工具 {#replacement-of-flash-based-tools-in-workfront}

所有依賴Flash技術的功能預計會在2018.3版中從Workfront移除，並更換為新解決方案。

如需受移除這些功能影響之所有區域的詳細資訊，以及瞭解哪些工具會取代這些功能，請參閱[在Adobe Workfront中取代Flash型工具](../../../../product-announcements/announcements/announcement-archive/replace-flash-tools.md)。

## 允許工作授權使用者存取專案的「排程」子標籤 {#allowing-work-license-users-to-access-the-scheduling-subtab-of-a-project}

擁有工作授權的使用者現在可以存取專案的「人員配置」標籤下的「排程」子標籤。

在此增強功能之前，只有擁有計畫授權的使用者才能存取此子標籤。

如需有關存取專案的「排程」子標籤所需存取權的資訊，請參閱「開始使用資源排程」。

>[!NOTE]
>
>已棄用資源排程工具，並已從Workfront的23.1版本中移除。 如需有關使用工作負載平衡器排程資源的資訊，請參閱[工作負載平衡器概覽](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md)。

## 改善資源規劃工具中的篩選器 {#improved-filters-in-the-resource-planner}

您現在可以篩選資源規劃工具中的資訊，以包含專案特定和使用者特定欄位，包括自訂欄位。

在此改善之前，您只能在資源規劃工具中篩選有限數量的內建欄位和條件。

如需有關在資源規劃工具中篩選資訊的資訊，請參閱資源規劃工具中的[篩選資訊](../../../../resource-mgmt/resource-planning/filter-resource-planner.md)。

## 在資源規劃工具中檢視實際時數 {#view-actual-hours-in-the-resource-planner}

您可以在資源規劃工具的使用者檢視中檢視實際時數。

在此改善之前，實際時數未顯示在資源規劃工具。

如需有關在資源規劃工具中檢視時數資訊的資訊，請參閱[資源規劃工具概觀](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md)。

## 業務案例匯出中的資源規劃工具資料 {#resource-planner-data-in-the-business-case-export}

當您將「業務案例」匯出至PDF時，匯出的檔案中的財務資訊現在會反映「資源預算」區域和「資源規劃工具」中的資訊。 

先前，匯出的檔案會反映舊版資源估算區域和Capacity Planner中的資訊。 

如需有關匯出業務案例的資訊，請參閱[為專案建立業務案例](../../../../manage-work/projects/define-a-business-case/create-business-case.md)中的[為專案建立業務案例](../../../../manage-work/projects/define-a-business-case/create-business-case.md)區段。

## 啟用公司層級收費率覆寫 {#enable-company-level-billing-rate-override}

您現在可以啟用允許公司層級收費率覆寫專案層級收費率的選項。 在公司層級更新計費率後，您可以手動重新計算專案的財務以反映這些變更。

如果啟用此設定，公司層級的收費率會覆寫專案上的歷史職務角色費率。

以前，除非您將公司從專案中移除，然後重新附加，否則無法將公司層級的計費率變更套用至專案。

如需詳細資訊，請參閱[以公司層級的收費率覆寫專案層級的收費率](../../../../manage-work/projects/project-finances/override-project-level-with-company-level-billing-rates.md)。 

## 簡化的角色型核准 {#simplified-role-based-approvals}

角色型核准現在僅在專案上運作。 現在，使用者必須指派給專案團隊，並在其使用者設定檔中指派角色，以檢視指派給其主要或次要角色的核准。

之前，您必須將使用者指派給專案團隊，確保他們在使用者設定檔中具有正確的角色，並在舊版團隊建立器中選取該角色。

如需詳細資訊，請參閱文章[專案團隊概述](../../../../manage-work/projects/planning-a-project/project-team-overview.md)中的[專案團隊概述](../../../../manage-work/projects/planning-a-project/project-team-overview.md)一節。

## 使用率報表：從新資源預算區域植入預算時數 {#utilization-report-populates-budgeted-hours-from-new-resource-budgeting-area}

>[!NOTE]
>
> 2018.2發行版本首次將此功能引入預覽環境。 它將在2018.3版本中發佈到生產環境。 

使用率報表中的預算時數現在會從業務案例的新資源預算區域可用的資訊植入。

在此變更之前，使用來自舊版資源估計區域的資訊。

如需詳細資訊，請參閱  [文章中的資源使用率報告概觀](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md)  [資源使用率報告概觀](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md)。

## 使用率報表：依使用者檢視專案的預算時數 {#utilization-report-view-budgeted-hours-by-user-on-a-project}

>[!NOTE]
>
>2018.2發行版本首次將此功能引入預覽環境。 它將在2018.3版本中發佈到生產環境。 

專案的「使用率」報告現在會依使用者顯示預算時數。

在此變更之前，「使用率」報告僅依工作角色顯示「預算時數」。 

如需詳細資訊，請參閱  [文章中的資源使用率報告概觀](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md)  [資源使用率報告概觀](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md)。

## 校訂檢視器不再支援SWF檔案 {#swf-files-no-longer-supported-in-the-proofing-viewer}

由於AdobeFlash的相關安全性問題，校訂檢視器不再支援從SWF檔案建立的校訂。 如果您開啟先前為SWF檔案建立的校訂，則會顯示一則訊息，指出校訂內容先前顯示在校訂檢視器中。 您可以在校訂上看到任何評論。 您也可以下載註解及下載原始SWF檔案。

如需詳細資訊，請參閱文章[支援的校訂檔案型別和大小限制概述](../../../../review-and-approve-work/proofing/proofing-overview/supported-proofing-file-types.md)中的[支援的校訂檔案型別和大小限制概述](../../../../review-and-approve-work/proofing/proofing-overview/supported-proofing-file-types.md)。 

## 可在校訂檢視器的「註解清單」中更快速地存取動作 {#actions-more-quickly-accessible-in-the-comment-list-in-the-proofing-viewer}

您現在可以在校訂檢視器中更快速地新增或變更註解的動作。 只需按一下任何評論上的「更多」圖示，然後在下拉式選單中按一下您想要的動作即可。

之前，您必須開啟註解、開啟下拉式功能表、開啟子功能表，然後按一下您想要的動作。

如需詳細資訊，請參閱[對校訂評論使用動作](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/use-actions-on-comments-in-viewer.md)。

## 校訂檢視器中的校訂共用改善 {#proof-sharing-improvement-in-the-proofing-viewer}

當您從校訂檢視器傳送URL時，顯示的選項現在會依照您從「檔案」區域共用URL時看到的選項組織。

以前，這些選項提供的功能與現在相同，但其組織與「檔案」清單中的對應選項不一致。

如需詳細資訊，請參閱區段  [分享文章中的URL](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/share-a-proof-in-proofing-viewer.md#sharing-the-url)  [從校訂檢視器共用校訂](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/share-a-proof-in-proofing-viewer.md)。

## 校訂檢視器中的「註解清單」增強功能 {#comments-list-enhancements-in-the-proofing-viewer}

「註解」清單中現在提供下列改良功能：

* 現在，淺灰色背景會出現在註解文字後面，使其與「註解」面板中出現的其它文字明顯不同，例如稽核者姓名、稽核時間和校訂頁碼。 唯有如此，您才想閱讀校訂意見反應，唯有如此，才能更輕鬆地進行閱讀。

  之前，「註解」面板的整個背景為白色。

  如需詳細資訊，請參閱。

* 評論的回覆現在會縮排在評論下。 這樣可讓您更輕鬆地區分回覆與其上方的原始評論。

  之前，評論底下的回覆會與評論靠左對齊。

  如需詳細資訊，請參閱中的。

* 當您解析校訂檢視器中的註解時，綠色的「已解析」核取記號圖示會出現，且註解右上角沒有任何文字。 這可以讓「註解」面板外觀更乾淨，更容易掃描您需要的資訊。

  以前，「已解決」核取記號圖示會出現在註解左上角的「已解決」一詞旁 

  如需詳細資訊，請參閱中的。

## 在校訂檢視器中縮放和平移視訊校訂 {#zoom-and-pan-video-proofs-in-the-proofing-viewer}

現在您可以放大視訊校樣，並將其平移至需要更仔細檢查的校樣區域。

## 校訂檢視器中的較亮背景 {#lighter-background-in-the-proofing-viewer}

校訂檢視器的背景現在會稍微變亮。 此變更可讓您更容易區分包含黑色背景和邊緣的校訂內容。

之前，校訂檢視器背景為黑色。

## 在校訂檢視器中編輯註解時提升可見度 {#better-visibility-when-a-comment-has-been-edited-in-the-proofing-viewer}

「已編輯」標籤現在會出現在稽核者已變更的任何評論上。 當您將滑鼠移到它上面時，會顯示檢閱者的名稱和變更的日期。

## 在校訂檢視器的「註解清單」中檢視與動作關聯的註解數 {#view-the-number-of-comments-associated-with-an-action-in-the-comment-list-in-the-proofing-viewer}

按一下「註解」清單中的「篩選」圖示，您現在可以看到與每個動作相關聯的註解數。

唯有為您的組織啟用動作，才可在「註解」清單中看到這些動作。

## 在校訂檢視器中指定將使用者新增到校訂時的階段 {#specify-the-stage-when-adding-users-to-a-proof-in-the-proofing-viewer}

當您將檢閱者新增到在校訂檢視器中具有自動化工作流程的校訂時，您可以指定您希望檢閱者處理校訂的階段。 這就像您將使用者新增到校訂檢視器以外的校訂時可用的功能。

先前，當您從校訂檢視器將檢閱者新增至校訂時，Workfront會將他們放置在目前作用中的階段。

如需詳細資訊，請參閱[分享校訂檢視器](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/share-a-proof-in-proofing-viewer.md)的校訂[透過新增使用者來分享校訂](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/share-a-proof-in-proofing-viewer.md#sharing-with-individual-users)。

## 從互動或靜態網站校訂開啟關聯的網站 {#opening-the-associated-website-from-an-interactive-or-static-website-proof}

當您檢閱包含互動或靜態網頁內容的校訂時，您現在可以按一下按鈕，以在校訂檢視器的新瀏覽器索引標籤中輕鬆開啟相關網站。 這可讓您使用兩個不同的索引標籤，將您在校樣中看到的內容與實際網站進行比較。

過去，只要將游標暫留在URL上，並按一下工具提示，即可開啟相關網站。 此方法容易存取且直覺。

## 列印摘要增強功能 {#print-summary-enhancements}

「列印摘要」頁面現在提供下列改善功能：

* 現在，您可以指定是否要在校樣中包含所有頁面，或僅包含評論的頁面。

  之前，您只能包含包含註釋的頁面。

* 如果您的校訂有階段，您現在可以包含圖表，顯示校訂階段的順序以及為每個階段作出的決定。

  之前無法使用此圖表。

* 現在，當多個標示與一個註解相關聯時，該註解的編號會顯示在「列印摘要」頁面的每個標示上。

  以前，評論編號只出現在與評論相關的第一個標籤上。 註解的其他標示顯示時沒有數字。

* 如果校訂是網頁擷取，則任何包含評論的頁面都會顯示擷取網頁的解析度。 例如，如果校樣包含行動裝置擷取的頁面，以及筆記型電腦和桌上型電腦擷取的相同頁面，則這項功能會很有幫助。
* 現在，當您按「動作」、「作者」或「未解決」狀態來篩選「列印摘要」頁面中的註解時，您的篩選器會套用至您匯出為PDF或Excel檔案的校樣，而不僅僅是列印的校樣。

如需詳細資訊，請參閱[在Adobe Workfront中列印校訂摘要](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/print-proof-summary-in-wf.md)。

## 改善的校訂載入時間 {#improved-proof-loading-time}

我們已進行一些效能改善，應該會導致開啟校樣時的載入時間改善。

如需開啟校訂的相關資訊，請參閱。

## Workfront行動應用程式中更新標籤的新外觀 {#new-look-and-feel-of-the-updates-tab-in-the-workfront-mobile-app}

行動應用程式上「更新」標籤的外觀和操作方式現已更新。 此項改善目前僅適用於Android的Workfront Beta版應用程式。

如需在Workfront行動應用程式中管理更新和評論的詳細資訊，請參閱區段  中的。
