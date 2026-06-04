---
product-area: portfolios
navigation-topic: portfolio-optimizer
title: 計算投資組合中淨值的風險
description: 在Portfolio Optimizer中，[!UICONTROL 淨值的風險]指標會考量由Portfolio Optimizer中顯示的所有專案所提供的淨值的潛在風險。
author: Alina
feature: Work Management, Strategic Planning
exl-id: 9e86f6eb-dd82-4731-aebb-ce8da1df5614
TQID: https://experienceleague.adobe.com/mClkaUv0y-Y9wiqg4oJivWYtmJDuKG701nOr5TU5rCA
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2: id: c10f2e93-7a58-4212-aa24-684c265ebe76id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 178
ht-degree: 0%

---

# 計算投資組合中[!UICONTROL 淨值的風險]

在[!UICONTROL Portfolio Optimizer]中，[!UICONTROL 淨值的風險]指標會考量由[!UICONTROL Portfolio Optimizer]中顯示的所有專案所提供的[!UICONTROL 淨值]的潛在風險。

若要在投資組合中達成最高效率，您想要看到[!UICONTROL 風險]指標低，[!UICONTROL 淨值]指標高。

[!UICONTROL 風險]和[!UICONTROL 淨值]指標是從它們相互關係的角度來表示的。

[!DNL Adobe Workfront]使用下列公式計算[!UICONTROL 風險]與[!UICONTROL 淨值]指標：

* [!UICONTROL 風險]指標的計算公式如下：

  ```
  Risk indicator = Risk / (Risk + Net Value)
  ```

* [!DNL Net Value]指標的計算公式如下：

  ```
  Net Value indicator = 1 - Risk / (Risk + Net Value)
  ```

  或

  ```
  Net Value indicator = Net Value / (Risk + Net Value)
  ```

>[!NOTE]
>
>[!UICONTROL 淨值的風險]指標是根據您在[!UICONTROL Portfolio Optimizer]中顯示的專案計算的，而不是根據與投資組合關聯的所有專案計算。
