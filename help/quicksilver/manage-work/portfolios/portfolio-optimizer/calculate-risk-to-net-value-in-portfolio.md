---
product-area: portfolios
navigation-topic: portfolio-optimizer
title: 計算投資組合中淨值的風險
description: 在Portfolio Optimizer中，[!UICONTROL 淨值的風險]指標會考量由Portfolio Optimizer中顯示的所有專案所提供的淨值的潛在風險。
author: Alina
feature: Work Management, Strategic Planning
exl-id: 9e86f6eb-dd82-4731-aebb-ce8da1df5614
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '178'
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
