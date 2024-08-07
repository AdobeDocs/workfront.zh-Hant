---
content-type: overview
product-area: projects
navigation-topic: task-information
title: 預計日期與估計日期概要
description: 有數種日期型別會顯示任務開始時間和完成時間之間的時間軸。
author: Alina
feature: Work Management
exl-id: 7cc68fc4-5f79-4ce6-a404-737ea8959ec3
source-git-commit: 811d8076a0b344e863b25aa253a0fb1c102f0435
workflow-type: tm+mt
source-wordcount: '924'
ht-degree: 0%

---

# 預計日期與估計日期概要

<!--Audited: 07/2024-->

有數種日期型別會顯示任務開始時間和完成時間之間的時間軸。 以下是顯示任務時間表的一些日期：

* 計劃開始與計畫完成日期
* 預計開始與預計完成日期
* 預估開始日期與預估到期日期
* 實際開始日期與實際完成日期

本文會說明專案的估計日期和預計日期之間的差異。

首次建立任務時，計畫、預計和估計日期通常應該相符。 有些例外情況存在。

如需Adobe Workfront中專案、任務和問題日期的詳細資訊，請參閱[Workfront中專案、任務和問題日期的概觀](../../../workfront-basics/navigate-workfront/workfront-navigation/definitions-pti-dates.md)。

## 計畫日期總覽

計畫日期是專案所有者定義為任務開始和結束日期的日期。 您或專案所有者可以手動修改任務的計畫日期。

## 實際日期概要

首次建立任務時，由於任務尚未開始或完成，因此沒有實際日期。

## 預計日期與估計日期概要

在專案存留期間，「預計日期」和「預估日期」更符合專案的實際情況，因為它們會考量哪些因素可能會影響任務的實際開始和結束。 這會導致他們從計畫日期變更。

處理任務的預計和估計日期時，請考慮下列事項：

* 您無法手動修改任務的預估日期或預計日期。 兩者皆由Adobe Workfront計算。
* 當您建立任務時，「預計」和「預計」日期應該相同，並且應該說明任務可以開始或結束的實際時間。\
  您對任務進行的特定更新會直接影響「預計日期」和「預計日期」的值。

  例如，如果使用者開始或完成任務，則任務會顯示影響任務的「預計日期」和「預估日期」的「實際開始日期」和「完成日期」。 此外，如果任務上的受分派者修改「認可日期」，此日期會影響任務的「預計日期」。

## 預計日期和估計日期之間的差異

「預計日期」與「預估日期」的差異為：

* 使用者若對任務進行下列更新，則會影響預計日期：

   * 透過新增固定任務限制來新增限制日期
   * 新增認可日期

* 「預估日期」只會考慮指定時間點上任務的實際進度。

**範例：**&#x200B;如果任務的計劃開始日期為9月20日，計畫完成日期為9月24日，且任務必須在限制時完成，即預計完成日期為9月24日。 此任務的工期為4天。

預估完成日期是根據任務上工作的目前進度計算的。 因此，如果今天是9月23日，任務尚未開始，則估計完成日期是9月27日（假設工作今天開始，應在4天後完成）。

如果任務今天已完成50%，則預計完成日期為9月25日（應在2天後完成，為任務期間的一半）。


### 瞭解任務的預計日期何時更新 {#understand-when-projected-dates-update-on-tasks}

「預計日期」可以與其他任務日期相符，或是Workfront根據任務的實際進度進行的計算。

下列清單顯示數個案例，說明在專案存留期內任務的「預計日期」會根據實際任務發生的情況而有所變更的情況：

* 當任務標示為完成時：

  `Projected Dates = Estimated Dates = Actual Dates`

* 當任務具有實際開始日期時：

  `Projected Start Date = Estimated Start Date = Actual Start Date`

* 當任務沒有實際開始日期，但對未來的「計劃開始日期」（必須開始於）有強制限制時：

  `Projected Start Date = Constraint Date`

  如需限制日期的詳細資訊，請參閱[Adobe Workfront術語表](../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md)。

* 當任務沒有實際開始日期且任務沒有強制限制日期時：

  `Projected Start Date = the next available date in the future that falls within working schedule`

* 當受指派人更新認可日期時：

  `Projected Completion Date = Commit Date`

  如需認可日期的相關資訊，請參閱[認可日期概觀](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md)。

* 當任務沒有更新的認可日期，並且任務具有未來計畫完成日期的強制限制（必須完成日期）時：

  `Projected Completion Date = Constraint Date`

* 當任務沒有更新的認可日期、強制限制日期在未來，或限制日期在過去：

  `Projected Completion Date = system calculation for the Completion Date based on the current progress and the work left to be done`

### 瞭解任務的估計日期何時更新 {#understand-when-the-estimated-dates-update-on-tasks}

相較於上述的「預計日期」案例，「預估日期」一律會反映Workfront對任務何時開始或完成的真實分析，不論「限制」或「認可日期」為何。

## 影響任務時間表的原因

以下是一些會影響任務實際時間表的範例：

* 與計畫日期和當天相關的任務進度
* 目前任務完成百分比
* 前置任務關係
* 前置任務進度
* 使用者分配

  >[!NOTE]
  >
  >如果使用者配置影響任務的完成速度，則可能會影響任務的估計完成日期。 例如，如果任務「期間型別」是「投入比導向」，您可以透過新增受指派人來讓任務更快地完成。 因此，「預估完成日期」會變更。
