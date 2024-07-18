---
product-area: reporting;user-management
keywords: 儲存，新增，報表，複製
navigation-topic: create-and-manage-reports
title: 建立報告副本
description: 您可以建立您有權存取的任何報表的復本。 您可以建立自訂報表的精確副本，也可以儲存預設報表的新版本。 複製報表後，您成為所複製報表的所有者，該報表會顯示在「我的報表」區段中。
author: Nolan
feature: Reports and Dashboards
exl-id: 84737f48-efc5-45f1-acd1-b9f5d353f80f
source-git-commit: 548e713700fda79070f59f3dc3457410d2c50133
workflow-type: tm+mt
source-wordcount: '676'
ht-degree: 0%

---

# 建立報告副本

您可以建立您有權存取的任何報表的復本。 您可以建立自訂報表的精確副本，也可以儲存預設報表的新版本。 複製報表後，您成為所複製報表的所有者，該報表會顯示在「我的報表」區段中。

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

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
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>編輯報告、儀表板、行事曆的存取權</p> <p>編輯對篩選器、檢視、群組的存取權</p> <p>注意：如果您還是沒有存取權，請詢問您的Workfront管理員，他們是否在您的存取層級中設定其他限制。 如需Workfront管理員如何修改存取層級的詳細資訊，請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>檢視報表許可權</p> <p>如需請求其他存取權的資訊，請參閱<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求物件</a>的存取權。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的Workfront管理員。

## 建立報表的精確副本

如果要製作您擁有者的報告副本，請執行以下操作：

1. 按一下Adobe Workfront右上角的&#x200B;**主要功能表**&#x200B;圖示![](assets/main-menu-icon.png)。

1. 按一下&#x200B;**報表**，然後按&#x200B;**所有報表**。
1. 開啟報表。
1. 按一下&#x200B;**報告動作**，然後按一下&#x200B;**複製**。

   >[!TIP]
   >
   >如果報表是預設報表，則複製選項不會出現在報表動作功能表中。\
   >如需如何建立預設報表復本的詳細資訊，請參閱[建立新版報表](#create-a-new-version-of-a-report)。

   ![複製報告](assets/nwe-fulllistofreportactions-2022.png)

   原始報告的復本是以預設名稱&#x200B;*原始報告]*&#x200B;的[名稱復本建立。 例如，報告「第4季已完成任務」會將「第4季已完成任務的副本」作為名稱。

1. （選擇性）若要重新命名報表，請開始輸入新名稱。

   >[!TIP]
   >
   >如果您在輸入新名稱之前取消選取標題，請選取報表標題、刪除名稱，然後輸入新名稱。

1. （選擇性）若要與其他使用者共用新版本的報告，請按一下&#x200B;**報告動作**，然後按&#x200B;**共用**。

   >[!NOTE]
   >
   >共用資訊不會從原始版本傳輸至複製的報表。\
   >若要瞭解如何檢視與誰共用前一個報告，請參閱[建立報告活動的報告](../../../reports-and-dashboards/reports/report-usage/create-report-reporting-activities.md#identify)。

1. （選用）如果您擁有原始報表的管理許可權，且不再需要原始報表，可以將其刪除，以移除Workfront中不必要的重複報表。

   若要刪除原始報表，請執行下列動作：

   1. 導覽至報表。
   1. 按一下&#x200B;**報告動作**，然後按一下&#x200B;**刪除**。

   1. 按一下&#x200B;**是，刪除**&#x200B;以確認您要刪除報表。

## 建立報告的新版本 {#create-a-new-version-of-a-report}

如果要建立預設報表的副本，請執行以下操作：

1. 按一下Adobe Workfront右上角的&#x200B;**主要功能表**&#x200B;圖示![](assets/main-menu-icon.png)。

1. 按一下&#x200B;**報表**，然後按&#x200B;**所有報表**。
1. 按一下預設報表的名稱以開啟。
1. 按一下&#x200B;**報告動作**，然後按一下&#x200B;**編輯**。

   ![編輯報告](assets/nwe-reportactionsfordefaultreport-2022.png)

1. 在報告的下列標籤中進行所需的任何修改：

   * **欄（檢視）**：如需自訂檢視的詳細資訊，請參閱Adobe Workfront中的文章[檢視總覽](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)。
   * **群組**：如需自訂群組的詳細資訊，請參閱文章[Adobe Workfront中的群組概觀](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)。
   * **篩選器**：如需自訂篩選器的詳細資訊，請參閱文章[篩選器概觀](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)。
   * **圖表**：如需自訂報表圖表的詳細資訊，請參閱文章[將圖表新增至報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md)。

1. 按一下右上角的&#x200B;**報告設定**。
1. 在&#x200B;**報告標題**&#x200B;欄位中，為報告提供新名稱。
1. 按一下&#x200B;**完成**。
1. 按一下&#x200B;**另存為新報告**。

   ![](assets/nwe-save-as-new-report-350x220.png)

1. （選擇性）若要與其他使用者共用新版本的報告，請按一下&#x200B;**報告動作**，然後按&#x200B;**共用**。
