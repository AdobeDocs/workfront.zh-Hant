---
content-type: release-notes
navigation-topic: product-releases-archive
title: R1預覽5
description: 本頁說明R1 Preview 5版本中「預覽」環境的所有可用變更。 此頁面的功能已於2017年3月16日在預覽環境中推出。
author: Luke
feature: Product Announcements
exl-id: 4fba14b5-6c5a-4b03-99a7-f0e6f75807c3
source-git-commit: f6335f4e94d286681adfb50165562b2c41b5acac
workflow-type: tm+mt
source-wordcount: '1281'
ht-degree: 13%

---

# R1預覽5

本頁說明R1 Preview 5版本中「預覽」環境的所有可用變更。 此頁面的功能已於2017年3月16日在預覽環境中推出。

如需R1中所有變更的清單，請參閱 [R1發行活動概覽](../../../../product-announcements/product-releases/quarterly-release-archive/r1-release-activity/r1-release-activity-overview.md).

## 使用使用情況報告追蹤專案進度

現在，擁有專案管理存取許可權的使用者可以使用使用情況報告來追蹤專案進度。

使用率報表可讓您快速檢視特定周或月，或整體專案的實際時數如何與預算時數或計畫時數進行追蹤，讓專案保持在預算範圍內。 此外，您可以檢視每個類別（預算、計畫和實際）中依工作角色或個別使用者分類的時數詳細資訊。

