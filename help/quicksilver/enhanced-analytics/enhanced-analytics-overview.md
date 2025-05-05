---
title: 增強型分析概述
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: 增強型分析是Adobe Workfront中的強大工具，具有預先建立的視覺效果，可讓您檢視專案資料，並透過計畫和完成來識別趨勢。 將此insight放入您的專案中有助於您管理目前的工作，並可讓您更準確地規劃未來的工作。
author: Nolan
feature: Reports and Dashboards
exl-id: a14ad57c-859b-43df-84c0-575ccda86e50
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '1246'
ht-degree: 3%

---

# 增強型分析概述

>[!IMPORTANT]
>
>增強型Analytics將於5月26日起一週從Workfront中移除。 Workfront Data Connect是全新的替代解決方案，可用來複製您目前使用的任何Enhanced Analytics視覺效果。 <br>如需詳細資訊，請參閱[Enhanced Analytics淘汰指南](/help/quicksilver/product-announcements/announcements/enhanced-analytics-deprecation.md)。


增強型分析是Adobe Workfront中的強大工具，具有預先建立的視覺效果，可讓您檢視專案資料，並透過計畫和完成來識別趨勢。 將此insight放入您的專案中有助於您管理目前的工作，並可讓您更準確地規劃未來的工作。

增強型分析可協助您識別：

* 您計畫專案的方式
* 將工作新增至專案時
* 不同專案正在完成的工作量
* 相較於主團隊已排程的時數或天數，完成專案所需的時數或天數
* 使用者在專案期間完成特定動作的頻率
* 專案的進度，以及專案中的個別任務

![分析](assets/nwe-full-screen-analytics-350x222.png)

