---
product-area: agile-and-teams
navigation-topic: iterations
title: 建立反複專案
description: 反複專案是Scrum敏捷團隊規劃工作容量的關鍵元件。 [!DNL Adobe Workfront] 可讓Scrum敏捷團隊透過建立多個反複專案來因應團隊需求管理其工作。
author: Jenny
feature: Agile
exl-id: a25cdd4a-f2e3-4b8a-a7f4-3757940b635e
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '1022'
ht-degree: 0%

---

# 建立反複專案

反複專案是Scrum敏捷團隊規劃工作容量的關鍵元件。 [!DNL Adobe Workfront]可讓Scrum敏捷團隊透過建立多個反複專案來適應團隊需求來管理其工作。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront套件</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td> <p>淺色或更高</p> 
   <p>評論或以上</p> </td> 
  </tr>
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 新增反複專案

您可以在清單中新增反複專案以快速建立反複專案，並在稍後新增任務和問題。

{{step1-to-team}}

1. （選擇性）按一下&#x200B;**[!UICONTROL 切換群組]**&#x200B;圖示![切換群組圖示](assets/switch-team-icon.png)，然後從下拉式功能表中選取新的Scrum群組或在搜尋列中搜尋群組。

1. 在&#x200B;**[!UICONTROL 反複專案]**&#x200B;索引標籤上，按一下&#x200B;**[!UICONTROL 新增反複專案]**。

   ![按一下新增反複專案](assets/click-add-iteration.png)

1. 指定下列專案：

   <table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL 反複專案名稱]</strong></td> 
      <td>輸入反複專案的名稱。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL 目標]</strong></td> 
      <td>新增您對此反複專案擁有的任何目標。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL 開始日期]</strong></td> 
      <td>輸入反複專案應該開始的日期。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL 結束日期]</strong></td> 
      <td><p>輸入反複專案應該結束的日期。 [!DNL Workfront]建議將結束日期設定為從開始日期起的4週內。</p><p>提示：請務必選擇工作日作為結束日期。 待執行工作圖表在計算中僅使用工作日。<br>根據預設，待執行工作圖表會使用預設排程來定義工作日（如<a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">建立排程</a>中所述）。 或者，為了合併團隊特定的非工作日，敏捷團隊可以選擇使用替代排程（如<a href="../../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md" class="MCXref xref">建立敏捷團隊</a>中「為待執行工作圖表定義替代團隊排程」中所述）。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL 容量]</strong></td> 
      <td> 指定反複專案的容量。 這是您的團隊在反複專案中能夠完成的點數或時數。 您輸入的數字必須等於或大於反複專案中所有劇本的總和中的點數或小時數。<br>[!DNL Workfront]預設會以50個容量預先填入此欄位。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL 焦點]</strong></td> 
      <td>指定團隊的焦點百分比。 如果團隊的所有成員將完全專注於此反複專案，則焦點將是100%。<br>[!DNL Workfront]預設會以100%預先填入此欄位。 </td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下&#x200B;**[!UICONTROL 新增反複專案]**。 現在您已建立反複專案，需要新增劇本。 如需詳細資訊，請參閱[將劇本新增至現有反複專案](../../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md)。

## 在[!UICONTROL 待處理專案]索引標籤上計畫反複專案

使用[!UICONTROL 計畫反複專案]功能，以使用待處理專案上的任務來建立反複專案。

{{step1-to-team}}

1. （選擇性）按一下&#x200B;**[!UICONTROL 切換群組]**&#x200B;圖示![切換群組圖示](assets/switch-team-icon.png)，然後從下拉式功能表中選取新的Scrum群組或在搜尋列中搜尋群組。

1. 在左側面板上選取&#x200B;**[!UICONTROL 待處理專案]**。

1. 在&#x200B;**內文**&#x200B;或&#x200B;**問題**&#x200B;索引標籤上，選取您要新增至反複專案的工作專案，然後按一下&#x200B;**[!UICONTROL 計畫反複專案]**。

