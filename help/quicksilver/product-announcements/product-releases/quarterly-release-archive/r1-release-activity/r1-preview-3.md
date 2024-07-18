---
content-type: release-notes
navigation-topic: product-releases-archive
title: R1預覽3
description: 本頁說明R1.3版本預覽環境中所有可用的變更。 此頁面的功能已於2017年2月1日在預覽環境中推出。
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: d1502a17-b131-4d29-9b0c-03ad44be4ba6
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '1347'
ht-degree: 2%

---

# R1預覽3

本頁說明R1.3版本預覽環境中所有可用的變更。 此頁面的功能已於2017年2月1日在預覽環境中推出。

如需R1中所有變更的清單，請參閱[R1發行活動概覽](../../../../product-announcements/product-releases/quarterly-release-archive/r1-release-activity/r1-release-activity-overview.md)。 

## 連結外部檔案的改良方法

從外部來源連結檔案的選項(例如Google磁碟機、Box、Dropbox等)現在位於檔案區域中更顯眼的位置。 

此外，在第一次從該提供者連結檔案之前授權檔案提供者的動作，現在更符合直覺（這只是從外部提供者連結檔案時的額外步驟）。

在這些變更之前，從外部來源連結檔案的選項位於「檔案」區域的「新增檔案」對話方塊中。 在第一次從外部來源連結檔案之前，連結檔案的使用者必須在設定區域中授權該檔案提供者。

如需詳細資訊，請參閱  [從外部應用程式連結檔案](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md)。

## 處理行事曆的已更新團隊

>[!NOTE]
>
>已棄用資源排程工具，並已從Workfront的23.1版本中移除。 如需有關使用工作負載平衡器排程資源的資訊，請參閱[工作負載平衡器概覽](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md)。

現在可供團隊使用的「處理中」行事曆包含其他功能和更新的外觀。 「處理中行事曆」團隊的功能現在類似於專案的資源排程工具。

處理行事曆的更新團隊包括以下改進：

* 依字母順序或按角色分組檢視使用者。
* 依專案優先順序、狀態和個別專案篩選排程時間表。 您也可以依角色和使用者來篩選排程時間表。 （排程專案資源時，「篩選」區域所含的選項較少。）
* 在排程時間表上包含問題。
* 顯示使用者分派並修改使用者每天分派至特定任務和問題的小時數。
* 檢視指示器，顯示使用者在任何指定日期何時過度配置。
* 設定是否在排程時間表上顯示已完成的工作。

排程專案資源時與資源排程工具的差異：

* 所有專案團隊成員都會顯示在「處理中的專案團隊」行事曆上。\
  當排程專案的資源時，只會顯示具有與其關聯的角色，且符合未指派區域中一或多個任務的角色的使用者。
* 「交換」工具無法使用，它未包含在「處理中工作」行事曆的專案團隊中。
* 任何專案團隊成員都可以對處理中專案團隊行事曆進行變更。\
  排程專案的資源時，只有資源管理員可以決定專案的資源。
* 依預設，問題會顯示在處理中團隊的行事曆上。\
  排程專案的資源時，預設不會顯示問題。

如需有關使用已更新的「團隊正在處理」行事曆的詳細資訊，請參閱「資源排程」。

## 資源排程增強功能

排程時間表包含下列增強功能：

* 「使用篩選器來控制哪些使用者要顯示在排程時間表上」
* 「使用者在被指派任務後仍然在時間軸上」

### 使用篩選器來控制排程時間表上要顯示哪些使用者 {#use-the-filter-to-control-which-users-are-displayed-on-the-scheduling-timeline}

>[!NOTE]
>
>已棄用資源排程工具，並已從Workfront的23.1版本中移除。 如需有關使用工作負載平衡器排程資源的資訊，請參閱[工作負載平衡器概覽](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md)。

篩選器現在可用於控制排程時間表上顯示的使用者，以及未指派區域中顯示的任務和問題。 在篩選器中選取使用者時，只會顯示您選取的使用者，無論他們是否有符合未指派區域中任務角色指派的角色指派。 所有目前指派給該使用者的任務也會一併顯示。

