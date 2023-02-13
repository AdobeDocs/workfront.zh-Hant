---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: 提交時間表以進行批准
description: 將時間表提交以進行批准，使您的經理能夠洞察您的工作時間。 批准者可以驗證所有記錄的時間都已分配到正確的區域，並且已記錄足夠的小時數。
author: Alina
feature: Timesheets
exl-id: 253e20c8-58f8-4b23-a769-b0e36557066a
source-git-commit: 210ca2e82286ff904bc7defb7b8c9c2559489d66
workflow-type: tm+mt
source-wordcount: '897'
ht-degree: 0%

---

# 提交時間表以進行批准

將時間表提交以進行批准，使您的經理能夠洞察您的工作時間。 批准者可以驗證所有記錄的時間都已分配到正確的區域，並且已記錄足夠的小時數。

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

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
   <td> <p>審核或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>查看對任務和問題的訪問權限或更高權限</p> <p>如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>檢視工作和問題的權限或更高權限</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 提交時間表以進行批准

* [提交時間表以進行批准](#submit-a-timesheet-for-approval)
* [查看已提交時間表的狀態](#view-the-status-of-a-submitted-timesheet)

### 提交時間表以進行批准

設定工時單審批者後(如 [指定工時單批准者](../../timesheets/create-and-manage-timesheets/timesheet-approvals.md#designating-a-timesheet-approver) 在文章中 [批准工時單](../../timesheets/create-and-manage-timesheets/timesheet-approvals.md)), **關閉** 時間表底部的按鈕將更改為 **提交以進行核准** 按鈕。

要提交時間表以進行審批，請執行以下操作：

1. 轉到已配置為具有批准者的時間表。
1. 記錄時間，如 [記錄時間](../../timesheets/create-and-manage-timesheets/log-time.md).
1. 按一下 **提交以進行核准** 啟動工時單審批流程。

   ![](assets/submit-for-approval-button-on-timesheet-nwe.png)

   此 **提交以進行核准** 按鈕被取代 **核准**, **拒絕**，和 **召回** 按鈕。 時間表的狀態更改為 **已提交**.

   提交工時單以進行審批時，審批人將查看 **核准** 區域 **首頁** 頁面。 可能發生下列情況：

   * 如果他們同意， **召回** 按鈕變更為 **重新開啟** 時間表狀態更新至 **開啟**.
   * 如果他們拒絕， **提交以進行核准** 按鈕會取代 **召回** 按鈕和工時單狀態更新至 **已拒絕**.

1. （選用）按一下 **召回** 如果您需要重新開啟時間表並更新時間。 如需詳細資訊，請參閱 [召回工時單](#recall-a-timesheet) 一節。

### 查看已提交時間表的狀態 {#view-the-status-of-a-submitted-timesheet}

在提交時間表後，您可以查看時間表的狀態。

如果Workfront管理員啟用了「用戶的工時單批准」和「用戶的工時單拒絕」事件處理程式，則在工時單被批准或拒絕後，將通知您。 如需啟用事件通知的相關資訊，請參閱 [Adobe Workfront中提供的事件通知](../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

沒有這些通知，您可以在Workfront的「工時單」區域中了解提交的工時單的狀態。

要查看時間表的狀態，請執行以下操作：

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角。
1. 按一下 **工時單**. 此 **全部** 依預設會選取篩選。

   ![](assets/timesheet-list-one-timesheet-selected-nwe-350x70.png)

1. （可選）執行下列操作之一以更新工時單清單中的篩選器：

   * 選擇 **我的時間表批准** 位於頁面的右上角，僅查看您批准的工時單

      或

      選擇 **我的工時單** 僅查看工時單。

      這會將「我的時間表批准」或「我的時間表」篩選器應用到時間表清單。

      ![](assets/my-timesheet-approvals-my-timesheets-pills-on-timesheets-list-nwe-350x58.png)

   * 按一下篩選圖示 ![](assets/filter-nwepng.png) 來套用不同的篩選，或建立新的篩選。 如需建立或更新篩選器的相關資訊，請參閱 [在Adobe Workfront中建立或編輯篩選器](../../reports-and-dashboards/reports/reporting-elements/create-filters.md).
   >[!NOTE]
   >
   >如果您的Workfront管理員或組管理員從「設定」區域的「清單控制項」或「佈局模板」中刪除了「我的時間表批准」和「我的時間表」篩選器，則「我的時間表批准」和「我的時間表」選項不會顯示在時間表清單的頂部或篩選器清單中。 如需詳細資訊，請參閱下列文章：
   >
   >   
   >   
   >   * [使用版面範本自訂篩選器、檢視和群組](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)


1. （條件性）如果您選取 **我的工時單**，請確定 **標準** 檢視已套用，請注意 **狀態** 欄。

   工時單可能具有以下狀態：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">開啟</td> 
      <td> <p>您的時間表當前處於開啟狀態，您可以記錄時間。 </p> <p>已調回的時間表顯示為「開啟」狀態。 如需詳細資訊，請參閱 <a href="#recall-a-timesheet" class="MCXref xref">召回工時單</a> 一節。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">已提交</td> 
      <td>您提交了時間表以進行批准，但尚未批准。 您可以重新調用提交的時間表以繼續編輯它。 如需詳細資訊，請參閱 <a href="#recall-a-timesheet" class="MCXref xref">召回工時單</a> 一節。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">已關閉</td> 
      <td> <p>存在下列情況：</p> 
       <ul> 
        <li> <p>如果時間表沒有批准者，您將保存時間並將其關閉。</p> </li> 
        <li> <p>如果時間表有批准者，則您已提交它以進行批准，並且它已被批准。</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">已拒絕</td> 
      <td>您提交了時間表進行審批，審批人拒絕了它。</td> 
     </tr> 
    </tbody> 
   </table>

## 召回工時單 {#recall-a-timesheet}

您可以重新調用已提交以供審批的時間表。 只能回收未獲批准的時間表。

要重新調用時間表，請執行以下操作：

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角。

1. 按一下 **工時單**.
1. 按一下 **我的工時單** 或選取 **我的工時單** 從 **篩選** ![](assets/filter-nwepng.png) 下拉式功能表。
1. 按一下狀態為 **已提交**.
1. 按一下 **召回**.

   工時單將重新變為可編輯狀態，其狀態將更改為 **開啟**.
