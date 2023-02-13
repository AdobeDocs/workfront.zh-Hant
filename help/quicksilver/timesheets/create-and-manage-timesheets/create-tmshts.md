---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: 建立單次使用的工時單
description: 如果希望時間表不是循環的，可以手動建立單次使用的時間表。 當到達工時單的結束日期，並且需要更多工時單時，必須建立新工時單。
author: Alina
feature: Timesheets
exl-id: b293dd50-a9b8-448b-afc1-8c7c7c79183b
source-git-commit: 210ca2e82286ff904bc7defb7b8c9c2559489d66
workflow-type: tm+mt
source-wordcount: '1090'
ht-degree: 1%

---

# 建立單次使用的工時單

如果希望時間表不是循環的，可以手動建立單次使用的時間表。 當到達工時單的結束日期，並且需要更多工時單時，必須建立新工時單。

有關建立工時單配置檔案以為用戶生成循環工時單而不需要您進一步干預（建議）的資訊，請參閱 [建立、編輯和分配工時單配置檔案](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

>[!NOTE]
>
>* 不能為組建立一次性工時單。

>  <!--
>  <span>Making sure with Lilit that this is correct</span>>
>  -->
>* 建立單次使用的工時單時，無法選擇要包含在工時單中的特定一般小時類型。 在系統中激活的所有常規小時類型都顯示在手動建立的工時表中。
>
>  如果您只想選擇某些一般小時類型以在工時單中顯示，請使用工時單配置檔案。 有關時間表配置檔案的詳細資訊，請參閱 [建立、編輯和分配工時單配置檔案](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

## 存取需求

您必須具備下列條件才能執行本文所述步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td> <p>計劃 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>必須具有對工時單的管理訪問權限。 </p> <p>如需詳細資訊，請參閱 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">授予用戶對特定區域的管理訪問權限</a>.</p> <p><b> 附註</b>

如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td>
</tr> 
 </tbody> 
</table>

*若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 建立單次使用的工時單

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角。

1. 按一下 **工時單**. 此 **全部** 依預設會選取篩選。 這將顯示您有權查看的所有工時單。

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
   >   * [使用版面範本自訂篩選器、檢視和群組](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)



1. （選用）按一下 **搜尋** 圖示 ![](assets/search-icon.png) 鍵入關鍵字並搜索特定時間表。 例如，您可以搜索所有者名稱的時間表時間範圍。

1. （選用）按一下 **檢視** ![](assets/view-icon.png) 或 **分組** ![](assets/grouping.png) 表徵圖，以應用不同的視圖或分組或建立新視圖。

   如需建立篩選器、檢視或群組的相關資訊，請參閱下列文章：

   * [在Adobe Workfront中建立或編輯篩選器](../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
   * [在Adobe Workfront中建立或編輯檢視](../../reports-and-dashboards/reports/reporting-elements/create-edit-views.md)
   * [在Adobe Workfront中建立群組](../../reports-and-dashboards/reports/reporting-elements/create-groupings.md)

1. 按一下 **新時間表** 時間表清單的頂部。

   指定下列資訊：

   <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
      <tr> 
      <td role="rowheader"><strong>建立以下項目的時程表：</strong> </td> 
      <td>開始輸入用戶、作業角色或要為其建立時間表的團隊的名稱，然後在清單中顯示時按一下它們。</td> 
      </tr> 
      <tr> 
      <td role="rowheader"><strong>從開始日期安排</strong> </td> 
      <td>這是時間表的開始日期。</td> 
      </tr> 
      <tr> 
      <td role="rowheader"><strong>結束日期</strong> </td> 
      <td> 這是工時單的結束日期。</td> 
      </tr> 
      <tr> 
      <td role="rowheader"><strong>核准者</strong> </td> 
      <td>批准者是批准與時間表關聯的用戶的時間表的用戶。 只能將具有時間表管理權限的用戶設定為批准者。 有關時間表管理權限的詳細資訊，請參閱 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">授予用戶對特定區域的管理訪問權限</a>.<br>開始輸入時間表批准者的名稱，並在清單中顯示時按一下它們。<br>時間表上可以有多個批准者。 在這種情況下，在某個批准者批准工時單後，工時單被標籤為 <strong>已關閉</strong> 它會從所有剩餘批准者的時間表批准清單中消失。</td> 
      </tr> 
      <tr> 
      <td role="rowheader"><strong>可編輯時間</strong> </td>

   <td> <p>如果要允許批准者編輯工時單上的工時，請選擇此選項。</p>

   此選項可與 **將時間表編輯限制給所有者和管理員** 在「設定」>「工時表和小時」>「首選項」區域中進行設定。 如需詳細資訊，請參閱 <a href="../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md">配置工時單和小時首選項</a>.

   存在下列情況：

   <ul>
      <li>當 <b>將時間表編輯限制給所有者和管理員</b> 選項：</li>
   <ul><li>批准者只能批准和拒絕時間表，無論 <b>可編輯時間</b> 是否啟用。 </li>
   <li>工時單所有者的經理只能查看其直接報表的工時單。</li></ul>
   <li>當 <b>將時間表編輯限制給所有者和管理員</b> 選項已停用：</li>
   <ul><li>當 <b>可編輯時間</b> 啟用後，批准者可以提交、重新開啟或關閉時間表，並可以編輯時間。</li>
   <li>當 <b>可編輯時間</b> 禁用時，批准者無法提交、重新開啟或關閉時間表，也無法編輯時間。 批准者只能批准或拒絕工時單。 </li>
   <li>工時單所有者的經理可以提交、重新調用、重新開啟和編輯其直接報告的工時單。</li></ul>
   </ul>

   <p><b>附註</b>

   一旦您提交工時單以進行審批，您就無法再編輯工時。 要將提交的時間表返回到可編輯狀態，請撤回時間表或讓審批人拒絕時間表。 如需詳細資訊，請參閱 <a href="../../timesheets/create-and-manage-timesheets/submit-timesheet-for-approval.md">提交時間表以進行批准</a> 和 <a href="../../timesheets/create-and-manage-timesheets/timesheet-approvals.md">批准工時單</a>.</p> </p>

   </td> 
      </tr>

   <tr>

   <td role="rowheader"><span style="font-weight: bold;">加班</span> </td> 
      <td>您可以選擇隱藏工時單上的「加班」框。 預設會停用此選項。</td> 
      </tr> 
      </tbody> 
   </table>

1. 按一下 **建立工時單**.

<!--the content in the table above will need to match the content in the Create timesheet profiles article-->

## 當任務和問題出現在用戶的工時單上時

如果任務或問題滿足以下任何條件，則分配給用戶的任務或問題將自動出現在用戶的時間表上：

* 用戶已登錄任務或問題的時數
* 任務或問題的計畫日期在時間表日期內
* 任務或問題具有實際起始日期（任務或問題狀態為「正在進行」）
* 任務或問題已固定到時間表
* 計畫完成日期在時間表的日期範圍內，且狀態為「正在進行」

若 **用預填時間表……** 首選項（位於「工時單」和「小時」首選項中）被取消選中，時間表將顯示狀態為「正在進行」的問題和任務。 有關「工時單和小時首選項」的詳細資訊，請參閱 [配置工時單和小時首選項](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).
