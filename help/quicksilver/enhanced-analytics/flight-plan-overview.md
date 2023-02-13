---
title: 在增強分析中檢視「飛行計畫」視覺效果
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: 「飛行計畫」視覺效果顯示有多少個項目（在套用的篩選條件內）正在執行，這些項目的整個生命週期中發生了哪些條件變化，以及這些項目遵守計畫完成期限的程度。
author: Nolan
feature: Reports and Dashboards
exl-id: c64ed752-151a-40f7-ab18-684e2cd032bc
source-git-commit: 1b1f3c22b8112cfde5b10bef39076eed11630d0f
workflow-type: tm+mt
source-wordcount: '862'
ht-degree: 2%

---

# 在增強分析中檢視「飛行計畫」視覺效果

「飛行計畫」視覺效果顯示有多少個項目（在套用的篩選條件內）正在執行，這些項目的整個生命週期中發生了哪些條件變化，以及這些項目遵守計畫完成期限的程度。

![](assets/flight-plan-350x132.png)

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
   <td> <p>檢視專案的存取權</p> <p>注意：如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。<br>如需Workfront管理員如何變更您的存取層級的詳細資訊，請參閱 <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>檢視專案的存取權</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 必要條件

如需使用增強分析的必要條件，請參閱 [增強的分析概觀](../enhanced-analytics/enhanced-analytics-overview.md).

## 了解飛行計畫視覺效果

在專案的實際期間中，您只能看到下列專案條件：

* 達成目標
* 有風險
* 陷入困境

若要了解專案條件，請參閱 [專案條件和條件類型概觀](../manage-work/projects/manage-projects/project-condition-and-condition-type.md).

「飛行計畫」視覺效果會顯示下列專案詳細資訊：

* **計畫期間**:水準藍線表示項目的計畫長度，線的任一端都有三角形表示開始日期和結束日期。

   ![](assets/planned-duration-line-350x37.png)

* **實際持續時間**:計畫期間下方的厚彩色線表示項目的實際長度。 線條的顏色會隨著專案在專案生命週期中該特定時間的專案狀況而改變。

   ![](assets/actual-duration-line.png)

* **實際條件**:厚的彩色線也會顯示專案在不同時間的條件。 線條的顏色會根據專案的條件而改變：

   * **綠色**:在Target上
   * **橙色**:風險
   * **紅色**:麻煩

   ![](assets/actual-condition-color.png)

在「飛行計畫」視覺效果中將滑鼠指標暫留在專案列上，您可以看到有關專案計畫時間範圍、目前專案條件，以及（如果適用）自訂條件的資訊。 若要深入了解可能影響持續時間或條件的項目，您可以在「增強分析」區域中查看其他視覺效果。

查看此資訊有助於您確定：

* 哪些事件會將項目延長到原始計畫完成日期之後。
* 當專案開始發生問題時。
* 同一時段內開啟的專案數量。
* 有多少個活動項目。
* 哪些項目需要額外的關注或支援。

如需如何取得此視覺效果最佳資料的詳細資訊，請參閱 [增強的分析概觀](../enhanced-analytics/enhanced-analytics-overview.md).

## 檢視飛行計畫視覺效果

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon-16x12.png)，然後選取 **Analytics**.
1. （可選）若要使用不同的日期範圍，請從日期範圍篩選器中選取新的開始日期和結束日期。

   ![](assets/filters-select-date-range-350x344.png)

   如需使用日期範圍篩選器的詳細資訊，請參閱 [在增強分析中套用篩選器](../enhanced-analytics/use-enhanced-analytics-filters.md).

1. （條件性）如果您需要限制專案資料集，請選取並套用您要使用的篩選器。

   如需在增強分析中新增篩選器的詳細資訊，請參閱 [在增強分析中套用篩選器](../enhanced-analytics/use-enhanced-analytics-filters.md).

   新增篩選器後，最多會顯示50個專案的資料，且即使您離開頁面或登出Workfront，篩選器仍保持作用中狀態。

1. （可選）若要放大日期範圍，請在視覺效果上選取日期範圍開始的點，然後拖曳至日期範圍結束。

   所有其他視覺效果都會更新至相同的日期範圍，並建立時間範圍篩選。

   ![](assets/timeframe-filter-350x220.png)

1. （可選）若要變更專案排序的方式，請按一下 **排序依據** 「飛行計畫」視覺效果右上角的功能表，然後選取新的排序選項：

   * **A - Z**
   * **Z - A**
   * **規劃完成日期**
   * **規劃開始日期**

   頁面上的所有其他視覺效果都會更新，以符合您的排序選取項目。

1. （條件性）如果資料集中有超過50個專案，請使用視覺效果左下角的箭頭，從50個專案群組導覽至下一個專案群組。

   頁面上的所有其他視覺效果都會更新，以符合您的頁面選取範圍。

   ![](assets/pagination-350x118.png)

1. 將滑鼠指標暫留在專案長條圖上，即可查看藍色日期線，以及下列詳細資料：

   * 計畫時間表
   * 目前條件
   * 自訂條件（若適用）

   ![](assets/project-bar-graph-350x143.png)

1. （選用）若要匯出視覺效果資料，請按一下 **匯出** 圖示 ![](assets/export.png) 在視覺效果的右上角，選取匯出格式：

   * **圖表 (PNG)**
   * **資料表(XSLX)**

1. 若要查看更多專案資訊，請按一下視覺效果上的專案，開啟「飛行時」視覺效果中的「燃耗」和「任務」。

   這些視覺效果可協助您深入了解導致專案偏離軌道的原因。 這些功能也讓您輕鬆登入進行中的專案。\
   如需「燃耗」視覺效果的詳細資訊，請參閱 [在Enhanced Analytics中檢視「燃耗」視覺效果](../enhanced-analytics/burndown-overview.md). 如需「飛行視覺效果中的任務」的詳細資訊，請參閱 [在Enhanced Analytics中檢視「飛行中的任務」視覺效果](../enhanced-analytics/tasks-in-flight-overview.md).

