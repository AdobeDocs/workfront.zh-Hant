---
title: 在Enhanced Analytics中檢視依團隊的活動視覺效果
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: 依團隊的活動視覺效果會顯示在主團隊的特定時間範圍內發生的活動，可讓您瞭解不同的主團隊在Adobe Workfront中花費時間的情況。 根據您的主團隊在Workfront中的設定方式，此視覺效果可提供您不同的深入見解並回答不同的問題。
author: Nolan
feature: Reports and Dashboards
exl-id: c4f9886c-ce76-43a8-bd43-cb64fff27e79
source-git-commit: 325334010d5f1206931cc9ace67f9511d614ffca
workflow-type: tm+mt
source-wordcount: '727'
ht-degree: 7%

---

# 在Enhanced Analytics中檢視依團隊的活動視覺效果

<!-- Audited: 12/2023 -->

依團隊的活動視覺效果會顯示在主團隊的特定時間範圍內發生的活動，可讓您瞭解不同的主團隊在Adobe Workfront中花費時間的情況。 根據您的主團隊在Workfront中的設定方式，此視覺效果可提供您不同的深入見解並回答不同的問題。

>[!NOTE]
>
>專案活動視覺效果類似於此視覺效果，但它是根據指派給專案的人顯示活動，而不是根據指派給主團隊的人顯示活動。\
>如需有關專案活動視覺效果的資訊，請參閱[在增強型分析中檢視專案活動視覺效果](../enhanced-analytics/project-activity-overview.md)。

![依團隊的活動](assets/activity-by-team-350x113.png){width="700"}

## 存取需求

+++ 展開以檢視存取需求。

您必須具有下列存取權才能執行本文中的步驟：

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
   <td>
      <p>新增：</p> 
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

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 先決條件

如需使用增強型分析的先決條件，請參閱[增強型分析概觀](../enhanced-analytics/enhanced-analytics-overview.md)中的「先決條件」一節。

## 依團隊瞭解活動視覺效果

不同的活動會以不同的顏色顯示，以總結經過篩選的時段內的特定事件：

* **登入的使用者**：紫色方塊顯示主團隊的人員當天登入。 顏色越深表示登入人數越多。

  ![個使用者已登入](assets/project-activity-users-logged-in.png)

* **任務狀態變更**：粉紅色方塊顯示主團隊的人員在當天變更了任務的狀態。 顏色深表示發生狀態變更的任務數量較多。

  ![任務狀態變更](assets/project-activity-task-status-changes.png)

* **已完成任務**：藍色方塊顯示主團隊中的人員已於當天完成任務。 顏色深表示完成的任務數量較多。

  ![個已完成的工作](assets/project-activity-tasks-completed.png)

將游標暫留在方塊上會顯示指定日期內完成動作的確切次數。 您可以選取一個團隊，以檢視主團隊中每個人的這些活動劃分。

查看這些資訊可協助您判斷：

* 主團隊中正在進行哪些活動以及以什麼速率進行。
* 哪些主團隊超負荷工作或更多地使用系統。
* 對於主團隊的工作分配是否適當。

若要瞭解如何取得此視覺效果的最佳資料，請參閱[增強型分析概述](../enhanced-analytics/enhanced-analytics-overview.md)。

## 依團隊檢視活動視覺效果

1. 按一下主功能表圖示![主功能表圖示](assets/main-menu-icon-16x12.png)，然後選取&#x200B;**Analytics**。
1. 在左側面板中，選取&#x200B;**人員**。

   ![人員區域](assets/people-area-cropped-qs-350x276.png)

1. （可選）若要使用不同的日期範圍，請從日期範圍篩選器中選取新的開始和結束日期。

   ![選取日期範圍](assets/filters-select-date-range-350x344.png)

   如需有關使用日期範圍篩選的資訊，請參閱[在增強型分析中套用篩選](../enhanced-analytics/use-enhanced-analytics-filters.md)。

1. （視條件而定）如果您尚未設定團隊篩選器，請新增團隊篩選器，並選取您要檢視其資料的每個團隊。

   如需在增強型分析中新增篩選器的詳細資訊，請參閱[在增強型分析中套用篩選器](../enhanced-analytics/use-enhanced-analytics-filters.md)。

   新增篩選器後，系統會顯示最多50個專案的資料，而且即使您離開頁面或登出Workfront，篩選器仍會保持作用中。

1. （可選）若要放大日期範圍，請在視覺效果上選取一個點，作為日期範圍的起點，並拖曳至日期範圍的終點。

   所有其他視覺效果會更新至相同的日期範圍，並建立時間範圍篩選器。

   ![時間範圍篩選器](assets/timeframe-filter-350x220.png)

1. 按一下團隊名稱

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   or role
   </MadCap:conditionalText>
   -->

   以檢視主團隊完成活動的更多詳細資料。

   清單會展開並顯示指派給主團隊的每個人的活動。

   <!--
   <span style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode"> Role not available</span>
   -->

1. 將游標停留在彩色方塊上，可檢視使用者完成動作的日期以及當天完成動作的次數。

   較暗的顏色表示較高的活動。

   ![依團隊的活動](assets/activity-by-team-activity-pop-up-350x155.png)

1. （選擇性）若要匯出視覺效果資料，請按一下視覺效果右上角的匯出圖示![匯出圖示](assets/export.png)，然後選取匯出格式：

   * **圖表(PNG)**
   * **資料表(XSLX)**

