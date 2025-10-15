---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: 提交時程表以供核准
description: 提交您的時程表以供核准，讓您的經理可以檢視您的工作時間。 核准者可以確認所有記錄時間均已分配至正確的區域，且已為該時段記錄足夠的時數。
author: Lisa
feature: Timesheets
exl-id: 253e20c8-58f8-4b23-a769-b0e36557066a
source-git-commit: 69cd5fb1d089b81b7a1673609b92537137b6b68e
workflow-type: tm+mt
source-wordcount: '839'
ht-degree: 0%

---

# 提交時程表以供核准

<!--Audited: 8/2024-->

提交您的時程表以供核准，讓您的經理可以檢視您的工作時間。 核准者可以確認所有記錄時間均已分配至正確的區域，且已為該時段記錄足夠的時數。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront套件</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront授權</td> 
   <td> <p>淺色或更高 </p>
   <p>評論或以上 </p>
  </tr> 
  <tr> 
   <td>存取層級設定</td> 
   <td> <p>檢視或更高的任務和問題存取權 </p> </td> 
  </tr> 
  <tr> 
   <td>物件許可權</td> 
   <td> <p>檢視或更高的時程表許可權</p> </td> 
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 提交時程表以供核准

* [提交時程表以供核准](#submit-a-timesheet-for-approval)
* [檢視已提交時程表的狀態](#view-the-status-of-a-submitted-timesheet)

### 提交時程表以供核准

在時程表核准者設定之後（如文章[核準時程表](../../timesheets/create-and-manage-timesheets/timesheet-approvals.md#designating-a-timesheet-approver)中的[指定時程表核准者](../../timesheets/create-and-manage-timesheets/timesheet-approvals.md)一節中所述），時程表底部的&#x200B;**關閉**&#x200B;按鈕變更為&#x200B;**提交核准**&#x200B;按鈕。

若要提交時程表以供核准，請執行下列步驟：

1. 移至已設定為擁有核准者的時程表。
1. 記錄時間，如[記錄時間](../../timesheets/create-and-manage-timesheets/log-time.md)中所述。
1. 按一下&#x200B;**提交以進行核准**&#x200B;以啟動時程表核准流程。

   ![](assets/submit-for-approval-button-on-timesheet-nwe.png)

   **提交以供核准**&#x200B;按鈕已由&#x200B;**核准**、**拒絕**&#x200B;和&#x200B;**撤銷**&#x200B;按鈕取代。 時程表的狀態變更為&#x200B;**已提交**。

   當您的時程表提交以進行核準時，核准者會在&#x200B;**首頁**&#x200B;區域的&#x200B;**我的核准** Widget中看到時程表清單。 可能會發生下列情況：

   * 如果他們核准，**撤銷**&#x200B;按鈕將變更為&#x200B;**重新開啟**，而時程表狀態更新為&#x200B;**開啟**。
   * 如果他們拒絕它，則&#x200B;**提交以進行核准**&#x200B;按鈕會取代&#x200B;**撤銷**&#x200B;按鈕和時程表狀態更新為&#x200B;**已拒絕**。

1. （選擇性）如果您需要重新開啟時程表並更新您的時間，請按一下&#x200B;**撤銷**。 如需詳細資訊，請參閱本文中的[撤回時間表](#recall-a-timesheet)區段。

### 檢視已提交時程表的狀態 {#view-the-status-of-a-submitted-timesheet}

您可以在提交時程表後檢視其狀態。

如果Workfront管理員已啟用「使用者的時程表核准」和「使用者的時程表拒絕」事件處理常式，在核准或拒絕時程表後，您會收到通知。 如需啟用事件通知的詳細資訊，請參閱[事件通知型別](../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md)。

如果沒有這些通知，您可以在Workfront的時程表區域中瞭解已提交時程表的狀態。

若要檢視時程表的狀態：

1. 按一下Adobe Workfront右上角的&#x200B;**主要功能表**&#x200B;圖示![](assets/main-menu-icon.png)。
1. 按一下&#x200B;**時程表**。 依預設會選取&#x200B;**全部**&#x200B;篩選器。

   ![](assets/timesheet-list-one-timesheet-selected-nwe-350x70.png)

1. （選用）執行下列任一項作業，更新時程表清單中的篩選器：

   * 選取頁面右上角的&#x200B;**我的時程表核准**，僅檢視您核准的時程表

     或

     選取&#x200B;**我的時程表**&#x200B;以僅檢視您的時程表。

     這會套用我的時程表核准或我的時程表篩選器到時程表清單。

     ![](assets/my-timesheet-approvals-my-timesheets-pills-on-timesheets-list-nwe-350x58.png)

   * 按一下「篩選」圖示![](assets/filter-nwepng.png)以套用不同的篩選，或建立新的篩選。 如需建立或更新篩選的資訊，請參閱[在Adobe Workfront中建立或編輯篩選器](../../reports-and-dashboards/reports/reporting-elements/create-filters.md)。

   >[!NOTE]
   >
   >如果您的Workfront管理員或群組管理員從「設定」區域的「清單控制項」或您的「版面配置範本」中移除了「我的時程表核准」和「我的時程表」，則「我的時程表核准」和「我的時程表」選項不會顯示在時程表清單頂端或篩選器清單中。 如需詳細資訊，請參閱下列文章：
   >
   >   
   >   
   >   * [使用配置範本自訂篩選器、檢視和群組](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)
   >   
   >

1. （視條件而定）若您選取&#x200B;**我的時程表**，請確定已套用&#x200B;**標準**&#x200B;檢視，並注意&#x200B;**狀態**&#x200B;欄。

   時程表可能有下列狀態：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">開啟</td> 
      <td> <p>您的時程表目前未完成，您可以記錄時間。 </p> <p>已召回的時程表會顯示為「開啟」狀態。 如需詳細資訊，請參閱本文中的<a href="#recall-a-timesheet" class="MCXref xref">撤回時間表</a>區段。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">已提交</td> 
      <td>您已提交時程表以供核准，但尚未獲得核准。 您可以撤回已提交的時程表以繼續編輯。 如需詳細資訊，請參閱本文中的<a href="#recall-a-timesheet" class="MCXref xref">撤回時間表</a>區段。 </td> 
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

1. 按一下Adobe Workfront右上角的&#x200B;**主要功能表**&#x200B;圖示![](assets/main-menu-icon.png)。

1. 按一下&#x200B;**時程表**。
1. 按一下畫面右上角的&#x200B;**我的時程表**，或從&#x200B;**篩選器** **下拉式選單中選取**&#x200B;我的時程表![](assets/filter-nwepng.png)。
1. 按一下狀態為&#x200B;**已提交**&#x200B;之時程表的時間範圍。
1. 按一下&#x200B;**撤銷**。

   時程表再次變為可編輯，其狀態變更為&#x200B;**開啟**。
