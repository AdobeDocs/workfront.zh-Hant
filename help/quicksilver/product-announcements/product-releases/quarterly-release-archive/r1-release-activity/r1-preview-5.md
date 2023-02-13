---
content-type: release-notes
navigation-topic: product-releases-archive
title: R1預覽5
description: 本頁介紹了R1預覽版本5中預覽環境中可用的所有更改。 本頁面的功能已於2017年3月16日在「預覽」環境中使用。
author: Luke
feature: Product Announcements
exl-id: 4fba14b5-6c5a-4b03-99a7-f0e6f75807c3
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '1283'
ht-degree: 13%

---

# R1預覽5

本頁介紹了R1預覽版本5中預覽環境中可用的所有更改。 本頁面的功能已於2017年3月16日在「預覽」環境中使用。

有關在R1中進行的所有更改的清單，請參見 [R1發行活動概觀](../../../../product-announcements/product-releases/quarterly-release-archive/r1-release-activity/r1-release-activity-overview.md).

## 使用利用率報告跟蹤項目進度

現在，擁有「管理」專案存取權的使用者可以使用使用率報表來追蹤專案進度。

利用率報表使您能夠快速了解實際小時跟蹤給定周或月或整個項目的預算小時數或計畫小時數的方式，從而使項目保持在預算內。 此外，您還可以查看按職務職責或單個用戶分類的每個類別（預算、計畫和實際）的小時數的詳細資訊。

