---
content-type: overview
product-area: agile-and-teams
navigation-topic: burndown
title: 敏捷待執行工作圖總覽
description: 待執行工作圖表提供內文在反複專案或專案中進度方式的視覺化表示。 實際待執行工作速率是根據反複專案或專案時間表理想的待執行工作速率來測量。
author: Lisa
feature: Agile
exl-id: 414e3315-35ed-4aa4-a2d8-be42ec585f29
source-git-commit: 91dc9946566e15bf32d0d89975e3e6b66b39e873
workflow-type: tm+mt
source-wordcount: '970'
ht-degree: 0%

---

# 敏捷待執行工作圖表總覽

待執行工作圖表提供內文在反複專案中的進度視覺化表示。 實際待執行工作速率是依照反複專案時間表的理想待執行工作速率來測量。

待執行工作圖表會根據選取的日期進行調整。 目前日期是預設值。 選取前一天時，會重新計算待執行工作圖表中的所有資料，以及待執行工作圖表上方[!UICONTROL 完成狀態]區段中的所有值，以呈現所選日期結束時的資料。 （您可以選取過去幾天或當天，但無法選取未來的天數。）

![](assets/agile-iteration-burndown-350x88.png)

## 視覺指示器

待執行工作圖表包含下列視覺化指示器：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <img src="assets/agile-iteration-burndown-dottedblue.png" alt="理想的待執行工作開始率"> </td> 
   <td> <p>理想的待執行工作速率（根據反複專案開始的時間）。</p> <p>如果反複專案的範圍從未變更（不會新增或移除時數或點），則不會顯示此行。</p> <p>此線條在休息日完成工作時顯示為平坦。 如需詳細資訊，請參閱<a title="使用敏捷待執行工作圖表" href="#how-days-off-affect-the-burndown-chart" class="MCXref xref">休假如何影響待執行工作圖表</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <img src="assets/agile-iteration-burndown-solidblue.png" alt="內文或工作的理想待執行工作率"> </td> 
   <td> <p>根據目前劇本或任務的理想待執行工作速率。</p> <p>當反複專案開始後，在反複專案中加入或移除時數或點時，目前的理想待執行專案速率（實心藍線）與原始的理想待執行專案速率（虛藍線）不同。</p> <p>此線條在休息日完成工作時顯示為平坦。</p> <p>如需詳細資訊，請參閱<a title="使用敏捷待執行工作圖表" href="#how-days-off-affect-the-burndown-chart" class="MCXref xref">休假如何影響待執行工作圖表</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <img src="assets/agile-iteration-burndown-red.png" alt="實際待執行工作速率（紅色）"> </td> 
   <td> <p>當待執行工作速率小於理想值（每天剩餘的點數或小時數多於理想的待執行工作計算）時，實際待執行工作速率會以紅色顯示。</p> <p>下列公式用於計算實際待執行工作速率：</p> <p>[SUM（進行中工作的點或小時值*完成百分比） +完成工作的點或小時值]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <img src="assets/agile-iteration-burndown-green.png" alt="實際燃盡率（綠色）"> </td> 
   <td> <p>當待執行工作速率等於或高於理想值（相等於或低於理想待執行工作計算的每日剩餘點數）時，實際待執行工作速率會以綠色顯示。</p> <p>下列公式用於計算實際待執行工作速率：</p> <p>[SUM（進行中工作的點或小時值*完成百分比） +完成工作的點或小時值]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <img src="assets/agile-iteration-burndown-scope.png" alt="範圍變更"> </td> 
   <td> <p>範圍變更（在反複專案中新增或移除時數或點）。</p> <p>範圍變更一律在白天中間顯示為垂直線。 此外，每當發生範圍變更時，中間都會顯示藍色圓點。</p> <p>待執行工作圖表的垂直軸顯示本文點或小時。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <img src="assets/agile-iteration-burndown-scope.png" alt="日期範圍變更"> </td> 
   <td> <p>日期範圍變更（反複專案持續時間會增加或減少）。</p> <p>任何反複專案持續時間變更的日子中間都會顯示一個藍色點。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <img src="assets/agile-iteration-burndown-scope.png" alt="為燒毀的工作製作綠點"> </td> 
   <td> <p>每次工作燒毀時，實際燒毀率都會顯示綠色或紅點。 （當當天的實際待執行工作速率是紅色時，點代表紅色；噹噹噹天的實際待執行工作速率是綠色時，點代表綠色。）</p> <p>發生下列任一情況時，工作就會被燒毀：</p> 
    <ul> 
     <li> [！UICONTROL完成百分比]會增加到劇本上。<br>[！UICONTROL完成百分比]在下列情況下會增加： 
      <ul> 
       <li> <p>手動變更</p> </li> 
       <li> <p>內文上的點數或小時數已更新</p> </li> 
      </ul></li>  
     <li>內文的狀態已變更為[！UICONTROL完成]</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## 休假如何影響待執行工作圖表 {#how-days-off-affect-the-burndown-chart}

在[!DNL Workfront]中定義的預設排程會透過從待執行工作排除休假（週末和假日）來影響待執行工作圖表。 待執行工作圖表使用預設排程來定義工作天（如所述）  [建立排程](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md))。

敏捷團隊可以透過定義替代排程來合併團隊特定的非工作日（如文章[使用待執行工作表的替代團隊排程](../../../agile/use-scrum-in-an-agile-team/burndown/use-alt-team-schedule-burndown-charts.md)中所述）。 然後，此替代排程會反映在指派給團隊之任何反複專案的待執行工作圖表中。 替代排程只會影響待執行工作圖表。

只有在下列情況下，休假才會反映在待執行工作圖表中：

* 工作先前是借一天休假來登入。 （會顯示工作記錄的日期。）

  當工作已登入休息日時：

   * 計算理想的待執行工作時不包括任何記錄的工作，因為團隊未排程進行任何工作。
   * 理想的待執行工作線（實心藍線和虛線藍線）會顯示在待執行工作圖中的任何一天或您檢視待執行工作圖的那一天（如果您在休息日檢視），顯示為平坦。
   * 計算其他待執行工作統計資料（例如預估完成和平均每日點數或時數）時，會包含記錄的工作。

* 您正在休息日檢視待執行工作圖表。 （您檢視的日期會顯示在待執行工作圖表上。）
* 您已在休息日完成疊代的總剩餘工作。

  當使用者在休假日完成反複運算的總剩餘工時時，[!UICONTROL 預估完成]欄位會顯示反複運算完成的日期。

  規劃反複專案時，如果您為非工作日設定反複專案結束日期，且反複專案正在追蹤以準時完成，則會為您設定的反複專案結束日期之前的最後一個工作日設定[!UICONTROL 預估完成]日期（因為未排定在非工作日燒錄工作）。

  當計畫反複專案時，會指定反複專案的結束日期，如文章[建立反複專案](../../../agile/use-scrum-in-an-agile-team/iterations/create-an-iteration.md)中所述。
