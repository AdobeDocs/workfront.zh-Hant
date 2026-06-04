---
content-type: reference
product-area: projects
navigation-topic: task-information
title: 計畫期間與任務期間之間的差異
description: 期間是工作專案的計劃開始與計畫完成日期之間的時間量。 任務在Adobe Workfront中有持續期間和計畫持續期間，視任務的持續期間型別而定。
author: Alina
feature: Work Management
exl-id: 183a3334-b4af-4f45-8e72-9e82ff3862a0
TQID: https://experienceleague.adobe.com/tVh55DKoBvOUZdq9lZ6y72rxZQ1WOoAYL-Pz8nlU588
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2: id: b91c0848-76c4-4da4-8b81-3aade0518dd0id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 272
ht-degree: 0%

---

# 計畫期間與任務期間之間的差異

期間是工作專案的計劃開始與計畫完成日期之間的時間量。 任務在Adobe Workfront中有持續期間和計畫持續期間，視任務的持續期間型別而定。

問題和專案無法與期間型別相關聯，並且它們只有期間。

## 任務工期

對於任務，「持續時間」和「計畫持續時間」通常顯示相同的值：任務的計劃開始日期與計畫完成日期之間的時間長度。

當任務的「期間型別」為「投入比導向」時，計畫期間會隨著您新增資源至任務而減少。

**範例：**&#x200B;如果工作驅動之工期型別的任務有3天的工期，而您指派一個具有全職排程的資源給該任務，則計畫工期也是3天。

如果您將三個具有全職排程的資源指派給相同的任務，「工期」會保留3天，但「計畫工期」會變成1天。計畫期間也會變更任務的計劃開始和計畫完成日期，以反映新的計畫期間。因此，專案的時間表也會受到影響。
當您將任務指派給多個資源時，可以使用「投入比導向的期間型別」。這可縮短在任務上完成工作所需的時間。

如需投入比導向期間型別的詳細資訊，請參閱[期間型別總覽：投入比導向](../../../manage-work/tasks/taskdurtn/effort-driven.md)。

## 問題和專案持續時間

問題和專案只有一個「持續時間」值，這是問題與專案的「計劃開始日期」和「計畫完成日期」之間的差異。
