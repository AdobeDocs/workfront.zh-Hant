---
title: 在Enhanced Analytics中檢視「飛行中的任務」視覺效果
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: 「飛行任務」視覺效果顯示項目正在進行的任務數（在應用的篩選條件內）、每個任務已完成的工作百分比，以及任務的排程方式。
author: Nolan
feature: Reports and Dashboards
exl-id: cc738450-362a-49e8-836f-611fa82057b5
source-git-commit: 1b1f3c22b8112cfde5b10bef39076eed11630d0f
workflow-type: tm+mt
source-wordcount: '717'
ht-degree: 0%

---

# 在Enhanced Analytics中檢視「飛行中的任務」視覺效果

「飛行任務」視覺效果顯示項目正在進行的任務數（在應用的篩選條件內）、每個任務已完成的工作百分比，以及任務的排程方式。

![](assets/tasks-in-flight-possible-replacement-350x104.png)

## 存取需求

您必須具備下列條件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">Adobe Workfront計畫</a>*</td> 
   <td> <p>業務或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront授權概觀</a>*</td> 
   <td> <p>審核或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>檢視專案的存取權</p> <p>查看對任務的訪問（要更新任務，需要編輯對任務的訪問。）</p> <p>注意：如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。<br>如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>查看對項目和任務對象的權限</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 必要條件

如需使用增強分析的必要條件，請參閱 [增強的分析概觀](../enhanced-analytics/enhanced-analytics-overview.md).

## 了解飛行視覺效果中的任務

「飛行計畫中的任務」視覺效果顯示以下任務詳細資訊：

* **計畫任務持續時間**:任務欄的長度指示基於任務起始日期和完成日期的計畫持續時間。

   ![](assets/tasks-in-flight-duration-350x80.png)

* **已完成工作**:任務欄中的深藍色表示任務已完成的工作量。 此完成百分比顯示在任務欄的右側。

   ![](assets/tasks-in-flight-dark-blue-350x35.png)

* **剩餘的工作**:任務欄內的淺藍色表示任務需要完成的工作量。

   ![](assets/tasks-in-flight-light-blue-350x35.png)

此資訊可協助您判斷：

* 工作重點集中的地方。
* 哪些任務可能會使項目面臨風險。
* 任務完成的距離。
* 你需要跟誰談一談特定任務。

若要了解如何取得此視覺效果的最佳資料，請參閱 [增強的分析概觀](../enhanced-analytics/enhanced-analytics-overview.md).

## 查看飛行視覺效果中的任務

1. 按一下「主菜單」表徵圖 ![](assets/main-menu-icon-16x12.png)，然後選取 **Analytics**.
1. （可選）若要使用不同的日期範圍，請從日期範圍篩選器中選取新的開始日期和結束日期。

   ![](assets/filters-select-date-range-350x344.png)

   如需使用日期範圍篩選器的詳細資訊，請參閱 [在增強分析中套用篩選器](../enhanced-analytics/use-enhanced-analytics-filters.md).

1. （條件性）如果您需要限制專案資料集，請選取並套用您要使用的篩選器。

   如需在增強分析中新增篩選器的詳細資訊，請參閱 [在增強分析中套用篩選器](../enhanced-analytics/use-enhanced-analytics-filters.md).

   新增篩選器後，最多會顯示50個專案的資料，且即使您離開頁面或登出Workfront，篩選器仍保持作用中狀態。

1. 在「飛行計畫」或「專案樹狀圖」視覺效果中，按一下專案以檢視詳細資訊。

   「飛行中的燃耗」和「任務」視覺效果顯示。

   >[!NOTE]
   >
   >若要進一步了解這些其他視覺效果，請參閱：
   >
   >   
   >   
   >   * [在增強分析中檢視「飛行計畫」視覺效果](../enhanced-analytics/flight-plan-overview.md)
   >   * [在增強的分析中檢視專案樹狀圖視覺效果](../enhanced-analytics/project-treemap-overview.md)
   >   * [在Enhanced Analytics中檢視「燃耗」視覺效果](../enhanced-analytics/burndown-overview.md)


1. （可選）若要放大日期範圍，請在視覺效果上選取日期範圍開始的點，然後拖曳至日期範圍結束。

   所有其他視覺效果都會更新至相同的日期範圍，並建立時間範圍篩選。

   ![](assets/timeframe-filter-350x220.png)

1. （可選）若要變更工作排序方式，請按一下 **排序依據** ，然後選擇新的排序選項：

   * **完成日期**
   * **依字母順序 A-Z**
   * **工作分解結構** （此選項與任務在項目中的顯示順序匹配。）

   頁面上的所有其他視覺效果都會更新，以符合您的排序選取項目。

1. 複查選定項目中任務的進度，然後將滑鼠移到特定任務上以查看計畫小時數、計畫到期日和完成百分比。

   ![](assets/tasks-in-flight-task-details-350x242.png)

1. 按一下任務可開啟螢幕右側的任務詳細資訊，您可以在其中查看有關任務、查看或輸入更新，或對任務進行更改的詳細資訊。

   ![](assets/task-details-qs-350x675.png)

1. （選用）若要匯出視覺效果資料，請按一下 **匯出圖示** ![](assets/export.png) 在視覺效果的右上角，選取匯出格式：

   * **圖表 (PNG)**
   * **資料表(XSLX)**

