---
product-area: agile-and-teams
navigation-topic: burndown
title: 對待執行工作圖表使用替代的小組排程
description: 在中定義的排程 [!DNL Adobe Workfront] 會透過從待執行工作排除休假（週末和假日）來影響待執行工作圖表。
author: Lisa
feature: Agile
exl-id: 72650c19-434d-463a-8924-49219604ff01
source-git-commit: ddff70b61a2c3b3479e278bb3bb8628ac83f5c97
workflow-type: tm+mt
source-wordcount: '315'
ht-degree: 0%

---

# 對待執行工作圖表使用替代的小組排程

在中定義的排程 [!DNL Adobe Workfront] 會透過從待執行工作排除休假（週末和假日）來影響待執行工作圖表。

根據預設，待執行工作圖表會使用預設排程。 除了預設排程外，敏捷團隊可以選擇使用替代排程，以便合併團隊特定的非工作日。 然後，此替代排程會反映在指派給團隊的任何疊代的待執行工作圖表中。 替代排程只會影響待執行工作圖表。 (如需有關預設排程的詳細資訊，以及 [!DNL Workfront] 管理員可以建立特定團隊的排程，請參閱 [建立排程](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).)

待執行工作圖表不會將部分天數列入考量。 例如，如果您的團隊每個星期五工作4小時，在待執行工作表中會以全天表示。

如需有關使用待執行工作圖表的詳細資訊，請參閱 [敏捷待執行工作圖表總覽](../../../agile/use-scrum-in-an-agile-team/burndown/burndown-chart-overview.md).

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 計畫*</strong></td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 授權*</strong></td> 
   <td> <p>[！UICONTROL Work]或更高版本</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫或授權型別，請連絡您的 [!DNL Workfront] 管理員。

## 對待執行工作圖表使用替代的小組排程

1. 確保 [!DNL Workfront] 管理員已建立替代排程，如中所述 [建立排程](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).
1. 按一下 **[!UICONTROL 主要功能表]** 圖示 ![](assets/main-menu-icon.png) 位於的右上角 [!DNL Adobe Workfront]，然後按一下 **[!UICONTROL 團隊]**.

1. （可選）按一下 **[!UICONTROL 切換群組]** 圖示 ![切換群組圖示](assets/switch-team-icon.png)，然後從下拉式選單中選取新的Scrum團隊或在搜尋列中搜尋團隊。

1. 選取您要管理的敏捷團隊。
1. 按一下 **[!UICONTROL 更多]** 功能表，然後選取 **[!UICONTROL 編輯]**.

1. 在 **[!UICONTROL 敏捷]** 區段，在 **[!UICONTROL 排程]** 區域，從下拉式選單中選取新排程。

1. 按一下「**[!UICONTROL 儲存變更]**」。
