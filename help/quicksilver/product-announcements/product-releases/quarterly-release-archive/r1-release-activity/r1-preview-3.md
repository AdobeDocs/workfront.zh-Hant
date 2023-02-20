---
content-type: release-notes
navigation-topic: product-releases-archive
title: R1預覽3
description: 本頁介紹了R1.3版本在「預覽」環境中可用的所有更改。 此頁面上的功能已於2017年2月1日在預覽環境中提供使用。
author: Luke
feature: Product Announcements
exl-id: d1502a17-b131-4d29-9b0c-03ad44be4ba6
source-git-commit: f4cc5ae89c8746ec4c40ece88bfdb21dc1996575
workflow-type: tm+mt
source-wordcount: '1345'
ht-degree: 2%

---

# R1預覽3

本頁介紹了R1.3版本在「預覽」環境中可用的所有更改。 此頁面上的功能已於2017年2月1日在預覽環境中提供使用。

有關在R1中進行的所有更改的清單，請參見 [R1發行活動概觀](../../../../product-announcements/product-releases/quarterly-release-archive/r1-release-activity/r1-release-activity-overview.md). 

## 連結外部檔案的改良方法

從外部源(如Google驅動器、盒、Dropbox等)連結文檔的選項現在位於「文檔」區域中更突出的位置。 

此外，在首次從提供者連結檔案之前授權檔案提供者的動作現在更符合直覺（這只是從外部提供者連結檔案時的額外步驟）。

在這些更改之前，從外部源連結檔案的選項位於「文檔」區域的「添加文檔」對話框中。 在首次從外部源連結文檔之前，連結文檔的用戶必須在「設定」區域中授權該文檔提供程式。

