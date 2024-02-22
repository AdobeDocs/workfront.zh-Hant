---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: 提交時程表以供核准
description: 提交您的時程表以供核准，讓您的經理可以檢視您的工作時間。 核准者可以確認所有記錄時間均已分配至正確的區域，且已為該時段記錄足夠的時數。
author: Alina
feature: Timesheets
exl-id: 253e20c8-58f8-4b23-a769-b0e36557066a
source-git-commit: afbf2e2fbfcc2c527223da008518bc7632872c23
workflow-type: tm+mt
source-wordcount: '894'
ht-degree: 0%

---

# 提交時程表以供核准

提交您的時程表以供核准，讓您的經理可以檢視您的工作時間。 核准者可以確認所有記錄時間均已分配至正確的區域，且已為該時段記錄足夠的時數。

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>評論或以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>檢視任務或問題的存取權或以上許可權</p> <p>如果您還是沒有存取權，請詢問您的Workfront管理員，他們是否在您的存取層級中設定其他限制。 如需有關Workfront管理員如何修改您的存取層級的資訊，請參閱 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>檢視或更高的任務和問題許可權</p> <p>如需請求其他存取許可權的詳細資訊，請參閱 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">要求物件的存取權 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的Workfront管理員。

## 提交時程表以供核准

* [提交時程表以供核准](#submit-a-timesheet-for-approval)
* [檢視已提交時程表的狀態](#view-the-status-of-a-submitted-timesheet)

### 提交時程表以供核准

在時程表核准者設定後（如一節所述） [指定時程表核准者](../../timesheets/create-and-manage-timesheets/timesheet-approvals.md#designating-a-timesheet-approver) 在文章中 [核准時間表](../../timesheets/create-and-manage-timesheets/timesheet-approvals.md))， **關閉** 時程表底部的按鈕變更為 **提交以進行核准** 按鈕。

若要提交時程表以供核准，請執行下列步驟：

1. 移至已設定為擁有核准者的時程表。
1. 記錄時間，如所述 [記錄時間](../../timesheets/create-and-manage-timesheets/log-time.md).
1. 按一下 **提交以進行核准** 以啟動時程表核准流程。

   ![](assets/submit-for-approval-button-on-timesheet-nwe.png)

   此 **提交以進行核准** 按鈕已取代為 **核准**， **拒絕**、和 **恢復** 按鈕。 時程表的狀態變更為 **已提交**.

   當您提交時程表以供核準時，核准者會看到 **核准** 區域 **首頁** 頁面。 可能會發生下列情況：

   * 如果他們核准， **恢復** 按鈕變更為 **重新開啟** 和時程表狀態更新至 **開啟**.
   * 如果他們拒絕， **提交以進行核准** 按鈕取代 **恢復** 按鈕和時程表狀態更新為 **已拒絕**.

1. （選用）按一下 **恢復** 如果您需要重新開啟時程表並更新時間。 如需詳細資訊，請參閱 [撤回時程表](#recall-a-timesheet) 一節。

### 檢視已提交時程表的狀態 {#view-the-status-of-a-submitted-timesheet}

您可以在提交時程表後檢視其狀態。

如果Workfront管理員已啟用「使用者的時程表核准」和「使用者的時程表拒絕」事件處理常式，在核准或拒絕時程表後，您會收到通知。 如需啟用事件通知的詳細資訊，請參閱 [事件通知型別](../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

如果沒有這些通知，您可以在Workfront的時程表區域中瞭解已提交時程表的狀態。

若要檢視時程表的狀態：

1. 按一下 **主要功能表** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角。
1. 按一下 **時間表**. 此 **全部** 依預設會選取篩選器。

   ![](assets/timesheet-list-one-timesheet-selected-nwe-350x70.png)

1. （選用）執行下列任一項作業，更新時程表清單中的篩選器：

   * 選取 **我的時程表核准** 在頁面的右上角，僅檢視您核准的時程表

     或

     選取 **我的時間表** 以僅檢視您的時間表。

     這會套用我的時程表核准或我的時程表篩選器到時程表清單。

     ![](assets/my-timesheet-approvals-my-timesheets-pills-on-timesheets-list-nwe-350x58.png)

   * 按一下篩選器圖示 ![](assets/filter-nwepng.png) 以套用不同的篩選，或建立新的篩選。 如需建立或更新篩選的資訊，請參閱 [在Adobe Workfront中建立或編輯篩選器](../../reports-and-dashboards/reports/reporting-elements/create-filters.md).

   >[!NOTE]
   >
   >如果您的Workfront管理員或群組管理員從「設定」區域的「清單控制項」或您的「版面配置範本」中移除了「我的時程表核准」和「我的時程表」，則「我的時程表核准」和「我的時程表」選項不會顯示在時程表清單頂端或篩選器清單中。 如需詳細資訊，請參閱下列文章：
   >
   >   
   >   
   >   * [使用版面配置範本自訂篩選器、檢視和群組](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)
   >   
   >

1. （視條件而定）如果您已選取 **我的時間表**，確認 **標準** 已套用檢視，請留意 **狀態** 欄。

   時程表可能有下列狀態：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">未結</td> 
      <td> <p>您的時程表目前未完成，您可以記錄時間。 </p> <p>已召回的時程表會顯示為「開啟」狀態。 如需詳細資訊，請參閱 <a href="#recall-a-timesheet" class="MCXref xref">撤回時程表</a> 一節。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">已提交</td> 
      <td>您已提交時程表以供核准，但尚未獲得核准。 您可以撤回已提交的時程表以繼續編輯。 如需詳細資訊，請參閱 <a href="#recall-a-timesheet" class="MCXref xref">撤回時程表</a> 一節。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">已關閉</td> 
      <td> <p>存在下列情況：</p> 
       <ul> 
        <li> <p>如果時程表沒有核准者，則您已儲存時間並將其關閉。</p> </li> 
        <li> <p>如果時程表有核准者，則表示您已提交該時程表以供核准，且該時程表已核准。</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">已拒絕</td> 
      <td>您已提交時程表進行核准，但核准者拒絕了。</td> 
     </tr> 
    </tbody> 
   </table>

## 撤回時程表 {#recall-a-timesheet}

您可以撤回已提交核准的時程表。 只有尚未核准的時程表才能撤銷。

若要撤回時程表：

1. 按一下 **主要功能表** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角。

1. 按一下 **時間表**.
1. 按一下 **我的時間表** 在熒幕右上角或選取 **我的時間表** 從 **篩選** ![](assets/filter-nwepng.png) 下拉式功能表。
1. 按一下狀態為的時程表的時間範圍 **已提交**.
1. 按一下 **恢復**.

   時程表再次變為可編輯，其狀態變更為 **開啟**.
