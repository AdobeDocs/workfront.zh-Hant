---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: 項目進度狀態概觀
description: Adobe Workfront會查看專案在其時間軸內的進展，借此決定專案的進度狀態。 您可以設定Workfront，以根據工作進度狀態的值來決定專案的條件。 如需設定專案條件的詳細資訊，請參閱專案條件和條件類型概覽一文。
author: Alina
feature: Work Management
exl-id: 922ca4cf-c526-4704-9966-de67b0c36a2a
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '383'
ht-degree: 1%

---

# 項目進度狀態概觀

Adobe Workfront會查看專案在其時間軸內的進展，借此決定專案的進度狀態。 您可以設定Workfront，以根據工作進度狀態的值來決定專案的條件。 如需設定專案條件的詳細資訊，請參閱文章 [專案條件和條件類型概觀](../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md).

以下是Workfront中專案的進度狀態：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>準時</td> 
   <td> <p>如果預計完成日期和預計完成日期均早於或等於項目計畫完成日期，則項目的進展狀態為 <strong>準時</strong>.</p> <p> <img src="assets/project-on-time-progress-status-350x69.png" style="width: 350;height: 69;"> </p> </td> 
  </tr> 
  <tr> 
   <td>有風險</td> 
   <td> <p>如果預計完成日期和預計完成日期均在將來，但遲於項目的計畫完成日期，而預計完成日期遲於預計完成日期，則項目進度狀態為 <strong>風險</strong>. </p> <p> <img src="assets/project-at-risk-progress-status-350x67.png" style="width: 350;height: 67;"> </p> </td> 
  </tr> 
  <tr> 
   <td>滞後</td> 
   <td> <p>如果預計完成日期和預計完成日期均在將來，但遲於項目的計畫完成日期，但預計完成日期不遲於預計完成日期，則項目進度狀態為 <strong>背後</strong>.</p> <p> <img src="assets/project-behind-progress-status-350x67.png" style="width: 350;height: 67;"> </p> </td> 
  </tr> 
  <tr> 
   <td>延遲</td> 
   <td> 
    <ul> 
     <li> <p>如果項目已完成，且實際完成日期晚於計畫完成日期，則項目的進展狀態為 <strong>延遲</strong>. </p> <p> <img src="assets/project-late-progress-status-350x66.png" style="width: 350;height: 66;"> </p> </li> 
     <li> <p>如果項目未完成，並且項目的計畫完成日期已過，則項目進展狀態為 <strong>延遲</strong>. </p> <p> <img src="assets/project-late-progress-status-incomplete-status-350x66.png" style="width: 350;height: 66;"> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

請考量下列事項：

* 項目的預計完成日期由關鍵路徑上具有最新預計完成日期的任務驅動。
* 項目的預計完成日期由關鍵路徑上具有最新預計完成日期的任務驅動。

有關項目關鍵路徑的資訊，請參見 [項目關鍵路徑概述](../../../manage-work/tasks/manage-tasks/critical-path.md).

有關預計完成日期的資訊，請參閱 [項目、任務和問題的預計完成日期概覽](../../../manage-work/projects/planning-a-project/project-projected-completion-date.md).
