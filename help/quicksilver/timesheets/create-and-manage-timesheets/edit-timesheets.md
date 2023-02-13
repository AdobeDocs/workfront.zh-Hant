---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: 編輯工時單資訊
description: 作為具有時間表管理訪問權限的用戶，您可以編輯Adobe Workfront中現有時間表的資訊。 例如，您可以編輯工時單的「所有者」、「批准者」或時間範圍。
author: Alina
feature: Timesheets
exl-id: e6cffe81-ab45-4c34-aafe-2f947f9a67fd
source-git-commit: 210ca2e82286ff904bc7defb7b8c9c2559489d66
workflow-type: tm+mt
source-wordcount: '677'
ht-degree: 2%

---

# 編輯工時單資訊

作為具有時間表管理訪問權限的用戶，您可以編輯Adobe Workfront中現有時間表的資訊。 例如，您可以編輯工時單的「所有者」、「批准者」或時間範圍。

您可以編輯單個工時單的資訊，也可以批量編輯多個工時單。

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
   <td> <p>必須具有對工時單的管理訪問權限。 </p> <p>如需詳細資訊，請參閱 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">授予用戶對特定區域的管理訪問權限</a>.</p> <p>注意：如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 編輯工時單

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **工時單**.

   此 **全部** 預設情況下，會選擇篩選器，該篩選器顯示您有權查看的所有工時單。

   ![](assets/timesheet-list-one-timesheet-selected-nwe-350x70.png)

1. （選用）按一下 **搜尋** 圖示 ![](assets/search-icon.png) 鍵入關鍵字並搜索特定時間表。 例如，您可以搜索時間表時間範圍或所有者名稱。

1. （可選）執行下列操作之一以更新工時單清單中的篩選器：

   * 選擇 **我的時間表批准** 位於頁面的右上角，僅查看您批准的工時單

      或

      選擇 **我的工時單** 僅查看工時單。

      這會將「我的時間表批准」或「我的時間表」篩選器應用到時間表清單。

      ![](assets/my-timesheet-approvals-my-timesheets-pills-on-timesheets-list-nwe-350x58.png)

   * 按一下篩選圖示 ![](assets/filter-nwepng.png) 來套用不同的篩選，或建立新的篩選。 如需建立或更新篩選器的相關資訊，請參閱 [在Adobe Workfront中建立或編輯篩選器](../../reports-and-dashboards/reports/reporting-elements/create-filters.md).
   >[!NOTE]
   >
   >如果您的Workfront管理員或組管理員從「設定」區域的「清單控制項」或「佈局模板」中刪除了「我的時間表批准」和「我的時間表」篩選器，則「我的時間表批准」和「我的時間表」選項不會顯示在時間表清單的頂部或篩選器清單中。 如需詳細資訊，請參閱下列文章：
   * [使用版面範本自訂篩選器、檢視和群組](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)


1. （選用）按一下&#x200B;**檢視** ![](assets/view-icon.png) 或 **分組** ![](assets/grouping.png) 表徵圖，以應用不同的視圖或分組或建立新視圖。

   如需建立篩選器、檢視或群組的相關資訊，請參閱下列文章：

   * [在Adobe Workfront中建立或編輯篩選器](../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
   * [在Adobe Workfront中建立或編輯檢視](../../reports-and-dashboards/reports/reporting-elements/create-edit-views.md)
   * [在Adobe Workfront中建立群組](../../reports-and-dashboards/reports/reporting-elements/create-groupings.md)

1. 選取一或多個工時單，然後按一下 **編輯** 圖示 ![](assets/edit-icon.png) 在時間表清單的頂部。
1. 檢視或指定下列資訊：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>所有者</strong> </td> 
      <td> <p>這是為其建立工時單的用戶名。 您無法編輯此欄位。 </p> <p>選擇多個工時單時，不顯示該欄位。 </p> </td> 
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
      <td> <p>批准者是批准與時間表關聯的用戶的時間表的用戶。 只能將具有管理權限的時間表用戶設定為批准者。 </p> <p>有關時間表管理權限的詳細資訊，請參閱 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">授予用戶對特定區域的管理訪問權限</a>.</p> <p>開始輸入時間表批准者的名稱，並在清單中顯示時選擇它們。</p> <p>時間表上可以有多個批准者。 在這種情況下，在某個批准者批准工時單後，工時單被標籤為 <strong>已關閉</strong> 它會從所有剩餘批准者的時間表批准清單中消失。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>可編輯時間</strong> </td> 
      <td> <p>如果要允許批准者編輯工時單上的工時，請選擇此選項。</p> <p>選擇多個工時單時，此選項不可用。 </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span style="font-weight: bold;">加班</span> </td> 
      <td> <p>您可以選擇隱藏工時單上的「加班」框。</p> <p>預設會停用此選項。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下儲存。
