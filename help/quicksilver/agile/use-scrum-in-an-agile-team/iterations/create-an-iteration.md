---
product-area: agile-and-teams
navigation-topic: iterations
title: 建立反複專案
description: 反複專案是Scrum敏捷團隊規劃工作容量的關鍵元件。 [!DNL Adobe Workfront] 可讓Scrum敏捷團隊透過建立多個疊代來因應團隊需求來管理其工作。
author: Lisa
feature: Agile
exl-id: a25cdd4a-f2e3-4b8a-a7f4-3757940b635e
source-git-commit: ddff70b61a2c3b3479e278bb3bb8628ac83f5c97
workflow-type: tm+mt
source-wordcount: '1057'
ht-degree: 0%

---

# 建立反複專案

反複專案是Scrum敏捷團隊規劃工作容量的關鍵元件。 [!DNL Adobe Workfront] 可讓Scrum敏捷團隊透過建立多個疊代來因應團隊需求來管理其工作。

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
   <td> <p>[！UICONTROL Review]或更高版本</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫或授權型別，請連絡您的 [!DNL Workfront] 管理員。

## 新增反複專案

使用 [!UICONTROL 新增反複專案] 快速建立疊代及稍後新增任務和問題的功能。

1. 按一下 **[!UICONTROL 主要功能表]** 圖示 ![](assets/main-menu-icon.png) 位於的右上角 [!DNL Adobe Workfront]，然後按一下 **[!UICONTROL 團隊]**.

1. （可選）按一下 **[!UICONTROL 切換群組]** 圖示 ![切換群組圖示](assets/switch-team-icon.png)，然後從下拉式選單中選取新的Scrum團隊或在搜尋列中搜尋團隊。

1. 在 **[!UICONTROL 反複專案]** 標籤，按一下 **[!UICONTROL 新增反複專案]**.\
   ![](assets/add-iteration-adobe-350x275.png)

1. 指定下列專案：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>[！UICONTROL反複專案名稱]</strong></td> 
      <td>輸入反複專案的名稱。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[！UICONTROL目標]</strong></td> 
      <td>新增您對此反複專案擁有的任何目標。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[！UICONTROL開始日期]</strong></td> 
      <td>輸入反複專案應該開始的日期。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[！UICONTROL結束日期]</strong></td> 
      <td><p>輸入反複專案應該結束的日期。 [!DNL Workfront] 建議結束日期設為從開始日期起的4週內。</p><p>提示：請務必選擇工作日作為結束日期。 待執行工作圖表在計算中僅使用工作日。<br>根據預設，待執行工作圖表會使用預設排程來定義工作天（如所述） <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">建立排程</a>)。 或者，若要合併特定團隊的非工作日，敏捷團隊可以選擇使用替代排程（如以下的「為待執行工作圖表定義替代團隊排程」中所述） <a href="../../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md" class="MCXref xref">建立敏捷團隊</a>)。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[！UICONTROL容量]</strong></td> 
      <td> 指定反複專案的容量。 這是您的團隊在反複專案中能夠完成的點數或時數。 您輸入的數字必須等於或大於反複專案中所有劇本的總和中的點數或小時數。<br>[!DNL Workfront] 預設會以50個容量預先填入此欄位。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[！UICONTROL焦點]</strong></td> 
      <td>指定團隊的焦點百分比。 如果團隊的所有成員將完全專注於此反複專案，則焦點將是100%。<br>[!DNL Workfront] 預設會以100%預先填入此欄位。 </td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下 **[!UICONTROL 提交]**. 現在您已建立反複專案，需要新增劇本。 如需詳細資訊，請參閱 [將劇本新增至現有反複專案](../../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md).

## 在上計畫反複專案 [!UICONTROL 待處理專案] 標籤

使用 [!UICONTROL 計畫反複專案] 使用待處理專案上的任務建立反複專案的功能。

1. 按一下 **[!UICONTROL 主要功能表]** 圖示 ![](assets/main-menu-icon.png) 位於的右上角 [!DNL Adobe Workfront]，然後按一下 **[!UICONTROL 團隊]**.

1. （可選）按一下 **[!UICONTROL 切換群組]** 圖示 ![切換群組圖示](assets/switch-team-icon.png)，然後從下拉式選單中選取新的Scrum團隊或在搜尋列中搜尋團隊。

