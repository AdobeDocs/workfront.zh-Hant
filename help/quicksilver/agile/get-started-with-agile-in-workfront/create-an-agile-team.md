---
product-area: agile-and-teams
navigation-topic: get-started-with-agile-in-workfront
title: 建立敏捷的團隊
description: Adobe Workfront可讓敏捷團隊以漸進且有組織的方式完成工作。
author: Lisa
feature: Agile
exl-id: 3afd16db-7829-4c9c-a981-461990c9dbc8
source-git-commit: 7fc6230643d0a24c3b483df8165294ceca6dcce7
workflow-type: tm+mt
source-wordcount: '967'
ht-degree: 0%

---

# 建立敏捷的團隊

[!DNL Adobe Workfront] 使敏捷的團隊能夠以增量式、有組織的方式完成工作。

組織中的任何使用者都可以查看敏捷團隊，並檢視團隊的所有敏捷元件，包括積壓、迭代、動態展示板和個別動態。 但是，只有具有 [!UICONTROL 編輯] 對工作的訪問可以對分配給團隊的工作進行更改。

[!DNL Workfront] 支援下列敏捷方法：

* **[!UICONTROL Scrum]**:各隊的工作積壓，需要完成。 當團隊準備好處理特定工作組時，工作將從積壓工作移到小版本。 如需管理Scrum團隊的詳細資訊，請參閱 [在敏捷的團隊中](../../agile/use-scrum-in-an-agile-team/scrum-in-an-agile-team.md).

* **[!UICONTROL 看板]:** 團隊在「看板」視圖中在預定狀態間移動工作。 預設狀態為：積壓、處理中和完成。 有關管理看板小組的詳細資訊，請參閱 [敏捷團隊中的看板](../../agile/use-kanban-in-an-agile-team/using-kanban-in-an-agile-team.md).

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
   <td> <p>[!UICONTROL計畫]，建立新的敏捷團隊；[!UICONTROL Work]或更高版本，將團隊轉換為敏捷團隊</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫或授權類型，請連絡您的 [!DNL Workfront] 管理員。

## 決定靈活的方法

您可以為敏捷團隊使用Scrum或Ganban方法。 每種方法都提供各種優點。 您敏捷團隊的運作方式決定了您選擇使用的敏捷方法。

中的Scrum和看板敏捷方法 [!DNL Workfront] 可讓您在動態展示板上移動動態，以指出動態的狀態變更和進度。

Scrum和看板敏捷方法 [!DNL Workfront] 不同之處如下：

### 在中使用看板的好處 [!DNL Workfront]

此 [!DNL Kanban] 敏捷方法 [!DNL Workfront] 可讓您在敏捷的動態展示板上輕鬆移動動態，同時限制進行中的工作量。 使用 [!DNL Kanban] 敏捷的方法。

下列功能支援此方法：

* 顯示 [!DNL Kanban] 敏捷的故事板。\
   如需詳細資訊，請參閱 [將積壓工作新增至 [!UICONTROL 看板] 展示板](../../agile/use-kanban-in-an-agile-team/view-the-backlog-on-the-kanban-board.md).

