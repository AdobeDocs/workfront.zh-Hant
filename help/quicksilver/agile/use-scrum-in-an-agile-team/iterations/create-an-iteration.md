---
product-area: agile-and-teams
navigation-topic: iterations
title: 建立小版本
description: 迭代是Scrum敏捷團隊規劃工作容量時的關鍵元件。 [!DNL Adobe Workfront] 可讓靈活的Scrum團隊透過建立多個反覆項目來管理其工作，以符合團隊的需求。
author: Lisa
feature: Agile
exl-id: a25cdd4a-f2e3-4b8a-a7f4-3757940b635e
source-git-commit: 6f817ca39c7489b85673ff601faf440fe51ab72c
workflow-type: tm+mt
source-wordcount: '1049'
ht-degree: 0%

---

# 建立小版本

迭代是Scrum敏捷團隊規劃工作容量時的關鍵元件。 [!DNL Adobe Workfront] 可讓靈活的Scrum團隊透過建立多個反覆項目來管理其工作，以符合團隊的需求。

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 計劃*</strong></td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 授權*</strong></td> 
   <td> <p>[!UICONTROL Review]或更高版本</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫或授權類型，請連絡您的 [!DNL Workfront] 管理員。

## 添加小版本

使用 [!UICONTROL 添加小版本] 功能，快速建立小版本，並稍後新增任務和問題。

1. 按一下 **[!UICONTROL 主菜單]** 圖示 ![](assets/main-menu-icon.png) 在 [!DNL Adobe Workfront]，然後按一下 **[!UICONTROL 團隊]**.

1. （選用）按一下 **[!UICONTROL 交換組]** 圖示 ![切換團隊表徵圖](assets/switch-team-icon.png)，然後從下拉式選單中選取新的Scrum團隊，或在搜尋列中搜尋團隊。

1. 在 **[!UICONTROL 迭代]** 按一下 **[!UICONTROL 添加小版本]**.\
   ![](assets/add-iteration-adobe-350x275.png)

1. 指定下列項目：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL迭代名]</strong></td> 
      <td>輸入小版本的名稱。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL目標]</strong></td> 
      <td>新增您對小版本擁有的任何目標。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL開始日期]</strong></td> 
      <td>輸入小版本的開始日期。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL結束日期]</strong></td> 
      <td><p>輸入小版本應結束的日期。 [!DNL Workfront] 建議設定結束日期不要超過開始日期的4週。</p><p>提示：請務必選擇工作日作為結束日期。 燃耗圖計算時只使用工作日。<br>預設情況下，燃耗圖會使用預設計畫來定義工作日(如 <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">建立排程</a>)。 或者，要合併特定於團隊的非工作日，敏捷團隊可以選擇使用替代計畫(如 <a href="../../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md" class="MCXref xref">建立敏捷的團隊</a>)。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL容量]</strong></td> 
      <td> 指定小版本的容量。 這是您的團隊在迭代中可完成的點數或小時數。 您輸入的數字必須等於或大於小版本中所有文章之和後的點數或小時數。<br>[!DNL Workfront] 預設會以50個容量預先填入此欄位。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL焦點]</strong></td> 
      <td>指定團隊的焦點百分比。 如果團隊的所有成員都將完全專注於此迭代，則重點將是100%。<br>[!DNL Workfront] 預設會以100%預先填入此欄位。 </td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下 **[!UICONTROL 提交]**. 現在您已建立了迭代，需要添加動態。 如需詳細資訊，請參閱 [將動態添加到現有小版本](../../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md).

## 在 [!UICONTROL 積壓] 標籤

使用 [!UICONTROL 計畫迭代] 功能，使用積壓工作建立小版本。

1. 按一下 **[!UICONTROL 主菜單]** 圖示 ![](assets/main-menu-icon.png) 在 [!DNL Adobe Workfront]，然後按一下 **[!UICONTROL 團隊]**.

1. （選用）按一下 **[!UICONTROL 交換組]** 圖示 ![切換團隊表徵圖](assets/switch-team-icon.png)，然後從下拉式選單中選取新的Scrum團隊，或在搜尋列中搜尋團隊。

