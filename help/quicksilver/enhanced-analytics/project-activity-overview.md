---
title: 在增強型分析中檢視專案活動視覺效果
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: 專案活動視覺效果會顯示專案層級的活動彙總檢視，也就是指派給專案的每個人的活動，這些活動發生在特定的時間範圍內。 您可以縮小焦點來瞭解專案中的活動，或在Adobe Workfront中將專案活動與其他專案進行比較。
author: Nolan
feature: Reports and Dashboards
exl-id: 9ef52be8-48d0-4f83-a214-dd32e794c73e
source-git-commit: 4e928defe9b6271cef64f6554e91af4fc31ddeca
workflow-type: tm+mt
source-wordcount: '757'
ht-degree: 8%

---

# 在增強型分析中檢視專案活動視覺效果

<!-- Audited: 12/2023 -->

專案活動視覺效果會顯示專案層級的活動彙總檢視，也就是指派給專案的每個人的活動，這些活動發生在特定的時間範圍內。 您可以縮小焦點來瞭解專案中的活動，或在Adobe Workfront中將專案活動與其他專案進行比較。

>[!NOTE]
>
>「依團隊的活動」視覺效果的行為與此視覺效果類似，但「依團隊的活動」視覺效果顯示所有專案的主要團隊活動。\
>如需「依團隊的活動」視覺效果的資訊，請參閱 [在Enhanced Analytics中檢視依團隊的活動視覺效果](../enhanced-analytics/activity-by-team-overview.md).

## 存取需求

您必須具備下列條件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">Workfront計畫</a></td> 
   <td> <p>商務或以上版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront授權總覽</a></td> 
   <td>   <p>新增：</p> 
   <ul><li>淺色或更高</li></ul>
   <p>目前：</p>
   <ul><li>評論或以上</li></ul>
 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>檢視專案的存取權</p> <!--<p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level.<br>For information on how a Workfront administrator can change your access level, see <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p>--> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>檢視</p> <!--<p>For information on requesting additional access, see <a href="../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p>--> </td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱 [Workfront檔案中的存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## 先決條件

如需使用增強型Analytics的必要條件，請參閱 [增強型分析概述](../enhanced-analytics/enhanced-analytics-overview.md).

## 瞭解專案活動視覺效果

專案活動會以不同顏色顯示，以隨著期間摘要出專案中的特定事件：

* **使用者已登入**：紫色方塊顯示指派給專案的使用者當天登入。 顏色越深表示登入人數越多。

  ![](assets/project-activity-users-logged-in.png)

* **任務狀態變更**：粉紅色方塊顯示人員當天變更了專案任務的狀態。 顏色深表示發生狀態變更的任務數量較多。

  ![](assets/project-activity-task-status-changes.png)

* **任務已完成**：藍色方塊顯示人員已完成專案的工作。 顏色深表示完成的任務數量較多。

  ![](assets/project-activity-tasks-completed.png)

將游標暫留在方塊上會顯示指定日期內完成動作的確切次數。 您可以選取專案，依專案上的每位投稿人來檢視這些活動的劃分。

查看這些資訊可協助您判斷：

* 特定專案的活動。
* 比較一個專案與另一個專案的活動。
* 哪些用戶正在處理項目以及頻率如何。

若要瞭解如何針對此視覺效果取得最佳資料，請參閱 [增強型分析概述](../enhanced-analytics/enhanced-analytics-overview.md).

## 檢視專案活動視覺效果

1. 按一下主要功能表圖示 ![](assets/main-menu-icon-16x12.png)，然後選取 **Analytics**.
1. （可選）若要使用不同的日期範圍，請從日期範圍篩選器中選取新的開始和結束日期。

   ![](assets/filters-select-date-range-350x344.png)

   如需有關使用日期範圍篩選的資訊，請參閱 [在增強型分析中套用篩選器](../enhanced-analytics/use-enhanced-analytics-filters.md).

   >[!NOTE]
   >
   >如果您選取的日期範圍超過3個月，專案活動視覺效果不會顯示任何資料。

1. （視條件而定）如果您需要限制專案資料集，請選取並套用您要使用的篩選器。

   如需在增強型分析中新增篩選器的詳細資訊，請參閱 [在增強型分析中套用篩選器](../enhanced-analytics/use-enhanced-analytics-filters.md).

   新增篩選器後，系統會顯示最多50個專案的資料，而且即使您離開頁面或登出Workfront，篩選器仍會保持作用中。

1. （可選）若要放大日期範圍，請在視覺效果上選取一個點，作為日期範圍的起點，並拖曳至日期範圍的終點。

   所有其他視覺效果會更新至相同的日期範圍，並建立時間範圍篩選器。

   ![](assets/timeframe-filter-350x220.png)

1. （選用）若要變更專案的排序方式，請按一下 **排序依據：** 功能表，然後選取新的排序選項：

   * **A - Z**
   * **Z - A**
   * **計畫完成日期**
   * **計劃開始日期**

   頁面上的其他所有視覺效果都會更新以符合您的排序選擇。

1. （條件式）如果您的資料集超過50個專案，請使用視覺效果左下角的箭頭，從一個50個專案群組瀏覽至下一個專案。

   頁面上的所有其他視覺效果都會更新以符合您的頁面選擇。

   ![](assets/pagination-350x118.png)

1. 按一下視覺效果中的專案，即可檢視專案的詳細資訊。

   清單會展開並顯示專案中每個貢獻者的活動。

1. 將滑鼠移至方塊上，可檢視使用者完成動作的日期，以及當天動作完成的次數。

   ![](assets/project-activity-activity-pop-up-350x137.png)

1. （選用）若要匯出視覺效果資料，請按一下 **「匯出」圖示** ![](assets/export.png) 然後選取匯出格式：

   * **圖表(PNG)**
   * **資料表格(XSLX)**

