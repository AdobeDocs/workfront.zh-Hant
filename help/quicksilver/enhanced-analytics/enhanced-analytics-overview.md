---
title: 增強的分析概觀
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: 增強分析是Adobe Workfront中功能強大的工具，具有預先建立的視覺效果，可讓您查看專案資料，並透過規劃和完成來識別趨勢。 這項專案分析可協助您管理目前的工作，並讓您為未來的工作更精確地規劃。
author: Nolan
feature: Reports and Dashboards
exl-id: a14ad57c-859b-43df-84c0-575ccda86e50
source-git-commit: 1b1f3c22b8112cfde5b10bef39076eed11630d0f
workflow-type: tm+mt
source-wordcount: '1354'
ht-degree: 2%

---

# 增強的分析概觀

增強分析是Adobe Workfront中功能強大的工具，具有預先建立的視覺效果，可讓您查看專案資料，並透過規劃和完成來識別趨勢。 這項專案分析可協助您管理目前的工作，並讓您為未來的工作更精確地規劃。

增強的分析功能可協助您識別：

* 您規劃專案的方式
* 將工作新增至專案時
* 為不同項目完成的工作量
* 完成項目所需的小時數或天數，與主團隊計畫的小時數或天數相比
* 使用者在專案期間完成特定動作的頻率
* 項目進度以及項目內的個別任務

![](assets/nwe-full-screen-analytics-350x222.png)

