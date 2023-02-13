---
title: 在增強分析中檢視專案活動視覺效果
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: 「項目活動」視覺效果顯示在特定時間範圍內發生的項目級別活動（指派給項目的每個人員的活動）的匯總視圖。 您可以縮小焦點來了解專案內的活動，或將專案活動與Adobe Workfront中的其他專案進行比較。
author: Nolan
feature: Reports and Dashboards
exl-id: 9ef52be8-48d0-4f83-a214-dd32e794c73e
source-git-commit: 1b1f3c22b8112cfde5b10bef39076eed11630d0f
workflow-type: tm+mt
source-wordcount: '800'
ht-degree: 1%

---

# 在增強分析中檢視專案活動視覺效果

「項目活動」視覺效果顯示在特定時間範圍內發生的項目級別活動（指派給項目的每個人員的活動）的匯總視圖。 您可以縮小焦點來了解專案內的活動，或將專案活動與Adobe Workfront中的其他專案進行比較。

>[!NOTE]
>
>「依團隊的活動」視覺效果的運作方式與此視覺效果類似，但「依團隊的活動」視覺效果會顯示所有專案的主團隊活動。\
>如需「依團隊劃分的活動」視覺效果的相關資訊，請參閱 [在Enhanced Analytics中依團隊視覺效果檢視活動](../enhanced-analytics/activity-by-team-overview.md).

<!--WRITER bad link; there is no Activity by Team.png
[![](assets/project-activity-350x114.png)](../Resources/Images/Analytics/Activity by Team.png)
-->

## 存取需求

您必須具備下列條件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">Workfront計畫</a>*</td> 
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

## 了解專案活動視覺效果

專案活動會以不同顏色顯示，匯總專案中一段時間的特定事件：

* **登入的使用者**:紫色方塊顯示指派給該專案的人員在當天登入。 較深的陰影表示登入的人數較多。

   ![](assets/project-activity-users-logged-in.png)

* **任務狀態更改**:粉紅色方塊顯示當天人們已變更專案任務的狀態。 較深的陰影表示任務狀態發生更多變化。

   ![](assets/project-activity-task-status-changes.png)

* **任務已完成**:藍色方塊顯示人員已完成專案的工作。 較深的陰影表示已完成的任務數量較多。

   ![](assets/project-activity-tasks-completed.png)

將滑鼠指標暫留在方塊上，會顯示指定一天中動作完成的確切次數。 您可以選取專案，依專案中每個個別貢獻者來查看這些活動的劃分。

查看此資訊有助於您確定：

* 特定專案上的活動。
* 與其他項目相比，一個項目的活動。
* 哪些使用者正在處理專案，以及以什麼頻率處理。

若要了解如何取得此視覺效果的最佳資料，請參閱 [增強的分析概觀](../enhanced-analytics/enhanced-analytics-overview.md).

## 檢視專案活動視覺效果

1. 按一下「主菜單」表徵圖 ![](assets/main-menu-icon-16x12.png)，然後選取 **Analytics**.
1. （可選）若要使用不同的日期範圍，請從日期範圍篩選器中選取新的開始日期和結束日期。

   ![](assets/filters-select-date-range-350x344.png)

   如需使用日期範圍篩選器的詳細資訊，請參閱 [在增強分析中套用篩選器](../enhanced-analytics/use-enhanced-analytics-filters.md).

   >[!NOTE]
   >
   >如果您選取的期間超過3個月的日期範圍，專案活動視覺效果不會顯示任何資料。

1. （條件性）如果您需要限制專案資料集，請選取並套用您要使用的篩選器。

   如需在增強分析中新增篩選器的詳細資訊，請參閱 [在增強分析中套用篩選器](../enhanced-analytics/use-enhanced-analytics-filters.md).

   新增篩選器後，最多會顯示50個專案的資料，且即使您離開頁面或登出Workfront，篩選器仍保持作用中狀態。

1. （可選）若要放大日期範圍，請在視覺效果上選取日期範圍開始的點，然後拖曳至日期範圍結束。

   所有其他視覺效果都會更新至相同的日期範圍，並建立時間範圍篩選。

   ![](assets/timeframe-filter-350x220.png)

1. （可選）若要變更專案排序的方式，請按一下 **排序依據** ，然後選擇新的排序選項：

   * **A - Z**
   * **Z - A**
   * **規劃完成日期**
   * **規劃開始日期**

   頁面上的所有其他視覺效果都會更新，以符合您的排序選取項目。

1. （條件性）如果資料集中有超過50個專案，請使用視覺效果左下角的箭頭，從50個專案群組導覽至下一個專案群組。

   頁面上的所有其他視覺效果都會更新，以符合您的頁面選取範圍。

   ![](assets/pagination-350x118.png)

1. 按一下視覺效果中的專案，即可查看專案的詳細資訊。

   清單會展開並顯示專案上每個貢獻者的活動。

1. 將滑鼠移至方塊上，可查看使用者完成動作的日期，以及該日的動作完成次數。

   ![](assets/project-activity-activity-pop-up-350x137.png)

1. （選用）若要匯出視覺效果資料，請按一下 **匯出圖示** ![](assets/export.png) 在視覺效果的右上角，選取匯出格式：

   * **圖表 (PNG)**
   * **資料表(XSLX)**

