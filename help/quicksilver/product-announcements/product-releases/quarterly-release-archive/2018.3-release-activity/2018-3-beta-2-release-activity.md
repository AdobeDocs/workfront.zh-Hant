---
content-type: release-notes
navigation-topic: product-releases-archive
title: 2018.3 Beta 2發行活動
description: 本頁說明2018.3 Beta 2版本預覽環境中最近可用的所有變更。 此功能將於2018年8月1日在預覽環境中提供。 Beta 2所發行的校訂增強功能將於7月18日星期三在預覽環境中提供。 它將於2018年11月在生產環境中提供。
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 97945661-e97d-43c8-b564-624c4388de2f
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '908'
ht-degree: 0%

---

# 2018.3 Beta 2發行活動

本頁說明2018.3 Beta 2版本預覽環境中最近可用的所有變更。 此功能將於2018年8月1日在預覽環境中提供。 Beta 2所發行的校訂增強功能將於7月18日星期三在預覽環境中提供。 它將於2018年11月在生產環境中提供。

>[!NOTE]
>
> 本頁所述的功能在生產環境使用之前可能會有所變更。

如需2018.3年所有變更的清單，請參閱  [2018.3發行活動總覽](../../../../product-announcements/product-releases/quarterly-release-archive/2018.3-release-activity/2018-3-release-activity-overview.md)。

2018.3 Beta 2版本包含適用於Workfront管理員和其他使用者的增強功能：

管理員的&#x200B;**&#x200B;**

* [以群組管理員的身分更新使用者設定檔中的電子郵件地址](#update-the-email-address-in-the-user-profile-as-a-group-administrator)

**所有使用者**

* [在首頁區域檢視委派給我的核准](#view-approvals-delegated-to-me-in-the-home-area)
* [匯出資源規劃工具中指定期間的資料](#export-data-for-a-given-period-in-the-resource-planner)
* 當使用者過度分配時，[每日總計現在會以紅色顯示](#daily-totals-now-display-in-red-when-the-user-is-overallocated)
* 最小化時，[排程時間表上會隱藏任務和問題](#tasks-and-issues-are-hidden-on-the-scheduling-timeline-when-minimized)
* [在校訂檢視器中依使用者篩選評論和回覆](#filter-comments-and-replies-by-user-in-the-proofing-viewer)
* [在視訊校訂中註解一段素材](#comment-on-a-range-of-footage-in-a-video-proof)
* [校訂檢視器中註解標籤的新折線工具](#new-polyline-tool-for-comment-markup-in-the-proofing-viewer)
* [針對報告、行事曆和檔案共用移除Flash](#flash-removal-for-report-calendar-and-document-sharing)

## 以群組管理員的身分更新使用者設定檔中的電子郵件地址 {#update-the-email-address-in-the-user-profile-as-a-group-administrator}

您現在可以更新屬於您管理之群組的使用者的電子郵件地址。 

之前，只有Workfront管理員可以更新其他使用者的電子郵件地址。 

如需詳細資訊，請參閱[群組管理員](../../../../administration-and-setup/manage-groups/group-roles/group-administrators.md)。

## 在首頁區域中檢視委派給我的核准 {#view-approvals-delegated-to-me-in-the-home-area}

您現在可以使用首頁區域來檢視已委派給您的專案、任務和問題核准。

在此變更之前，您只能在「我的工作」區域中檢視委派的核准。

如需詳細資訊，請參閱[委派核准要求](../../../../review-and-approve-work/manage-approvals/delegate-approval-requests.md)。

## 匯出資源規劃工具中指定期間的資料 {#export-data-for-a-given-period-in-the-resource-planner}

現在，在資源規劃工具中匯出資訊時，會顯示一個新視窗，可讓您為匯出的檔案選取特定的時間範圍。

在此增強功能之前，您只能匯出畫面上顯示的資訊。

如需有關從資源規劃工具匯出資料的詳細資訊，請參閱文章[資源規劃工具導覽概觀](../../../../resource-mgmt/resource-planning/resource-planner-navigation.md)中的[資源規劃工具導覽概觀](../../../../resource-mgmt/resource-planning/resource-planner-navigation.md)。

## 當使用者過度分配時，每日總計現在會以紅色顯示 {#daily-totals-now-display-in-red-when-the-user-is-overallocated}

>[!NOTE]
>
>已棄用資源排程工具，並已從Workfront的23.1版本中移除。 如需有關使用工作負載平衡器排程資源的資訊，請參閱[工作負載平衡器概覽](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md)。

當使用者被過度分配時，該使用者被過度分配的天數的每日總計現在顯示為紅色。 只有在排程時間表設定中啟用顯示每日計畫時數總計選項時，才會顯示此選項。 在此增強功能之前，使用者過度配置的天數有紅色長條指標，但每日總計顯示時沒有紅色反白顯示。

如需使用者配置的詳細資訊，請參閱「在排程區域中管理使用者配置」。

## 最小化時，排程時間表上會隱藏任務和問題 {#tasks-and-issues-are-hidden-on-the-scheduling-timeline-when-minimized}

當您將排程時間表上的任務和問題最小化時，如果您的設定中啟用了「顯示每日規劃時數總計」選項，使用者和角色現在可以隱藏這些任務和問題。 未指派區域中的任務和問題會以壓縮檢視顯示。

以前，當最小化任務和問題時，任務和問題將保留在使用者和角色的排程時間表上，但將以壓縮檢視顯示。

如需有關在排程時間表中將任務和問題最小化的詳細資訊，請參閱  開始使用資源排程。

## 在校訂檢視器中依使用者篩選評論和回覆 {#filter-comments-and-replies-by-user-in-the-proofing-viewer}

現在，當您篩選指定使用者的評論時，可以包含回覆。 如果您想要聚焦於重要稽核者（例如客戶或專案經理）提出的所有意見回饋，這會很有用。

以前，按使用者篩選僅限於由您指定的稽核者所創作（開始）的評論。

## 對視訊校訂中的某個範圍的影片進行註解 {#comment-on-a-range-of-footage-in-a-video-proof}

您可以為視訊校樣中的某個範圍的素材建立註解。 例如，當您需要指出需要重新拍攝或移除素材區段時，這個選項會很有用。

過去，您只能為視訊時間軸上的單一點建立註解。

## 校訂檢視器中註解標示的新折線工具 {#new-polyline-tool-for-comment-markup-in-the-proofing-viewer}

現在，當您將註解新增至校樣時，可以使用折線標籤來繪製分段線條和形狀。 您可以建立開放的分段線或封閉的形狀。 這項工具在處理複雜影像（例如技術或架構影像）時特別有用。

先前，在標示校樣以新增註解時，您可以繪製矩形、直線、手繪線或形狀，或箭頭。

## 針對報告、行事曆和檔案共用移除Flash {#flash-removal-for-report-calendar-and-document-sharing}

我們已從Workfront中的下列「共用」對話方塊中移除Flash：

* 報告
* 行事曆
* 文件

您仍然可以像之前一樣共用這些物件，但現在的體驗不再依賴Flash。
