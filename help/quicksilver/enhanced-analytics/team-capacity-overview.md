---
title: 在Enhanced Analytics中檢視「團隊容量」視覺效果
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: 「團隊能力」視覺效果顯示主團隊的總容量，無論它們被過度分配還是分配不足，以及容量在一段時間內的動態程度。
author: Nolan
feature: Reports and Dashboards
exl-id: cfeb1a87-01be-4088-9e33-53a97e3871ad
source-git-commit: 1b1f3c22b8112cfde5b10bef39076eed11630d0f
workflow-type: tm+mt
source-wordcount: '735'
ht-degree: 0%

---

# 在Enhanced Analytics中檢視「團隊容量」視覺效果

「團隊能力」視覺效果顯示主團隊的總容量，無論它們被過度分配還是分配不足，以及容量在一段時間內的動態程度。

![](assets/team-capacity-350x110.png)

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

## 了解團隊容量視覺效果

「團隊能力」視覺效果會顯示指定日期指派給主團隊的工作量。

* **倦怠**:當較深的藍色填充顏色高於虛線時，主團隊分配給他們的工作時間多於他們在團隊可用工作時間內完成的工作時間。 這表明，該團隊被過度配置，可能正在接近倦怠。

   ![](assets/team-capacity-over-capacity.png)

* **無挑戰**:當點線下方的深藍色填色顏色時，主團隊可用的工作時間超過分配給他們的工作量。 這表示該團隊分配不足，可能沒有受到挑戰。

   ![](assets/team-capacity-under-capacity.png)

* **餘額**:當顏色較淺或更透明的藍色填充顏色正上方、正下方或虛線時，主團隊會為他們分配一定的工作時間，以便他們能夠在可用的工作時間內完成工作。 這表示該團隊的工作量更平衡。

   ![](assets/team-capacity-at-capacity.png)

將滑鼠游標暫留在視覺效果的任何點上，可顯示指定日的下列詳細資料：

* **排程小時數**:這是團隊需要完成的計畫工時數。
* **可用時數**:這是該團隊可工作的工時數。
* **容量**:除了能力百分比外，還顯示「能力」、「能力不足」或「能力過剩」的標識。

查看此資訊有助於您確定：

* 當主團隊被過度分配或分配不足時。
* 如果每天總隊被過度分配或分配不足。
* 家庭團隊的工作量每天如何一致。
* 如果新工作造成容量問題。

若要了解如何取得此視覺效果的最佳資料，請參閱 [增強的分析概觀](../enhanced-analytics/enhanced-analytics-overview.md).

## 檢視「團隊能力」視覺效果

1. 按一下「主菜單」表徵圖 ![](assets/main-menu-icon-16x12.png)，然後選取 **Analytics**.
1. 在左側面板中，選取 **人員**.

   ![](assets/people-area-cropped-qs-350x276.png)

1. （可選）若要使用不同的日期範圍，請從日期範圍篩選器中選取新的開始日期和結束日期。

   ![](assets/filters-select-date-range-350x344.png)

   如需使用日期範圍篩選器的詳細資訊，請參閱 [在增強分析中套用篩選器](../enhanced-analytics/use-enhanced-analytics-filters.md).

1. （條件性）如果您尚未設定團隊篩選，請新增團隊篩選，並選取您要查看資料的每個團隊。

   如需在增強分析中新增篩選器的詳細資訊，請參閱 [在增強分析中套用篩選器](../enhanced-analytics/use-enhanced-analytics-filters.md).

   新增篩選器後，最多會顯示50個專案的資料，且即使您離開頁面或登出Workfront，篩選器仍保持作用中狀態。

1. 在「資源容量」視覺效果上，按一下團隊以查看詳細資訊。

   團隊容量視覺效果隨即顯示。

   如需「資源容量」視覺效果的詳細資訊，請參閱 [在Enhanced Analytics中檢視「資源容量」視覺效果](../enhanced-analytics/resource-capacity-overview.md).

1. （可選）若要放大日期範圍，請在視覺效果上選取日期範圍開始的點，然後拖曳至日期範圍結束。

   所有其他視覺效果都會更新至相同的日期範圍，並建立時間範圍篩選。

   ![](assets/timeframe-filter-350x220.png)

1. 將滑鼠指標暫留在圖表線上的某個點上，可查看指定日期的計畫小時數和計畫小時數，以及容量百分比，以及當時主團隊是否已結束、未滿或未滿。

   ![](assets/team-capacity-capacity-pop-up-350x351.png)

1. （選用）若要匯出視覺效果資料，請按一下 **匯出圖示** ![](assets/export.png) 在視覺效果的右上角，選取匯出格式：

   * **圖表 (PNG)**
   * **資料表(XSLX)**