若要查看使用案例或進一步了解如何透過Enhanced Analytics管理目前的工作和規劃未來的工作，請參閱 [增強的分析學習路徑](https://one.workfront.com/s/enhanced-analytics-program).

## 必要條件

若要存取「增強分析」區域，您必須：

* 制定業務或企業計畫。

   如需詳細資訊，請參閱 [Workfront計畫](https://www.workfront.com/plans).

* 請Workfront管理員將Enhanced Analytics新增至版面範本。

   如需詳細資訊，請參閱 [增強的分析功能：將分析新增至版面範本](https://one.workfront.com/s/managed-content-videos/enhanced-analytics-adding-analytics-to-layout-templates-MCH7URDSIXRREHHHF7TRTYYP2LTE).

要查看項目和任務的資訊，您必須：

* 具有訪問級別中「項目」和「任務」區域的「查看」權限。

   如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 [建立或修改自訂存取層級](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

* 具有特定任務和/或項目的「查看」權限。

   有關請求其他訪問的資訊，請參閱 [請求對對象的訪問](../workfront-basics/grant-and-request-access-to-objects/request-access.md).

## 增強分析的最佳作法

為了取得專案的最佳資料，請使用具有精確計畫小時數和持續時間天數的範本。 您也需要確定您的使用者盡可能準確地輸入及更新下方欄位。

>[!NOTE]
>
>下列部分欄位是Workfront根據使用者輸入的資訊執行的計算。 您無法手動更新這些欄位。

* 計畫小時

   這是最需要填寫的欄位。

   >[!NOTE]
   >
   >如果您的團隊未使用計畫小時數，您仍可以根據專案持續時間查看一些資料。\
   >如需詳細資訊，請參閱 [持續時間檢視](#duration-view) 這篇文章。

* 專案名稱

   名稱應該是專案的描述性名稱。

* 專案狀況
* 專案狀態
* 項目計劃開始日期
* 計畫完成日期
* 項目實際開始日期
* 項目實際結束日期
* 專案持續時間小時
* 項目實際小時數
* 任務狀態（包括標籤任務已完成。）
* 任務名稱
* 任務完成百分比
* 任務計畫起始日期
* 任務計畫完成日期

>[!IMPORTANT]
>
>對工作和專案所做的變更需要最多24小時，才能在Enhanced Analytics中反映。

## 持續時間檢視 {#duration-view}

依預設，「燃耗」和「專案」樹狀圖視覺效果是根據計畫小時數。 如果您的團隊未使用計畫小時數，您可以根據專案持續時間來查看這些視覺效果。

在增強分析中，專案的持續時間是透過下列公式計算：

* 計畫時間範圍:

   ```
   Planned Completion Date of the project - Start Date of the project
   ```

* 已工作天數:

   ```
   Planned Duration for tasks completed in the selected date range / Typical hours per work day
   ```

   >[!NOTE]
   >
   >8小時是 **每個工作日的一般小時數**. Adobe Workfront管理員可以更新 **每個工作日的一般小時數** 設定 **設定** > **專案偏好設定** > **專案** > **時間軸**.\
   >若要進一步了解，請參閱 [配置系統範圍的項目首選項](../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

有關計畫持續時間的資訊，請參閱 [專案期間概觀](../manage-work/projects/planning-a-project/project-duration.md).

## 鍵盤快速鍵

您可以在鍵盤上使用下列鍵值，導覽或完成「增強分析」區域中的特定動作：

| 密鑰 | 動作 |
|---|---|
| **標籤** | 導覽至頁面上的每個元素，以及含有未顯示於頁面之每個視覺效果資訊的表格 |
| **輸入** | 開啟日曆Widget、刪除現有篩選器、開啟新增篩選器選項、選取/取消選取篩選值、套用您建立的篩選器、開啟每個視覺效果上的匯出選項、開啟「燃耗」、「正在處理的任務」和「專案樹狀圖」視覺效果上的下拉式功能表 |
| **方向鍵** | 導覽至日曆介面工具集上的日期，透過新增篩選時的篩選選項，以及透過視覺效果上所有下拉式功能表中的選項 |
| **空格鍵** | 在日曆Widget中選取日期，在新增篩選時選取篩選類型，從每個視覺效果的下拉式選單中選取匯出選項，然後從「燃耗」、「飛行中任務」和「專案樹狀圖」視覺效果的下拉式選單中選取選項 |

{style=&quot;table-layout:auto&quot;}

如果您使用螢幕閱讀軟體或外掛程式，螢幕閱讀器會朗讀螢幕上的資訊，並說明您使用上列鍵時要完成的操作。

## 增強的分析檢視和功能

若要進一步了解Enhanced Analytics中特定功能的詳細資訊、您可以完成的動作以取得進一步的深入分析，以及可從這些資料中學到的內容，請參閱下列文章：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>文章</th> 
   <th>說明</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><a href="../enhanced-analytics/use-enhanced-analytics-filters.md" class="MCXref xref">在增強分析中套用篩選器</a> </td> 
   <td> <p>您可以套用自訂篩選器、專案欄位篩選器或團隊篩選器，以僅檢視符合特定條件的專案。 新增篩選器時，專案的數量會隨之更新。</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/understand-enhanced-analytics-kpis.md" class="MCXref xref">了解增強的分析KPI</a> </td> 
   <td> <p>特定時間範圍內所有專案的關鍵績效指標(KPI)位於畫面頂端。</p> </td> 
  </tr> 
  <tr> 
   <td> <p><a href="../enhanced-analytics/flight-plan-overview.md" class="MCXref xref">在增強分析中檢視「飛行計畫」視覺效果</a> </p> </td> 
   <td> <p>此 <b>飛行計畫</b> 視覺效果顯示在專案生命週期中，條件已變更。 與視覺效果互動可提供特定日期的詳細資訊。 選取專案會開啟「燃盡」和「飛行中的任務」視覺效果。</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/burndown-overview.md" class="MCXref xref">在Enhanced Analytics中檢視「燃耗」視覺效果</a> </td> 
   <td> <p>此 <b>Burndown</b> 視覺效果顯示與實際專案逗留時數相比，專案的計畫速度。 與視覺效果互動可讓您進一步了解專案在特定日期的狀況。</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/tasks-in-flight-overview.md" class="MCXref xref">在Enhanced Analytics中檢視「飛行中的任務」視覺效果</a> </td> 
   <td> <p>此 <b>飛行任務</b> 視覺效果會顯示專案內每個任務的狀態。 與視覺效果互動可讓您快速輕鬆地變更工作。</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/project-activity-overview.md" class="MCXref xref">在增強分析中檢視專案活動視覺效果</a> </td> 
   <td> <p>此 <b>專案活動</b> 視覺效果顯示當指派給登入Workfront的專案的使用者、變更該專案中的任務狀態，以及完成該專案中的任務時的熱度圖。 與視覺效果互動可讓您查看每個使用者的這些詳細資料。 您也可以查看這些動作的特定日期，以及每個動作完成的次數。</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/project-treemap-overview.md" class="MCXref xref">在增強的分析中檢視專案樹狀圖視覺效果</a> </td> 
   <td> <p>此 <b>專案樹狀圖</b> 視覺效果會顯示與其他專案相比，某些專案所花費的時間。 與視覺效果互動可提供專案條件、計畫專案完成和實際專案完成的詳細資訊。</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/activity-by-team-overview.md" class="MCXref xref">在Enhanced Analytics中依團隊視覺效果檢視活動</a> </td> 
   <td> <p>此 <b>活動（依團隊）</b> 視覺效果會顯示首頁團隊的使用者登入Workfront、變更工作狀態及完成工作時的熱度圖。 與視覺效果互動可讓您查看每個個別使用者的這些詳細資料。 您也可以查看這些動作的特定日期，以及每個動作完成的次數。</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/resource-capacity-overview.md" class="MCXref xref">在Enhanced Analytics中檢視「資源容量」視覺效果</a> </td> 
   <td> <p>此 <b>資源容量</b> 視覺效果會顯示哪些主要團隊有能力承擔更多工作，以及哪些主要團隊擁有的工作指派量超過其完成量。 與視覺效果互動可讓您查看有關已完成工作的詳細資訊，以及更多工作的可用時數。 選取團隊會開啟「團隊能力」視覺效果。</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/team-capacity-overview.md" class="MCXref xref">在Enhanced Analytics中檢視「團隊容量」視覺效果</a> </td> 
   <td> <p>此 <b>團隊容量</b> 視覺效果顯示家庭團隊已完成的工作量中分配給他們的工作量的百分比。 與視覺效果互動可讓您查看特定日期的排程小時數和計畫小時數，以及容量百分比，以及主團隊是否在當天結束、關閉或停止運作。</p> </td> 
  </tr> 
 </tbody> 
</table>
