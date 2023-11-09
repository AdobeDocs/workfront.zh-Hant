---
title: 在增強型分析中檢視資源容量視覺效果
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: 「資源產能」視覺效果會顯示團隊產能是否超出、不足或不足。
author: Nolan
feature: Reports and Dashboards
exl-id: 5bb45ef6-9e49-4063-8e53-c9f3bc994870
source-git-commit: bcafa607da733b89747f6b448dd295d9b906d060
workflow-type: tm+mt
source-wordcount: '826'
ht-degree: 0%

---

# 在增強型分析中檢視資源容量視覺效果

「資源產能」視覺效果會顯示團隊產能是否超出、不足或不足。

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
   <td> <p>檢視專案的存取權</p> <p>注意：如果您還是沒有存取權，請詢問您的Workfront管理員，他們是否在您的存取層級中設定其他限制。<br>如需有關Workfront管理員如何變更您的存取層級的資訊，請參閱 <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>檢視</p> <p>如需請求其他存取許可權的詳細資訊，請參閱 <a href="../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">要求物件的存取權 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的Workfront管理員。

## 必要條件

如需使用增強型Analytics的必要條件，請參閱 [增強型分析概述](../enhanced-analytics/enhanced-analytics-overview.md).

## 瞭解資源容量視覺效果

「資源產能」視覺效果會顯示團隊產能是否超出、不足或不足。 這項計算是根據：

* **可用容量**：主團隊在篩選過的時段內可工作的總時數

  >[!NOTE]
  >
  >如果您檢視的是未來時段，可用容量是根據團隊過去7天的容量計算得出的。 因此，不會考慮任何已排程的PTO。

* **計畫容量**：在篩選的時段內，主團隊預期的計畫工作時數總計

此主團隊計畫時數與實際排程時數的比較可協助您判斷您是否未指派足夠的工作給主團隊，或他們是否可能因大量工作負荷而感到倦怠。

![](assets/resource-capacity-350x110.png)

在「資源產能」視覺效果上，您可以看到下列詳細資料：

* **計畫容量**：與主團隊名稱內聯，藍色圓圈代表指派給主團隊的計畫時數。

  ![](assets/resource-capacity-blue-circle.png)

* **實際容量**：與主團隊名稱內聯，垂直線代表主團隊可用的小時數。

  ![](assets/resource-capacity-vertical-line.png)

* **超出容量**：當水平線和藍色圓圈顯示在垂直線的右側時，主團隊被指派了比他們可以在可用時數中完成更多的工作量。 這表示該團隊在篩選過的時段內可能超出容量。 團隊需要完成的剩餘小時數會顯示在藍色圓圈的右側。

  ![](assets/resource-capacity-over-capacity.png)

* **容量不足**：當水平線和藍色圓圈顯示在垂直線的左側時，主團隊的可用時數多於指派給他們的計畫工作時數。 這表示該團隊在篩選過的時段內可能沒有足夠的容量。 主團隊完成工作的額外可用時數會顯示在藍色圓圈的左側。

  ![](assets/resource-capacity-under-capacity.png)

將游標暫留在列上會顯示計畫容量和可用容量的確切小時數，以及主團隊超出或不足容量的小時數。

檢視此資訊可協助您判斷：

* 如果主團隊配置過多或不足。
* 主團隊專注的最大專案是什麼。
* 哪些主團隊可以工作。

若要瞭解如何針對此視覺效果取得最佳資料，請參閱 [增強型分析概述](../enhanced-analytics/enhanced-analytics-overview.md).

## 檢視資源產能視覺效果

1. 按一下主要功能表圖示 ![](assets/main-menu-icon-16x12.png)，然後選取 **Analytics**.
1. 在左側面板中，選取 **人員**.

   ![](assets/people-area-cropped-qs-350x276.png)

1. （可選）若要使用不同的日期範圍，請從日期範圍篩選器中選取新的開始和結束日期。

   ![](assets/filters-select-date-range-350x344.png)

   如需有關使用日期範圍篩選的資訊，請參閱 [在增強型分析中套用篩選器](../enhanced-analytics/use-enhanced-analytics-filters.md).

1. （視條件而定）如果您尚未設定團隊篩選器，請新增團隊篩選器，並選取您要檢視其資料的每個團隊。

   如需在增強型分析中新增篩選器的詳細資訊，請參閱 [在增強型分析中套用篩選器](../enhanced-analytics/use-enhanced-analytics-filters.md).

   新增篩選器後，系統會顯示最多50個專案的資料，而且即使您離開頁面或登出Workfront，篩選器仍會保持作用中。

1. （可選）若要放大日期範圍，請在視覺效果上選取一個點，作為日期範圍的起點，並拖曳至日期範圍的終點。

   所有其他視覺效果會更新至相同的日期範圍，並建立時間範圍篩選器。

   ![](assets/timeframe-filter-350x220.png)

1. 將滑鼠停留在主團隊線上可檢視還有多少小時可供排程、主團隊要完成的計畫時數以及標籤為超出、不足或處於產能的工作小時總數。

   ![](assets/resource-capacity-capacity-pop-up-350x213.png)

1. （選用）若要匯出視覺效果資料，請按一下 **「匯出」圖示** ![](assets/export.png) 然後選取匯出格式：

   * **圖表 (PNG)**
   * **資料表格(XSLX)**

1. 按一下主團隊名稱可檢視團隊容量視覺效果中的更多資訊。

   若要深入瞭解團隊容量視覺效果，請參閱 [在Enhanced Analytics中檢視團隊容量視覺效果](../enhanced-analytics/team-capacity-overview.md).


