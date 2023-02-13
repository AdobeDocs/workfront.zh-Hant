---
title: 在Enhanced Analytics中檢視「燃耗」視覺效果
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: 「燃耗」(Burndown)視覺效果顯示特定項目的隨時間的燃耗，並幫助您了解項目條件、速度和剩餘小時數（或天數）之間的關係。
author: Nolan
feature: Reports and Dashboards
exl-id: e67c92d5-b309-406b-b6f0-4d414d0e7dcc
source-git-commit: d337008d4fca8c41b98b10f9059ec1cc379811e1
workflow-type: tm+mt
source-wordcount: '797'
ht-degree: 0%

---

# 在Enhanced Analytics中檢視「燃耗」視覺效果

「燃耗」(Burndown)視覺效果顯示特定項目的隨時間的燃耗，並幫助您了解項目條件、速度和剩餘小時數（或天數）之間的關係。

![](assets/burndown-350x112.png)

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
   <td> <p>檢視專案的存取權</p> <p>注意：如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。<br>如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>檢視</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 必要條件

如需使用增強分析的必要條件，請參閱 [增強的分析概觀](../enhanced-analytics/enhanced-analytics-overview.md).

## 了解燃耗視覺效果

實藍線顯示從開始日期到計畫完成日期的計畫速度。 此行會隨著工作的添加、刪除或更新而調整，並在項目達到計畫完成日期時變為虛線。

![](assets/burndown-planned-line.png)

實際行顯示項目在一段時間內的逗留小時數（或天數）。 此行的顏色指示每天項目的條件：

* **綠色**:專案已鎖定目標。

   ![](assets/burndown-green.png)

* **橙色**:這個項目面臨風險。

   ![](assets/burndown-orange.png)

* **紅色**:項目有問題。

   ![](assets/burndown-red.png)

如需這些專案條件的詳細資訊，請參閱 [專案條件和條件類型概觀](../manage-work/projects/manage-projects/project-condition-and-condition-type.md).

當實際線條垂直向上移動時，已將工作添加到項目中。 當直線垂直向下移動時，已為項目刪除或完成工作。

在視覺效果的x軸下方，您可以看到有關指定日如何變更工作和小時（或天）的詳細資訊（新增數量、完成數量，以及兩者之間的差異）。

在「燃耗」視覺效果中查看所有這些資訊，有助於您判斷：

* 個別專案隨時間的健康狀況
* 傳入（或計畫外工作）的問題如何影響計畫內工作。
* 哪些事件將您的項目延長到原始完成日期之後。

若要了解如何取得此視覺效果的最佳資料，請參閱 [增強的分析概觀](../enhanced-analytics/enhanced-analytics-overview.md).

## 檢視「燃耗」視覺效果

1. 按一下「主菜單」表徵圖 ![](assets/main-menu-icon-16x12.png)，然後選取 **Analytics**.
1. （可選）若要使用不同的日期範圍，請從日期範圍篩選器中選取新的開始日期和結束日期。

   ![](assets/filters-select-date-range-350x344.png)

   如需使用日期範圍篩選器的詳細資訊，請參閱 [在增強分析中套用篩選器](../enhanced-analytics/use-enhanced-analytics-filters.md).

1. （條件性）如果您需要限制專案資料集，請選取並套用您要使用的篩選器。

   如需在增強分析中新增篩選器的詳細資訊，請參閱 [在增強分析中套用篩選器](../enhanced-analytics/use-enhanced-analytics-filters.md).

   新增篩選器後，最多會顯示50個專案的資料，且即使您離開頁面或登出Workfront，篩選器仍保持作用中狀態。

1. （可選）若要放大日期範圍，請在視覺效果上選取日期範圍開始的點，然後拖曳至日期範圍結束。

   所有其他視覺效果都會更新至相同的日期範圍，並建立時間範圍篩選。

   ![](assets/timeframe-filter-350x220.png)

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
   >   * [在Enhanced Analytics中檢視「飛行中的任務」視覺效果](../enhanced-analytics/tasks-in-flight-overview.md)


1. （可選）將檢視從計畫時數變更為 **持續時間**.

   預設會選取計畫小時數。

   >[!NOTE]
   >
   >選取 **持續時間** 將所有小時資訊更改為天。\
   >![](assets/duration-burndown-350x112.png)\
   >如需「增強」分析區域持續時間的詳細資訊，請參閱 [增強的分析概觀](../enhanced-analytics/enhanced-analytics-overview.md).

1. 按一下線圖上的任何點。

   下面顯示所選日期的確切日期，以及有關任務和小時（或天）的詳細資訊。

   ![](assets/burndown-task-and-hour-changes-350x121.png)

   >[!NOTE]
   >
   >如果實際速度是沿著視覺效果的x軸（以0小時或0天為內嵌）執行的平直線，這表示專案中未新增計畫小時數（或天數）。\
   >如果實際速度是從不下降的x軸上方的平直線（內嵌數小時或天數），這表示在篩選的時段內未完成任務。

1. （選用）若要匯出視覺效果資料，請按一下 **匯出** 圖示 ![](assets/export.png)在視覺效果的右上角，選取匯出格式：

   * **圖表 (PNG)**
   * **資料表(XSLX)**

1. （可選）要查看所選項目中任務進度的詳細資訊，請查看「燃耗」視覺效果下方的「飛行任務」視覺效果。