如需詳細資訊，請參閱  [從外部應用程式連結文檔](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

## 更新日曆上的團隊

>[!NOTE]
>
>Workfront 23.1版已淘汰資源排程工具，並將其從中移除。 有關使用工作負載平衡器調度資源的資訊，請參見 [工作負載平衡器概述](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

適用於團隊的「工作中」日曆現在包含其他功能和更新的外觀。 「工作日曆」團隊的功能現在類似於項目的資源調度工具。

更新的團隊「工作於」日曆包含下列改良功能：

* 按角色的字母順序或分組查看用戶。
* 依專案優先順序、狀態和個別專案篩選排程時間表。 您也可以依角色和使用者篩選排程時間軸。 （「篩選」區域包含的選項比排程專案資源時少。）
* 納入排程時間表的問題。
* 顯示用戶分配並修改用戶每天分配給某些任務和問題的小時數。
* 檢視在任何指定日期過度配置使用者的時間。
* 配置是否在計畫時間表上顯示已完成的工作。

與資源調度工具在計畫項目資源時的差異：

* 所有團隊成員都顯示在「工作」(Working On)日曆上。\
   排程專案資源時，只會顯示與專案相關聯的角色符合「未指派」區域中一或多個任務角色的使用者。
* 「換用」工具不可用，該工具未包含在「工作日」日曆中。
* 任何團隊成員都可以在「工作於日曆」(Working On calendar)上進行更改。\
   在計畫項目的資源時，只有資源管理器才能為項目做出資源決策。
* 預設情況下，問題會顯示在工作日曆上。\
   排程專案資源時，預設不會顯示問題。

有關使用更新的團隊「工作日曆」的詳細資訊，請參閱「資源計畫」。

## 資源計畫增強功能

排程時間表包含下列增強功能：

* &quot;使用篩選器來控制在計畫時間表上顯示的用戶&quot;
* &quot;分配任務後，用戶仍在時間軸上&quot;

### 使用篩選器可控制哪些用戶顯示在計畫時間表上 {#use-the-filter-to-control-which-users-are-displayed-on-the-scheduling-timeline}

>[!NOTE]
>
>Workfront 23.1版已淘汰資源排程工具，並將其從中移除。 有關使用工作負載平衡器調度資源的資訊，請參見 [工作負載平衡器概述](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

此篩選器現在可用於控制在計畫時間表上顯示的用戶，以及在「未分配」區域中顯示的任務和問題。 在篩選器中選擇用戶時，將只顯示您選擇的用戶，而不管他們是否具有與「未分配」區域中任務的角色分配匹配的角色分配。 也會顯示目前指派給該使用者的所有工作。

在此更改前，篩選器僅控制哪些任務和問題顯示在「未分配」區域中。 只有當用戶與「未分配」區域中的任務的角色分配匹配時，才會在計畫時間軸中顯示用戶。

有關使用篩選器來控制計畫時間表上顯示內容的詳細資訊，請參閱「在計畫區域中篩選資訊」和「在計畫區域中手動分配未分配的任務和問題」。

### 為用戶分配任務後，用戶將保持在時間軸上 {#users-remain-on-the-timeline-after-being-assigned-a-task}

在分配任務或問題後，即使沒有剩餘任務或問題具有匹配角色分配，用戶仍停留在計畫時間線上。 這可讓您在指派使用者後進行任何必要的變更。

在此更改之前，如果「未分配」區域中沒有任務或問題，且分配了匹配的角色，則在分配任務或問題後，用戶將立即從計畫時間軸中消失。

如需詳細資訊，請參閱「在排程區域中手動指派未指派的任務和問題」。

## 透過變更物件名稱來自訂Workfront術語

您現在可以透過變更特定物件的名稱來自訂Workfront術語。\
您現在可以使用「佈局模板」(Layout Template)更改以下工作對象的名稱，以滿足貴組織的需求：

* 專案組合
* 方案
* 專案
* 任務
* 問題

例如，如果您在組織中使用促銷活動而非專案，則可將「專案」物件的名稱取代為「促銷活動」。

進行此替換時，應用程式的以下區域將顯示對象的更新名稱：

* 全域導覽列
* 所有標籤
* 所有菜單 
* 報告建立工具和報告元素（檢視、篩選和群組）
* 保存按鈕
* 匯出的檔案
* 電子郵件

以下區域不顯示對象的更新名稱：

* 資源估計
* 資源預算管理器
* 產能規劃工具
* 資源格線
* 團隊建立者
* Portfolio優化程式 
* 行動應用程式
* Outlook插件

如需如何使用版面範本自訂Workfront術語的詳細資訊，請參閱「建立和管理版面範本」中的「自訂術語」一節，以及 [了解Adobe Workfront中的物件](../../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

## 在報表中包含核准開始和結束日期

您現在可以在建立或修改報表時加入下列欄位：

* 核准路徑開始日期
* 批准路徑完成日期

這些欄位可讓您深入了解目前或最近的核准路徑何時開始，以及何時標示為完成。

如需這些欄位的詳細資訊，請參閱 [Adobe Workfront術語表](../../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

如需核准路徑、其建立和觸發方式，以及其在核准程式中所提供功能的詳細資訊，請參閱 [建立工作項的審批流程](../../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

下列欄位已從Workfront中移除，不再能納入報告（這些欄位提供了有關項目的資訊，而不是有關核准本身的資訊，且經常被濫用）:

* 批准計劃開始日期
* 預計核准開始日期
* 預計的核准開始日期

## 「我已提出請求」的新電子郵件摘要選項

「每日摘要傳送」選項已新增至「通知」設定的「已提出請求」區域。

如需詳細資訊，請參閱 [啟用或停用您自己的事件通知](../../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

請記得更新與您的帳戶相關聯的電子郵件地址，以便能夠測試此功能。 這是必要操作，因為「預覽沙箱」會清除所有使用者的電子郵件地址。

## 更新檔案核准電子郵件通知的外觀和風格

已使用新UI更新「檔案核准」通知的外觀和風格：

如需電子郵件通知的詳細資訊，請參閱 [Adobe Workfront通知](../../../../workfront-basics/using-notifications/wf-notifications.md).

請記得更新與您的帳戶相關聯的電子郵件地址，以便能夠測試此功能。 這是必要操作，因為「預覽沙箱」會清除所有使用者的電子郵件地址。

## 「里程碑」檢視中的增強功能

檢視專案清單或專案報表時可用的「里程碑」檢視現在包含下列增強功能：

* 可編輯計畫日期
* 項目和任務的完成百分比隨即顯示

在此變更前，若要編輯日期或檢視完成百分比，您必須前往個別工作。

如需詳細資訊，請參閱 [使用里程碑檢視](../../../../reports-and-dashboards/reports/reporting-elements/use-milestone-view.md).
