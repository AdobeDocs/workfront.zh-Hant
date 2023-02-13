---
content-type: overview
product-area: agile-and-teams
navigation-topic: burndown
title: 敏捷燃耗圖概述
description: 燃耗圖以視覺化方式呈現動態在迭代或專案中的進度。 實際燃耗率是根據迭代或項目時間軸的理想燃耗率測量的。
author: Lisa
feature: Agile
exl-id: 414e3315-35ed-4aa4-a2d8-be42ec585f29
source-git-commit: 373f2522b85196d6395f189ae6cfe03449cac61a
workflow-type: tm+mt
source-wordcount: '936'
ht-degree: 0%

---

# 敏捷燃耗圖概述

燃耗圖以視覺化方式呈現動態在迭代中的進度。 實際燃耗率根據迭代時間軸的理想燃耗率來測量。

燃耗圖會根據所選日期進行調整。 預設為當天。 選擇前一天時，燃耗圖中的所有資料和 [!UICONTROL 完成狀態] 系統會重新計算燃耗圖上方的區段，以呈現所選日期結束時的資料。 (您可以選取過去天數或當天；您無法選擇未來天數。)

![](assets/agile-iteration-burndown-350x88.png)

## 視覺指標

燃耗圖包含以下可視指示器：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <img src="assets/agile-iteration-burndown-dottedblue.png" alt=""> </td> 
   <td> <p>基於迭代開始時的理想燃耗率。</p> <p>如果小版本的範圍從未更改（小時或點從未添加或刪除），則不會顯示此行。</p> <p>這行在休息一天完成工作時會顯示為平整。 如需詳細資訊，請參閱 <a title="使用敏捷燃耗圖" href="#how-days-off-affect-the-burndown-chart" class="MCXref xref">休息天數如何影響燃耗圖</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <img src="assets/agile-iteration-burndown-solidblue.png" alt=""> </td> 
   <td> <p>基於當前故事或任務的理想燃耗率。</p> <p>當小時或點在迭代開始後添加到迭代或從迭代中刪除時，當前的理想燃耗率（實藍線）與原始的理想燃耗率（虛藍線）不同。</p> <p>這行在休息一天完成工作時會顯示為平整。</p> <p>如需詳細資訊，請參閱 <a title="使用敏捷燃耗圖" href="#how-days-off-affect-the-burndown-chart" class="MCXref xref">休息天數如何影響燃耗圖</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <img src="assets/agile-iteration-burndown-red.png" alt=""> </td> 
   <td> <p>當燃耗率小於理想值時，實際燃耗率以紅色顯示（比理想燃耗計算剩餘的點數或小時數多）。</p> <p>以下公式用於計算實際燃耗率：</p> <p>[SUM（進行中工作的點值或小時值*完成百分比）+已完成工作的點值或小時值]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <img src="assets/agile-iteration-burndown-green.png" alt=""> </td> 
   <td> <p>當燃耗率等於或優於理想時，實際燃耗率以綠色表示（等於或小於理想燃耗計算時的每天剩餘點）。</p> <p>以下公式用於計算實際燃耗率：</p> <p>[SUM（進行中工作的點值或小時值*完成百分比）+已完成工作的點值或小時值]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <img src="assets/agile-iteration-burndown-scope.png" alt=""> </td> 
   <td> <p>範圍的更改（小時或點從小版本中添加或刪除）。</p> <p>範圍變更一律會在當天中旬顯示為垂直線。 此外，在發生範圍更改的任何一天的中間都顯示一個藍點。</p> <p>燃耗圖的垂直軸顯示故事點或小時。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <img src="assets/agile-iteration-burndown-scope.png" alt=""> </td> 
   <td> <p>日期範圍的變更（迭代持續時間可以增加或減少）。</p> <p>在小版本持續時間變更的任何一天中，都會顯示一個藍點。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <img src="assets/agile-iteration-burndown-scope.png" alt=""> </td> 
   <td> <p>每次工作被燒毀時，實際燃耗率上都會顯示一個綠色或紅色點。 (當當天實際燃耗率為紅色時，點為紅色；當當天的實際燃耗率為綠色時，點為綠色。)</p> <p>發生下列任一情況時，將燒毀工作：</p> 
    <ul> 
     <li> [!UICONTROL百分比完成]在文章中增加。<br>[!UICONTROL百分比完成]在下列情況下增加： 
      <ul> 
       <li> <p>手動變更</p> </li> 
       <li> <p>動態更新的點數或小時數</p> </li> 
      </ul></li>  
     <li>動態狀態已變更為[!UICONTROL Complete]</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## 休息天數如何影響燃耗圖 {#how-days-off-affect-the-burndown-chart}

中定義的預設排程 [!DNL Workfront] 通過從燃耗中排除休假天數（週末和節假日），影響燃耗圖。 燃耗圖使用預設計畫來定義工作日(如  [建立排程](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md))。

敏捷團隊可定義替代排程，以合併特定於團隊的非工作日（如文章所述） [對折磨圖使用替代的團隊計畫](../../../agile/use-scrum-in-an-agile-team/burndown/use-alt--team-schedule-burndown-charts.md))。 然後，此替代計畫將反映在分配給團隊的任何小版本的燃耗圖中。 備用計畫只影響燃耗圖。

只有符合以下條件時，燃耗圖才會反映天數：

* 工作之前是在休息日登錄的。 （會顯示記錄工作的日期。）

   當工作記錄在休息日時：

   * 計算理想燃耗時不包括記錄的任何工作，因為沒有計畫團隊執行任何工作。
   * 理想的燃耗線（實藍線和虛藍線）在工作完成時或查看燃耗圖的當天（如果您在休息日查看），在燃耗圖中顯示為扁平。
   * 計算其他燃耗統計資料（如估計完成情況和每天的平均點數或小時數）時，將包括記錄的工作。

* 你在休息一天查看燃耗圖。 （您檢視的日期會顯示在燃耗圖上。）
* 您在休息日完成小版本的剩餘總工作。

   當用戶在一天外完成小版本的剩餘工作總計時， [!UICONTROL 估計完成] 欄位顯示完成小版本的日期。

   在計畫小版本時，如果為非工作日設定小版本結束日期，而小版本正在跟蹤以按時完成，則 [!UICONTROL 估計完成] 日期設定在您設定的迭代結束日期之前的最後一個工作日（因為沒有計畫在非工作日燒錄工作）。

   在計畫小版本時指定小版本的終止日期，如文章所述 [建立小版本](../../../agile/use-scrum-in-an-agile-team/iterations/create-an-iteration.md).
