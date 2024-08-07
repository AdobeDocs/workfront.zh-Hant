---
content-type: release-notes
navigation-topic: product-releases-archive
title: 2017.3 Beta 1發行活動
description: 本頁說明2017.3版預覽環境中最近可用的所有變更。 此頁面的功能已於2017年8月9日在預覽環境中推出。 它將在2017年11月初的生產環境中提供。
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 33a91c25-98ec-4f08-b444-4e11e05e464b
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '1426'
ht-degree: 0%

---

# 2017.3 Beta 1發行活動

本頁說明2017.3版預覽環境中最近可用的所有變更。 此頁面的功能已於2017年8月9日在預覽環境中推出。 它將在2017年11月初的生產環境中提供。

>[!IMPORTANT]
>
> 本頁所述的功能在生產環境使用之前可能會有所變更。

如需2017.3年度所有變更的清單，請參閱  [2017.3發行活動總覽](../../../../product-announcements/product-releases/quarterly-release-archive/2017.3-release-activity/2017-3-release-activity-overview.md)。

2017.3 Beta 1版本包含適用於Workfront管理員和其他使用者的增強功能：

管理員的&#x200B;**：**

* [記錄時數時防止刪除任務和問題](#prevent-tasks-and-issues-from-being-deleted-when-hours-are-logged)
* [從設定區域](#removal-of-the-early-access-setting-from-the-setup-area)移除「搶先存取」設定
* [Workfront預設電子郵件地址變更](#workfront-default-email-address-change)

所有使用者的&#x200B;**：**

* [資源排程改善](#resource-scheduling-improvements)
* [寬熒幕顯示器](#widescreen-display)
* [調整報表和清單中的欄大小並重新排序](#resize-and-reorder-columns-in-reports-and-lists)
* 複製任務和問題時[清除自訂資料選項](#clear-custom-data-option-when-copying-tasks-and-issues)
* [直接從範本建立專案](#create-a-project-directly-from-a-template)
* 訂閱物件的[應用程式內通知](#in-app-notification-for-subscribed-objects)
* 預覽環境中目前無法使用[@Tagging](#tagging-currently-not-available-in-the-preview-environment)
* [在專案的使用率報告中包含使用者配置資訊](#include-user-allocation-information-in-the-utilization-report-on-a-project)

## 資源排程改善 {#resource-scheduling-improvements}

>[!NOTE]
>
>已棄用資源排程工具，並已從Workfront的23.1版本中移除。 如需有關使用工作負載平衡器排程資源的資訊，請參閱[工作負載平衡器概覽](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md)。

為團隊、專案或多個專案排程資源時，若以資源經理的身分，可使用下列資源排程改進：

* [以全熒幕模式檢視排程區域](#view-scheduling-area-in-full-screen-mode)
* [更多檢視資源排程區域的日期範圍選項](#more-date-range-options-for-viewing-the-resource-scheduling-area)
* [在排程時間表上檢視預計日期](#view-projected-dates-on-the-scheduling-timeline)

### 以全熒幕模式檢視排程區域 {#view-scheduling-area-in-full-screen-mode}

您可以以全熒幕模式檢視排程時間表，讓您在單一檢視中檢視更多資訊。 

如需詳細資訊，請參閱「開始使用資源排程」。

### 檢視資源排程區域的更多日期範圍選項 {#more-date-range-options-for-viewing-the-resource-scheduling-area}

檢視排程時間表時，您可以檢視下列其他日期範圍選項：

* 單日檢視
* 4週檢視
* 6週檢視

在此變更之前，您只能在1週、2週或3週的檢視中檢視排程時間表。 除了新日期範圍之外，您仍可使用這些日期範圍。

當您在單日檢視中檢視排程時間表時，無法顯示使用者配置（包括每日總時數）。

如需詳細資訊，請參閱「開始使用資源排程」。

### 在排程時間表上檢視預計日期 {#view-projected-dates-on-the-scheduling-timeline}

現在您可以設定排程時間表以顯示任務和問題的預計日期，而不是計畫日期。 

在此變更之前，排程時間表上的任務和問題僅顯示計畫日期。

當您在排程時間表上檢視「預計日期」時，無法顯示使用者配置（包括每日總時數）。

如需詳細資訊，請參閱「開始使用資源排程」。

## 寬熒幕顯示器 {#widescreen-display}

當您在Workfront中顯示下列任何物件時，系統會自動填入整個瀏覽器視窗：

* 專案
* 任務
* 問題
* 報告
* 儀表板
* 行事曆

在此變更之前，顯示區域的兩側都有兩個白色側欄。 現在，寬熒幕檢視會動態調整熒幕與瀏覽器視窗的寬度。

## 調整報表和清單中的欄大小及重新排序 {#resize-and-reorder-columns-in-reports-and-lists}

您現在可以重新排序報表或清單中的欄並調整其大小，而無需編輯報表。 (今年早些時候，隨著搶先存取環境的淘汰，此功能被移除。 目前正在重新匯入。)

此功能不適用於儀表板清單或報表，因為這些清單已在新的資料網格結構中重新設計。 所有其他清單都會在此版本中啟用此功能。

如需重新調整欄位大小與重新排序的詳細資訊，請參閱[修改欄位寬度和順序](../../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md)。

## 複製任務和問題時清除自訂資料選項 {#clear-custom-data-option-when-copying-tasks-and-issues}

複製任務或問題時，您現在可以選擇選項以清除任何自訂資料。 當您選擇清除任務或問題的自訂資料時，表單會複製到新專案，但表單上的自訂資料不會。 清除自訂資料也會影響附加到附加到專案的檔案的自訂表單，或附加到任務支出的自訂表單。

在此變更之前，當您複製任務或問題時，自訂表單中包含的自訂資料也會複製到新專案。 

如需複製工作的詳細資訊，請參閱[複製和複製工作](../../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md)。

如需複製問題的詳細資訊，請參閱[複製問題](../../../../manage-work/issues/manage-issues/copy-issues.md)。

## 直接從範本建立專案 {#create-a-project-directly-from-a-template}

您現在可以在範本層級從範本建立專案。

在此變更之前，您只能使用&#x200B;**從範本新增專案**&#x200B;選項，在Workfront的「專案」區域的「專案」索引標籤上，從範本建立專案。

如需從範本建立專案的詳細資訊，請參閱[使用範本建立專案](../../../../manage-work/projects/create-projects/create-project-from-template.md)。

## 防止在記錄時數時刪除任務和問題 {#prevent-tasks-and-issues-from-being-deleted-when-hours-are-logged}

您現在可以設定Workfront允許或防止刪除記錄時數的任務和問題。

在此變更之前，當您刪除記錄時數的任務或問題時，時數會隨任務或問題刪除，或它們被移動到專案，具體取決於您的時程表和時數偏好設定。

如需有關刪除工作的詳細資訊，請參閱[刪除工作](../../../../manage-work/tasks/manage-tasks/delete-tasks.md)。

如需有關刪除問題的詳細資訊，請參閱[刪除問題](../../../../manage-work/issues/manage-issues/delete-issues.md)。

如需啟用系統設定以進行任務和問題刪除的詳細資訊，請參閱[設定系統範圍的任務和問題偏好設定](../../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md)。

## 移除設定區域中的「搶先存取」設定 {#removal-of-the-early-access-setting-from-the-setup-area}

我們正在移除允許Workfront管理員註冊使用者以參與搶先存取環境的設定。 此功能自2016年底起已被取代。 我們尚未在2017年發佈任何新功能到Early Access，該環境中剩餘的所有功能已移至生產環境。

在此變更之前，雖然沒有可存取的新功能，Workfront管理員仍可將使用者新增至搶先存取環境。

## Workfront預設電子郵件地址變更 {#workfront-default-email-address-change}

Workfront傳出郵件的預設電子郵件地址已從[noreply@attask.com](mailto:noreply@attask.com)變更為[noreply@my.workfront.com](mailto:noreply@workfront.com)。

如果您目前篩選從Workfront傳送的電子郵件，則需要變更篩選器以反映新的預設地址。 

預設位址中的變更對已設定的Workfront電子郵件地址沒有影響。 

如需詳細資訊，請參閱。

## 訂閱物件的應用程式內通知 {#in-app-notification-for-subscribed-objects}

當使用者對您訂閱的專案、任務和問題發表評論時，您現在會收到應用程式內通知。 若要深入瞭解訂閱應用程式內通知，請參閱[檢視及管理應用程式內通知](../../../../workfront-basics/using-notifications/view-and-manage-in-app-notifications.md)。

根據您的Workfront管理員啟用的功能，您還可以收到訂閱專案的電子郵件通知。 您可以透過訂閱電子郵件上的連結，輕鬆取消訂閱專案，如[Adobe Workfront通知](../../../../workfront-basics/using-notifications/wf-notifications.md)所述。

在此變更之前，您一律會收到訂閱專案的電子郵件通知，並且沒有選項可接收應用程式內通知。

雖然您可以停用訂閱電子郵件，但無法停用訂閱專案的應用程式內通知。 如需詳細資訊，請參閱[為系統中的每個人設定事件通知](../../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md)。

若要進一步瞭解訂閱專案，請參閱[在Adobe Workfront中訂閱專案](../../../../workfront-basics/using-notifications/subscribe-to-items-in-workfront.md)。

## 預覽環境中目前沒有可用的@Tagging案 {#tagging-currently-not-available-in-the-preview-environment}

當我們將RTF格式功能帶入更新流時，您暫時無法使用@符號在更新流中為預覽環境中的以下物件標籤其他使用者：

* 專案
* 任務
* 問題
* 時程表

您仍然可以按一下&#x200B;**包含此更新中的其他人**&#x200B;圖示來標籤其他人。

如需詳細資訊，請參閱[標籤其他人的更新](../../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md)。

## 在專案的使用率報告中包含使用者配置資訊 {#include-user-allocation-information-in-the-utilization-report-on-a-project}

>[!NOTE]
>
>已棄用資源排程工具，並已從Workfront的23.1版本中移除。 如需有關使用工作負載平衡器排程資源的資訊，請參閱[工作負載平衡器概覽](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md)。

專案的利用報告現在會考慮是否已將計畫時數重新分配給整個任務期間。 修改時數的使用者配置時（如「在排程區域中管理使用者配置」中所述），如果在使用率報表中選取的日期只包含任務的一部分，則可能會影響使用率報表中的資料。

如需詳細資訊，請參閱[資源使用率報告概覽](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md)。
