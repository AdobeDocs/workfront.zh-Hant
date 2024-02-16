---
content-type: release-notes
navigation-topic: product-releases-archive
title: 2017.2 Beta最終版
description: 本頁說明2017.2版預覽環境中最近可用的所有變更。 此頁面的功能已於2017年6月28日在預覽環境中推出。 它將於2017年7月26日在生產環境中提供。
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 768e9aad-d7e7-4a3c-9f93-926cf588ddc7
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '2314'
ht-degree: 0%

---

# 2017.2 Beta最終版

本頁說明2017.2版預覽環境中最近可用的所有變更。 此頁面的功能已於2017年6月28日在預覽環境中推出。 它將於2017年7月26日在生產環境中提供。

>[!IMPORTANT]
>
>本頁所述的功能在生產環境使用之前可能會有所變更。

如需2017.2年度所有變更的清單，請參閱 [2017.2版本活動概覽](../../../../product-announcements/product-releases/quarterly-release-archive/2017.2-release-activity/2017-2-release-activity-overview.md).

2017.2測試版最終版本包含適用於Workfront管理員和其他使用者的增強功能：

**對於管理員：**

* [判斷HTML5視訊校訂檢視器(ProofHQ和Workfront)的可用性](#determine-the-availability-of-the-html5-video-proofing-viewer-proofhq-and-workfront)
* [支援SAML 2.0的SHA-256憑證](#support-sha-256-certificates-for-saml-2-0)
* [對應屬性的預先輸入](#type-ahead-for-mapping-attributes)
* [API增強功能：存取使用者配置](#api-enhancement-access-user-allocations)

**針對所有使用者：**

* [資源規劃工具](#resource-planner)
* [專案中的新排程區域(Team Builder)](#new-scheduling-area-in-a-project-team-builder)
* [資源排程：預設顯示較少專案](#resource-scheduling-show-fewer-items-by-default)
* [資源排程：在拖曳任務和問題時顯示下拉指標與過度配置](#resource-scheduling-display-drop-indicator-and-over-allocation-when-dragging-tasks-and-issues)
* [資源排程：使用者配置不再四捨五入到最接近的半小時](#resource-scheduling-user-allocations-are-no-longer-rounded-to-the-nearest-half-hour)
* [以TSV和PDF格式匯出使用情況報表](#export-the-utilization-report-in-tsv-and-pdf-formats)
* [2017.2 Beta最終版](#user-calendar-enhancements-in-the-my-work-area%22)
* [2017.2 Beta最終版](#layout-template-determines-whether-the-new-or-legacy-calendar-displays-in-the-my-work-area)
* [校訂決定顯示在我的工作區域(Workfront)](#proof-decision-displays-in-the-my-work-area-workfront)
* [以預設解析度檢視多媒體校樣(ProofHQ和Workfront)](#view-rich-media-proofs-in-preset-resolutions-proofhq-and-workfront)
* [在多媒體校樣(ProofHQ和Workfront)的評論中檢視子頁面的URL](#view-url-to-sub-pages-in-comments-on-rich-media-proofs-proofhq-and-workfront)
* [根據現有的標準檢視建立自訂檢視(ProofHQ)](#create-custom-views-based-on-existing-standard-views-proofhq)
* [篩選報告區域(ProofHQ)](#filter-the-reporting-area-proofhq)
* [在報告中顯示最小值和最大值(ProofHQ)](#display-minimum-and-maximum-values-in-reports-proofhq)
* [用於校訂核准的應用程式內通知](#in-app-notification-for-proof-approval)
* [行動裝置改良](#mobile-improvements)
* [新增斜線以篩選包含逗號的欄位值陳述式](#slash-added-to-filter-statements-for-field-values-that-contain-commas)
* [多重收費率](#multiple-billing-rates)
* [新資源預算時數欄位](#new-resource-budgeted-hour-field)
* [在任務與問題的詳細資訊頁面上的「指派至」區域顯示使用者工作角色](#show-user-job-role-in-assigned-to-area-on-the-details-page-for-tasks-and-issues)

>[!NOTE]
>
>已棄用資源排程工具，並已從Workfront的23.1版本中移除。 如需有關使用工作負載平衡器排程資源的資訊，請參閱 [工作負載平衡器概覽](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

## 專案中的新排程區域(Team Builder) {#new-scheduling-area-in-a-project-team-builder}

專案中的排程區域（先前稱為團隊建立器）已重新設計，提供更新且更直覺的使用者介面。 新的排程功能現在更符合Workfront其他區域目前可用的資源排程功能。

改善專案包括：

* 檢視專案團隊成員的目前資源配置，讓您在指派時做出更明智的決策
* 排程時間表上任務持續時間的視覺化表示
* 篩選在排程時間表上顯示的資訊
* 直接從排程時間表輕鬆新增和移除專案團隊中的使用者

排程資源時，下列功能可在工具的其他區域使用，但在「小組排程」區域中排程資源時無法使用：

* 設定要在排程時間表上顯示的父系任務
* 設定要在排程時間表上顯示的專案名稱
* 使用交換工具修改使用者指派
* 依投資組合、方案和專案篩選

如需「小組排程」區域中可用功能的詳細資訊，請參閱「開始使用資源排程」。

## 資源排程：預設顯示較少專案 {#resource-scheduling-show-fewer-items-by-default}

依預設，指定使用者的排程時間表現在每天最多顯示10個工作專案。 您可以展開清單以檢視目前指派給該使用者的所有任務和問題。

這可讓您在使用者被指派許多工和問題時，更輕鬆地瀏覽排程時間表。

在此變更之前，將一律顯示所有使用者的所有任務和問題。

如需有關在排程時間表上指派任務和問題給使用者的詳細資訊，請參閱「在排程區域中手動指派未指派的任務和問題」。

## 資源排程：在拖曳任務和問題時顯示下拉指標與過度配置 {#resource-scheduling-display-drop-indicator-and-over-allocation-when-dragging-tasks-and-issues}

透過拖放方式在排程時間表上將任務或問題指派給使用者時，現在會在核發任務或問題並完成指派之前顯示下列資訊：

* 放置指示器會顯示在使用者的列中。 這可讓您檢視在進行指定之前在何處指定專案。
* 如果在排程時間表上啟用使用者配置，則當完成指派將導致使用者過度配置時，會顯示紅色過度配置指示器。

在這些變更之前，在發佈任務或問題之前不顯示任何資訊。

如需有關在排程時間表上指派任務和問題給使用者的詳細資訊，請參閱「在排程區域中手動指派未指派的任務和問題」。

## 資源排程：使用者配置不再四捨五入到最接近的半小時 {#resource-scheduling-user-allocations-are-no-longer-rounded-to-the-nearest-half-hour}

當多個使用者被指派到一個任務或問題時，或當一個任務或問題跨越多天時，Workfront會嘗試將計畫時數平均分配給指派的使用者和天數。 依預設，小時會四捨五入到最接近的百位數（例如1.33）。

先前，當您手動修改分散式時數時，時數會經過調整，並舍入至最接近的半小時（例如，1.33會舍入至1.5）。

現在，時數不再調整，並舍入至最接近的半小時（例如，1.33仍為1.33）。

## API增強功能：存取使用者配置 {#api-enhancement-access-user-allocations}

您現在可以透過Workfront API存取使用者配置陰影。

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">For more information, see <a href="../../../../wf-api/api/access-proj-allocation-info-api.md" class="MCXref xref" xrefformat="{para}">Access Project Allocation Information via the API</a>.</p>
-->

## 以TSV和PDF格式匯出使用情況報表 {#export-the-utilization-report-in-tsv-and-pdf-formats}

除了XLSX格式以外，您現在可以匯出TSV和PDF格式之專案的「使用率」報告。

在此變更之前，您只能以XLSX格式匯出「使用率」報告。

如需有關匯出「使用率」報告的詳細資訊，請參閱 [資源使用率報表概要](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md) 在 [資源使用率報表概要](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

## 校訂決定顯示在我的工作區域(Workfront) {#proof-decision-displays-in-the-my-work-area-workfront}

現在，當您在「我的工作」區域的「我的核准」標籤中檢視校訂核準時，校訂決定會顯示在「我的工作」區域中，並且會一直保留，直到您按一下Workfront中的新「重新整理」按鈕或直到您下次重新整理瀏覽器頁面為止。

在此變更之前，沒有跡象表明已在校訂上做出決定，並且在您重新整理瀏覽器之前，校訂保留在我的核准索引標籤上。

如需詳細資訊，請參閱 [核准工作](../../../../review-and-approve-work/manage-approvals/approving-work.md) 在 [核准工作](../../../../review-and-approve-work/manage-approvals/approving-work.md).

## 以預設解析度檢視多媒體校樣(ProofHQ和Workfront) {#view-rich-media-proofs-in-preset-resolutions-proofhq-and-workfront}

在舊版的「預覽」環境中，我們匯入了調整多媒體校樣解析度的功能，其方式為指定自訂解析度或將影像拖曳至所需的解析度。

您現在可以從各種手機、平板電腦、筆記型電腦和桌上型電腦的預設解析度選項中選取。

如需詳細資訊，請參閱以下的「檢視預設解析度」： [在校訂檢視器中變更互動式校訂解析度](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/view-interactive-content-as-it-appears-in-device.md).

## 在多媒體校樣(ProofHQ和Workfront)的評論中檢視子頁面的URL {#view-url-to-sub-pages-in-comments-on-rich-media-proofs-proofhq-and-workfront}

>[!NOTE]
>
>此功能目前可在生產環境中使用。

現在，當您對多媒體校訂中的子頁面進行評論時，該子頁面的URL會顯示在評論上。

在此變更之前，不清楚該評論指的是哪個子頁面。

如需詳細資訊，請參閱

## 判斷HTML5視訊校訂檢視器(ProofHQ和Workfront)的可用性 {#determine-the-availability-of-the-html5-video-proofing-viewer-proofhq-and-workfront}

身為ProofHQ中的Workfront管理員，您可以決定組織中的使用者是否擁有視訊校訂的新HTML5校訂檢視器的存取權。

如需在Workfront中設定此選項的詳細資訊，請參閱中的。

## 根據現有的標準檢視建立自訂檢視(ProofHQ) {#create-custom-views-based-on-existing-standard-views-proofhq}

現在您可以根據標準檢視建立自訂檢視。 依預設，標準檢視中的欄、排序和篩選器選項會納入新檢視中。

在此變更之前，為了建立自訂檢視，您必須從頭開始建立檢視。 

如需詳細資訊，請參閱 [建立自訂檢視](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/create-and-manage-custom-views.md#creating) 在 [在Workfront Proof Proof中建立和管理自訂檢視](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/create-and-manage-custom-views.md).

## 篩選報告區域(ProofHQ) {#filter-the-reporting-area-proofhq}

依預設，「報表」標籤上顯示的資料包含來自ProofHQ系統的所有資訊。 您現在可以使用篩選器只顯示與需求相關的資訊。 

如需詳細資訊，請參閱 [篩選報表](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/run-reports.md#filtering-reports) 在  [在Workfront Proof中執行報告](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/run-reports.md).

## 在報告中顯示最小值和最大值(ProofHQ) {#display-minimum-and-maximum-values-in-reports-proofhq}

您現在可以設定檢視報表時圖形中是否顯示最小值和最大值。

如需詳細資訊，請參閱 [檢視報表](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/run-reports.md#viewing-reports) 在  [在Workfront Proof中執行報告](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/run-reports.md).

## 支援SAML 2.0的SHA-256憑證 {#support-sha-256-certificates-for-saml-2-0}

使用SAML 2.0為SSO設定Workfront時，我們現在支援安全雜湊演演算法256 (SHA-256)。在此版本之前，我們僅支援安全雜湊演演算法1 (SHA-1)。

如需使用SAML 2.0設定Workfront的詳細資訊，請參閱 [使用SAML 2.0設定Adobe Workfront](../../../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md)

## 對應屬性的預先輸入 {#type-ahead-for-mapping-attributes}

「屬性對應」對話方塊中的「預設值」欄位型別已更新為預先輸入欄位。 在此變更之前，預設值欄位的型別是下拉式清單。

此變更適用於下列SSO通訊協定：

* 主動式目錄
* LDAP
* SAML 2.0

SAML 1.1不支援屬性對應。

## 行動裝置改良 {#mobile-improvements}

>[!NOTE]
>
> 行動應用程式會獨立於Workfront主應用程式發行。 本節所述的功能將於8月初發佈。

您將在Android和iOS平台的行動應用程式上看到下列新增功能：

* 從行動應用程式提交請求
* 行動應用程式上的時程表新專案
* 從行動應用程式編輯自訂表單
* 行動應用程式上的校訂核准請求

Android平台將針對其中部分功能提供公開測試版計畫。

如需即將推出的行動測試版計畫的詳細資訊，請參閱  [「貝塔斯」](https://support.workfront.com/hc/en-us/sections/115000743248) 頁面。

如需使用Workfront行動應用程式的詳細資訊，請參閱。  

## 新增斜線以篩選包含逗號的欄位值陳述式 {#slash-added-to-filter-statements-for-field-values-that-contain-commas}

在文字模式中建立篩選器，並篩選包含逗號的欄位值時，您必須在分隔值的逗號前加上斜線(&quot;/&quot;)，以確保值作為一個篩選器選項讀取。 這僅適用於下列欄位型別：

* 下拉式清單
* 單選按鈕
* 核取方塊

在此變更之前，您無法篩選選項中包含逗號的欄位。

如需此變更的詳細資訊，請參閱 [篩選器概觀](../../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

## 多重收費率 {#multiple-billing-rates}

您現在可以在專案層級為相同職務角色新增多個收費率覆寫。 透過這項新功能，您可以定義每個收費率覆寫的日期範圍。 在指定的日期範圍內，針對指派給專案上任務的工作角色，會套用不同的收費率。 記帳費率乘以專案上的時數來計算收入。 在計費費率的日期範圍內計算的收入仍以該費率鎖定，並且不會更新為專案更新時工作角色的費率。 在實際收入中，覆寫收費率之前沒有記錄的時數將會重新計算以反映目前的收費率。 將記帳費率覆寫新增到專案之前記錄的小時將與當時工作角色的記帳費率相關聯。

在此變更之前，您只能覆寫工作角色的計費費率一次，並且實際收入將重新計算以反映在計費費率變更之前記錄的所有時數的目前計費率。

如需有關收費率和收入的詳細資訊，請參閱 [帳單與收入概要](../../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

如需有關在專案層級覆寫職務角色收費率的詳細資訊，請參閱 [覆寫工作角色帳單費率與計算專案收入的概要](../../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

## 資源規劃工具 {#resource-planner}

在此版本中，我們將介紹「資源規劃工具」的第一階段，這是重新設計人員區域中新「計畫」標籤的一部分。 透過使用資源規劃工具，您可以預算資源集區中的使用者在您身為資源管理員的所有目前專案中配置的時數。 您可以在「資源規劃工具」中按專案、職務角色及使用者檢視下列配置編號：

* 可用時數
* 規劃時數
* 預算時數
* 時數差額（預算與計畫時數之間）
* 淨時數差異（可用與預算時數之間）

如需有關使用資源規劃工具的詳細資訊，請參閱 [資源規劃工具概觀](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

## 新資源預算時數欄位 {#new-resource-budgeted-hour-field}

為了支援新的「計畫」功能和「資源規劃工具」，已新增一個欄位至Report Builder，可讓您報告資源預算時數。 此欄位會擷取資源在專案中預算的時數。 使用「舊版資源規劃」功能編列資源預算時，無法使用此欄位。

如需有關在資源規劃工具中使用預算時數的詳細資訊，請參閱 [資源規劃工具概觀](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

## 用於校訂核准的應用程式內通知 {#in-app-notification-for-proof-approval}

當您被指定為校訂的核准者時，您會收到有關校訂核准的應用程式內通知，以等待您的決定。 通知會顯示下列文字： `<User name>` 要您核准此校訂」。 如果無法取得使用者資訊，通知會變更為「此校訂需要您的核准」。

在此增強功能之前，您被指定為校訂核准者的唯一視覺指示是「我的工作」區域中的新校訂請求。

如需應用程式內通知的詳細資訊，請參閱 [檢視及管理應用程式內通知](../../../../workfront-basics/using-notifications/view-and-manage-in-app-notifications.md).

## 在任務與問題的詳細資訊頁面上的「指派至」區域顯示使用者工作角色 {#show-user-job-role-in-assigned-to-area-on-the-details-page-for-tasks-and-issues}

現在，當檢視任務或問題的詳細資訊頁面時，工作角色顯示在指派至區域中的受指派人名稱下方。 此工作角色代表符合任務或問題之工作角色指派之使用者工作角色。 如果任務或問題未指派給工作角色，則會顯示指派使用者的主要工作角色。

在此變更之前，在指派至區域中，僅使用者的標題顯示在使用者名稱下方。 
