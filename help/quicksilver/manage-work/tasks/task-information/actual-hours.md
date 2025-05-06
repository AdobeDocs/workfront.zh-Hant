---
content-type: overview
product-area: projects
navigation-topic: task-information
title: 檢視實際小時
description: 您在Adobe Workfront中登入工作專案的時數會視為實際時數。
author: Alina
feature: Work Management
exl-id: c4b0e431-1765-416d-89f5-6ac663ac1d4f
source-git-commit: 3827e834a71084f14a99cb27aadefd97327b02d7
workflow-type: tm+mt
source-wordcount: '759'
ht-degree: 0%

---

# 檢視實際小時

<!-- Audited: 5/2025 -->

您在Adobe Workfront中登入工作專案的時數會視為實際時數。

實際時數代表您完成任務、問題或專案所用的實際時間。

我們建議在工作專案（任務和問題）上記錄時數。 不過，身為Workfront管理員，您可以根據您組織的工作流程，允許使用者也登入專案時間。

如需有關如何設定系統以允許使用者將時間登入專案的詳細資訊，請參閱[設定時程表和小時偏好設定](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md)。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具有下列存取權才能執行本文中的步驟：

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
   <td> 
   <p>新增：標準<p>
   <p>或</p>
   <p>目前：工作或以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>檢視或更高的任務、專案或問題存取權</p> <p>注意：如果您還是沒有存取權，請詢問您的Workfront管理員，他們是否在您的存取層級中設定其他限制。 如需Workfront管理員如何修改存取層級的詳細資訊，請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>檢視任務、專案或問題的許可權或更高</p> <p>如需請求其他存取權的資訊，請參閱<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求物件</a>的存取權。</p> </td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 任務和問題的實際小時與專案的實際小時比較

任務和問題的實際時數代表直接記錄到任務和問題上的時數。

子系任務的實際時數向上彙整至父系任務的實際時數。 下列公式適用於父系任務的「實際時數」：

```
Parent Task Actual Hours = All Tasks Actual Hours + Parent Task Actual Hours
```

專案實際時數代表所有專案任務的實際時數總計（包括直接記錄於父系任務的時數）、所有專案的問題，以及記錄於專案本身的實際時數。

下列公式適用於專案的實際時數：

```
Project Actual Hours = All Tasks Actual Hours + All Issues Actual Hours + All Project Actual Hours
```

## 尋找實際小時

為任務、專案和問題尋找專案實際時數的值是相同的。

您可以在下列位置找到有關作業的「實際時數」資訊：

* [詳細資訊區段中的實際時數](#actual-hours-in-the-details-section)
* [時數區段中的實際時數](#actual-hours-in-the-hours-section)
* 報表中的[實際時數](#actual-hours-in-reports)
* [資源管理工具中的實際時數](#actual-hours-in-resource-management-tools)

### 詳細資訊區段中的實際小時 {#actual-hours-in-the-details-section}

在詳細資訊區段中尋找實際時數，專案、任務和問題的結果完全相同。

若要在作業詳細資訊中找出實際時數：

1. 移至您要檢閱其實際時數的工作。
1. 在左側面板中，按一下&#x200B;**工作詳細資料**。 **總覽**&#x200B;區段隨即顯示。
1. 在&#x200B;**工作時間**&#x200B;區段中找到&#x200B;**實際時數**&#x200B;值。 這是記錄在此任務的總時數。

### 時數區段中的實際時數 {#actual-hours-in-the-hours-section}

在專案、任務和問題中，在時數區段中尋找實際時數是相同的。

若要找出實際時數區段：

1. 移至您要檢閱其實際時數的工作。

1. 在左側面板中，按一下&#x200B;**小時**。 工作上所記錄的小時專案清單隨即顯示，**小時**&#x200B;欄顯示工作的實際小時總數。

1. 請確定&#x200B;**標準**&#x200B;檢視和&#x200B;**專案**&#x200B;群組已套用至此清單。

### 報表中的實際小時 {#actual-hours-in-reports}

建立任務、問題或專案報告時，您可以在報告中顯示每個任務、問題或專案的實際時數值。

若要在任務報告中顯示實際時數：

{{step1-to-reports}}

1. 在&#x200B;**報表**&#x200B;頁面上，按一下&#x200B;**新增報表**，然後選擇&#x200B;**工作**&#x200B;作為物件。
1. 在頁面的右下角，按一下&#x200B;**新增欄**。
1. 在出現的&#x200B;**顯示在此欄**&#x200B;下拉式欄位中，開始輸入&#x200B;**實際時數**，然後選取出現在清單中的欄位。

1. 在頁面的左下角，按一下&#x200B;**儲存+關閉**&#x200B;以儲存報告。

1. 在「**將此報告命名以儲存**」對話方塊中，輸入新的報告名稱，然後按一下「**套用**」。

### 資源管理工具中的實際時數 {#actual-hours-in-resource-management-tools}

如果您想檢視使用者對其指派的任務和問題所做的工作進度，可在以下資源管理工具中檢視它們：

* 使用率報表。\
  如需詳細資訊，請參閱[資源使用率報告概覽](../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md)。

* 資源規劃工具。

  如需相關資訊，請參閱使用使用者檢視時[資源規劃工具中的可用檢視、計畫時數與實際時數，或FTE](../../../resource-mgmt/resource-planning/view-hours-fte-user-view-resource-planner.md)。

## 記錄時間

您可以透過多種方式登入任務、問題和專案的時間。

如需詳細資訊，請參閱[記錄時間](../../../timesheets/create-and-manage-timesheets/log-time.md)。
