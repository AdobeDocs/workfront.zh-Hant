---
title: 在Enhanced Analytics中檢視小眾測試版中的任務視覺效果
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: 小眾測試版中的任務視覺效果會顯示專案中正在進行的任務數（在套用的篩選條件內）、每個任務完成的工作百分比，以及任務的排程方式。
author: Nolan
feature: Reports and Dashboards
exl-id: cc738450-362a-49e8-836f-611fa82057b5
source-git-commit: 1b1f3c22b8112cfde5b10bef39076eed11630d0f
workflow-type: tm+mt
source-wordcount: '716'
ht-degree: 4%

---

# 在Enhanced Analytics中檢視小眾測試版中的任務視覺效果

小眾測試版中的任務視覺效果會顯示專案中正在進行的任務數（在套用的篩選條件內）、每個任務完成的工作百分比，以及任務的排程方式。

![](assets/tasks-in-flight-possible-replacement-350x104.png)

## 存取需求

您必須具備下列條件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">Adobe Workfront計畫</a>*</td> 
   <td> <p>商務或以上版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront授權總覽</a>*</td> 
   <td> <p>評論或以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>檢視專案的存取權</p> <p>檢視任務的存取權（若要更新任務，您需要任務的編輯存取權。）</p> <p>注意：如果您還是沒有存取權，請詢問您的Workfront管理員，他們是否在您的存取層級中設定其他限制。<br>如需Workfront管理員如何修改存取層級的詳細資訊，請參閱<a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>檢視專案和任務物件的許可權</p> <p>如需請求其他存取權的資訊，請參閱<a href="../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求物件</a>的存取權。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的Workfront管理員。

## 先決條件

如需使用增強型分析的先決條件，請參閱[增強型分析概觀](../enhanced-analytics/enhanced-analytics-overview.md)中的「先決條件」一節。

## 瞭解小眾測試版中的任務視覺效果

小眾測試版中的任務計畫視覺效果會顯示以下任務詳細資訊：

* **計畫任務期間**：任務列的長度表示計畫期間，此計畫期間是以任務的開始日期和完成日期為基礎。

  ![](assets/tasks-in-flight-duration-350x80.png)

* **已完成的工作量**：工作列內的深藍色表示工作已完成的工作量。 此完成百分比會顯示在工作列的右側。

  ![](assets/tasks-in-flight-dark-blue-350x35.png)

* **剩餘的工作量**：工作列內的淺藍色表示工作需要完成的工作量。

  ![](assets/tasks-in-flight-light-blue-350x35.png)

此資訊可協助您確定：

* 將工作集中在何處。
* 哪些任務可能會使專案面臨風險。
* 任務距離完成有多近。
* 您需要與誰討論特定任務。

若要瞭解如何取得此視覺效果的最佳資料，請參閱[增強型分析概述](../enhanced-analytics/enhanced-analytics-overview.md)。

## 檢視小眾測試版中的任務視覺效果

1. 按一下主要功能表圖示![](assets/main-menu-icon-16x12.png)，然後選取&#x200B;**Analytics**。
1. （可選）若要使用不同的日期範圍，請從日期範圍篩選器中選取新的開始和結束日期。

   ![](assets/filters-select-date-range-350x344.png)

   如需有關使用日期範圍篩選的資訊，請參閱[在增強型分析中套用篩選](../enhanced-analytics/use-enhanced-analytics-filters.md)。

1. （視條件而定）如果您需要限制專案資料集，請選取並套用您要使用的篩選器。

   如需在增強型分析中新增篩選器的詳細資訊，請參閱[在增強型分析中套用篩選器](../enhanced-analytics/use-enhanced-analytics-filters.md)。

   新增篩選器後，系統會顯示最多50個專案的資料，而且即使您離開頁面或登出Workfront，篩選器仍會保持作用中。

1. 在「小眾測試版計畫」或「專案樹狀圖」視覺效果上，按一下專案以檢視更多資訊。

   顯示待執行工作與小眾測試版中的任務視覺效果。

   >[!NOTE]
   >
   >若要進一步瞭解這些其他視覺效果，請參閱：
   >
   >   
   >   
   >   * [在增強型分析中檢視小眾測試版計畫視覺效果](../enhanced-analytics/flight-plan-overview.md)
   >   * [在增強型分析中檢視專案樹狀圖視覺效果](../enhanced-analytics/project-treemap-overview.md)
   >   * [在增強型分析中檢視待執行工作視覺效果](../enhanced-analytics/burndown-overview.md)
   >   
   >

1. （可選）若要放大日期範圍，請在視覺效果上選取一個點，作為日期範圍的起點，並拖曳至日期範圍的終點。

   所有其他視覺效果會更新至相同的日期範圍，並建立時間範圍篩選器。

   ![](assets/timeframe-filter-350x220.png)

1. （選擇性）若要變更工作的排序方式，請按一下&#x200B;**排序依據**&#x200B;功能表，然後選取新的排序選項：

   * **完成日期**
   * **字母順序A-Z**
   * **工作分解結構** （此選項符合任務在專案中的顯示順序。）

   頁面上的其他所有視覺效果都會更新以符合您的排序選擇。

1. 檢閱所選專案中的任務進度，然後將滑鼠指標停留在特定任務上，即可檢視計畫時數、計畫到期日和完成百分比。

   ![](assets/tasks-in-flight-task-details-350x242.png)

1. 按一下工作以開啟畫面右側的工作詳細資訊，您可以在此檢視工作的詳細資訊、檢視或輸入更新，或變更工作。

   ![](assets/task-details-qs-350x675.png)

1. （選擇性）若要匯出視覺效果資料，請按一下視覺效果右上角的&#x200B;**匯出圖示** ![](assets/export.png)，然後選取匯出格式：

   * **圖表(PNG)**
   * **資料表(XSLX)**

