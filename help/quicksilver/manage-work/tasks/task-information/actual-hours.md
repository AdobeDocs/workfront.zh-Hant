---
content-type: overview
product-area: projects
navigation-topic: task-information
title: 查看實際小時數
description: 您在Adobe Workfront中登入工作項目的小時數視為實際小時數。
author: Alina
feature: Work Management
exl-id: c4b0e431-1765-416d-89f5-6ac663ac1d4f
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '796'
ht-degree: 0%

---

# 查看實際小時數

您在Adobe Workfront中登入工作項目的小時數視為實際小時數。

實際小時數表示完成任務、問題或項目所花的實際時間。

我們建議您在工作項目上記錄數小時，這些是任務和問題。

不過，身為Workfront管理員，您也可以根據您組織中的工作流程，讓使用者登入專案的時間。

有關如何設定系統以允許用戶登錄項目的詳細資訊，請參閱 [配置工時單和小時首選項](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

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
   <td> <p>查看或更高程度地訪問任務、項目或問題</p> <p>注意：如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>查看任務、項目或問題的或更高權限</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 任務和問題的實際小時數與項目的實際小時數

任務和問題的實際小時數表示直接記錄任務和問題的小時數。

>[!NOTE]
>
>子任務的實際小時數累計到父任務的實際小時數。 以下公式適用於父任務的實際小時數：

```
Parent Task Actual Hours = All Tasks Actual Hours + Parent Task Actual Hours
```

項目的實際小時數表示項目上所有任務的實際小時數總計（包括直接登錄父項任務的小時數）、項目上的所有問題以及項目本身的實際小時數。

以下公式適用於項目的實際小時數：

```
Project Actual Hours = All Tasks Actual Hours + All Issues Actual Hours + All Project Actual Hours
```

## 查找實際小時數

查找項目的「實際小時數」值對於任務、項目和問題相同。

您可以在以下位置找到有關任務的「實際小時數」資訊：

* [「詳細資訊」部分中的實際小時數](#actual-hours-in-the-details-section)
* [「小時」部分中的實際小時數](#actual-hours-in-the-hours-section)
* [報表中的實際小時數](#actual-hours-in-reports)
* [資源管理工具中的實際小時數](#actual-hours-in-resource-management-tools)

### 「詳細資訊」部分中的實際小時數 {#actual-hours-in-the-details-section}

對於專案、工作和問題，「詳細資料」區段中的「尋找實際小時數」是相同的。

要查找任務詳細資訊中的實際小時數，請執行以下操作：

1. 轉到要複查實際小時數的任務。
1. 按一下 **任務詳細資訊** 中。
1. 按一下 **概述** 並注意 **實際小時數** 值。

   這是此任務記錄的總小時數。

### 「小時」部分中的實際小時數 {#actual-hours-in-the-hours-section}

對於專案、任務和問題，「小時」區段中的「尋找實際小時數」是相同的。

若要找出「小時數」區段中的實際小時數：

1. 轉到要複查實際小時數的任務。
1. 按一下 **小時** 中。

   視您的設定而定，「小時」區段可能會列在 **顯示更多**.

   這將顯示任務上記錄的小時條目清單。

1. 確保 **標準** 檢視和 **專案** 分組會套用至此清單。

   在分組行中顯示的數字 **小時** column是任務的「實際小時數」總數。

### 報表中的實際小時數 {#actual-hours-in-reports}

在建立任務、問題或項目報告時，您可以在報告中顯示每個任務、問題或項目的實際小時數值。

將「實際小時數」欄新增至任務檢視，類似於在報表中建立檢視。

要在任務報表中顯示實際小時數，請執行以下操作：

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Workfront的右上角，然後按一下 **報表**.
1. 按一下 **新增報表**，然後選擇 **任務** 作為物件。

1. 按一下 **添加列**，然後開始輸入 **實際小時數** 當 **顯示在此列中** 下拉式欄位隨即顯示。 選取欄位出現在清單中時。

1. 按一下 **儲存+關閉** 以儲存報表。

   「實際小時數」列顯示每個任務記錄的小時數。

### 資源管理工具中的實際小時數 {#actual-hours-in-resource-management-tools}

如果您想查看用戶在其分配的任務和問題上的工作進展，則可以在以下資源管理工具中查看它們：

* 利用率報告。\
   有關利用率報告的資訊，請參見 [資源利用率報告概覽](../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

* 資源規劃工具.

   有關在資源計畫器中查看實際小時數的資訊，請參閱 [使用「用戶」視圖時，查看資源計畫員中的可用小時數、計畫小時數和實際小時數或FTE](../../../resource-mgmt/resource-planning/view-hours-fte-user-view-resource-planner.md).

## 記錄時間

您可以透過多種方式登入工作、問題和專案。

如需Workfront中記錄時間的詳細資訊，請參閱 [記錄時間](../../../timesheets/create-and-manage-timesheets/log-time.md).
