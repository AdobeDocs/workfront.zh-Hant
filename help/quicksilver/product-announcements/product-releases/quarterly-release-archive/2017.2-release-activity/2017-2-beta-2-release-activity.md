---
content-type: release-notes
navigation-topic: product-releases-archive
title: 2017.2 Beta 2發行活動
description: 本頁說明2017.2 Beta 2版本預覽環境中所有可用的變更。 此頁面的功能已於2017年5月24日在預覽環境中推出。 它將在2017年7月底到8月初期間在生產環境中可用。
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 0aa8d61e-cf8c-46a7-b093-a0dbc90d37fd
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '792'
ht-degree: 0%

---

# 2017.2 Beta 2發行活動

本頁說明2017.2 Beta 2版本預覽環境中所有可用的變更。 此頁面的功能已於2017年5月24日在預覽環境中推出。 它將在2017年7月底到8月初期間在生產環境中可用。

>[!IMPORTANT]
>
>本頁所述的功能在生產環境使用之前可能會有所變更。

如需2017.2年度所有變更的清單，請參閱[2017.2年度發行活動概觀](../../../../product-announcements/product-releases/quarterly-release-archive/2017.2-release-activity/2017-2-release-activity-overview.md)。

2017.2 Beta 2版本包含適用於Workfront管理員和其他使用者的增強功能：

管理員的&#x200B;**：**

* [API增強功能：事件訂閱](#api-enhancement-event-subscriptions)

所有使用者的&#x200B;**：**

* [訂閱專案](#subscribe-to-projects)
* [從電子郵件取消訂閱專案](#unsubscribe-from-items-from-email)
* [設定里程碑在甘特圖上的顯示方式](#configure-how-milestones-are-displayed-on-the-gantt-chart)
* [資源集區範本](#resource-pools-templates)
* [在Workfront中檢視校訂檔案的版本](#view-versions-of-proofed-documents-within-workfront)
* [校訂核准報告中的新要求者物件](#new-requester-object-in-proof-approval-report)

## API增強功能：事件訂閱 {#api-enhancement-event-subscriptions}

當事件訂閱支援的Workfront物件上發生動作時，您現在可以設定Workfront將回應傳送至您想要的端點。 這表示您的整合可與Workfront API即時互動。

如需詳細資訊，請參閱[事件訂閱API](../../../../wf-api/general/event-subs-api.md)。 

## 訂閱專案 {#subscribe-to-projects}

您現在可以訂閱您不屬於專案團隊之專案的新註解。 在此版本之前，您只能訂閱關於問題和任務的評論。

如需訂閱專案的詳細資訊，請參閱[在Adobe Workfront中訂閱專案](../../../../workfront-basics/using-notifications/subscribe-to-items-in-workfront.md)

## 從電子郵件取消訂閱專案 {#unsubscribe-from-items-from-email}

您可以使用訂閱電子郵件內的「取消訂閱」連結，取消訂閱專案。 之前，您只能從Workfront介面取消訂閱專案。

如需取消訂閱訂閱電子郵件的詳細資訊，請參閱[Adobe Workfront通知](../../../../workfront-basics/using-notifications/wf-notifications.md)中的「選擇退出電子郵件通知」一節 

## 設定里程碑在甘特圖上的顯示方式 {#configure-how-milestones-are-displayed-on-the-gantt-chart}

***更正&#x200B;**：此功能目前不在預覽沙箱環境中。 計畫於稍後日期（2017年6月）發行。*

在甘特圖中，現在有兩個檢視里程碑資訊的選項。 您可以設定下列其中一個或兩個里程碑指標：

* 里程碑菱形（圖示）

  此圖示會顯示在甘特圖中與里程碑相關聯的任何任務之後。

* 里程碑線

  在甘特圖中，與里程碑相關聯的任何任務後面都會顯示一條直線。

在此變更之前，只有一個選項可讓里程碑顯示在甘特圖上，稱為「里程碑」。 此選項會同時啟用里程碑菱形圖示和里程碑線。 無法分隔這些指標。 這兩個選項現在可用於所有甘特圖，包括所有專案清單和報告。 

如需有關設定資訊在甘特圖中的顯示方式的詳細資訊，請參閱[設定資訊在甘特圖上的顯示方式](../../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md)。

## 資源集區範本 {#resource-pools-templates}

您現在可以為範本指定資源集區。 在此版本之前，您只能將資源集區與使用者和專案建立關聯。

如需資源集區的詳細資訊，請參閱[資源集區概觀](../../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md)

## 在Workfront中檢視校訂檔案的版本 {#view-versions-of-proofed-documents-within-workfront}

您現在可以在Workfront介面中檢視校訂檔案所有版本的校訂。 

在此變更之前，您只能檢視校訂檔案的最新版本。

沒有校訂授權的使用者可以：

* 在校訂檔案的先前版本上開啟校訂

擁有校訂授權的使用者可以執行下列任一操作：

* 在校訂檔案的先前版本上開啟校訂
* 在校訂檔案的先前版本上檢視校訂詳細資訊

如需詳細資訊，請參閱[管理檔案版本](../../../../documents/managing-documents/manage-document-versions.md)中的[管理檔案版本](../../../../documents/managing-documents/manage-document-versions.md)。

## 校訂核准報告中的新要求者物件 {#new-requester-object-in-proof-approval-report}

現在，建立校訂核准報告時，有新的請求者物件。 此物件可讓您報告有關請求校訂核准之使用者的資訊。 

「校訂核准報告」中的新「請求者」物件包含其他物件報告型別中現有「使用者」物件可用的所有欄位。

>[!NOTE]
>
> 此報表中提供的資訊，僅限於此功能首次引進至個別預覽或生產環境時的資訊；此報表中提供的資訊，不適用引進此功能之前有關請求者物件的資訊。

您在建立校訂核准報告時存取請求者物件，如[建立自訂報告](../../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)中所述。

如需校訂核准物件報告的詳細資訊，請參閱[瞭解Adobe Workfront中的物件](../../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md)中的[瞭解Adobe Workfront中的物件](../../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md)一節。
