---
product-area: agile-and-teams
navigation-topic: burndown
title: 使用待執行工作圖表的替代小組排程
description: 在[!DNL Adobe Workfront]中定義的排程會透過從待執行工作排除休假（週末和假日）來影響待執行工作圖表。
author: Courtney
feature: Agile
exl-id: 72650c19-434d-463a-8924-49219604ff01
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: 'https://experienceleague.adobe.com/BWnnytUMaoygpGpDdjQ5dmdBZrR1IWAu7onkwVizvUc'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
    internal-label: Work management
subfeature_v2:
  - id: ce22a157-dd2c-405f-b740-c2f204bb4c1a
    internal-label: Timesheets
  - id: be65ef36-43e4-48e1-a062-caa3778e15be
    internal-label: Agile
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 4c642a8ef31f3b9a03288f2d74e704be6ee86c55
workflow-type: tm+mt
source-wordcount: '304'
ht-degree: 7%
---
# 對待執行工作圖表使用替代的小組排程

在[!DNL Adobe Workfront]中定義的排程會透過從待執行工作排除休假（週末和假日）來影響待執行工作圖表。

根據預設，待執行工作圖表會使用預設排程。 除了預設排程外，敏捷團隊可以選擇使用替代排程，以便合併團隊特定的非工作日。 然後，此替代排程會反映在指派給團隊的任何疊代的待執行工作圖表中。 替代排程只會影響待執行工作圖表。 （如需有關預設排程的詳細資訊，以及[!DNL Workfront]管理員如何建立特定團隊的排程，請參閱[建立排程](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)。）

待執行工作圖表不會將部分天數列入考量。 例如，如果您的團隊每個星期五工作4小時，在待執行工作表中會以全天表示。

如需有關使用待執行工作圖表的詳細資訊，請參閱[敏捷待執行工作圖總覽](../../../agile/use-scrum-in-an-agile-team/burndown/burndown-chart-overview.md)。

## 存取權要求

+++ 展開以檢視這篇文章中所述功能的存取權要求。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 封裝</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td> <p>標準</p> 
   <p>工作或更高層級</p> </td> 
  </tr>
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 對待執行工作圖表使用替代的小組排程

1. 請確定[!DNL Workfront]管理員已建立替代排程，如[建立排程](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)中所述。

{{step1-to-team}}

1. （選擇性）按一下&#x200B;**[!UICONTROL 切換群組]**&#x200B;圖示![切換群組圖示](assets/switch-team-icon.png)，然後從下拉式功能表中選取新的Scrum群組或在搜尋列中搜尋群組。

1. 選取您要管理的敏捷團隊。
1. 按一下&#x200B;**[!UICONTROL 更多]**&#x200B;功能表，然後選取&#x200B;**[!UICONTROL 編輯]**。

1. 在&#x200B;**[!UICONTROL 敏捷]**&#x200B;區段的&#x200B;**[!UICONTROL 排程]**&#x200B;區域，從下拉式功能表選取新排程。

1. 按一下「**[!UICONTROL 儲存變更]**」。
