---
product-area: agile-and-teams
navigation-topic: get-started-with-agile-in-workfront
title: 建立敏捷團隊
description: Adobe Workfront可讓敏捷團隊以漸進式、有條理的方式完成工作。
author: Lisa
feature: Agile
exl-id: 3afd16db-7829-4c9c-a981-461990c9dbc8
source-git-commit: 79da9f7ed5149ca33f6eaeac347188149f410695
workflow-type: tm+mt
source-wordcount: '1003'
ht-degree: 1%

---

# 建立敏捷團隊

<!--Audited: 01/2024-->

[!DNL Adobe Workfront]可讓敏捷團隊以漸進式、有條理的方式完成工作。

組織中的任何使用者都可以檢視敏捷團隊並檢視團隊的所有敏捷元件，包括待處理專案、反複專案、劇本面板和個別劇本。 但是，只有具有[!UICONTROL 編輯]工作存取權的團隊成員才能變更指派給團隊的工作。

[!DNL Workfront]支援下列敏捷方法：

* **[!UICONTROL Scrum]**：團隊有需要完成的待處理工作。 當團隊準備好處理特定區塊的工作時，該工作會從待處理專案移至疊代。 如需有關管理Scrum團隊的詳細資訊，請參閱[敏捷團隊中的Scrum](../../agile/use-scrum-in-an-agile-team/scrum-in-an-agile-team.md)。

* **[!UICONTROL 看板]：**&#x200B;團隊在看板檢視中跨預先決定的狀態移動工作。 預設狀態為：待處理專案、處理中及完成。 如需有關管理Kanban團隊的詳細資訊，請參閱[敏捷團隊中的Kanban](../../agile/use-kanban-in-an-agile-team/using-kanban-in-an-agile-team.md)。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計劃</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權</td> 
   <td> <p>新增：標準</p>
   目前： 
   <ul><li><p>[！UICONTROL計畫]以建立新的敏捷團隊</p></li> 
   <li><p>[！UICONTROL Work]或更高版本，可將團隊轉換為敏捷團隊</p></li></ul> </td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 決定敏捷方法

您可以為敏捷團隊使用Scrum或Kanban敏捷方法。 每種方法都有各種優點。 敏捷團隊的工作方式決定了您選擇使用的敏捷方法。

[!DNL Workfront]中的Scrum和Kanban敏捷方法都可讓您跨故事板移動故事，以指示故事的狀態變更和進度。

[!DNL Workfront]中的Scrum和Kanban敏捷方法有下列差異：

### 在[!DNL Workfront]中使用看板的好處

[!DNL Workfront]中的[!DNL Kanban]敏捷方法可讓您更輕鬆地在敏捷故事板上移動故事，同時限制進行中的工作量。 使用[!DNL Kanban]敏捷方法時沒有開始和結束日期。

下列功能支援此方法：

* 在[!DNL Kanban]敏捷劇本板上顯示待處理專案。
如需詳細資訊，請參閱[將待處理專案新增至[!UICONTROL Kanban]展示板](../../agile/use-kanban-in-an-agile-team/view-the-backlog-on-the-kanban-board.md)。