若要檢視使用案例，或瞭解更多有關使用增強型分析管理目前工作和規劃未來工作的資訊，請參閱[增強型分析學習路徑](https://experienceleague.adobe.com/zh-hant/docs/workfront-learn/tutorials-workfront/home)。

## 先決條件

若要存取增強型分析區域，您必須：

* 擁有業務或企業計畫。

  如需詳細資訊，請參閱[Workfront計畫](https://business.adobe.com/products/workfront/pricing.html)。

* 請您的Workfront管理員將增強型分析新增至您的版面配置範本。

  如需詳細資訊，請參閱[增強型分析：新增分析至配置範本](https://experienceleague.adobe.com/zh-hant/docs/workfront/using/home)。

若要檢視專案與任務的資訊，您必須：

* 擁有存取層級中「專案」和「任務」區域的檢視許可權。

  如需Workfront管理員如何修改存取層級的詳細資訊，請參閱[建立或修改自訂存取層級](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)。

* 擁有特定任務和/或專案的檢視許可權。

  如需請求其他存取權的資訊，請參閱[請求物件的存取權](../workfront-basics/grant-and-request-access-to-objects/request-access.md)。

## 增強型分析的最佳作法

為了取得您專案的最佳資料，請使用具有準確計畫時數和持續時間天的範本。 您也必須確保使用者儘可能準確地輸入及更新下列欄位。

>[!NOTE]
>
>下列部分欄位是Workfront根據使用者輸入的資訊而執行的計算。 您無法手動更新這些欄位。

* 規劃時數

  這是要填寫的最重要欄位。

  >[!NOTE]
  >
  >如果您的團隊未使用計畫時數，您仍然可以看到一些基於專案持續時間的資料。\
  >如需詳細資訊，請參閱本文中的[期間檢視](#duration-view)一節。

* 專案名稱

  名稱應為專案的描述性。

* 專案狀況
* 專案狀態
* 專案規劃開始日期
* 規劃完成日期
* 專案實際開始日期
* 專案實際結束日期
* 專案期間小時
* 專案實際時數
* 任務狀態（包括將任務標示為「已完成」）。
* 任務名稱
* 任務完成百分比
* 任務規劃開始日期
* 任務規劃完成日期

>[!IMPORTANT]
>
>對任務和專案進行的變更最多可能需要24小時的時間，才能反映在「增強分析」中。

## 期間檢視 {#duration-view}

預設情況下，「待執行工作」和「專案樹狀圖」視覺效果是根據計畫時數。 如果您的團隊不使用計畫時數，您可以根據專案持續時間檢視這些視覺效果。

在增強型分析中，專案期間的計算公式如下：

* 計畫時間範圍：

  ```
  Planned Completion Date of the project - Start Date of the project
  ```

* 工作天數：

  ```
  Planned Duration for tasks completed in the selected date range / Typical hours per work day
  ```

  >[!NOTE]
  >
  >8小時是&#x200B;**每個工作日一般小時數**&#x200B;的預設值。 Adobe Workfront管理員可以在&#x200B;**設定** > **專案偏好設定** > **專案** > **時間表**&#x200B;下更新&#x200B;**每工作日一般時數**&#x200B;設定。\
  >若要深入瞭解，請參閱[設定全系統的專案偏好設定](../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)。

如需計畫期間的相關資訊，請參閱[專案期間概觀](../manage-work/projects/planning-a-project/project-duration.md)。

## 鍵盤快速鍵

您可以在鍵盤上使用以下按鍵，導覽或完成增強型分析區域中的特定動作：

| 索引鍵 | 動作 |
|---|---|
| **標籤** | 導覽至頁面上的每個元素，以及未在頁面上顯示的每個視覺效果相關資訊的表格 |
| **輸入** | 開啟行事曆Widget、刪除現有篩選器、開啟新增篩選器選項、選取/取消選取篩選器值、套用您已建立的篩選器、開啟每個視覺效果的匯出選項、開啟「待執行工作」、「執行中的任務」和「專案樹狀圖」視覺效果上的下拉式功能表 |
| **方向鍵** | 瀏覽至行事曆Widget上的日期、新增篩選器時的篩選器選項，以及視覺效果上所有下拉式功能表中的選項 |
| **空白鍵** | 在行事曆Widget中選取日期、新增篩選器時選取篩選器型別、從每個視覺效果上的下拉式選單中選取匯出選項，以及從「待執行工作」、「執行中任務」和「專案樹狀圖」視覺效果上的下拉式選單中選取選項 |

{style="table-layout:auto"}

如果您使用熒幕閱讀軟體或外掛程式，熒幕閱讀程式會朗讀熒幕上的資訊，並描述您使用上述按鍵時所要執行的動作。

## 增強的分析檢視和功能

若要深入瞭解增強型分析中特定功能的詳細資料、可完成以取得更多insight的動作，以及可從此資料瞭解的內容，請參閱下列文章：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>文章</th> 
   <th>解釋</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><a href="../enhanced-analytics/use-enhanced-analytics-filters.md" class="MCXref xref">在增強型分析中套用篩選器</a> </td> 
   <td> <p>您可以套用自訂篩選器、專案欄位篩選器或團隊篩選器，以僅檢視符合特定條件的專案。 當您新增篩選器時，專案數量會隨之更新。</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/understand-enhanced-analytics-kpis.md" class="MCXref xref">瞭解增強型分析KPI</a> </td> 
   <td> <p>特定時間範圍內所有專案的關鍵績效指標(KPI)位於畫面頂端。</p> </td> 
  </tr> 
  <tr> 
   <td> <p><a href="../enhanced-analytics/flight-plan-overview.md" class="MCXref xref">在增強型分析中檢視小眾測試版計畫視覺效果</a> </p> </td> 
   <td> <p><b>小眾測試版計畫</b>視覺效果會顯示專案整個生命週期中的狀況已變更。 與視覺效果互動可為您提供有關特定日期的更多詳細資料。 選取專案會開啟「待執行工作」和「小眾測試版中的任務」視覺效果。</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/burndown-overview.md" class="MCXref xref">在增強型分析中檢視待執行工作視覺效果</a> </td> 
   <td> <p><b>待執行工作</b>視覺效果會顯示專案與專案實際逗留時數的比較計畫速度。 與視覺效果互動可為您提供有關特定日期專案狀況的更多詳細資訊。</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/tasks-in-flight-overview.md" class="MCXref xref">在增強型分析中檢視小眾測試版中的任務視覺效果</a> </td> 
   <td> <p>小眾測試版中的<b>任務</b>視覺效果會顯示專案中每個任務的狀態。 與視覺效果互動可讓您快速輕鬆地變更任務。</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/project-activity-overview.md" class="MCXref xref">在增強型分析中檢視專案活動視覺效果</a> </td> 
   <td> <p><b>專案活動</b>視覺效果會顯示熱度圖，其中顯示指派給專案的使用者登入Workfront、變更該專案中任務的狀態，以及該專案中已完成任務的時間。 與視覺效果互動可讓您檢視每個使用者的這些詳細資訊。 您也可以檢視這些動作的特定日期，以及每個動作的完成次數。</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/project-treemap-overview.md" class="MCXref xref">在增強型分析中檢視專案樹狀圖視覺效果</a> </td> 
   <td> <p><b>專案樹狀圖</b>視覺效果會顯示某些專案相較於其他專案所花費的時間。 與視覺效果互動可提供專案狀況、計畫專案完成和實際專案完成的詳細資訊。</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/activity-by-team-overview.md" class="MCXref xref">在增強型分析中檢視依團隊視覺效果的活動</a> </td> 
   <td> <p><b>依團隊的活動</b>視覺效果會顯示熱度圖，其中顯示主團隊的使用者登入Workfront、變更任務狀態及完成任務的時間。 與視覺效果互動可讓您檢視每個使用者的這些詳細資訊。 您也可以檢視這些動作的特定日期，以及每個動作的完成次數。</p> </td> 
  </tr> 
  <!-- Features permanently removed from Workfront
  <tr> 
   <td><a href="../enhanced-analytics/resource-capacity-overview.md" class="MCXref xref">View the Resource capacity visualization in Enhanced analytics</a> </td> 
   <td> <p>The <b>Resource capacity</b> visualization shows you which home teams have the capacity to take on more work and which home teams have more work assigned to them than they can complete. Interacting with the visualization allows you to see more details about work completed and available hours for more work.&nbsp;Selecting a team opens the Team capacity visualization.</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/team-capacity-overview.md" class="MCXref xref">View the Team capacity visualization in Enhanced analytics</a> </td> 
   <td> <p>The <b>Team capacity</b> visualization shows you a percentage of the amount of work a home team has completed out of the amount of work assigned to them. Interacting with the visualization allows you to see scheduled hours and planned hours for a specific date, as well as the capacity percentage and whether the home team was over, under, or at capacity on that day.</p> </td> 
  </tr>--> 
 </tbody> 
</table>
