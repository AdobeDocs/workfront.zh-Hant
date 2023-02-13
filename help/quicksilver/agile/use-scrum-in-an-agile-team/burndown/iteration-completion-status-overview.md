---
content-type: overview
product-area: agile-and-teams
navigation-topic: burndown
title: 迭代完成狀態概覽
description: 本文描述的完成資訊顯示在燃耗圖上方。
author: Lisa
feature: Agile
exl-id: cc6bebdb-f2aa-4e85-9f9f-15e7753d84cb
source-git-commit: 373f2522b85196d6395f189ae6cfe03449cac61a
workflow-type: tm+mt
source-wordcount: '636'
ht-degree: 0%

---

# 迭代完成狀態概覽

本文描述的完成資訊顯示在燃耗圖上方。

小版本的完成百分比：

![](assets/burndown-percentcomplete-350x47.png)

此資訊指示當前在燃耗圖中選擇的日期的小版本的完成狀態。 依預設，完成狀態會根據當天的日期顯示。

提供下列資訊：

* **[!UICONTROL 完成百分比]:** 迭代的總體進度

   [!UICONTROL 完成百分比] 根據迭代內每個動態或任務的完成百分比進行調整，包括僅部分完成的動態或任務。

   顏色 [!UICONTROL 完成百分比] 狀態欄顯示為紅色或綠色，以符合實際燃耗率的顏色。 當燃耗率小於理想值時（比理想值時每天剩餘的點數或小時數多），當燃耗率等於或大於理想值時（比理想值時每天剩餘的點數少），則以紅色顯示。

* **[!UICONTROL 已完成的動態]:** （僅在迭代中可用）標示的動態數 [!UICONTROL 完成]. 這會與迭代中的動態總數相關。 例如，「6之3」表示小版本中的6層中有3層已標籤 [!UICONTROL 完成].
* **[!UICONTROL 完成的點數/小時]:** （僅在迭代中可用）標籤的點數或小時數 [!UICONTROL 完成]. 與小版本中的總點數或小時數相對顯示。 例如，「11的5篇」表示小版本中的11篇文章中有5篇已標示 [!UICONTROL 完成]. 此數字與 [!UICONTROL 完成百分比] 計算，並同時更新 [!UICONTROL 完成百分比] 已更新。

   點數和小時數與動態相關。 當文章被標籤時 [!UICONTROL 完成]，則與該動態相關的點數或小時會標示為「完成」。

   預設會使用點。 您可以修改團隊的設定以變更此項目，如 [建立敏捷的團隊](../../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md).

* **[!UICONTROL 每日點數/小時]:** （僅在迭代中可用）標示的平均點數或小時數 [!UICONTROL 完成] 從迭代開始到當天的每天。

   這會以完成的總點數或小時數除以當天的總天數計算。 （部分天數會記錄為一整天。）

   此資訊在規劃將來的迭代時非常有用。

* **[!UICONTROL 估計完成]:** 根據「每天點數/小時數」（適用於小版本）中的當前速率，預計完成小版本的日期。

   當 [!UICONTROL 估計完成] 日期晚於為小版本定義的結束日期，剩餘的工作天數會以紅色顯示在小版本旁邊的括弧中 [!UICONTROL 估計完成] 日期。

   當 [!UICONTROL 估計完成] 日期早於小版本的計畫結束日期，剩餘工作天數將以綠色顯示。 (計畫小版本時指定小版本的終止日期，如 [建立小版本](../../../agile/use-scrum-in-an-agile-team/iterations/create-an-iteration.md);專案的結束日期為 [!UICONTROL 計畫完成日期]，若 [!UICONTROL 計畫完成日期] 是過去。 此 [!UICONTROL 計畫完成日期] 針對專案，會根據專案中的工作持續時間計算。) 在計畫小版本時，如果為非工作日設定小版本終止日期，並且小版本正在按時跟蹤完成，則在您設定的小版本終止日期之前的最後一個工作日設定估計完成日期（因為沒有計畫在非工作日燒錄工作）。

   例如，「（+9天）」表示「估計完成日期」比迭代的計畫結束日期晚9個工作日。

   如需詳細資訊，請參閱 [迭代完成狀態概覽](#Understanding-How-Days-Off-Affect-the-Burndown-Chart).
