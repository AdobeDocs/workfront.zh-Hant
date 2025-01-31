---
product-previous: workfront-goals
navigation-topic: goal-management
title: Adobe Workfront目標中的目標進度和條件概觀
description: 目標進度是由活動、結果或子目標等進度指標所驅動。 目標條件是由目前時間中目標的進度所決定。
author: Alina
feature: Workfront Goals
exl-id: 3050f7ff-a579-4fb8-82fd-bef850f27c20
source-git-commit: 7c1bd52c6d1878b556bc92849b5d65fd0e89f51b
workflow-type: tm+mt
source-wordcount: '827'
ht-degree: 1%

---

# Adobe Workfront目標中的目標進度和條件概觀

您的組織必須具備下列專案，才能使用本文所述的功能：

* 對於新計畫和授權結構：

   * Ultimate計畫

     或

     適用於Prime或選取Adobe Workfront計畫的Adobe Workfront目標的其他授權。

* 對於目前的計畫與授權結構：

   * A Pro或更高版本
   * 除了Adobe Workfront授權之外，還有Workfront目標授權。

請連絡您的Workfront客戶經理，以瞭解Workfront Goals授權。

如需存取Workfront目標的詳細資訊，請參閱[使用Workfront目標的需求](../../workfront-goals/goal-management/access-needed-for-wf-goals.md)。

Adobe Workfront會根據其進度指示器，自動計算目標進度。

## 目標進度和臨界值概觀

啟用目標後，Workfront目標會開始計算其進度和條件，並在您暫留在「進度」欄位時顯示下列指標：

| 指標 | 指標說明 |
|---|---|
| 實際完成百分比 | 目前為止實際完成多少目標。 Workfront目標會計算此值，方法是平均與目標相關聯之所有進度指示器的完成百分比。 |
| 預期完成百分比 | 目前應該完成多少目標才能準時完成。 Workfront目標會檢視目標的持續期間和目前的時間點，以計算此值。 如果要在目前時間完成，目標應顯示此值。 |
| 進度 | 指出目標是否準時完成的目標，或是否有風險或無法完成的標籤。 |

![](assets/in-trouble-goal-progress-expanded.png)

<!--drafted for the redesign: replace the screen shot above with the redesigned one which is white, not black-->

* [實際完成百分比](#actual-percent-complete)
* [預期完成百分比](#expected-percent-complete)
* [進度和條件](#progress)

### 實際完成百分比 {#actual-percent-complete}

Workfront目標會根據目標進度指標的完成百分比平均數，自動計算目標的實際完成百分比。

下列專案會視為目標的進度指示器：

* 結果

  如需將結果新增至目標的詳細資訊，請參閱[在Adobe Workfront目標中新增結果](../../workfront-goals/results-and-activities/add-results-to-goals.md)。

* 活動

  如需新增活動（包括專案至目標）的相關資訊，請參閱[在Adobe Workfront目標中新增活動](../../workfront-goals/results-and-activities/add-activities-to-goals.md)。

* 校準的子目標

  如需有關父目標和子目標的資訊，請參閱[在Adobe Workfront目標中連線目標以對齊目標](../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md)。

  Workfront目標使用下列公式計算實際完成百分比：

  ```
  Actual percent complete of goal = SUM(Percent complete of goal progress indicators)* 100 / Number of progress indicators
  ```

  例如，如果目標的結果為20%完成、手動進度列為30%完成、專案為10%完成且子目標為40%完成，則目標完成百分比為25%。

### 預期完成百分比 {#expected-percent-complete}

Workfront目標會根據目標期間的總天數，以及自目標開始日期起已過的天數，自動計算目標的預期完成百分比。

Workfront目標使用下列公式計算預期的完成百分比：

```
Expected percent complete of goal = Number of days since the goal start date * 100/ Number of days in the goal duration
```

例如，如果目標應在90天內完成，而今天是該期間的第45天，則預期完成百分比為50%。

### 進度和條件 {#progress}

Workfront目標會根據目前時間中「預期完成百分比」的完成百分比，計算進度百分比並將進度標籤指派給目標。 目標完成百分比列的顏色會變更，以指出目標的進度。

目標的條件也會據此更新，以指出目標是否準時完成目標，或落後。

Workfront目標使用下列公式計算目標的進度百分比：

```
Goal progress percentage = Actual percent complete * 100 / Expected percent complete
```

例如，如果目前的「預期完成百分比」為53%，而「實際完成百分比」為30%，則「目標」進度完成百分比為56%。 Workfront目標將此目標標籤為「存在問題」狀態。

下列圖表說明條件標籤與進度百分比之間的關係：

![](assets/progress-status-labels-charted-after-match-with-project-condition-350x147.png)

下表列出目標條件標籤以及與每個標籤相關聯的目標進度百分比。

>[!TIP]
>
>目標條件標籤符合Workfront專案條件名稱和顏色。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><b>目標進度名稱</b></td> 
   <td><b>目標進度定義</b></td> 
   <td><b>目標進度百分比</b></td> 
   <td><b>完成百分比列的色彩</b></td> 
   <td><b>條件指標圖示</b></td> 
  </tr> 
  <tr> 
   <td>新增</td> 
   <td> <p>目標是新建立的，尚未記錄進度。 目標進度會顯示為「新增」，直到有人首次更新其進度為止。 </p> <p>如需有關更新目標進度的資訊，請參閱<a href="../../workfront-goals/goal-review-and-workfront-goals-sections/check-in-goals.md" class="MCXref xref">在Adobe Workfront目標中更新目標進度</a>。</p> </td> 
   <td>無百分比</td> 
   <td>無長條圖</td> 
   <td><img src="assets/new-goal-icon-condition.png" alt="new_goal_icon_condition.png"></td>
  </tr> 
  <tr> 
   <td> <p><span>在目標</span>上 </p> </td> 
   <td>目標正在如預期般執行，極有可能將準時完成。 </td> 
   <td>90-100%</td> 
   <td>綠色</td> 
    <td><img src="assets/on-target-icon-condition.png" alt="on_target_icon_condition.png"></td>
  </tr> 
  <tr> 
   <td> <p><span>有風險</span> </p> </td> 
   <td>目標有所延遲，但仍可按時完成。 </td> 
   <td>70-89.99%</td> 
   <td>黃色</td>
   <td><img src="assets/at-risk-icon-condition.png" alt="at_risk_icon_condition.png"></td> 
  </tr> 
  <tr> 
   <td> <p><span>存在問題</span> </p> </td> 
   <td> <p>目標很可能無法按時完成。 </p> </td> 
   <td>0-69.99%</td> 
   <td>紅色</td> 
   <td><img src="assets/in-trouble-icon-condition.png" alt="in_trouble_icon_condition.png"></td> 
  </tr> 
 </tbody> 
</table>