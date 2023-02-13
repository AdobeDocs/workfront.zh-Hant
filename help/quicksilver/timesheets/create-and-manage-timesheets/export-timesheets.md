---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: 導出工時單清單
description: 作為人員管理員或時間表審批人，您可能需要下載時間表清單，以快速查看有關您負責的人員的時間表的資訊。 可通過導出時間表清單來執行此操作。
author: Alina
feature: Timesheets
exl-id: cb5b1c6c-7800-48f4-ae2c-c4007a161a6c
source-git-commit: 210ca2e82286ff904bc7defb7b8c9c2559489d66
workflow-type: tm+mt
source-wordcount: '536'
ht-degree: 2%

---

# 導出工時單清單

作為人員管理員或時間表審批人，您可能需要下載時間表清單，以快速查看有關您負責的人員的時間表的資訊。 可通過導出時間表清單來執行此操作。

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
   <td> <p>查看工時單或更高權限</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*若要了解您擁有的計畫或授權類型，請聯絡您的Workfront管理員。

## 導出工時單清單

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角。

1. 按一下 **工時單**. 此 **全部** 依預設會選取篩選。

   ![](assets/timesheet-list-one-timesheet-selected-nwe-350x70.png)

1. （選用）按一下 **搜尋** 圖示 ![](assets/search-icon.png) 鍵入關鍵字並搜索特定時間表。 例如，您可以搜尋時間集時間範圍或擁有者名稱。

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


1. （選用）按一下 **檢視** ![](assets/view-icon.png) 或 **分組** ![](assets/grouping.png) 表徵圖，以應用不同的視圖或分組或建立新視圖。

   如需建立篩選器、檢視或群組的相關資訊，請參閱下列文章：

   * [在Adobe Workfront中建立或編輯篩選器](../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
   * [在Adobe Workfront中建立或編輯檢視](../../reports-and-dashboards/reports/reporting-elements/create-edit-views.md)
   * [在Adobe Workfront中建立群組](../../reports-and-dashboards/reports/reporting-elements/create-groupings.md)

1. 選擇要導出的工時單，然後按一下 **匯出**  ![](assets/export-38x15.png) 表徵圖。

   ![](assets/all-timesheets-list-with-export-button-nwe-350x262.png)

1. 從以下選項中選擇要導出時間表清單的檔案類型：

   * PDF景觀
   * PDF縱向
   * PDF其他大小
   * Excel
   * Excel (xlsx)
   * 頁籤分隔檔

   時間表清單以選定格式下載到您的電腦，並包括以下時間表資訊：

   * 日期範圍
   * 所有者名稱
   * 總時數
   * 加班費
   * 批准者名稱
   * 狀態
