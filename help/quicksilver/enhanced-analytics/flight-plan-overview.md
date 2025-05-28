---
title: 在Enhanced Analytics中檢視小眾測試版計畫視覺效果
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: 「外部測試計畫」視覺效果會顯示外部測試中的專案數目（在套用的篩選條件範圍內）、這些專案在整個生命週期中發生了哪些狀況變更，以及這些專案與其計畫的完成截止日期之間的粘附度。
author: Nolan
feature: Reports and Dashboards
exl-id: c64ed752-151a-40f7-ab18-684e2cd032bc
source-git-commit: 2a6e767036ae702f6c19dc71cdb11dae8e9e37ea
workflow-type: tm+mt
source-wordcount: '924'
ht-degree: 4%

---

# 在Enhanced Analytics中檢視小眾測試版計畫視覺效果

>[!IMPORTANT]
>
>增強型Analytics已於5月27日從Workfront移除。 Workfront Data Connect是全新的替代解決方案，可用來複製您目前使用的任何Enhanced Analytics視覺效果。 <br>如需詳細資訊，請參閱[Enhanced Analytics淘汰指南](/help/quicksilver/product-announcements/announcements/enhanced-analytics-deprecation.md)。


「外部測試計畫」視覺效果會顯示外部測試中的專案數目（在套用的篩選條件範圍內）、這些專案在整個生命週期中發生了哪些狀況變更，以及這些專案與其計畫的完成截止日期之間的粘附度。

![小眾測試版計畫](assets/flight-plan-350x132.png)

## 存取需求

您必須具備下列條件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://business.adobe.com/products/workfront/pricing.html" target="_blank">Adobe Workfront計畫</a>*</td> 
   <td> <p>商務或以上版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront授權總覽</a>*</td> 
   <td> <p>評論或以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>檢視專案的存取權</p> <p>注意：如果您還是沒有存取權，請詢問您的Workfront管理員，他們是否在您的存取層級中設定其他限制。<br>如需Workfront管理員如何變更存取層級的詳細資訊，請參閱<a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>檢視專案的存取權</p> <p>如需請求其他存取權的資訊，請參閱<a href="../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求物件</a>的存取權。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的Workfront管理員。

## 先決條件

如需使用增強型分析的先決條件，請參閱[增強型分析概觀](../enhanced-analytics/enhanced-analytics-overview.md)中的「先決條件」一節。

## 瞭解小眾測試版計畫視覺效果

在實際專案期間中，您只能看到下列專案狀況：

* 達成目標
* 有風險
* 陷入困境

若要瞭解專案狀況，請參閱[專案狀況與狀況型別概觀](../manage-work/projects/manage-projects/project-condition-and-condition-type.md)。

小眾測試版計畫視覺效果會顯示下列專案詳細資料：

* **規劃期間**：水準藍線代表專案的規劃長度，其兩端的三角形代表開始日期和結束日期。

  ![計畫持續時間](assets/planned-duration-line-350x37.png)

* **實際工期**：計畫工期下方的彩色粗線代表專案的實際長度。 線條的顏色會隨著專案在專案生命週期中特定時間的狀況而改變。

  ![實際持續時間](assets/actual-duration-line.png)

* **實際狀況**：粗的彩色線條也會在不同時間顯示專案狀況。 線條的顏色會隨著專案狀況而改變：

   * **綠色**：目標上
   * **橙色**：有風險
   * **紅色**：發生問題

  ![實際狀況](assets/actual-condition-color.png)

在「小眾測試版計畫」視覺效果中，將滑鼠游標停留在專案列上，即可檢視有關專案計畫時間範圍、目前專案狀態以及（如果適用）自訂狀態的資訊。 若要更深入地瞭解影響持續時間或條件的因素，您可以檢視「增強分析」區域中的其他視覺效果。

查看這些資訊可協助您判斷：

* 哪些事件會使專案延長超過原始計畫完成日期。
* 專案在什麼時候開始發生問題。
* 同一時段內有多少個專案處於未完成狀態。
* 有多少專案是進行中。
* 哪些專案需要額外注意或支援。

如需如何取得此視覺效果最佳資料的詳細資訊，請參閱[增強型分析總覽](../enhanced-analytics/enhanced-analytics-overview.md)。

## 檢視小眾測試版計畫視覺效果

1. 按一下&#x200B;**主功能表**&#x200B;圖示![主功能表圖示](assets/main-menu-icon-16x12.png)，然後選取&#x200B;**Analytics**。
1. （可選）若要使用不同的日期範圍，請從日期範圍篩選器中選取新的開始和結束日期。

   ![選取日期範圍](assets/filters-select-date-range-350x344.png)

   如需有關使用日期範圍篩選的資訊，請參閱[在增強型分析中套用篩選](../enhanced-analytics/use-enhanced-analytics-filters.md)。

1. （視條件而定）如果您需要限制專案資料集，請選取並套用您要使用的篩選器。

   如需在增強型分析中新增篩選器的詳細資訊，請參閱[在增強型分析中套用篩選器](../enhanced-analytics/use-enhanced-analytics-filters.md)。

   新增篩選器後，系統會顯示最多50個專案的資料，而且即使您離開頁面或登出Workfront，篩選器仍會保持作用中。

1. （可選）若要放大日期範圍，請在視覺效果上選取一個點，作為日期範圍的起點，並拖曳至日期範圍的終點。

   所有其他視覺效果會更新至相同的日期範圍，並建立時間範圍篩選器。

   ![時間範圍篩選器](assets/timeframe-filter-350x220.png)

1. （可選）若要變更專案的排序方式，請按一下小眾測試版計畫視覺效果右上角的&#x200B;**排序依據**&#x200B;功能表，然後選取新的排序選項：

   * **A - Z**
   * **Z - A**
   * **計畫完成日期**
   * **計劃開始日期**

   頁面上的其他所有視覺效果都會更新以符合您的排序選擇。

1. （條件式）如果您的資料集超過50個專案，請使用視覺效果左下角的箭頭，從一個50個專案群組瀏覽至下一個專案。

   頁面上的所有其他視覺效果都會更新以符合您的頁面選擇。

   ![分頁](assets/pagination-350x118.png)

1. 將滑鼠停留在專案橫條圖上可檢視藍色日期線以及下列詳細資訊：

   * 計畫時間表
   * 目前狀況
   * 自訂條件（如果適用）

   ![專案橫條圖](assets/project-bar-graph-350x143.png)

1. （選擇性）若要匯出視覺效果資料，請按一下視覺效果右上角的&#x200B;**匯出**&#x200B;圖示![匯出圖示](assets/export.png)，然後選取匯出格式：

   * **圖表(PNG)**
   * **資料表(XSLX)**

1. 若要檢視更多專案資訊，請按一下視覺效果上的專案，以開啟小眾測試版中的「待執行工作」和「任務」視覺效果。

   這些視覺效果可協助您更深入瞭解insight為何導致專案偏離軌道。 它們還可以讓您輕鬆簽入進行中的專案。\
   如需有關待執行工作視覺效果的詳細資訊，請參閱[在增強型分析中檢視待執行工作視覺效果](../enhanced-analytics/burndown-overview.md)。 如需小眾測試版中任務的詳細資訊，請參閱[在增強型分析中檢視小眾測試版中的任務](../enhanced-analytics/tasks-in-flight-overview.md)。

