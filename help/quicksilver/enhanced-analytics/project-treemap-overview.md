---
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
title: 在增強的分析中檢視專案樹狀圖視覺效果
description: 「項目樹狀圖」視覺效果是特定時間窗口內工作的小時（或天）視圖，與其他工作時間（或天）相比較。 這可協助您了解使用者專為專案所花的時間。
author: Nolan
feature: Reports and Dashboards
exl-id: 6216465e-c3bb-4f2f-b71c-766ad0c2ed40
source-git-commit: 1b1f3c22b8112cfde5b10bef39076eed11630d0f
workflow-type: tm+mt
source-wordcount: '858'
ht-degree: 1%

---

# 在增強的分析中檢視專案樹狀圖視覺效果

「項目樹狀圖」視覺效果是特定時間窗口內工作的小時（或天）視圖，與其他工作時間（或天）相比較。 這可協助您了解使用者專為專案所花的時間。

![](assets/project-treemap-350x126.png)

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
   <td> <p>檢視</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 必要條件

如需使用增強分析的必要條件，請參閱 [增強的分析概觀](../enhanced-analytics/enhanced-analytics-overview.md).

## 了解專案樹狀圖視覺效果

「專案樹狀圖」視覺效果中的方塊代表專案，而方塊的大小則顯示不同專案所花時間的比較。 方塊越大，專案逗留的時間就越多。

「專案樹狀圖」視覺效果由下列部分組成：

* **較小的淺藍色框**:小時數（或天數）較少的專案會顯示為藍色較小的方塊。

   ![](assets/project-treemap-smaller-box.png)

* **更大的深藍色框**:有較長時間（或天數）的專案會顯示為深藍色的較大方塊。

   ![](assets/project-treemap-larger-box-350x205.png)

* **中型藍盒**:介於兩個類別之間的專案會顯示為中等大小的方塊，在深藍色和淺藍色之間有藍色的陰影。 中型盒子有3種可能的藍色。

右側的圖例顯示每個藍色陰影的已完成小時數劃分。 此圖例為動態圖例，會根據資料更新。

![](assets/project-treemap-hours-completed.png)

>[!NOTE]
>
>如果您是依期間（而非依計畫小時）查看「專案樹狀圖」視覺效果，此圖例會顯示每個藍色陰影的工作天數劃分。\
>![](assets/project-treemap-days-worked.png)>

查看此資訊有助於您確定：

* 在所選日期範圍內處理之項目的優先順序。
* 哪些團隊在花時間。
* 如果團隊關注正確的事情。
* 按一下特定專案後，該時段內專案的範圍變更了多少。

若要了解如何取得此視覺效果的最佳資料，請參閱 [增強的分析概觀](../enhanced-analytics/enhanced-analytics-overview.md).

## 檢視專案樹狀圖視覺效果

1. 按一下「主菜單」表徵圖 ![](assets/main-menu-icon-16x12.png)，然後選取 **Analytics**.
1. （可選）若要使用不同的日期範圍，請從日期範圍篩選器中選取新的開始日期和結束日期。

   ![](assets/filters-select-date-range-350x344.png)

   如需使用日期範圍篩選器的詳細資訊，請參閱 [在增強分析中套用篩選器](../enhanced-analytics/use-enhanced-analytics-filters.md).

1. （條件性）如果您需要限制專案資料集，請選取並套用您要使用的篩選器。

   如需在增強分析中新增篩選器的詳細資訊，請參閱 [在增強分析中套用篩選器](../enhanced-analytics/use-enhanced-analytics-filters.md).

   新增篩選器後，最多會顯示50個專案的資料，且即使您離開頁面或登出Workfront，篩選器仍保持作用中狀態。

1. （可選）若要變更專案排序的方式，請按一下 **排序依據** 「專案樹狀圖」視覺效果的右上角，選取新的排序選項：

   * **A - Z**
   * **Z - A**
   * **規劃完成日期**
   * **規劃開始日期**

   頁面上的所有其他視覺效果都會更新，以符合您的排序選取項目。

1. （條件性）如果資料集中有超過50個專案，請使用視覺效果左下角的箭頭，從50個專案群組導覽至下一個專案群組。

   頁面上的所有其他視覺效果都會更新，以符合您的頁面選取範圍。

   ![](assets/pagination-350x118.png)

1. （可選）將檢視從 **計畫小時數** to **持續時間**.

   預設會選取計畫小時數。

1. 將滑鼠指標暫留在專案上，即可查看專案條件，以及總計畫小時數、總完成小時數，以及每日在專案上逗留的平均小時數。

   ![](assets/project-treemap-project-details-350x404.png)

   >[!NOTE]
   >
   >如果您選取 **持續時間** 檢視，您會看到下列持續時間詳細資訊：
   >
   >* **計畫時間範圍**:計畫完成項目的天數。
   >* **工作天數**:在頂部所選日期範圍內完成的每個任務的計畫持續時間，除以一天中的小時數。

   >   
   >![](assets/duration-treemap-350x159.png)
   >
   >如需持續時間的詳細資訊，請參閱 [增強的分析概觀](../enhanced-analytics/enhanced-analytics-overview.md).

1. （選用）若要匯出視覺效果資料，請按一下 **匯出圖示** ![](assets/export.png) 在視覺效果的右上角，選取匯出格式：

   * **圖表 (PNG)**
   * **資料表(XSLX)**

1. 按一下專案以開啟飛行視覺效果中的「燃盡」和「任務」，以便深入了解任務和小時數（或天數）對專案大小的貢獻。

如需「燃耗」視覺效果的詳細資訊，請參閱 [在Enhanced Analytics中檢視「燃耗」視覺效果](../enhanced-analytics/burndown-overview.md). 如需「飛行視覺效果中的任務」的詳細資訊，請參閱 [在Enhanced Analytics中檢視「飛行中的任務」視覺效果](../enhanced-analytics/tasks-in-flight-overview.md).

