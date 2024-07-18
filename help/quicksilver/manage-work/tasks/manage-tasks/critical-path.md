---
content-type: overview
product-area: projects
navigation-topic: manage-tasks
title: 專案關鍵路徑概觀
description: 決定專案的關鍵路徑是Adobe Workfront標籤專案中可能影響專案時間表的一系列任務時的自動方式。 可能會影響專案時間表的任務會標示為「關鍵路徑」任務。
author: Alina
feature: Work Management
exl-id: 9cbc84bf-d02b-4bb7-8d5d-922554d1262e
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '764'
ht-degree: 0%

---

# 專案關鍵路徑概觀

決定專案的關鍵路徑是Adobe Workfront標籤專案中可能影響專案時間表的一系列任務時的自動方式。 可能會影響專案時間表的任務會標示為「關鍵路徑」任務。

下列功能可能會影響專案的關鍵路徑：

* 專案的工作分解結構。

  如需工作分解結構的詳細資訊，請參閱[決定專案中的工作分解結構](../../../manage-work/projects/planning-a-project/determine-project-work-breakdown-structure.md)

* 完成每項工作所需的時間（持續時間）。
* 工作之間的相依性。

  請考量下列事項：

   * 當「關鍵路徑」上的任務具有前置任務關係時，如果前置任務或後置任務日期上的變更直接影響其相依專案，則其前置任務與後置任務也會在「關鍵路徑」上。

     >[!TIP]
     >
     >當任務的後續任務的日期未直接影響其相依任務的日期，並且不影響專案日期時，後續任務不會在「關鍵路徑」上。
     >
     >
     >![](assets/successor-not-on-critical-path-350x150.png)     >
     >

   * 當子任務被識別為「關鍵路徑」任務時，如果父任務的「預計開始日期」和時間與子任務的「預計開始日期」和時間相同，則父任務也會被識別為「關鍵路徑」任務。

考慮到這些功能，系統會使用最早任務與決定專案結束的任務之間的最長路徑，來計算「關鍵路徑」。 「關鍵路徑計算」會考量每個任務可以開始和完成的最早和最晚時間，而不需要延長專案。 此程式會判斷哪些任務為「關鍵」（且屬於最長路徑），以及哪些任務具有「總浮動」（可以延遲，而不會造成專案時間更長）。

關鍵路徑上任務活動的任何延遲會直接影響專案的預計完成日期（關鍵路徑上沒有浮點）。

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
   <td> <p>工作或更高</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>檢視或更高的任務存取權</p> <p>注意：如果您還是沒有存取權，請詢問您的Workfront管理員，他們是否在您的存取層級中設定其他限制。 如需Workfront管理員如何修改存取層級的詳細資訊，請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>檢視任務或更高的許可權 </p> <p>如需請求其他存取權的資訊，請參閱<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求物件</a>的存取權。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的Workfront管理員。

## 檢視關鍵路徑

您可以在Workfront應用程式的下列區域中檢視屬於關鍵路徑的任務：

* [檢視甘特圖中的關鍵路徑](#view-the-critical-path-in-the-gantt-chart)
* [檢視工作清單或報告中的關鍵路徑](#view-the-critical-path-in-a-task-list-or-report)

### 在甘特圖中檢視關鍵路徑 {#view-the-critical-path-in-the-gantt-chart}

若要在甘特圖檢視關鍵路徑上的工作：

1. 移至您要檢視其關鍵路徑的專案。
1. 按一下左側面板中的&#x200B;**工作**。
1. 按一下工作清單右上角的&#x200B;**甘特圖**&#x200B;圖示。

   ![gantt_chart_icon__1_.png](assets/gantt-chart-icon--1-.png)

1. 展開&#x200B;**選項**&#x200B;功能表，然後啟用&#x200B;**重要路徑**&#x200B;選項。

   位於關鍵路徑上的任務在甘特圖中的時間表上方有一條紅線。

   ![crtical_path_on_gantt__1_.png](assets/crtitical-path-on-gantt--1--350x137.png)

### 檢視工作清單或報告中的關鍵路徑 {#view-the-critical-path-in-a-task-list-or-report}

若要檢視任務清單中關鍵路徑上的任務，請執行下列動作：

1. 移至您要檢視其關鍵路徑的專案。
1. 按一下左側面板中的&#x200B;**工作**。
1. 從&#x200B;**檢視**&#x200B;下拉式功能表中，選取&#x200B;**狀態**。

   關鍵路徑上的任務在清單的&#x200B;**旗標**&#x200B;欄中有&#x200B;**關鍵路徑**&#x200B;旗標。

   您可以將相同的檢視套用至任務報告。

   如需有關建立報告的詳細資訊，請參閱文章[建立自訂報告](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)。

   或

   從&#x200B;**篩選器**&#x200B;下拉式功能表中，選取&#x200B;**新增篩選器**。

1. 按一下&#x200B;**新增篩選器規則**&#x200B;並開始在&#x200B;**只顯示包含……**&#x200B;欄位的任務中輸入&#x200B;**Is Critical**。

1. 當它出現在清單中時選取它。
1. 按一下「**儲存篩選器**」。

   清單應只顯示關鍵路徑上的工作。
