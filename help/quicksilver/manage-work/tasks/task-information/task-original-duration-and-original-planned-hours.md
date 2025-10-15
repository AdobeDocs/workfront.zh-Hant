---
content-type: overview
product-area: projects
navigation-topic: task-information
title: 任務原始工期與原始計畫時數概要
description: 作為計畫專案的一部分，您應該決定專案中每個任務的「計畫時數」和「期間」（或「計畫期間」）的值。
author: Alina
feature: Work Management
exl-id: 96d77d9f-3d5f-457e-a4ad-10edc371a991
source-git-commit: 7427706f6ce6cad3370b91269c1b4e7a10ed09f9
workflow-type: tm+mt
source-wordcount: '578'
ht-degree: 1%

---

# 任務原始期間與原始計畫時數概觀

作為計畫專案的一部分，您應該決定專案中每個任務的「計畫時數」和「期間」（或「計畫期間」）的值。

如需有關工作的計畫時數的詳細資訊，請參閱[計畫時數總覽](../../../manage-work/tasks/task-information/planned-hours.md)。

如需有關工作持續時間的詳細資訊，請參閱[工作持續時間和持續期間型別概觀](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md)。

您可以在「任務詳細資訊」標籤中或編輯任務時檢視這些值。

如果您建立任務清單或任務報告的檢視，則還可以檢視任務的原始計畫時數和原始工期欄位。

## 原始規劃時數

任務的原始計畫時數表示任務在成為父任務之前的原始計畫時數。 當任務變為父任務時，子任務的計畫時數將上滾到父任務以指示父任務的計畫時數。

在任務報告或清單中顯示原始計畫時數欄位，您可以在任務繼承其子系的計畫時數之前檢視原始計畫時數。

>[!NOTE]
>
>建立任務時，原始計畫時數為零。 如果任務成為父系任務，則此欄位的值會填入任務在變更為父系之前的計畫時數。 即使任務恢復為獨立任務，此值仍會保留在此欄位中。

## 初始期間

任務的原始期間是任務成為父任務之前的原始期間（以分鐘為單位）。 當任務成為父系時，最早子系的計劃開始日期與最後一個子系的計畫完成日期之間的期間會累計至父系任務，並成為父系任務的期間。 這會取代原始任務的工期。

在任務報告或清單中顯示「原始工期」欄位，您可以看到任務在繼承其子系工期之前的原始工期天數。

>[!NOTE]
>
>當您建立任務時，「原始持續時間」為零。 如果任務成為父系任務，則此欄位的值會填入任務的「持續時間」，之後才會將其變更為父系。 即使任務恢復為獨立任務，此值仍會保留在此欄位中。 此值以分鐘為單位顯示。

## 範例

例如，當兩個任務為獨立任務時，其原始持續時間和原始計畫時數為零。

![original_planned_hours_and_duration_without_parent.png](assets/original-planned-hours-and-duration-without-parent-350x38.png)

當第一個任務成為第二個任務的父系時，原始期間和原始計畫時數欄位會填入任務成為父系之前的「期間」和「計畫時數」值。 原始期間會以分鐘為單位顯示。 子系的「期間」和「計畫時數」會變成父系的「期間」和「計畫時數」。

![original_and_planned_hours_with_a_parent_task.png](assets/original-and-planned-hours-with-a-parent-task-350x38.png)

當父系再次成為獨立任務時，持續時間和計畫時數恢復為原始值，而原始持續時間和原始計畫時數保持填入。 它們不會還原為零。

![original_duration_and_planned_hours_after_reversal_of_a_parent.png](assets/original-duration-and-planned-hours-after-reversal-of-a-parent-350x39.png)