1. 選擇 **[!UICONTROL 積壓]** 在左側面板上。 然後，按一下 **[!UICONTROL 計畫迭代]**.

1. 指定下列資訊：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL迭代名]</strong></td> 
      <td>指定小版本的名稱。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL開始日期]</strong></td> 
      <td> 指定小版本的開始日期。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL結束日期]</strong> </td> 
      <td><p>指定小版本應結束的日期。 [!DNL Workfront] 建議設定結束日期不要超過開始日期的4週。</p><p>提示：請務必選擇工作日作為結束日期。 燃耗圖計算時只使用工作日。<br>預設情況下，燃耗圖會使用預設計畫來定義工作日(如 <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">建立排程</a>)。 或者，要合併特定於團隊的非工作日，敏捷團隊可以選擇使用替代計畫(如 <a href="../../../agile/use-scrum-in-an-agile-team/burndown/use-alt--team-schedule-burndown-charts.md" class="MCXref xref">對折磨圖使用替代的團隊計畫</a>)。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL焦點]</strong></td> 
      <td>指定團隊的焦點百分比。 如果團隊的所有成員都將完全專注於此迭代，則重點將是100%。<br>[!DNL Workfront] 使用您團隊過去反覆項目的平均值預先填入此欄位。 如果這是您團隊的第一個小版本，則此欄位值預設為0。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><br><strong>[!UICONTROL容量]</strong></td> 
      <td> 指定小版本的容量。 這是您的團隊在迭代中可完成的點數或小時數。 您輸入的數字必須等於或大於小版本中所有文章之和後的點數或小時數。<br>[!DNL Workfront] 使用您團隊過去反覆項目的平均值預先填入此欄位。 如果這是您團隊的第一個小版本，則此欄位值預設為0。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><br><strong>[!UICONTROL目標]</strong></td> 
      <td> 指定小版本的目標。 此欄位不是必填欄位。</td> 
     </tr> 
    </tbody> 
   </table>

1. （可選）選擇文章以立即將其添加到小版本，或者您可以跳過此步驟，稍後將文章添加到小版本。 在積壓最重要的故事是更優先的。 當故事適合時，它們會以綠色突出顯示；如果沒有，則會以紅色強調顯示。\
   您可以將任務和問題都新增至單一迭代：

   * **要向小版本添加任務：** 在 **[!UICONTROL 積壓]** 標籤，確保 **[!UICONTROL 故事]** 頁簽（在查看積壓時，預設會選中此頁簽）。 選擇要添加到小版本的文章。\

      將任務添加到小版本時，任務的開始日期將按照 [[!UICONTROL 了解] 添加到迭代時如何計算任務開始日期](#understand-how-task-start-dates-are-calculated-when-added-to-an-iteration).

   * **要向小版本添加問題：** 在 **[!UICONTROL 積壓]** ，按一下 **[!UICONTROL 問題]** 標籤。 選擇要添加到小版本的問題。

1. 按一下&#x200B;**[!UICONTROL 儲存]。**
將建立小版本。

1. （可選）若要將動態新增至現有的小版本，請參閱 [將動態添加到現有小版本](../../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md).

## 了解在將任務開始日期添加到小版本時如何計算任務開始日期 {#understand-how-task-start-dates-are-calculated-when-added-to-an-iteration}

將任務作為動態添加到小版本時， [!UICONTROL 必須完成任務] 每個文章都會使用限制。 在大多數情況下，任務的計畫起始日期是根據以下公式計算的：

[!UICONTROL 迭代結束日期] 減號(-) [!UICONTROL 任務持續時間] 等於(=) [!UICONTROL 任務計畫起始日期]

此 [!UICONTROL 專案結束日期] 如果項目起始日期晚於小版本起始日期，而項目終止日期晚於小版本終止日期，則使用此選項代替。

您可以設定個別Scrum團隊，依預設使用專案日期，而非迭代日期。 如需詳細資訊，請參閱 [配置將工作項添加到小版本時如何應用日期](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configur5) 在文章中 [配置Scrum](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md).
