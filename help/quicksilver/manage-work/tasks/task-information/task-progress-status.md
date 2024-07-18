---
content-type: overview
product-area: projects
navigation-topic: task-information
title: 任務進度狀態總覽
description: Adobe Workfront會透過檢視任務在時間表中的進度來確定任務的進度狀態。 您可以設定Workfront以根據任務的進度狀態值決定專案狀態。 如需有關設定專案條件的詳細資訊，請參閱文章專案條件和條件型別概觀。
author: Alina
feature: Work Management
exl-id: 38e5f89e-bdfa-433c-9371-3c3003ada3a3
source-git-commit: 70d173ca3781d8d143a66ce7e963dcaf66bece19
workflow-type: tm+mt
source-wordcount: '777'
ht-degree: 0%

---

# 任務進度狀態總覽

<!-- Audited: 1/2024 -->

Adobe Workfront會透過檢視任務在時間表中的進度來確定任務的進度狀態。 您可以設定Workfront以根據任務的進度狀態值決定專案狀態。 如需有關設定專案條件的詳細資訊，請參閱文章[專案條件和條件型別概觀](../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md)。

## 決定任務進度狀態的條件

如需有關專案進度狀態的資訊，請參閱[專案進度狀態概觀](../../../manage-work/projects/planning-a-project/project-progress-status.md)。

如需追蹤工作進度的相關資訊，請參閱[工作追蹤模式概觀](../../../manage-work/tasks/task-information/task-tracking-mode.md)。

下列條件決定任務的進度狀態：

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
   <td scope="col"> <p> </p> <p><strong>開啟時間</strong> </p> </td> 
   <td scope="col"> <p>當所有計畫日期符合預計日期時，任務視為<strong>時間</strong>。 此進度狀態也表示專案比排程提前，且預計日期可能比計畫日期早。</p> <p>如需有關預計日期的詳細資訊，請參閱<a href="../../../manage-work/projects/planning-a-project/project-projected-completion-date.md" class="MCXref xref">專案、任務和問題的預計完成日期總覽</a>。</p> <p>如需有關任務計畫完成日期的詳細資訊，請參閱下列文章：</p> 
    <ul> 
     <li> <p><a href="../../../manage-work/tasks/task-information/task-planned-start-date.md" class="MCXref xref">任務計劃開始日期總覽</a> </p> </li> 
     <li> <p><a href="../../../manage-work/tasks/task-information/task-planned-completion-date.md" class="MCXref xref">任務計畫完成日期總覽</a> </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td><p></p> <p><strong>有風險</strong> </p> </td> 
   <td><p>當預估完成日期晚於計畫完成日期且晚於預計完成日期時，任務會視為<strong>有風險</strong>。 當任務的限製為<strong>必須完成於</strong>或<strong>必須開始於</strong>，但任務的完成百分比或前置任務關係顯示它無法在指定的日期完成或開始時，就會發生這種情況。 </p><p> 將任務限制設定為<strong>必須在</strong>完成手動將計畫完成日期設定為特定日期。 在此情況下，預計完成日期與計畫完成日期相符。 在此限制的情況下，Workfront會分析任務以根據完成百分比計算完成時間。 此計算會儲存為「預估到期日」。 如果「預估到期日」在「預估完成日期」之後，則作業會被視為有延遲的風險。 </p> <p> 將任務限制設定為<strong>必須於</strong>開始，手動將計劃開始日期設定為特定日期。 在此案例中，預計開始日期與計劃開始日期相符。 在此限制的情況下，Workfront會分析任務以根據其前置任務關係計算開始時間。 此計算會儲存為「預估開始日期」。 如果有強制性的前置任務，不允許任務在指定的開始日期開始，則預估開始日期可以在預計完成日期之後。 該任務會被視為有延遲的風險。 </p> <p>注意：除了使用<strong>必須在</strong>開始或<strong>必須在</strong>完成之外，通常預估日期與預計日期相符。 在這些情況下，「預估日期」會根據完成百分比和其他因素（前置任務關係）繼續計算，而「預估日期」會強制符合手動設定的「計畫日期」。</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>落後</strong> </p> </td> 
   <td> <p>當預估完成日期晚於或等於計畫完成日期，且早於預計完成日期時，任務會視為<strong>落後</strong>。</p> <p>預計完成日期是根據先前進度完成任務的即時檢視。 雖然任務開始較晚，但不會視為較晚，因為「計畫完成日期」與「預計完成日期」仍在未來，任務可能仍準時完成。</p> <p>注意： <strong>落後</strong>和<strong>有風險</strong>進度狀態幾乎相同。 但是，<strong>有風險</strong>表示計畫日期之一或兩者上有某些強制的任務限制（必須完成日期、必須開始日期、固定日期）。 如果作業沒有強制限制，則預計日期會與預估日期相同，並反映系統根據作業目前進度計算的「完成日期」。 任務尚未被視為延遲，因為「計畫完成日期」與「預計完成日期」仍在未來，任務可能仍準時完成。<br>如需預計日期和預估日期的詳細資訊，請參閱<a href="../../../manage-work/tasks/task-information/differentiate-projected-estimated-dates.md" class="MCXref xref">區分預計日期和預估日期</a>。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>延遲</strong> </p> </td> 
   <td> <p>當計畫完成日期早於今天日期時，任務為<strong>延遲</strong>。<br></p> </td> 
  </tr> 
 </tbody> 
</table>

<!--hiding this because some users find the images confusing, as they don't really show the dates mentioned in the descriptions above. Keep the pictures though, in case some users will complain that we hid them. 

## How task Progress Status updates over time

The different date types in our projects tell us how tasks are progressing over time:

* On Time

  ![](assets/on-time-progress-status-350x233.png)

* At Risk

  ![](assets/at-risk-progress-status-350x233.png)

* Behind

  ![](assets/behind-progress-status-350x233.png)

* Late

  ![](assets/late-progress-status-350x233.png)

-->