1. 選取 **[!UICONTROL 待處理專案]** 位於左側面板。 然後，按一下 **[!UICONTROL 計畫反複專案]**.

1. 指定下列資訊：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>[！UICONTROL反複專案名稱]</strong></td> 
      <td>指定反複專案的名稱。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[！UICONTROL開始日期]</strong></td> 
      <td> 指定反複專案應該開始的日期。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[！UICONTROL結束日期]</strong> </td> 
      <td><p>指定反複專案應該結束的日期。 [!DNL Workfront] 建議結束日期設為從開始日期起的4週內。</p><p>提示：請務必選擇工作日作為結束日期。 待執行工作圖表在計算中僅使用工作日。<br>根據預設，待執行工作圖表會使用預設排程來定義工作天（如所述） <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">建立排程</a>)。 或者，若要納入團隊特定的非工作日，敏捷團隊可以選擇使用替代排程（如所述） <a href="../../../agile/use-scrum-in-an-agile-team/burndown/use-alt-team-schedule-burndown-charts.md" class="MCXref xref">對待執行工作圖表使用替代的小組排程</a>)。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[！UICONTROL焦點]</strong></td> 
      <td>指定團隊的焦點百分比。 如果團隊的所有成員將完全專注於此反複專案，則焦點將是100%。<br>[!DNL Workfront] 會使用您團隊過去反複專案的平均值預先填入此欄位。 如果這是您團隊的第一個反複專案，預設情況下此欄位值為0。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><br><strong>[！UICONTROL容量]</strong></td> 
      <td> 指定反複專案的容量。 這是您的團隊在反複專案中能夠完成的點數或時數。 您輸入的數字必須等於或大於反複專案中所有劇本的總和中的點數或小時數。<br>[!DNL Workfront] 會使用您團隊過去反複專案的平均值預先填入此欄位。 如果這是您團隊的第一個反複專案，預設情況下此欄位值為0。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><br><strong>[！UICONTROL目標]</strong></td> 
      <td> 指定反複專案的目標。 此欄位不是必填欄位。</td> 
     </tr> 
    </tbody> 
   </table>

1. （可選）選取劇本以立即將其新增至疊代，或者您可以略過此步驟，稍後將劇本新增至疊代。 待處理專案最上方的劇本優先順序較高。 符合容量大小的內文會以綠色反白顯示；若不符合，則會以紅色反白顯示。\
   您可以將任務和問題新增至單一反複專案：

   * **若要將任務新增至反複專案，請執行下列動作：** 在 **[!UICONTROL 待處理專案]** 標籤，確認 **[!UICONTROL 劇本]** 標籤會選取（檢視待處理專案時，預設會選取此標籤）。 選取您要新增至反複專案的劇本。\

     將任務新增至疊代時，會依照中的說明計算任務的開始日期 [[!UICONTROL 瞭解] 新增至疊代時如何計算任務開始日期](#understand-how-task-start-dates-are-calculated-when-added-to-an-iteration).

   * **若要將問題新增至反複專案：** 在 **[!UICONTROL 待處理專案]** 索引標籤，按一下 **[!UICONTROL 問題]** 標籤。 選取您要新增至疊代的問題。

1. 按一下「**[!UICONTROL 儲存]」。**
反複專案隨即建立。

1. （可選）若要將內文新增至現有反複專案，請參閱 [將劇本新增至現有反複專案](../../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md).

## 瞭解任務開始日期新增至疊代時如何計算 {#understand-how-task-start-dates-are-calculated-when-added-to-an-iteration}

當您將任務新增為劇本至疊代時， [!UICONTROL 必須完成任務] 限制用於每個劇本。 在大多數情況下，任務的計劃開始日期會根據下列公式計算：

[!UICONTROL 反複專案結束日期] 減號(-) [!UICONTROL 任務工期] 等於(=) [!UICONTROL 任務計劃開始日期]

此 [!UICONTROL 專案結束日期] 如果專案開始日期在反複專案開始日期之後，而專案結束日期在反複專案結束日期之後，則會使用而非。

您可以設定個別Scrum團隊以預設使用專案日期，而不是反複專案日期。 如需詳細資訊，請參閱區段 [設定將工作專案新增至疊代時日期的套用方式](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configur5) 在文章中 [設定Scrum](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md).