如需追蹤專案中使用率的詳細資訊，請參閱 [資源利用率報告概覽](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

作為系統管理員，您可以配置「利用率」頁簽是否可供用戶使用。 預設情況下，「利用率」頁簽位於項目的「更多」下拉菜單中。 您可以將「利用率」頁簽移動到其他位置，也可以完全隱藏它。 如果您已為組織中的用戶定義了自定義佈局模板，則需要手動將「利用率」頁簽添加到自定義佈局模板中。

有關配置「利用率」頁簽位置的詳細資訊，請參閱「建立和管理佈局模板」中的「自定義頁簽」。

## 修改單個對象的現有全局批准流程

現在，當您將全局審批流程與對象關聯時，可以修改現有的全局審批流程。 您所做的修改僅適用於您要關聯對象的審批流程。

如需詳細資訊，請參閱 [將新審批流程或現有審批流程與工作關聯](../../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md) in [將新審批流程或現有審批流程與工作關聯](../../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md)

## 配置報表以預設顯示新甘特圖

您可以配置所建立的項目和任務報告，以預設顯示新甘特圖，並配置新選項「預設顯示甘特視圖中的此報告」。

有關配置報告以顯示新甘特圖的詳細資訊，請參見 [編輯報表設定](../../../../reports-and-dashboards/reports/creating-and-managing-reports/edit-report-settings.md).

有關在項目報告和任務報告中查看甘特圖的詳細資訊，請參閱 [在甘特圖中查看資訊](../../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md)在 [在甘特圖中查看資訊](../../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md).

## 資源回收筒改進：任務和子任務將恢復為其上一順序

現在，在刪除任務或子任務後恢復任務或子任務時，該任務或子任務將恢復到其上一個位置（在任務清單中或父任務下），其順序與刪除前的顯示順序相同。

在此更改之前，恢復的任務和子任務始終被還原為最後一個任務（在任務清單中或父任務下），而不管它們在被刪除前出現的順序如何。

如需在Workfront中還原物件的詳細資訊，請參閱 [還原已刪除的項](../../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

## 里程碑檢視改善

現在，在「里程碑」檢視中檢視專案清單或專案報表時，可使用下列改良功能：

* **配置視圖中是否顯示「進度狀態」和「完成百分比」：** 有一個新選項可讓您設定「里程碑」檢視中是否顯示「進度狀態」圖示。 此外，您還可以配置是否顯示與項目和任務相關的「完成百分比」資訊。\
   如需詳細資訊，請參閱 [使用里程碑檢視](../../../../reports-and-dashboards/reports/reporting-elements/use-milestone-view.md) in [使用里程碑檢視](../../../../reports-and-dashboards/reports/reporting-elements/use-milestone-view.md).

* **直接從「里程碑」檢視編輯「完成百分比」：** 現在，您可以直接從「里程碑」檢視編輯專案和工作的「完成百分比」。\
   如需詳細資訊，請參閱 [使用里程碑檢視](../../../../reports-and-dashboards/reports/reporting-elements/use-milestone-view.md) in [使用里程碑檢視](../../../../reports-and-dashboards/reports/reporting-elements/use-milestone-view.md). 

## 更新數個系統設定頁面的外觀和風格

已更新「設定」區域的「系統」菜單中的以下頁面的外觀和風格（功能保持不變）:

* 診斷
* 單一登入(SSO)，包括：

   * 主動式目錄
   * LDAP
   * SAML 1.1
   * SAML 2.0

* 更新使用者以使用 SSO

## 更新「電子郵件設定」區域中的事件通知分組

「電子郵件設定」區域中「事件通知」的組織標題現在與使用者設定檔設定區域中使用的區段標題相符。

如需事件通知的詳細資訊，請參閱  [為系統中的每個人配置事件通知](../../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

## 選擇退出即時通知：內容摘要設定

下列選項現在可在即時電子郵件通知中使用。 這些選項僅適用於同時具有每日摘要對應項的即時通知：

* “將此項目新增到每日提要”
* &quot;停止此類電子郵件&quot;

現在，當您收到即時電子郵件通知時，可以將該通知新增至每日摘要通知，或完全取消訂閱該通知。

電子郵件通知中提供這些選項。 如需接收電子郵件通知的詳細資訊，請參閱 [Adobe Workfront通知](../../../../workfront-basics/using-notifications/wf-notifications.md)

## 各種電子郵件通知從「需要的動作」區段移至其他專案相關區段

數個通知已從使用者設定檔頁面的「需要的動作」區段移至其他區段，如下所示：

如需設定電子郵件通知的詳細資訊，請參閱 [啟用或停用您自己的事件通知](../../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md)

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>通知</strong> </th> 
   <th><strong>舊區段</strong> </th> 
   <th><strong>新區段</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>向我持有的專案新增了一個問題</td> 
   <td> <p> 需要動作 </p> </td> 
   <td>   <p>關於我擁有的專案資訊</p></td> 
  </tr> 
  <tr> 
   <td>向我所在的專案新增了一個問題</td> 
   <td>   <p>需要動作</p><p> </p></td> 
   <td> <p> 關於我擁有的專案資訊 </p>   </td> 
  </tr> 
  <tr> 
   <td>向我持有的專案新增未指派的問題</td> 
   <td>   <p>需要動作</p></td> 
   <td>   <p>關於我擁有的專案資訊</p></td> 
  </tr> 
  <tr> 
   <td> <p> 向我所在的專案新增了一個未指派問題 </p> </td> 
   <td> <p> 需要動作 </p>   </td> 
   <td> <p> 關於我擁有的專案資訊 </p>   </td> 
  </tr> 
  <tr> 
   <td> <p> 我的其中一項專案上的任務認可日期變更 </p> </td> 
   <td>   <p>需要動作</p></td> 
   <td>   <p>關於我擁有的專案資訊</p></td> 
  </tr> 
  <tr> 
   <td> <p> 認可日期因我專案上的一個問題變更 </p>   </td> 
   <td>   <p>需要動作</p></td> 
   <td> <p> 關於我擁有的專案資訊 </p>   </td> 
  </tr> 
  <tr> 
   <td> <p> 在指派給我的一項任務上變更了到期日期 </p> </td> 
   <td>   <p>需要動作</p></td> 
   <td>   <p>關於指派給我的工作資訊</p></td> 
  </tr> 
  <tr> 
   <td> <p> 在指派給我的問題上變更到期日期 </p> </td> 
   <td> <p> 需要動作 </p>   </td> 
   <td>   <p>關於指派給我的工作資訊</p></td> 
  </tr> 
  <tr> 
   <td> <p> 一項指派給我的任務狀態發生變更 </p>   </td> 
   <td> <p> 需要動作 </p>   </td> 
   <td> <p> 關於指派給我的工作資訊 </p>   </td> 
  </tr> 
 </tbody> 
</table>

## 新的資源規劃功能（R1的生產中不提供）

>[!NOTE]
>
>預覽環境目前提供此功能。 在R1發行到生產環境前大約一個月，它將從預覽環境中刪除。 然後，它將重新引入R2預覽1中的預覽環境。

 

為了支援未來的資源規劃功能，添加了以下更改：

* 在「人員」區域中，當前的「資源規劃」頁簽已更名為「舊資源規劃」。 
* 「人員」區域已導入新的「資源規劃」頁簽，將在其中開發新功能。\
   有關新的「資源規劃」頁簽的詳細資訊，請參閱 [開始使用資源規劃](../../../../resource-mgmt/resource-planning/get-started-resource-planning.md) 

* 當前的「資源池」對象已更名為「舊資源池」。\
   有關建立新的基於用戶的資源池的詳細資訊，請參見 [資源池概述](../../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md)

* 已建立新的「資源池」對象以支援新的（基於用戶的）資源池。

   >[!NOTE]
   * 如果當前正在運行現有舊資源池的報告，則現有報告將不會更改。
   * 如果要為現有（基於作業角色的）舊資源池建立新報告，則需要選擇「舊資源池」作為報告的對象。
   * 如果要為新的（基於用戶的）資源池建立新報告，則需要選擇「資源池」作為報告的對象。

  >   