如需有關追蹤專案使用率的詳細資訊，請參閱 [資源使用率報表概要](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

作為系統管理員，您可以配置使用者是否可以使用「使用率」標籤。 依預設，「使用率」索引標籤位於專案內的「更多」下拉式功能表中。 您可以將「使用率」標籤移至其他位置，或完全隱藏該標籤。 如果您已為您組織中的使用者定義了自訂版面配置範本，則需要手動將Utilization索引標籤新增到自訂版面配置範本。

如需有關設定「使用率」標籤位置的詳細資訊，請參閱建立和管理版面配置範本中的「自訂標籤」。

## 修改個別物件的現有全域核准流程

現在，當您將全域核准流程與物件相關聯時，可以修改現有的全域核准流程。 您所做的修改只會套用至關聯物件的核准程式。

如需詳細資訊，請參閱 [將新的或現有的核准流程與工作建立關聯](../../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md) 在 [將新的或現有的核准流程與工作建立關聯](../../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md)

## 設定報告以預設顯示新的甘特圖

您可以設定您建立的專案與任務報告，以預設使用新選項「預設在甘特圖檢視中顯示此報告」來顯示新的甘特圖。

如需有關設定報表以顯示新甘特圖的詳細資訊，請參閱 [編輯報表設定](../../../../reports-and-dashboards/reports/creating-and-managing-reports/edit-report-settings.md).

如需有關在專案報告和任務報告中檢視甘特圖的詳細資訊，請參閱 [檢視甘特圖中的資訊](../../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md)&quot; in [檢視甘特圖中的資訊](../../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md).

## 資源回收筒改善：任務和子任務已還原到先前的順序

現在，當您在刪除任務或子任務後恢復該任務或子任務時，該任務或子任務會恢復至其先前位置（位於任務清單中或父任務下方），其順序與刪除前出現的順序相同。

在此變更之前，已還原的任務和子任務一律會還原為最後一個任務（位於任務清單中或父任務下方），無論它們在被刪除之前出現的順序為何。

如需有關在Workfront中還原物件的詳細資訊，請參閱 [還原已刪除的專案](../../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

## 里程碑檢視改進

在「里程碑」檢視中檢視專案清單或專案報告時，現在提供下列改善專案：

* **設定是否在檢視中顯示進度狀態和完成百分比：** 有一個新選項可讓您設定進度狀態圖示是否顯示在里程碑檢視中。 此外，您也可以設定是否顯示與專案及任務相關的「完成百分比」資訊。\
  如需詳細資訊，請參閱 [使用里程碑檢視](../../../../reports-and-dashboards/reports/reporting-elements/use-milestone-view.md) 在 [使用里程碑檢視](../../../../reports-and-dashboards/reports/reporting-elements/use-milestone-view.md).

* **直接從「里程碑」檢視編輯完成百分比：** 現在您可以直接從「里程碑」檢視編輯專案和任務的完成百分比。\
  如需詳細資訊，請參閱 [使用里程碑檢視](../../../../reports-and-dashboards/reports/reporting-elements/use-milestone-view.md) 在 [使用里程碑檢視](../../../../reports-and-dashboards/reports/reporting-elements/use-milestone-view.md). 

## 更新數個系統設定頁面的外觀

已更新「設定」區域「系統」選單中下列頁面的外觀與風格（功能保持不變）：

* 診斷
* 單一登入(SSO)包括：

   * 主動式目錄
   * LDAP
   * SAML 1.1
   * SAML 2.0

* 更新使用者以使用 SSO

## 已更新電子郵件設定區域中的事件通知群組

電子郵件設定區域中事件通知的組織標題現在與使用者設定檔設定區域中使用的區段標題相符。

如需有關事件通知的詳細資訊，請參閱  [為系統中的每個人設定事件通知](../../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

## 選擇退出即時通知：內容摘要設定

立即電子郵件通知現在提供下列選項。 這些選項僅適用於也有每日文摘對應的即時通知：

* &quot;將此項目新增到每日摘要&quot;
* 「停止此型別的電子郵件」

現在，當您收到立即電子郵件通知時，您可以將該通知新增到每日摘要通知，或者您可以完全取消訂閱該通知。

這些選項可在電子郵件通知中使用。 如需接收電子郵件通知的詳細資訊，請參閱 [Adobe Workfront通知](../../../../workfront-basics/using-notifications/wf-notifications.md)

## 各種電子郵件通知已從「需要動作」區段移至其他專案相關區段

有幾個通知已從使用者設定檔頁面的「需要動作」區段移至其他區段，如下所示：

如需設定電子郵件通知的詳細資訊，請參閱 [修改您自己的電子郵件通知](../../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md)

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>通知</strong> </th> 
   <th><strong>舊區段</strong> </th> 
   <th><strong>新增章節</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>我擁有的專案中新增了一個問題</td> 
   <td> <p> 需要動作 </p> </td> 
   <td>   <p>我擁有的專案的相關資訊</p></td> 
  </tr> 
  <tr> 
   <td>我參與的專案中新增了一個問題</td> 
   <td>   <p>需要動作</p><p> </p></td> 
   <td> <p> 我擁有的專案的相關資訊 </p>   </td> 
  </tr> 
  <tr> 
   <td>我擁有的專案中新增了一個未指派的問題</td> 
   <td>   <p>需要動作</p></td> 
   <td>   <p>我擁有的專案的相關資訊</p></td> 
  </tr> 
  <tr> 
   <td> <p> 我參與的專案中新增了一個未指派問題 </p> </td> 
   <td> <p> 需要動作 </p>   </td> 
   <td> <p> 我擁有的專案的相關資訊 </p>   </td> 
  </tr> 
  <tr> 
   <td> <p> 我的專案中有一項任務的提交日期發生變更 </p> </td> 
   <td>   <p>需要動作</p></td> 
   <td>   <p>我擁有的專案的相關資訊</p></td> 
  </tr> 
  <tr> 
   <td> <p> 我的專案中有一個問題的提交日期發生變更 </p>   </td> 
   <td>   <p>需要動作</p></td> 
   <td> <p> 我擁有的專案的相關資訊 </p>   </td> 
  </tr> 
  <tr> 
   <td> <p> 指派給我的一項任務到期日發生變更 </p> </td> 
   <td>   <p>需要動作</p></td> 
   <td>   <p>指派給我的工作的相關資訊</p></td> 
  </tr> 
  <tr> 
   <td> <p> 我被指派處理的問題到期日發生變更 </p> </td> 
   <td> <p> 需要動作 </p>   </td> 
   <td>   <p>指派給我的工作的相關資訊</p></td> 
  </tr> 
  <tr> 
   <td> <p> 一項指派給我的任務狀態發生變更 </p>   </td> 
   <td> <p> 需要動作 </p>   </td> 
   <td> <p> 指派給我的工作的相關資訊 </p>   </td> 
  </tr> 
 </tbody> 
</table>

## 新的資源計畫功能（不適用於R1的生產環境）

>[!NOTE]
>
>此功能目前可在預覽環境中使用。 它將會在R1發行至生產環境前約一個月從預覽環境中移除。 然後，它將被重新引入R2 Preview 1中的預覽環境。

 

已新增下列變更，以支援未來的「資源規劃」功能：

* 目前的「資源規劃」標籤已重新命名為「人員」區域中的「舊版資源規劃」。 
* 在將要開發新功能的「人員」區域引入新的「資源規劃」標籤。\
  如需有關新「資源規劃」頁標的詳細資訊，請參閱 [開始使用資源規劃](../../../../resource-mgmt/resource-planning/get-started-resource-planning.md) 

* 目前的「資源集區」物件已重新命名為「舊版資源集區」。\
  如需有關建立新的使用者型資源集區的詳細資訊，請參閱 [資源集區概觀](../../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md)

* 已建立新的「資源集區」物件，以支援新的（以使用者為基礎的）資源集區。

  >[!NOTE]
  >
  >
  >   
  >   
  * 如果您目前正在現有舊版資源集區上執行報表，則現有報表不會變更。
  * 如果要為現有（職務角色型）舊版資源集區建立新報表，您必須選取「舊版資源集區」作為報表的物件。
  * 如果要為新的（以使用者為基礎的）資源集區建立新報告，您必須選取「資源集區」作為報告的物件。
  >   
  >
