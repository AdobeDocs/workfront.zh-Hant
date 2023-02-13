---
content-type: overview
product-area: projects
navigation-topic: task-information
title: 任務進度狀態概述
description: Adobe Workfront會查看任務在其時間軸上的進展，以確定任務的進展狀態。 您可以設定Workfront，以根據工作進度狀態的值來決定專案的條件。 如需設定專案條件的詳細資訊，請參閱專案條件和條件類型概覽一文。
author: Alina
feature: Work Management
exl-id: 38e5f89e-bdfa-433c-9371-3c3003ada3a3
source-git-commit: 65f25a3b1198f491f7357efef11e2ae075e9721a
workflow-type: tm+mt
source-wordcount: '805'
ht-degree: 1%

---

# 任務進度狀態概述

Adobe Workfront會查看任務在其時間軸上的進展，以確定任務的進展狀態。 您可以設定Workfront，以根據工作進度狀態的值來決定專案的條件。 如需設定專案條件的詳細資訊，請參閱文章 [專案條件和條件類型概觀](../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md).

## 確定任務進度狀態的標準

如需專案進度狀態的相關資訊，請參閱 [項目進度狀態概觀](../../../manage-work/projects/planning-a-project/project-progress-status.md).

有關跟蹤任務進度的資訊，請參閱 [任務追蹤模式概觀](../../../manage-work/tasks/task-information/task-tracking-mode.md).

以下標準確定任務的進度狀態：

<table> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>進度狀態</strong> </p> </th> 
   <th> <p><strong>決定條件</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr valign="top"> 
   <td scope="col"> <p> </p> <p><strong>準時</strong> </p> </td> 
   <td scope="col"> <p>考慮任務 <strong>準時</strong> 當所有計畫日期均與預計日期匹配時。 此進度狀態也可能意味著項目提前，預計日期可能早於計畫日期。</p> <p>有關預計日期的詳細資訊，請參閱 <a href="../../../manage-work/projects/planning-a-project/project-projected-completion-date.md" class="MCXref xref">項目、任務和問題的預計完成日期概覽</a>.</p> <p>有關任務計畫完成日期的詳細資訊，請參閱以下文章：</p> 
    <ul> 
     <li> <p><a href="../../../manage-work/tasks/task-information/task-planned-start-date.md" class="MCXref xref">任務計畫起始日期概覽</a> </p> </li> 
     <li> <p><a href="../../../manage-work/tasks/task-information/task-planned-completion-date.md" class="MCXref xref">任務計畫完成日期概覽</a> </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td><p></p> <p><strong>有風險</strong> </p> </td> 
   <td><p>考慮任務 <strong>風險</strong> 當估計完成日期遲於計畫完成日期和遲於預計完成日期時。 當任務具有 <strong>必須完成</strong> 或 <strong>必須開始</strong> 但任務的完成百分比或前置關係表明它不能在指定日期完成或開始。 </p><p> 將任務約束設定為 <strong>必須完成</strong> 人工將計畫完成日期設定為特定日期。 在這種情況下，預計完成日期與計畫完成日期匹配。 在此限制的情況下，Workfront會分析任務，以根據完成的百分比計算任務何時完成。 此計算會儲存為「預計到期日」。 如果預計到期日晚於預計完成日期，則將考慮任務延遲的風險。 </p> <p> 將任務約束設定為 <strong>必須開始</strong> 人工將計畫起始日期設定為特定日期。 在這種情況下，預計起始日期與計畫起始日期匹配。 在此限制的情況下，Workfront會分析任務，以根據其前置關係計算其何時開始。 此計算會儲存為「預計開始日期」。 如果有強制的前置任務不允許任務在指定的起始日期開始，則預計起始日期可以在預計完成日期之後。 這項任務被認為有遲到的風險。 </p> <p>注意：通常，預計日期與預計日期相符，但 <strong>必須開始</strong> 或 <strong>必須完成</strong> 中所有規則的URL區段。 在這些情況下，「預計日期」繼續根據完成百分比和其他因素（前置關係）進行計算，而「預計日期」將強制與人工設定的計畫日期匹配。</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>滞後</strong> </p> </td> 
   <td> <p>任務被視為 <strong>背後</strong> 當估計完成日期遲於或等於計畫完成日期時，並且早於預計完成日期。</p> <p>預計完成日期是根據先前進度即時查看任務何時完成的視圖。 儘管任務已延遲啟動，但它尚未被視為延遲，因為計畫和預計完成日期仍在將來，並且任務可能仍按時完成。</p> <p>注意：此 <strong>背後</strong> 和 <strong>風險</strong> 進度狀態幾乎相同。 不過， <strong>風險</strong> 指示在一個或兩個計畫日期上存在某些強制任務約束（必須結束、必須開始、固定日期）。 如果任務沒有強制約束，則預計日期與估計日期相同，並反映基於任務當前進度的完成日期的系統計算。 任務尚未被視為延遲，因為計畫和預計完成日期仍在將來，並且任務可能仍按時完成。<br>有關預計日期和預計日期的詳細資訊，請參閱 <a href="../../../manage-work/tasks/task-information/differentiate-projected-estimated-dates.md" class="MCXref xref">區分預計日期和預計日期 </a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>延遲</strong> </p> </td> 
   <td> <p>任務是 <strong>延遲</strong> 當計畫完成日期早於今天的日期。<br></p> </td> 
  </tr> 
 </tbody> 
</table>

## 任務進度狀態隨時間的變化如何更新

項目中的不同日期類型告訴我們任務在一段時間內的進展情況：

* 準時

   ![](assets/on-time-progress-status-350x233.png)

* 有風險

   ![](assets/at-risk-progress-status-350x233.png)

* 滞後

   ![](assets/behind-progress-status-350x233.png)

* 延遲

   ![](assets/late-progress-status-350x233.png)
