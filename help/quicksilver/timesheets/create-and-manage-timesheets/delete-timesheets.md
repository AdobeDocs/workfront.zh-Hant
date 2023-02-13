---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: 刪除Adobe Workfront中的工時單
description: 您對時間表配置檔案所做的更改對於當前現有的時間表不立即有效，如建立、編輯和分配時間表配置檔案中所述。 要使更改在現有工時單上可見，必須刪除已生成的工時單，並生成新的工時單。 這僅適用於通過將時間表配置檔案與用戶關聯而生成的時間表。
author: Alina
feature: Timesheets
exl-id: c6a86c1b-8580-4896-8933-d4e2818e98ed
source-git-commit: 210ca2e82286ff904bc7defb7b8c9c2559489d66
workflow-type: tm+mt
source-wordcount: '810'
ht-degree: 0%

---

# 刪除Adobe Workfront中的工時單

您對時間表配置檔案所做的更改對於當前現有的時間表不立即有效，如 [建立、編輯和分配工時單配置檔案](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md). 要使更改在現有工時單上可見，必須刪除已生成的工時單，並生成新的工時單。 這僅適用於通過將時間表配置檔案與用戶關聯而生成的時間表。

>[!NOTE]
>
>通過重新生成工時單，無法重新建立手動建立的工時單，除非用戶自手動建立工時單以來已與工時單配置檔案關聯。 刪除手動建立的時間表可能導致資料丟失。 有關建立單個工時單的資訊，請參閱 [建立單次使用的工時單](../../timesheets/create-and-manage-timesheets/create-tmshts.md).

Adobe Workfront管理員或群組管理員可為系統中的每個人產生時間表。 有關手動生成工時單的詳細資訊，請參閱：

* [手動生成工時單](../../timesheets/create-and-manage-timesheets/manually-generate-timesheets.md)
* [建立和管理組的時間表配置檔案](../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-timesheet-profiles.md)

>[!IMPORTANT]
>
>* 無法恢復已刪除的時間表。
>* 建議您不要刪除過去的工時單，因為這些工時單不會根據工時單配置檔案自動生成。 如果希望新時間表中立即顯示對工時單配置檔案的更改，則可以刪除當前和將來的工時單並手動生成它們。
>* 刪除工時單時，系統不會刪除根據任務、問題和項目記錄的工時。 只有「一般時數」會隨時間表一起刪除。 在單獨的文本編輯器中，記下與時間表關聯的「一般小時數」。 刪除工時單後，您就可以將其記錄在新工時單中。
>


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
   <td> <p>必須具有對工時單的管理訪問權限。 </p> <p>如需詳細資訊，請參閱 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">授予用戶對特定區域的管理訪問權限</a>.</p> <p>如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 刪除清單中的工時單

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角。

1. 按一下 **工時單**. 此 **全部** 預設情況下，篩選器將被選中，它將顯示您有權查看的所有工時單。

   ![](assets/timesheet-list-one-timesheet-selected-nwe-350x70.png)

1. （可選）執行下列操作之一以更新工時單清單中的篩選器：

   * 選擇 **我的時間表批准** 位於頁面的右上角，僅查看您批准的工時單

      或

      選擇 **我的工時單** 僅查看工時單。

      這會將「我的時間表批准」或「我的時間表」篩選器應用到時間表清單。

      ![](assets/my-timesheet-approvals-my-timesheets-pills-on-timesheets-list-nwe-350x58.png)

   * 按一下篩選圖示 ![](assets/filter-nwepng.png) 來套用不同的篩選，或建立新的篩選。 如需建立或更新篩選器的相關資訊，請參閱 [在Adobe Workfront中建立或編輯篩選器](../../reports-and-dashboards/reports/reporting-elements/create-filters.md).
   >[!NOTE]
   如果您的Workfront管理員或組管理員從「設定」區域的「清單控制項」或「佈局模板」中刪除了「我的時間表批准」和「我的時間表」篩選器，則「我的時間表批准」和「我的時間表」選項不會顯示在時間表清單的頂部或篩選器清單中。 如需詳細資訊，請參閱下列文章：
   * [使用版面範本自訂篩選器、檢視和群組](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)


1. （選用）按一下 **檢視** ![](assets/view-icon.png) 或 **分組** ![](assets/grouping.png) 表徵圖，以應用不同的視圖或分組或建立新視圖。

   如需建立篩選器、檢視或群組的相關資訊，請參閱下列文章：

   * [在Adobe Workfront中建立或編輯篩選器](../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
   * [在Adobe Workfront中建立或編輯檢視](../../reports-and-dashboards/reports/reporting-elements/create-edit-views.md)
   * [在Adobe Workfront中建立群組](../../reports-and-dashboards/reports/reporting-elements/create-groupings.md)

1. 選擇要刪除的一個或多個時間表，然後按一下 **刪除**  ![](assets/delete.png) 表徵圖。

1. 按一下 **刪除**.

   選定的時間表被刪除，無法恢復。

   要生成新工時單，請確保用戶與工時單配置檔案相關聯，並請求Workfront管理員或組管理員生成新工時單。

   如需詳細資訊，請參閱下列內容：

   * [建立、編輯和分配工時單配置檔案](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md)
   * [手動生成工時單](../../timesheets/create-and-manage-timesheets/manually-generate-timesheets.md)
   * [建立和管理組的時間表配置檔案](../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-timesheet-profiles.md)

## 從工時單頁中刪除工時單

1. 按一下 [!UICONTROL **主菜單**] 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角。
1. 按一下要刪除的時間表以開啟它。
1. 按一下 [!UICONTROL **更多**] 圖示 ![](assets/more-icon.png) 在時間表名稱的右側，按一下 **刪除**.

   ![從工時單頁刪除工時單](assets/delete-timesheet-from-timesheet-page.png)
1. 按一下 [!UICONTROL **刪除**] 確認。

   時間表被刪除，無法恢復。