在此變更之前，篩選器僅控制在「未指派」區域中顯示的任務和問題。 只有當使用者符合「未指派」區域中任務的角色指派時，才會顯示在排程時間表中。

如需使用篩選來控制排程時間表上所顯示內容的詳細資訊，請參閱「在排程區域中篩選資訊」和「在排程區域中手動指派未指派的任務和問題」。

### 使用者在被指派任務後仍留在時間軸上 {#users-remain-on-the-timeline-after-being-assigned-a-task}

使用者在被指派任務或問題後，即使沒有具有相符角色指派的剩餘任務或問題，仍會停留在排程時間表上。 這可讓您在指派使用者後進行任何必要的變更。

在此變更之前，如果在具有相符角色指派的未指派區域中沒有任何剩餘的任務或問題，則在指派任務或問題後，使用者將立即從排程時間表中消失。

如需詳細資訊，請參閱「在排程區域中手動指派未指派的任務和問題」。

## 變更物件名稱以自訂Workfront術語

您現在可以變更特定物件的名稱，以自訂Workfront術語。\
使用版面範本，您現在可以變更以下工作物件的名稱，以符合組織中的需求：

* 專案組合
* 方案
* 專案
* 任務
* 問題

例如，如果在您的組織中您使用行銷活動而非專案，您可以將「專案」物件的名稱取代為「行銷活動」。

當您進行此取代時，應用程式的下列區域會顯示物件的更新名稱：

* 全域導覽列
* 所有標籤
* 所有功能表 
* Report Builder和報告元素（檢視、篩選器和群組）
* 儲存按鈕
* 匯出的檔案
* 電子郵件

下列區域不會顯示物件的更新名稱：

* 資源估計
* 資源預算管理器
* 產能規劃工具
* 資源格線
* 團隊建立者
* Portfolio最佳化工具 
* 行動應用程式
* Outlook增益集

如需有關如何使用版面配置範本自訂Workfront術語的詳細資訊，請參閱「建立和管理版面配置範本」中的「自訂術語」一節，以及[瞭解Adobe Workfront中的物件](../../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md)中的「瞭解自訂物件名稱的影響」一節。

## 在報表中包含核准開始和結束日期

您現在可以在建立或修改報表時包括下列欄位：

* 核准路徑開始日期
* 核准路徑完成日期

這些欄位可讓您深入瞭解目前或最近核准路徑何時開始，以及何時標籤為完成。

如需這些欄位的詳細資訊，請參閱[Adobe Workfront術語表](../../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md)。

如需核准路徑、其建立與觸發方式，及其在核准程式中作用的詳細資訊，請參閱[建立工作專案的核准程式](../../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md)。

下列欄位已從Workfront中移除，無法再包含在報表中（這些欄位提供專案的相關資訊，而非核准本身的資訊，且經常遭到誤用）：

* 核准計劃開始日期
* 預計核准開始日期
* 核准預估開始日期

## 「我已提出要求」的新電子郵件摘要選項

每日摘要傳送選項已新增至通知設定的「我已提出請求」區域。

如需詳細資訊，請參閱[修改您自己的電子郵件通知](../../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md)。

請記得更新與您的帳戶相關聯的電子郵件地址，以便測試此功能。 此為必要操作，因為「預覽沙箱」會清除所有使用者的電子郵件地址。

## 更新檔案核准電子郵件通知的外觀

「檔案核准」通知的外觀和使用新UI更新：

如需電子郵件通知的詳細資訊，請參閱[Adobe Workfront通知](../../../../workfront-basics/using-notifications/wf-notifications.md)。

請記得更新與您的帳戶相關聯的電子郵件地址，以便測試此功能。 此為必要操作，因為「預覽沙箱」會清除所有使用者的電子郵件地址。

## 里程碑檢視中的增強功能

檢視專案清單或專案報告時可用的里程碑檢視現在包含下列增強功能：

* 可編輯計畫日期
* 專案與任務的完成百分比隨即顯示

在此變更之前，為了編輯日期或檢視完成百分比，您必須移至個別任務。

如需詳細資訊，請參閱[使用里程碑檢視](../../../../reports-and-dashboards/reports/reporting-elements/use-milestone-view.md)。
