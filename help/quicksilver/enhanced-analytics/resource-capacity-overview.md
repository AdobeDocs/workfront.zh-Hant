---
title: 在Enhanced Analytics中檢視「資源容量」視覺效果
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: 「資源能力」視覺效果會顯示團隊是否已結束、未滿或已滿。 此計算基於 — EDIT ME。
author: Nolan
feature: Reports and Dashboards
exl-id: 5bb45ef6-9e49-4063-8e53-c9f3bc994870
source-git-commit: 1b1f3c22b8112cfde5b10bef39076eed11630d0f
workflow-type: tm+mt
source-wordcount: '833'
ht-degree: 0%

---

# 在Enhanced Analytics中檢視「資源容量」視覺效果

「資源能力」視覺效果會顯示團隊是否已結束、未滿或已滿。

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

## 了解資源容量視覺效果

「資源能力」視覺效果會顯示團隊是否已結束、未滿或已滿。 此計算基於：

* **可用容量**:家庭團隊在經過篩選的時間段內可工作的總小時數

   >[!NOTE]
   >
   >如果您查看的是未來時段，則可用容量會根據團隊過去7天的容量計算。 因此，不會考慮任何計畫PTO。

* **計畫容量**:在經過篩選的時段內，預計由主團隊完成的總計工作時數

將家庭團隊的計畫時間與實際的計畫時間進行比較可以幫助您確定是否沒有為家庭團隊分配足夠的工作，或者他們是否可能因工作量過重而筋疲力盡。

![](assets/resource-capacity-350x110.png)

在「資源容量」視覺效果上，您可以看到下列詳細資料：

* **計畫容量**:藍色圓圈內嵌在主團隊名稱中，代表分配給主團隊的計畫小時數。

   ![](assets/resource-capacity-blue-circle.png)

* **實際能力**:垂直線內嵌在主團隊名稱中，表示主團隊可用的小時數。

   ![](assets/resource-capacity-vertical-line.png)

* **超容量**:當水準線和藍色圓圈顯示在垂直線的右側時，家庭小組被分配的工作量超過了他們在可用小時數內完成的工作量。 這表示在篩選的時段內，團隊可能超過容量。 藍色圓圈右側顯示團隊完成所需的剩餘小時數。

   ![](assets/resource-capacity-over-capacity.png)

* **能力不足**:當水準線和藍色圓圈顯示在垂直線的左側時，主團隊的可用小時數多於他們分配的計畫工時數。 這表示該團隊在經過篩選的時段內可能容量不足。 藍色圓圈左側會顯示家庭團隊完成工作的額外可用小時數。

   ![](assets/resource-capacity-under-capacity.png)

將滑鼠暫留在行上，可顯示計畫容量和可用容量的確切小時數，以及主團隊超出或低於容量的小時數。

查看此資訊有助於您確定：

* 如果主團隊的分配過多或分配不足。
* 最大的項目是家庭團隊關注的。
* 哪些主隊可以工作。

若要了解如何取得此視覺效果的最佳資料，請參閱 [增強的分析概觀](../enhanced-analytics/enhanced-analytics-overview.md).

## 檢視資源容量視覺效果

1. 按一下「主菜單」表徵圖 ![](assets/main-menu-icon-16x12.png)，然後選取 **Analytics**.
1. 在左側面板中，選取 **人員**.

   ![](assets/people-area-cropped-qs-350x276.png)

1. （可選）若要使用不同的日期範圍，請從日期範圍篩選器中選取新的開始日期和結束日期。

   ![](assets/filters-select-date-range-350x344.png)

   如需使用日期範圍篩選器的詳細資訊，請參閱 [在增強分析中套用篩選器](../enhanced-analytics/use-enhanced-analytics-filters.md).

1. （條件性）如果您尚未設定團隊篩選，請新增團隊篩選，並選取您要查看資料的每個團隊。

   如需在增強分析中新增篩選器的詳細資訊，請參閱 [在增強分析中套用篩選器](../enhanced-analytics/use-enhanced-analytics-filters.md).

   新增篩選器後，最多會顯示50個專案的資料，且即使您離開頁面或登出Workfront，篩選器仍保持作用中狀態。

1. （可選）若要放大日期範圍，請在視覺效果上選取日期範圍開始的點，然後拖曳至日期範圍結束。

   所有其他視覺效果都會更新至相同的日期範圍，並建立時間範圍篩選。

   ![](assets/timeframe-filter-350x220.png)

1. 將滑鼠指標暫留在主團隊線上，查看仍可計畫的小時數、主團隊要完成的計畫小時數，以及標籤為「超過」、「不足」或「容量」的工作小時數總計。

   ![](assets/resource-capacity-capacity-pop-up-350x213.png)

1. （選用）若要匯出視覺效果資料，請按一下 **匯出圖示** ![](assets/export.png) 在視覺效果的右上角，選取匯出格式：

   * **圖表 (PNG)**
   * **資料表(XSLX)**

1. 按一下主團隊名稱，以在「團隊容量」視覺效果中查看詳細資訊。

   若要進一步了解「團隊能力」視覺效果，請參閱 [在Enhanced Analytics中檢視「團隊容量」視覺效果](../enhanced-analytics/team-capacity-overview.md).