* 設定待處理專案上的專案，以便在其他專案移至等同於完成的狀態時，自動新增至[!UICONTROL Kanban]敏捷故事板。
如需詳細資訊，請參閱文章[設定Kanban](../../agile/get-started-with-agile-in-workfront/configure-kanban.md)中的[設定要自動從待處理專案新增的劇本](../../agile/get-started-with-agile-in-workfront/configure-kanban.md#configur5)一節。

* 設定要在[!UICONTROL Kanban]敏捷故事板上顯示的進行中工作(WIP)限制。
如需詳細資訊，請參閱[在Kanban展示板上管理進行中的工作(WIP)限制](../../agile/use-kanban-in-an-agile-team/work-in-progress-limit-on-the-kanban-board.md)。

### 在[!DNL Workfront]中使用Scrum的好處

[!DNL Workfront]中的Scrum敏捷方法可讓您新增一組劇本至敏捷反複專案，並為該反複專案建立劇本面板。 反複專案是根據您定義的開始和結束日期。

下列功能支援此方法：

* 在[!UICONTROL Scrum]故事板上包含問題
* 包括敏捷團隊待處理專案上的問題
* 子任務可以顯示在[!UICONTROL Scrum]故事板上
* 檢視待執行工作圖表，以檢視反複專案期間內文的進度
如需詳細資訊，請參閱[敏捷待執行工作圖表總覽](../../agile/use-scrum-in-an-agile-team/burndown/burndown-chart-overview.md)。

## 建立敏捷團隊

{{step1-to-team}}

1. 按一下&#x200B;**[!UICONTROL 切換團隊]**&#x200B;圖示![切換團隊圖示](assets/switch-team-icon.png)，然後按一下&#x200B;**[!UICONTROL 建立新團隊]**。

   ![選取[建立新團隊]](assets/create-new-team.png)

   「新專案團隊」方塊隨即顯示。

1. 指定下列資訊：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>[！UICONTROL團隊名稱]</strong> </td> 
      <td>輸入新敏捷團隊的名稱。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[！UICONTROL這是敏捷團隊]</strong> </td> 
      <td>選取此選項可將此新團隊設定為敏捷團隊。</td> 
     </tr>

   <tr> 
      <td role="rowheader"><strong>[！UICONTROL作用中]</strong> </td> 
      <td>選取此選項以啟動此團隊。 其他使用者看不到非作用中的團隊以指派給工作。 </td> 
     </tr>


   <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
      <td role="rowheader"><strong>[！UICONTROL群組]</strong> </td> 
      <td> <p>開始鍵入要加入團隊的群組名稱，然後在名稱出現在下拉式清單中時選取名稱。</p> <p><b>附註</b></p> <p> 將專案團隊指派給群組或子群組時，該群組或子群組的任何群組管理員都可以管理專案團隊，而無需成為專案團隊的成員。 群組管理員可以從[！UICONTROL主功能表]前往[！UICONTROL團隊]區域，然後按一下[！UICONTROL切換團隊]箭頭<img src="assets/switch-team-icon.png" alt="切換群組圖示">，列出指派給其管理群組的所有團隊。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[！UICONTROL團隊成員]</strong> </td> 
      <td>開始輸入加入團隊的使用者名稱，然後在名稱出現在下拉式清單中時選取名稱。<br>重複此程式，將多位使用者新增至團隊。<br>由於使用者可以位於多個團隊中，因此他們可以同時位於敏捷和非敏捷團隊中。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[！UICONTROL描述]</strong> </td> 
      <td><p>輸入團隊的說明。</p> <p>選擇團隊時，說明會顯示在[！UICONTROL團隊]區域的右上方。</p>
      <p>如果說明很長，您可以按一下該說明，在快顯視窗中顯示完整說明。 如果您有權編輯[！UICONTROL團隊設定]，也可以直接在快顯視窗中編輯說明。</p></td>
     </tr> 
    </tbody> 
   </table>

1. 按一下「**[!UICONTROL 建立]**」。

   如需有關設定敏捷團隊的資訊，請參閱下列文章：

   * [設定[!UICONTROL Kanban]](../../agile/get-started-with-agile-in-workfront/configure-kanban.md)
   * [設定[!UICONTROL Scrum]](../../agile/get-started-with-agile-in-workfront/configure-scrum.md)

## 將現有團隊轉換為敏捷團隊

您可以將現有團隊轉換為敏捷團隊：

{{step1-to-team}}

1. 按一下&#x200B;**[!UICONTROL 切換群組]**&#x200B;圖示![切換群組圖示](assets/switch-team-icon.png)，然後從下拉式功能表中選取新群組或在搜尋列中搜尋群組。

1. 選取您要轉換為敏捷團隊的團隊。
1. 按一下&#x200B;**[!UICONTROL 更多]**&#x200B;功能表，然後選取&#x200B;**[!UICONTROL 編輯]**。

   只有擁有[!UICONTROL 標準]、[!UICONTROL 計畫]或[!UICONTROL 工作]授權的團隊成員才能看到此選項。
   ![選取編輯](assets/edit-team-settings.png)

1. 在&#x200B;**[!UICONTROL Agile]**&#x200B;區段中，選取&#x200B;**[!UICONTROL 這是一個Agile團隊]**。

1. 在&#x200B;**[!UICONTROL 方法]**&#x200B;區段中，選取團隊將使用&#x200B;**[!UICONTROL Scrum]**&#x200B;或&#x200B;**[!UICONTROL Kanban]**&#x200B;敏捷方法。

1. 按一下「**儲存變更**」。

   團隊會儲存為敏捷團隊。 編輯團隊時，您可以將新團隊設定為Scrum或Kanban團隊。

   如需詳細資訊，請參閱下列文章：

   * [設定[!UICONTROL Kanban]](../../agile/get-started-with-agile-in-workfront/configure-kanban.md)
   * [設定[!UICONTROL Scrum]](../../agile/get-started-with-agile-in-workfront/configure-scrum.md)
