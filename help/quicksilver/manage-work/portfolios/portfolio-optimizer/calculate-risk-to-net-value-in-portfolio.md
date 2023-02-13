---
product-area: portfolios
navigation-topic: portfolio-optimizer
title: 計算投資組合中的淨值風險
description: 在Portfolio優化程式中， [!UICONTROL 淨值風險] 指標會考量Portfolio優化程式中顯示之所有專案所提供的淨值，以評估潛在風險。
author: Alina
feature: Work Management, Strategic Planning
exl-id: 9e86f6eb-dd82-4731-aebb-ce8da1df5614
source-git-commit: b6defd7dba91a06feb365ead74bd9c48f5165c77
workflow-type: tm+mt
source-wordcount: '178'
ht-degree: 0%

---

# 計算 [!UICONTROL 淨值風險] 在產品組合中

在 [!UICONTROL Portfolio優化程式], [!UICONTROL 淨值風險] 指標衡量潛在風險，並考慮 [!UICONTROL 淨值] 由顯示於 [!UICONTROL Portfolio優化程式]. 

為了在產品組合中達到最高效率，您希望 [!UICONTROL 風險] 指示器低， [!UICONTROL 淨值] 指標很高。 

此 [!UICONTROL 風險] 和 [!UICONTROL 淨值] 指標是從它們彼此的關係角度來表示的。

[!DNL Adobe Workfront] 計算 [!UICONTROL 風險] 和 [!UICONTROL 淨值] 指標使用下列公式：

* 此 [!UICONTROL 風險] 指標的計算公式如下：

   ```
   Risk indicator = Risk / (Risk + Net Value)
   ```

* 此 [!DNL Net Value] 指標的計算公式如下：

   ```
   Net Value indicator = 1 - Risk / (Risk + Net Value)
   ```

   或

   ```
   Net Value indicator = Net Value / (Risk + Net Value)
   ```

>[!NOTE]
>
>此 [!UICONTROL 淨值風險] 指標會根據您顯示於 [!UICONTROL Portfolio優化程式]，而非關聯至與產品組合關聯的所有專案。 