>[!NOTE]
>
> 在「待處理專案」標籤上規劃反複專案時，您無法在「內文」或「問題」標籤之間切換，或新增其他任務。 反複專案建立後，您就可以新增現有內文或問題。 如需詳細資訊，請參閱下方的[待處理專案]索引標籤[上的](#add-tasks-or-issues-to-an-existing-iteration-on-the-backlog-tab)將任務或問題新增到現有反複專案。


1. 指定下列資訊：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL 反複專案名稱]</strong></td> 
      <td>指定反複專案的名稱。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL 開始日期]</strong></td> 
      <td> 指定反複專案應該開始的日期。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL 結束日期]</strong> </td> 
      <td><p>指定反複專案應該結束的日期。 [!DNL Workfront]建議將結束日期設定為從開始日期起的4週內。</p><p>提示：請務必選擇工作日作為結束日期。 待執行工作圖表在計算中僅使用工作日。<br>根據預設，待執行工作圖表會使用預設排程來定義工作日（如<a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">建立排程</a>中所述）。 或者，若要合併特定團隊的非工作日，敏捷團隊可以選擇使用替代排程（如<a href="../../../agile/use-scrum-in-an-agile-team/burndown/use-alt-team-schedule-burndown-charts.md" class="MCXref xref">使用待執行工作表的替代團隊排程</a>中所述）。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL 焦點]</strong></td> 
      <td>指定團隊的焦點百分比。 如果團隊的所有成員將完全專注於此反複專案，則焦點將是100%。<br>[!DNL Workfront]會使用您團隊過去反複專案的平均值預先填入此欄位。 如果這是您團隊的第一個反複專案，預設情況下此欄位值為0。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><br><strong>[!UICONTROL 容量]</strong></td> 
      <td> 指定反複專案的容量。 這是您的團隊在反複專案中能夠完成的點數或時數。 您輸入的數字必須等於或大於反複專案中所有劇本的總和中的點數或小時數。<br>[!DNL Workfront]會使用您團隊過去反複專案的平均值預先填入此欄位。 如果這是您團隊的第一個反複專案，預設情況下此欄位值為0。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><br><strong>[!UICONTROL 目標]</strong></td> 
      <td> 指定反複專案的目標。 此欄位不是必填欄位。</td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下「**[!UICONTROL 儲存]」。**&#x200B;已建立反複專案。

## 將任務或問題新增到待處理專案索引標籤上的現有反複專案

1. 在&#x200B;**待處理專案**&#x200B;索引標籤中，按一下&#x200B;**劇本**&#x200B;或&#x200B;**問題**&#x200B;索引標籤。

1. 選取您想要新增至疊代的內文或問題。 待處理專案最上方的劇本優先順序較高。

   ![移動工作專案](assets/move-to-iteration.png)

   >[!NOTE]
   >
   >  將任務新增至疊代時，任務的開始日期會依照[[!UICONTROL 瞭解]中所述計算任務開始日期的方式新增至疊代](#understand-how-task-start-dates-are-calculated-when-added-to-an-iteration)時，任務的開始日期。


## 瞭解任務開始日期新增至疊代時如何計算 {#understand-how-task-start-dates-are-calculated-when-added-to-an-iteration}

將任務新增為內文至反複專案時，每個內文都會使用[!UICONTROL 必須在任務上完成]限制。 在大多數情況下，任務的計劃開始日期會根據下列公式計算：

[!UICONTROL 反複專案結束日期]減(-) [!UICONTROL 任務期間]等於(=) [!UICONTROL 任務計劃開始日期]

如果專案開始日期在反複專案開始日期之後，而專案結束日期在反複專案結束日期之後，則使用[!UICONTROL 專案結束日期]取代反複專案結束日期。

您可以設定個別Scrum團隊以預設使用專案日期，而不是反複專案日期。 如需詳細資訊，請參閱[設定Scrum](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configure-how-dates-are-applied-when-adding-work-items-to-an-iteration)一文中的[設定將工作專案新增至疊代](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md)時如何套用日期一節。
