---
product-area: reporting;user-management
keywords: 儲存，新，報表，複製
navigation-topic: create-and-manage-reports
title: 建立報表副本
description: 您可以建立任何您有權存取之報表的復本。 您可以建立自訂報表的確切副本，或儲存新版本的預設報表。 複製報表後，您會成為複製報表的擁有者，報表會顯示在「我的報表」區段中。
author: Nolan
feature: Reports and Dashboards
exl-id: 84737f48-efc5-45f1-acd1-b9f5d353f80f
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '682'
ht-degree: 0%

---

# 建立報表副本

您可以建立任何您有權存取之報表的復本。 您可以建立自訂報表的確切副本，或儲存新版本的預設報表。 複製報表後，您會成為複製報表的擁有者，報表會顯示在「我的報表」區段中。

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
   <td> <p>計劃 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>編輯對報表、控制面板、日曆的存取</p> <p>編輯對篩選器、檢視、群組的存取</p> <p>注意：如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>檢視報表的權限</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 建立報表的精確副本

如果您想要製作報表副本（您是的擁有者），請執行下列作業：

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角。

1. 按一下 **報表**，然後&#x200B;**所有報表**.
1. 開啟報表。
1. 按一下 **報表動作**，然後 **複製**.

   >[!TIP]
   >
   >如果報表為預設報表，則「複製」選項不會出現在「報表動作」功能表中。\
   >如需如何建立預設報表副本的詳細資訊，請參閱 [建立新版本的報表](#create-a-new-version-of-a-report).

   ![複製報表](assets/nwe-fulllistofreportactions-2022.png)

   原始報表的復本會以 *副本 [原始報表的名稱]*. 例如，「第4季度已完成任務」報表的名稱會是「第4季度已完成任務的副本」。

1. （選用）若要重新命名報表，請開始輸入新名稱。

   >[!TIP]
   >
   >如果您在輸入新名稱之前取消選取標題，請選取報表標題、刪除名稱，然後輸入新名稱。

1. （選用）若要與其他使用者共用新版本的報表，請按一下 **報表動作**，然後 **共用**.

   >[!NOTE]
   >
   >共用資訊不會從原始版本轉移至複製的報表。\
   >如需如何查看上次報表共用給誰的詳細資訊，請參閱 [建立報告活動的報告](../../../reports-and-dashboards/reports/report-usage/create-report-reporting-activities.md#identify).

1. （選用）如果您對原始報表具有「管理」權限，而不再需要原始報表，則可以刪除該權限，以移除Workfront中不必要的重複報表。

   要刪除原始報告，請執行以下操作：

   1. 導覽至報表。
   1. 按一下 **報表動作**，然後 **刪除**.

   1. 按一下 **是，刪除它** 確認您要刪除報表。

## 建立新版本的報表 {#create-a-new-version-of-a-report}

如果要建立預設報表的復本，請執行下列操作：

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角。

1. 按一下 **報表**，然後&#x200B;**所有報表**.
1. 按一下預設報表的名稱以開啟它。
1. 按一下 **報表動作**，然後 **編輯**.

   ![編輯報表](assets/nwe-reportactionsfordefaultreport-2022.png)

1. 在報表的下列標籤中進行任何您需要的修改：

   * **欄（檢視）**:如需自訂檢視的詳細資訊，請參閱文章 [Adobe Workfront中的檢視概觀](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).
   * **分組**:如需自訂群組的詳細資訊，請參閱文章 [Adobe Workfront中的群組概觀](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).
   * **篩選器**:如需自訂篩選器的詳細資訊，請參閱文章 [Adobe Workfront中的篩選器概觀](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).
   * **圖表**:如需自訂報表圖表的詳細資訊，請參閱文章 [新增圖表至報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

1. 在右上角，按一下 **報表設定**.
1. 在 **報表標題** 欄位中，為報表指定新名稱。
1. 按一下 **完成**.
1. 按一下 **另存為新報表**.

   ![](assets/nwe-save-as-new-report-350x220.png)

1. （選用）若要與其他使用者共用新版本的報表，請按一下 **報表動作**，然後 **共用**.