* 設定積壓上的項目，以自動新增至 [!UICONTROL 看板] 當其他項目移至等於「完成」的狀態時，敏捷展示板。\
   如需詳細資訊，請參閱 [配置要自動從積壓中添加的動態](../../agile/get-started-with-agile-in-workfront/configure-kanban.md#configur5) 在文章中 [配置看板](../../agile/get-started-with-agile-in-workfront/configure-kanban.md).

* 配置要在 [!UICONTROL 看板] 敏捷的故事板。\
   如需詳細資訊，請參閱 [管理看板板上的在製品(WIP)限制](../../agile/use-kanban-in-an-agile-team/work-in-progress-limit-on-the-kanban-board.md).

### 在中使用Scrum的優點 [!DNL Workfront]

Scrum敏捷方法 [!DNL Workfront] 可讓您將一組動態新增至敏捷的迭代，並為該迭代建立動態展示板。 小版本以您定義的開始和結束日期為基礎。

下列功能支援此方法：

* 包括 [!UICONTROL Scrum] 故事板
* 包括有關敏捷團隊積壓的問題
* 子任務可顯示在 [!UICONTROL Scrum] 故事板
* 查看燃耗圖，查看迭代期間的動態進度\
   如需詳細資訊，請參閱 [敏捷燃耗圖概述](../../agile/use-scrum-in-an-agile-team/burndown/burndown-chart-overview.md).

## 建立新的敏捷團隊

1. 按一下 **[!UICONTROL 主菜單]** 圖示 ![](assets/main-menu-icon.png) 在 [!DNL Adobe Workfront]，然後按一下 **[!UICONTROL 團隊]**.
1. 按一下 **[!UICONTROL 切換團隊]** 圖示 ![切換團隊表徵圖](assets/switch-team-icon.png)，然後按一下 **[!UICONTROL 建立新團隊]**.

   ![選擇「建立新團隊」。](assets/create-new-team-350x198.png)

1. 請在 [!UICONTROL 新團隊] 對話框：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL團隊名稱]</strong> </td> 
      <td>輸入新敏捷團隊的名稱。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL這是Agile團隊]</strong> </td> 
      <td>選擇此選項可將此新團隊配置為敏捷團隊。</td> 
     </tr> 
     <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
      <td role="rowheader"><strong>[!UICONTROL組]</strong> </td> 
      <td> <p>開始鍵入要添加到團隊的組名稱，然後在下拉清單中顯示名稱時選擇該名稱。</p> <p>注意：將團隊分配給組或子組時，該組或子組的任何組管理員都可以管理該團隊，而不是其成員。 群組管理員可從[!UICONTROL主菜單]前往[!UICONTROL團隊]區域，然後按一下[!UICONTROL切換團隊]箭頭 <img src="assets/switch-team-icon.png" alt="切換團隊表徵圖"> 列出分配給其管理的組的所有團隊。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL團隊成員]</strong> </td> 
      <td>開始鍵入要在團隊中的用戶的名稱，然後在下拉清單中出現時選擇該名稱。<br>重複此過程以向團隊添加多個用戶。<br>因為使用者可以在多個團隊中，他們可以在敏捷和非敏捷的團隊中。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL描述]</strong> </td> 
      <td><p>輸入團隊的說明。</p> <p>選取團隊時，說明會顯示在[!UICONTROL團隊]區域的右上角。</p>
      <p>如果說明較長，您可以按一下該說明以在快顯視窗中顯示完整說明。 如果您有權編輯[!UICONTROL團隊設定]，也可以直接在快顯視窗中編輯說明。</p></td>
     </tr> 
    </tbody> 
   </table>

1. 按一下 **[!UICONTROL 建立]**。

   如需設定Agile團隊的詳細資訊，請參閱下列文章：

   * [設定 [!UICONTROL 看板]](../../agile/get-started-with-agile-in-workfront/configure-kanban.md)
   * [設定 [!UICONTROL Scrum]](../../agile/get-started-with-agile-in-workfront/configure-scrum.md)

## 將現有團隊轉換為敏捷團隊

您可以將現有團隊轉換為敏捷團隊：

1. 按一下 **[!UICONTROL 主菜單]** 圖示 ![](assets/main-menu-icon.png) 在 [!DNL Adobe Workfront]，然後按一下 **[!UICONTROL 團隊]**.
1. 按一下 **[!UICONTROL 交換組]** 圖示 ![切換團隊表徵圖](assets/switch-team-icon.png)，然後從下拉式選單中選取新團隊，或在搜尋列中搜尋團隊。

1. 選擇要轉換為敏捷團隊的團隊。
1. 按一下 **[!UICONTROL 更多]** ，然後選取 **[!UICONTROL 編輯]**.\
   僅包含 [!UICONTROL 計畫] 或 [!UICONTROL 工作] 許可證請參閱此選項。\
   ![](assets/edit-team-settings-350x205.png)

1. 在 **[!UICONTROL 敏捷]** 部分，選擇 **[!UICONTROL 這是敏捷團隊]**.

1. 在 **[!UICONTROL 方法]** 部分，選擇團隊是否將使用 **[!UICONTROL Scrum]** 或 **[!UICONTROL 看板]** 敏捷的方法。

1. 按一下 **儲存變更。**

   如需設定Agile團隊的詳細資訊，請參閱下列文章：

   * [設定 [!UICONTROL 看板]](../../agile/get-started-with-agile-in-workfront/configure-kanban.md)
   * [設定 [!UICONTROL Scrum]](../../agile/get-started-with-agile-in-workfront/configure-scrum.md)
