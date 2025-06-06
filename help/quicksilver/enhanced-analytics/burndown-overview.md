---
title: 在增強型分析中檢視待執行工作視覺效果
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: 「待執行工作」視覺效果會顯示特定專案在一段時間內的待執行工作，並可協助您瞭解專案狀況、速度和剩餘時數（或天數）之間的關係。
author: Nolan
feature: Reports and Dashboards
exl-id: e67c92d5-b309-406b-b6f0-4d414d0e7dcc
source-git-commit: 2a6e767036ae702f6c19dc71cdb11dae8e9e37ea
workflow-type: tm+mt
source-wordcount: '834'
ht-degree: 0%

---

# 在增強型分析中檢視待執行工作視覺效果

>[!IMPORTANT]
>
>增強型Analytics已於5月27日從Workfront移除。 Workfront Data Connect是全新的替代解決方案，可用來複製您目前使用的任何Enhanced Analytics視覺效果。 <br>如需詳細資訊，請參閱[Enhanced Analytics淘汰指南](/help/quicksilver/product-announcements/announcements/enhanced-analytics-deprecation.md)。


<!-- Audited: 12/2023 -->

「待執行工作」視覺效果會顯示特定專案在一段時間內的待執行工作，並可協助您瞭解專案狀況、速度和剩餘時數（或天數）之間的關係。

![增強型分析待執行工作範例](assets/burndown120623.png)

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫</td> 
   <td>
      <p>新增：任何</p>
      <p>或</p>
      <p>目前：商務或以上</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td>
      <p>新增：淺色或更高</p>
      <p>或</p>
      <p>目前：檢閱或以上</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>檢視專案的存取權</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>檢視</p> </td>
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

## 先決條件

如需使用增強型分析的先決條件，請參閱[增強型分析概觀](../enhanced-analytics/enhanced-analytics-overview.md)中的「先決條件」一節。

## 瞭解待執行工作視覺效果

實心藍色線顯示從開始日期到計畫完成日期的計畫速度。 當工作新增、移除或更新時，這條線就會隨之調整，當專案達到計畫完成日期時，它就會變成垂直虛線。

![計畫速度](assets/burndown-planned-line.png)

實際線條顯示一段時間內專案所花費的時數或天數。 此行的顏色表示每天的專案狀態：

* **綠色**：專案已達目標。

  ![目標](assets/burndown-green.png)

* **橙色**：專案有風險。

  ![有風險](assets/burndown-orange.png)

* **紅色**：專案發生問題。

  ![發生問題](assets/burndown-red.png)

如需這些專案條件的詳細資訊，請參閱[專案條件和條件型別概觀](../manage-work/projects/manage-projects/project-condition-and-condition-type.md)。

當實際明細行垂直向上移動時，工作已新增至專案。 當線條垂直向下移動時，專案的工作已移除或完成。

在視覺效果的x軸下方，您可以看到有關在指定日期的工作和時數（或天數）如何變更的詳細資訊（新增的數量、完成的數量以及兩者的差異）。

在「待執行工作」視覺效果中檢視所有這些資訊，可協助您判斷：

* 個別專案在一段時間內的健康情況
* 來自（或未計畫工作）的問題如何影響計畫工作
* 哪些事件將您的專案延長到超過原始完成日期

若要瞭解如何取得此視覺效果的最佳資料，請參閱[增強型分析概述](../enhanced-analytics/enhanced-analytics-overview.md)。

## 檢視待執行工作視覺效果

{{step1-to-analytics}}

1. （可選）若要使用不同的日期範圍，請從日期範圍篩選器中選取新的開始和結束日期。

   ![選取日期](assets/filters-select-date-range-350x344.png)

   如需有關使用日期範圍篩選的資訊，請參閱[在增強型分析中套用篩選](../enhanced-analytics/use-enhanced-analytics-filters.md)。

1. （視條件而定）如果您需要限制專案資料集，請選取並套用您要使用的篩選器。

   如需在增強型分析中新增篩選器的詳細資訊，請參閱[在增強型分析中套用篩選器](../enhanced-analytics/use-enhanced-analytics-filters.md)。

   新增篩選器後，系統會顯示最多50個專案的資料，而且即使您離開頁面或登出Workfront，篩選器仍會保持作用中。

1. （可選）若要放大日期範圍，請在視覺效果上選取日期範圍開頭的點，並將其拖曳至日期範圍的結尾。

   所有其他視覺效果都會更新至相同的日期範圍，並自動建立時間範圍篩選器。

   ![時間範圍篩選器](assets/timeframe-filter-350x220.png)

1. 在「小眾測試版計畫」或「專案樹狀圖」視覺效果上，按一下專案以檢視更多資訊。

   顯示待執行工作與小眾測試版中的任務視覺效果。

   >[!NOTE]
   >
   >若要進一步瞭解這些其他視覺效果，請參閱：
   >
   >   * [在增強型分析中檢視小眾測試版計畫視覺效果](../enhanced-analytics/flight-plan-overview.md)
   >   * [在增強型分析中檢視專案樹狀圖視覺效果](../enhanced-analytics/project-treemap-overview.md)
   >   * [在增強型分析中檢視小眾測試版中的任務視覺效果](../enhanced-analytics/tasks-in-flight-overview.md)
   >

1. （選用）將檢視從計畫時數變更為&#x200B;**持續時間**。

   預設會選取計畫時數。

   >[!NOTE]
   >
   >選取&#x200B;**持續時間**&#x200B;會將所有時數資訊變更為天數。\
   >![期間待執行工作](assets/duration-burndown-350x112.png)\
   >如需有關增強分析區域中持續時間的詳細資訊，請參閱[增強分析總覽](../enhanced-analytics/enhanced-analytics-overview.md#duration-view)中的「持續時間檢視」一節。

1. 按一下線圖上的任一點。

   確切的日期會顯示，而圖形下方會顯示所選日期的任務與時數（或天數）的其他相關資訊。

   ![待執行工作詳細資料](assets/burndown-task-and-hour-changes-350x121.png)

   >[!NOTE]
   >
   >如果實際速度是沿著視覺效果x軸（內嵌0小時或0天）運行的平面線，這表示沒有將計畫時數（或天數）新增到專案。\
   >如果實際速度是x軸上方的平直線（與小時數或天數內嵌），且永不下降，則表示在篩選期間內未完成任何工作。

1. （選擇性）若要匯出視覺效果資料，請按一下視覺效果右上角的&#x200B;**匯出**&#x200B;圖示![匯出圖示](assets/export.png)，然後選取匯出格式：

   * 圖表 (PNG)
   * 資料表格(XSLX)

1. （可選）若要檢視有關所選專案中任務進度的詳細資訊，請檢視「待執行工作」視覺效果下方顯示的「小眾測試版中的任務」視覺效果。 如需詳細資訊，請參閱[在增強型分析中檢視小眾測試版中的任務](/help/quicksilver/enhanced-analytics/tasks-in-flight-overview.md)。
