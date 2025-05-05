---
content-type: release-notes
navigation-topic: product-releases-archive
title: 2017.2 Beta 3發行活動
description: 本頁說明2017.2 Beta 2版本預覽環境中所有可用的變更。 此頁面的功能已於2017年5月24日在預覽環境中推出。 它將在2017年7月底到8月初期間在生產環境中可用。
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 9647f3c6-f287-426c-a5e7-eb33b8b22a34
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '1387'
ht-degree: 0%

---

# 2017.2 Beta 3發行活動

本頁說明2017.2 Beta 2版本預覽環境中所有可用的變更。 此頁面的功能已於2017年5月24日在預覽環境中推出。 它將在2017年7月底到8月初期間在生產環境中可用。

>[!IMPORTANT]
>
>本頁所述的功能在生產環境使用之前可能會有所變更。

如需2017.2年度所有變更的清單，請參閱[2017.2年度發行活動概觀](../../../../product-announcements/product-releases/quarterly-release-archive/2017.2-release-activity/2017-2-release-activity-overview.md)。

2017.2 Beta 2版本包含適用於Workfront管理員和其他使用者的增強功能：

管理員的&#x200B;**：**

* [正在從資源回收筒大量還原專案](#restoring-items-in-bulk-from-the-recycle-bin)
* [使用者資訊會從Workfront同步到ProofHQ (ProofHQ和Workfront)](#user-information-is-synchronized-from-workfront-to-proofhq-proofhq-and-workfront)

所有使用者的&#x200B;**：** 

* [檢視訂閱的使用者](#view-subscribed-users)
* [設定里程碑在甘特圖上的顯示方式](#configure-how-milestones-are-displayed-on-the-gantt-chart)
* 匯出至PDF時[包含甘特圖圖例](#include-the-gantt-chart-legend-when-exporting-to-pdf)
* [在我的工作區(Workfront)中檢視校訂核准](#view-proof-approvals-in-the-my-work-area-workfront)
* 從我的工作區域(Workfront)處理校訂核准請求時[檢視使用者名稱](#view-user-names-when-addressing-proofing-approval-requests-from-the-my-work-area-workfront)
* [已改善視訊校訂的校訂檢視器(ProofHQ和Workfront)](#improved-proofing-viewer-for-video-proofs-proofhq-and-workfront)
* [以替代解析度(ProofHQ和Workfront)檢視多媒體校樣](#view-rich-media-proofs-in-alternate-resolutions-proofhq-and-workfront)
* [檔案版本報告(Workfront)中的新「校訂建立者」物件](#new-proof-creator-object-in-document-version-report-workfront)
* [新的資源集區功能暫時從預覽移除](#new-resource-pool-functionality-temporarily-removed-from-preview)

## 正在從資源回收筒大量還原專案 {#restoring-items-in-bulk-from-the-recycle-bin}

您現在一次最多可以還原10個已刪除的專案、任務、問題或檔案。

在此變更之前，您一次只能還原一個已刪除的專案。

如需還原專案的詳細資訊，請參閱[還原已刪除的專案](../../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md)。

## 檢視訂閱的使用者 {#view-subscribed-users}

您現在可以透過展開訂閱連結旁顯示的訂閱者數目，來檢視誰訂閱了專案。

在此增強功能之前，您無法檢視誰訂閱了任何專案。

如需訂閱專案的詳細資訊，請參閱[在Adobe Workfront中訂閱專案](../../../../workfront-basics/using-notifications/subscribe-to-items-in-workfront.md)。 

## 設定里程碑在甘特圖上的顯示方式 {#configure-how-milestones-are-displayed-on-the-gantt-chart}

在甘特圖中，現在有兩個檢視里程碑資訊的選項。 您可以設定下列其中一個或兩個里程碑指標：

* 里程碑菱形（圖示）

  此圖示會顯示在甘特圖中與里程碑相關聯的任何任務之後。

* 里程碑線

  任何與里程碑相關聯的任務之後會顯示一條線，橫跨甘特圖中的所有任務。

在此變更之前，只有一個選項可讓里程碑顯示在甘特圖上，稱為「里程碑」。 此選項會同時啟用里程碑菱形圖示和里程碑線。 無法分隔這些指標。

如需有關設定資訊在甘特圖中的顯示方式的詳細資訊，請參閱[設定資訊在甘特圖上的顯示方式](../../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md)。

## 匯出為PDF時包含甘特圖圖例 {#include-the-gantt-chart-legend-when-exporting-to-pdf}

現在，當您將「甘特圖」匯出至PDF時，可以選取是否要同時匯出圖表的圖例以及圖表本身。 圖例中包含的專案只是您已啟用在UI的甘特圖中顯示之選項。 如果這些選項存在於專案上的任務中，則會包含在圖例中。 例如，如果您啟用在甘特圖中顯示里程碑，圖例也會顯示里程碑，但前提是至少有一個工作與里程碑關聯。

在此變更之前，您無法從匯出的PDF中排除圖例，並且該圖例包含甘特圖的所有可能選項和標籤，無論這些選項和標籤在UI中是已啟用還是存在。

如需有關匯出甘特圖的詳細資訊，請參閱[將甘特圖匯出至PDF](../../../../manage-work/gantt-chart/use-the-gantt-chart/export-gantt-chart-to-pdf.md)。

## 使用者資訊會從Workfront同步到ProofHQ (ProofHQ和Workfront) {#user-information-is-synchronized-from-workfront-to-proofhq-proofhq-and-workfront}

現在於Workfront中建立或更新使用者時，使用者資訊（名稱和電子郵件）會從Workfront同步至ProofHQ。 

如需有關使用者從Workfront同步到ProofHQ的詳細資訊，請參閱。

## 檔案版本報告(Workfront)中的新「校訂建立者」物件

{#new-proof-creator-object-in-document-version-report-workfront}

現在，建立檔案版本報告時，會有新的校訂建立者物件。 此物件可讓您報告有關建立校訂之使用者的資訊。 

「檔案版本」報表中的新「校訂建立者」物件包含其他物件報表型別中現有使用者物件可用的所有欄位。

>[!NOTE]
>
> 此報表中提供的資訊，僅限於此功能首次引進至個別預覽或生產環境時的資訊；此報表中提供的資訊，不適用引進此功能之前有關請求者物件的資訊。

建立檔案版本報告時，您可以存取校訂建立者物件，如[建立自訂報告](../../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)中所述。

如需有關「檔案版本物件」報表的詳細資訊，請參閱[瞭解Adobe Workfront中的物件](../../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md)中的[瞭解Adobe Workfront中的物件](../../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md)一節。

## 在我的工作區域中(Workfront)檢視校訂核准 {#view-proof-approvals-in-the-my-work-area-workfront}

您提交供核准的所有校訂核准現在都顯示在「我的工作」區域中「我已提交供核准的工作」**&#x200B;**&#x200B;索引標籤中。

在此變更之前，我已提交核准的&#x200B;**工作**&#x200B;索引標籤不包含校訂核准。

只有在符合以下條件時，才會顯示校訂核准：

* 核准目前正在等候核准
* 核准流程會指派給具有授權Workfront使用者的使用者(不會顯示指派給未授權Workfront使用者的核准流程)
* 核准處理是在此功能發行後啟動（不會顯示發行此功能之前啟動的核准處理）

如需詳細資訊，請參閱[檢視核准](../../../../review-and-approve-work/manage-approvals/view-approvals.md)中的[檢視核准](../../../../review-and-approve-work/manage-approvals/view-approvals.md)。

## 從「我的工作區」(Workfront)處理校訂核准請求時檢視使用者名稱 {#view-user-names-when-addressing-proofing-approval-requests-from-the-my-work-area-workfront}

現在，當從「我的工作」區域核准校訂核準時，現在顯示請求核准的使用者名稱。

如需詳細資訊，請參閱[核准工作](../../../../review-and-approve-work/manage-approvals/approving-work.md)中的[核准工作](../../../../review-and-approve-work/manage-approvals/approving-work.md)。 

## 改善視訊校訂的校訂檢視器(ProofHQ和Workfront) {#improved-proofing-viewer-for-video-proofs-proofhq-and-workfront}

Workfront和ProofHQ中的校訂檢視器已更新為全新的外觀、可提升效能的HTML5架構，並支援新功能。

新的校訂檢視器包含下列改善專案：

* 逐格校訂
* 視訊緩衝
* 評論清單中的搜尋功能
* 在註解上設定的任何動作都會顯示在「註解清單」的每個註解上
* 全熒幕模式
* 以更快或更慢的速度檢閱內容
* 新增評論和回覆時的拼字檢查程式

### 預覽

新的校訂檢視器可用於以下預覽環境中測試：

* ProofHQ預覽環境

  如需ProofHQ預覽環境的詳細資訊，請參閱[預覽沙箱測試環境 — Workfront Proof](../../../../workfront-proof/wp-getstarted/system-information/preview-sandbox.md)。

* Workfront預覽環境（當您的帳戶已啟用校訂時）

  如需Workfront預覽環境的詳細資訊，請參閱  [Adobe Workfront預覽沙箱環境](../../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md)。

在這個版本中，新的校訂檢視器僅支援視訊校訂。 這表示所有視訊校訂都運用新的校訂檢視器，而所有靜態和多媒體校訂都繼續運用現有的校訂檢視器。

### 生產

透過17.2版發佈至生產環境時，管理員可選擇新校訂或舊版校訂檢視器是否適合組織內的使用者。 依預設，將會使用舊版校訂檢視器。

如需有關如何使用新視訊校訂檢視器的資訊，請參閱  

## 以替代解析度檢視多媒體校樣(ProofHQ和Workfront) {#view-rich-media-proofs-in-alternate-resolutions-proofhq-and-workfront}

您現在可以指定自訂解析度或將影像拖曳到所需的解析度，以調整多媒體校訂的解析度。

在此變更之前，您可以僅使用您檢閱內容的畫面或裝置固有的解析度來檢閱校樣。

您可以使用「比較」模式來比較不同的校訂解析度。

如需詳細資訊，請參閱[在案頭校訂檢視器中開啟校訂](../../../../review-and-approve-work/proofing/use-the-desktop-proofing-viewer/open-proofs-in-dpv.md)。 

## 新的資源集區功能暫時從預覽移除 {#new-resource-pool-functionality-temporarily-removed-from-preview}

由於開發上的挑戰，我們已決定移除新的「資源規劃」標籤，並將「舊版資源規劃」標籤重新命名回其原始名稱「資源規劃」。

新的資源集區功能也隨此變更而移除。 「資源規劃」的新標籤和「資源集區」的功能將於2017年6月底返回「預覽沙箱」環境。
