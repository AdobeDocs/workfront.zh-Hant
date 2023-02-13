---
content-type: overview
product-area: projects
navigation-topic: manage-tasks
title: 項目關鍵路徑概述
description: 決定專案的關鍵路徑是Adobe Workfront自動為專案中可能影響專案時間軸的一系列任務加上標籤的方式。 可能會影響項目時間軸的任務被標籤為關鍵路徑任務。
author: Alina
feature: Work Management
exl-id: 9cbc84bf-d02b-4bb7-8d5d-922554d1262e
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '771'
ht-degree: 0%

---

# 項目關鍵路徑概述

決定專案的關鍵路徑是Adobe Workfront自動為專案中可能影響專案時間軸的一系列任務加上標籤的方式。 可能會影響項目時間軸的任務被標籤為關鍵路徑任務。

以下功能會影響項目的關鍵路徑：

* 專案的工作劃分結構。

   如需「工作劃分結構」的詳細資訊，請參閱 [確定項目中的工作細分結構](../../../manage-work/projects/planning-a-project/determine-project-work-breakdown-structure.md)

* 每個任務完成所需的時間（持續時間）。
* 任務之間的依賴項。

   請考量下列事項：

   * 當關鍵路徑上的任務具有前置關係時，如果前置任務或後置任務的日期更改直接影響其家屬，則其前置任務和後置任務也處於關鍵路徑上。

      >[!TIP]
      >
      >當任務的後續日期不直接影響其從屬任務的日期，也不影響項目的日期時，後續任務不在關鍵路徑上。
      >
      >
      >![](assets/successor-not-on-critical-path-350x150.png)     >

   * 將子任務標識為關鍵路徑任務時，如果父任務的預計起始日期和時間與子任務的預計起始日期和時間相同，則父任務也標識為關鍵路徑任務。

考慮到這些特性，系統通過使用最早任務與確定項目結束的任務之間的最長路徑來計算關鍵路徑。 關鍵路徑計算考慮了每個任務可以開始和完成的最早和最晚時間，而不會使項目更長。 此過程確定哪些任務是「關鍵」（屬於最長路徑），哪些任務具有「總浮點數」（可以延遲，而不使項目更長）。

關鍵路徑上任務活動的任何延遲都直接影響項目的預計完成日期（關鍵路徑上沒有浮點）。

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
   <td> <p>工作或更高</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>查看或更高程度地訪問任務</p> <p>注意：如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>查看任務的或更高權限 </p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 查看關鍵路徑

您可以在Workfront應用程式的以下區域中查看屬於關鍵路徑的任務：

* [在甘特圖中查看關鍵路徑](#view-the-critical-path-in-the-gantt-chart)
* [在任務清單或報告中查看關鍵路徑](#view-the-critical-path-in-a-task-list-or-report)

### 在甘特圖中查看關鍵路徑 {#view-the-critical-path-in-the-gantt-chart}

要在甘特圖中查看關鍵路徑上的任務：

1. 轉到要查看其關鍵路徑的項目。
1. 按一下 **工作** 中。
1. 按一下 **甘特圖** 表徵圖。

   ![甘特圖表表徵圖__1_.png](assets/gantt-chart-icon--1-.png)

1. 展開 **選項** ，然後啟用 **關鍵路徑** 選項。

   關鍵路徑上的任務在甘特圖中其時間軸上方有一條紅線。

   ![critical_path_on_gantt__1_.png](assets/crtitical-path-on-gantt--1--350x137.png)

### 在任務清單或報告中查看關鍵路徑 {#view-the-critical-path-in-a-task-list-or-report}

要查看任務清單中關鍵路徑上的任務，請執行以下操作：

1. 轉到要查看其關鍵路徑的項目。
1. 按一下 **工作** 中。
1. 從 **檢視** 下拉式功能表，選取 **狀態**.

   關鍵路徑上的任務具有 **關鍵路徑** 旗標 **標幟** 欄。

   您可以將相同的檢視套用至任務報表。

   如需建立報表的詳細資訊，請參閱文章 [建立自訂報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

   或

   從 **篩選** 下拉式功能表，選取 **新增篩選**.

1. 按一下 **新增篩選規則** 開始輸入 **關鍵** 在 **僅顯示……** 欄位。

1. 在清單中出現時選取它。
1. 按一下 **儲存篩選**.

   清單應僅顯示關鍵路徑上的任務。
