---
title: 在Enhanced Analytics中依團隊視覺效果檢視活動
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: 「依團隊的活動」視覺效果顯示家庭團隊的特定時間範圍期間發生的活動，讓您了解不同家庭團隊在Adobe Workfront中的逗留時間。 根據您在Workfront中的首頁團隊設定方式，此視覺效果可提供不同的深入分析並回答不同的問題。
author: Nolan
feature: Reports and Dashboards
exl-id: c4f9886c-ce76-43a8-bd43-cb64fff27e79
source-git-commit: 1b1f3c22b8112cfde5b10bef39076eed11630d0f
workflow-type: tm+mt
source-wordcount: '734'
ht-degree: 0%

---

# 在Enhanced Analytics中依團隊視覺效果檢視活動

「依團隊的活動」視覺效果顯示家庭團隊的特定時間範圍期間發生的活動，讓您了解不同家庭團隊在Adobe Workfront中的逗留時間。 根據您在Workfront中的首頁團隊設定方式，此視覺效果可提供不同的深入分析並回答不同的問題。

>[!NOTE]
>
>「專案」活動視覺效果類似於此視覺效果，但會根據指派給專案的人員，而非指派給主團隊的人員，來顯示活動。\
>如需「專案活動」視覺效果的相關資訊，請參閱 [在增強分析中檢視專案活動視覺效果](../enhanced-analytics/project-activity-overview.md).

![](assets/activity-by-team-350x113.png)

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

## 依團隊視覺效果了解活動

不同的活動會以不同的顏色顯示，以匯總篩選時段內的特定事件：

* **登入的使用者**:紫色方塊顯示主團隊中的人員當天登入。 較深的陰影表示登入的人數較多。

   ![](assets/project-activity-users-logged-in.png)

* **任務狀態更改**:粉紅色方塊顯示主團隊的人員在當天變更了工作的狀態。 較深的陰影表示任務狀態發生更多變化。

   ![](assets/project-activity-task-status-changes.png)

* **任務已完成**:藍色方塊顯示主團隊的人員在當天完成工作。 較深的陰影表示已完成的任務數量較多。

   ![](assets/project-activity-tasks-completed.png)

將滑鼠指標暫留在方塊上，會顯示指定一天中動作完成的確切次數。 您可以選取一個團隊，依據主團隊中的每個人，查看這些活動的劃分。

查看此資訊有助於您確定：

* 家庭團隊內發生的活動以及發生的頻率。
* 哪些主團隊工作過度，或更多地使用系統。
* 如果工作分配適合本隊。

若要了解如何取得此視覺效果的最佳資料，請參閱 [增強的分析概觀](../enhanced-analytics/enhanced-analytics-overview.md).

## 依團隊視覺效果檢視活動

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

1. 按一下團隊名稱

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   or role
   </MadCap:conditionalText>
   -->

   查看主團隊完成的活動的詳細資訊。

   清單會展開並顯示指派給主團隊之每個人員的活動。

   <!--
   <span style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode"> Role not available</span>
   -->

1. 將滑鼠指標暫留在彩色方塊上，可查看使用者完成動作的日期，以及該動作在該天完成的次數。

   較深的顏色表示活動較高。

   ![](assets/activity-by-team-activity-pop-up-350x155.png)

1. （選用）若要匯出視覺效果資料，請按一下「匯出」圖示 ![](assets/export.png) 在視覺效果的右上角，選取匯出格式：

   * **圖表 (PNG)**
   * **資料表(XSLX)**

