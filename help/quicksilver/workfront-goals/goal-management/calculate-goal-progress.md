---
product-previous: workfront-goals
navigation-topic: goal-management
title: Adobe Workfront目標中的目標進度和條件概覽
description: 目標進展由活動、結果或兒童目標等進展指標驅動。 目標條件由目標在當前時刻的進度決定。
author: Alina
feature: Workfront Goals
exl-id: 3050f7ff-a579-4fb8-82fd-bef850f27c20
source-git-commit: 1d221d10e5845e477dff825f853330b9b4df0adf
workflow-type: tm+mt
source-wordcount: '821'
ht-degree: 1%

---

# Adobe Workfront目標中的目標進度和條件概覽

<!--drafted for P&P release: the note at the top will need to be replaced with this:

Your organization must have the following to use the functionality described in this article:

* For the legacy plan and license structure: 

  * A Pro or higher [Adobe Workfront plan](https://www.workfront.com/plans). 
  * An Adobe Workfront Goals license in addition to a Workfront license.

* For the current plan and license structure:

  * An Ultimate plan 
    
    Or
    
    An additional license for Adobe Workfront Goals for the Prime or Select Adobe Workfront plans. <is there a link we can add here for the plans and what they contain?!>

Contact your Workfront account manager to learn about a Workfront Goals license.

For additional information about access to Workfront Goals, see [Requirements to use Workfront Goals](../../workfront-goals/goal-management/access-needed-for-wf-goals.md).
-->

>[!NOTE]
>
>貴組織必須具備下列條件才能使用本文所述的功能：
>
>* Pro或更高版本 [Adobe Workfront計畫](https://www.workfront.com/plans).
>* 除了Adobe Workfront授權，還有Workfront授權。
>
>請連絡您的Workfront客戶經理，以了解Workfront Target授權。
>如需存取Workfront目標的詳細資訊，請參閱 [使用Workfront目標的需求](../../workfront-goals/goal-management/access-needed-for-wf-goals.md).

Adobe Workfront根據進度指標的進展情況自動計算目標進展。

## 必要條件

您必須具備下列條件，才能開始：

* 一種佈局模板，在主菜單中包括目標區域。

## 目標進度和臨界值概覽

在您啟動目標後，Workfront目標會開始計算其進度和條件，當您將游標暫留在「進度」欄位上時，會顯示下列指標：

| 指標 | 指標說明 |
|---|---|
| 實際完成百分比 | 目標到目前為止已經完成了多少。 Workfront目標通過平均與目標相關聯的所有進度指標的完成百分比來計算此值。 |
| 預期完成百分比 | 目標到目前為止應完成多少，才能按時完成。 Workfront Target會查看目標的持續時間和目前的時間，來計算此值。 如果目標要按時完成，則應在目前時間顯示此值。 |
| 進度 | 指出目標是否按時完成，或目標是否有風險或無法完成的標籤。 |

![](assets/in-trouble-goal-progress-expanded.png)

<!--drafted for the redesign: replace the screen shot above with the redesigned one which is white, not black-->

* [實際完成百分比](#actual-percent-complete)
* [預期完成百分比](#expected-percent-complete)
* [進度與條件](#progress)

### 實際完成百分比 {#actual-percent-complete}

Workfront目標會根據目標進度指標的完成百分比平均值自動計算目標的實際完成百分比。

以下項目被視為目標的進度指標：

* 結果

   如需將結果新增至目標的相關資訊，請參閱 [將結果新增至Adobe Workfront目標中的目標](../../workfront-goals/results-and-activities/add-results-to-goals.md).

* 活動

   如需將活動（包括專案）新增至目標的相關資訊，請參閱 [將活動新增至Adobe Workfront目標中的目標](../../workfront-goals/results-and-activities/add-activities-to-goals.md).

* 協調兒童目標

   如需有關父項和子項目標的資訊，請參閱 [在Adobe Workfront目標中將目標連結起來，以協調目標](../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md).

   Workfront Target使用下列公式計算實際完成百分比：

   ```
   Actual percent complete of goal = SUM(Percent complete of goal progress indicators)* 100 / Number of progress indicators
   ```

   例如，如果目標的結果是完成20%，手動進度條是完成30%，項目是完成10%，子項目標是完成40%，則目標完成百分比是25%。

### 預期完成百分比 {#expected-percent-complete}

Workfront目標會根據目標期間的總天數，以及自目標開始日期以來經過的天數，自動計算目標的預期完成百分比。

Workfront Target使用下列公式計算預期完成百分比：

```
Expected percent complete of goal = Number of days since the goal start date * 100/ Number of days in the goal duration
```

例如，如果目標要在90天內完成，而今天是該期間的第45天，則預期完成百分比為50%。

### 進度與條件 {#progress}

Workfront目標會根據目前的時間已達到預期完成百分比的百分比，計算進度百分比，並為目標指派進度標籤。 目標百分比完成欄的顏色會改變，以指示目標的進度。

目標的條件也會隨之更新，以指出目標是按時完成，還是落後。

Workfront Target使用下列公式計算目標的進度百分比：

```
Goal progress percentage = Actual percent complete * 100 / Expected percent complete
```

例如，如果當前時間的預期完成百分比為53%，而實際完成百分比為30%，則目標完成百分比為56%。 Workfront目標會將此目標標示為「有麻煩」條件。

下圖說明條件標籤與進度百分比之間的關係：

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
   <td><b>百分比完整條的顏色</b></td> 
   <td><b>條件指示器表徵圖</b></td> 
  </tr> 
  <tr> 
   <td>新增</td> 
   <td> <p>目標是新建立的，尚未記錄進度。 目標進度會顯示為「新增」，直到有人首次更新其進度為止。 </p> <p>有關更新目標進度的資訊，請參閱 <a href="../../workfront-goals/goal-review-and-workfront-goals-sections/check-in-goals.md" class="MCXref xref">更新Adobe Workfront目標中的目標進度</a>.</p> </td> 
   <td>無百分比</td> 
   <td>無條</td> 
   <td><img src="assets/new-goal-icon-condition.png" alt="new_goal_icon_condition.png"></td>
  </tr> 
  <tr> 
   <td> <p><span>達成目標</span> </p> </td> 
   <td>目標如預期般執行，且極有可能按時完成。 </td> 
   <td>90-100%</td> 
   <td>綠色</td> 
    <td><img src="assets/on-target-icon-condition.png" alt="on_target_icon_condition.png"></td>
  </tr> 
  <tr> 
   <td> <p><span>有風險</span> </p> </td> 
   <td>目標落後，但仍有可能按時完成。 </td> 
   <td>70-89.99%</td> 
   <td>黃色</td>
   <td><img src="assets/at-risk-icon-condition.png" alt="at_risk_icon_condition.png"></td> 
  </tr> 
  <tr> 
   <td> <p><span>陷入困境</span> </p> </td> 
   <td> <p>目標很可能不會按時完成。 </p> </td> 
   <td>0-69.99%</td> 
   <td>紅色</td> 
   <td><img src="assets/in-trouble-icon-condition.png" alt="in_trouble_icon_condition.png"></td> 
  </tr> 
 </tbody> 
</table>