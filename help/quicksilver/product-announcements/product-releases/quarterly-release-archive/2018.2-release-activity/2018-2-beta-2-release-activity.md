---
content-type: release-notes
navigation-topic: product-releases-archive
title: 2018.2 Beta 2發行活動
description: 本頁說明2018.2 Beta 2版本預覽環境中最近可用的所有變更。 預覽環境已於2018年4月5日提供此功能。 它將於2018年6月在生產環境中提供。
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: c8ef68f5-53db-4c3c-af0f-e1c98521ec27
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '901'
ht-degree: 0%

---

# 2018.2 Beta 2發行活動

本頁說明2018.2 Beta 2版本預覽環境中最近可用的所有變更。 預覽環境已於2018年4月5日提供此功能。 它將於2018年6月在生產環境中提供。

>[!IMPORTANT]
>
> 本頁所述的功能在生產環境使用之前可能會有所變更。

如需2018.2年度所有變更的清單，請參閱  [2018.2發行活動總覽](../../../../product-announcements/product-releases/quarterly-release-archive/2018.2-release-activity/2018-2-release-activity-overview.md)。

2018.2 Beta 2版本包含下列增強功能：

* [直接從主區域編輯欄位](#edit-fields-directly-from-the-home-area)
* [以天數記錄時間](#log-time-in-days)
* [在專案清單的甘特圖上檢視跨專案前置任務關係](#view-cross-project-predecessor-relationships-on-the-gantt-chart-in-a-list-of-projects)
* [在Portfolio最佳化工具中使用預算成本來計算Portfolio財務](#use-budgeted-cost-in-the-portfolio-optimizer-to-calculate-portfolio-finances)
* [使用率報告：從新資源預算區域](#utilization-report-populates-budgeted-hours-from-new-resource-budgeting-area)填入預算時數（僅預覽）

* [使用率報告：檢視專案上使用者的預算時數](#utilization-report-view-budgeted-hours-by-user-on-a-project) （僅預覽）

* [檔案清單中的校訂進度可供非校訂使用者使用](#proof-progress-from-the-document-list-available-to-non-proofing-users)
* [行動裝置改良](#mobile-improvements)

## 直接從首頁區域編輯欄位 {#edit-fields-directly-from-the-home-area}

現在，當您在「首頁」區域中選取物件時，可以直接從「首頁」區域的右側面板編輯與該物件相關聯的欄位。 

在此變更之前，只能在「首頁」區域檢視資訊，不能編輯。

如需詳細資訊，請參閱文章的[首頁]區域[&#128279;](../../../../workfront-basics/using-home/using-the-home-area/update-and-edit-work-item-home.md)中的更新或編輯工作專案  [更新或編輯首頁區域中的工作專案](../../../../workfront-basics/using-home/using-the-home-area/update-and-edit-work-item-home.md)。

## 以天為單位記錄時間 {#log-time-in-days}

Workfront管理員現在可以設定組織中的使用者是以天或小時記錄時間。 擁有Planner授權的使用者可以自行設定此設定。

在此變更之前，使用者只能以小時記錄時間。

您可以編輯使用者設定檔來設定此設定。 如需詳細資訊，請參閱[設定以小時或天記錄時間](../../../../timesheets/config-timesheet-prefs/config-time-logged-hrs-days.md)。

如需使用者如何在此設定更新後以天數記錄時間的詳細資訊，請參閱[記錄時間](../../../../timesheets/create-and-manage-timesheets/log-time.md)。

## 在專案清單的甘特圖上檢視跨專案前置任務關係 {#view-cross-project-predecessor-relationships-on-the-gantt-chart-in-a-list-of-projects}

您現在可以在甘特圖上檢視下列專案清單中的跨專案前置任務關係：

* 投資組合或方案內的專案索引標籤
* 在專案報表中

在此變更之前，您只能檢視專案層級個別任務的跨專案前置任務關係。

如需詳細資訊，請參閱[設定資訊在甘特圖上的顯示方式](../../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md)。 

## 使用Portfolio最佳化工具中的預算成本來計算Portfolio財務 {#use-budgeted-cost-in-the-portfolio-optimizer-to-calculate-portfolio-finances}

新的「Portfolio最佳化程式」現在會使用業務案例新「資源預算」區域或「資源規劃工具」的預算成本，來計算下列欄位：

* 淨值
* 投資報酬率(ROI)
* 成本

先前，新版和舊版Portfolio最佳化工具都使用舊版預算成本。 舊版Portfolio最佳化工具仍會使用舊版預算成本來計算淨值、投資報酬率和成本。

我們也在Portfolio財務欄位中新增了兩個欄位：舊版ROI和舊版淨值，以便從新的資源管理工具中擷取新的值。

如需詳細資訊，請參閱文章中的[Portfolio最佳化工具概觀](../../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md)  [Portfolio最佳化工具概觀](../../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md)。

## 使用率報表：從新資源預算區域植入預算時數 {#utilization-report-populates-budgeted-hours-from-new-resource-budgeting-area}

>[!NOTE]
>
>2018.2版正式發行的「預覽」環境不包含此功能。 它將在2018.3版本的Beta版期間重新引入，並將在2018.3版本中發佈到生產環境。 

使用率報表中的預算時數現在會從業務案例的新資源預算區域可用的資訊植入。

在此變更之前，使用來自舊版資源估計區域的資訊。

如需詳細資訊，請參閱文章中的[資源使用率報告概觀](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md)  [資源使用率報告概觀](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md)。

## 使用率報表：依使用者檢視專案的預算時數 {#utilization-report-view-budgeted-hours-by-user-on-a-project}

>[!NOTE]
>
>2018.2版正式發行的「預覽」環境不包含此功能。 它將在2018.3版本的Beta版期間重新引入，並將在2018.3版本中發佈到生產環境。 

專案的「使用率」報告現在會依使用者顯示預算時數。

在此變更之前，「使用率」報告僅依工作角色顯示「預算時數」。 

如需詳細資訊，請參閱[資源使用率報告概述](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md)一文中的[資源使用率報告概述](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md)。

## 檔案清單中的校訂進度可供非校訂使用者使用 {#proof-progress-from-the-document-list-available-to-non-proofing-users}

現在向所有檢視檔案清單的使用者顯示校訂進度指示器（已傳送、已開啟、已作出評論和決定）。 這包括無法產生校訂的使用者(如需有關讓使用者產生校訂的詳細資訊，請參閱小節。

在此變更之前，校訂進度指標僅適用於可以產生校訂的使用者。

如需詳細資訊，請參閱[校訂進度與狀態概觀](../../../../review-and-approve-work/proofing/proofing-overview/view-progress-status-proof.md)。

## 行動裝置改良 {#mobile-improvements}

行動應用程式包含下列增強功能：

* 您在其他行動應用程式中共用的連結，現在會在Workfront行動應用程式中開啟。

  如需共用連結的詳細資訊，請參閱。

  此更新現在可在iOS和Android上取得。

* 我們已更新iOS平台的支援需求，以支援iPhone X。

  如需支援的行動裝置和作業系統的詳細資訊，請參閱。 
