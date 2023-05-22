---
content-type: reference
product-area: agile-and-teams
navigation-topic: boards
title: 管理工作流
description: 工作流是一組可配置的用於協作工作的主板和卡。
author: Lisa
feature: Agile
exl-id: c46c42e8-e14d-414d-b883-c4d885338e42
source-git-commit: 14175ce94c1395138a31f47ad72951f0120f11ee
workflow-type: tm+mt
source-wordcount: '853'
ht-degree: 3%

---

# 管理工作流

工作流是一組可配置的用於協作工作的主板和卡。 工作流可以包括根據模板建立的不同類型的主板和工作項目的卡片清單。 在工作流中，可以跟蹤小版本或短點中的工作。

有關詳細資訊，請參見 [使用卡清單](/help/quicksilver/agile/use-boards-agile-planning-tools/use-card-list.md) 和 [在工作流中建立小版本](/help/quicksilver/agile/use-boards-agile-planning-tools/create-an-iteration-in-workstream.md)。

工作流與您有權訪問的不屬於工作流的各個主板一起出現在儀表板上。 有關主板控制板的資訊，請參見 [使用主板儀表板](/help/quicksilver/agile/get-started-with-boards/use-boards-page.md)。 可按一下操控板上的任何板名以將其開啟。

## 訪問要求

您必須具有以下訪問權限才能執行本文中的步驟：

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
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 許可證*</strong></td> 
   <td> <p>[!UICONTROL請求]或更高版本</p> </td> 
  </tr> 
 </tbody> 
</table>

## 建立工作流

{{step1-to-boards}}

1. 按一下 **[!UICONTROL 添加工作流]** 的 [!UICONTROL 工作流] 的子菜單。
1. 鍵入要替換的名稱 **[!UICONTROL 無標題工作流]** 按Enter鍵。

   可將主板添加到工作流中，或按一下 [!UICONTROL **所有主板**] 的子菜單。

## 在工作流中建立新板

1. 如果尚未在工作流中，請按一下 [!UICONTROL **查看工作流**] 開啟現有工作流。
1. 按一下 **[!UICONTROL 添加板]** 的 [!UICONTROL 主板] 的子菜單。
1. 為主板選擇模板。

| 範本 | 說明 |
|---------|----------|
| 基本展示板 | 板上提供三個預設列。 可以添加新列，並更名或刪除預設列。 <p>未應用列策略。 |
| Kanban 展示板 | 主板上提供以下欄目：積壓、新建、正在執行、完成和暫掛。 可以添加新列，並更名或刪除預設列。<p>要使用積壓工作，必須設定進氣列的篩選器。 有關資訊，請參見 [向主板添加進氣柱](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md)。 <p>要查看每列的預設策略，請按一下 [!UICONTROL **更多** 菜單] 在列上選擇 [!UICONTROL **編輯**]。 您可以更改這些預設策略中的任何一個。 有關資訊，請參見 [管理板列](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md)。 |
| 追溯展示板 | 主板上提供以下欄目：什麼進展順利？ 有哪些可以改進的地方? 我們應該為誰慶祝? 我們可以做些什麼來加快進度? 可以添加新列，並更名或刪除預設列。 <p>未應用列策略。 |
| 疊代程序 | 這是用於定義和運行迭代的板。 <p>主板上提供以下欄目：積壓、新建、正在執行、完成和暫掛。 不能將任何列添加到主板。 <p>要查看每列的預設策略，請按一下 [!UICONTROL **更多**] 菜單，然後選擇 [!UICONTROL **編輯**]。 您可以更改這些預設策略中的任何一個。 有關資訊，請參見 [管理板列](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md)。 |

有關設定主板的詳細資訊，請參閱 [建立或編輯電路板](/help/quicksilver/agile/get-started-with-boards/create-edit-board.md)。

## 篩選工作流上的主板清單

當將除預設值之外的濾鏡應用到主板清單時，在濾鏡表徵圖上顯示一個指示器 ![已應用篩選器](assets/boards-filterapplied-30x30.png)。 按一下 [!UICONTROL **全部清除**] 刪除所有濾鏡，然後按一下 [!UICONTROL **隱藏篩選器**] 按鈕。

{{step1-to-boards}}

1. 在儀表板上，按一下 [!UICONTROL **查看工作流**] 開啟工作流。
1. 按一下 [!UICONTROL **主板**] 的子菜單。
1. 按一下 [!UICONTROL **篩選**]。
1. 選擇要按狀態查看的主板（存檔的主板、活動的主板或所有主板）。
1. 選擇要按模板查看的主板。

## 將成員添加到工作流

在查看工作流及其內容之前，必須將人員和團隊作為成員添加到工作流中。 工作流成員可以添加和刪除工作流上的成員，並查看工作流中的哪些主板。

>[!NOTE]
>
>工作流成員在作為成員添加到該特定板之前無法開啟工作流上的板。

{{step1-to-boards}}

1. 在儀表板上，按一下 [!UICONTROL **查看工作流**] 開啟工作流。
1. 按一下 **[!UICONTROL 添加成員]** 表徵圖 ![添加成員](assets/boards-addmember-spectrum-25x25.png) 將成員和團隊添加到工作流。

   這與向主板添加成員的過程相同。 有關詳細資訊，請參見 [添加或從主板中刪除成員](/help/quicksilver/agile/get-started-with-boards/add-members-to-board.md)。

## 配置工作流

{{step1-to-boards}}

1. 在儀表板上，按一下 [!UICONTROL **查看工作流**] 開啟工作流。
1. 按一下 [!UICONTROL **配置**] 開啟 [!UICONTROL 配置工作流] 的子菜單。
1. （可選）鍵入工作流的說明。 此說明顯示在儀表板上。
1. （可選）向工作流添加標籤。 有關詳細資訊，請參見 [添加標籤](/help/quicksilver/agile/get-started-with-boards/add-tags.md)。

   「卡清單」部分顯示的卡總數、指向的卡數和迭代次數。 按一下 [!UICONTROL **查看清單**] 開啟清單並添加卡片。 有關詳細資訊，請參見 [使用卡清單](/help/quicksilver/agile/use-boards-agile-planning-tools/use-card-list.md)。

   如果已定義小版本，則顯示其開始日期、卡數和點數。 按一下 [!UICONTROL **查看迭代板**] 來開啟板子。 有關詳細資訊，請參見 [在工作流中建立小版本](/help/quicksilver/agile/use-boards-agile-planning-tools/create-an-iteration-in-workstream.md)。

1. 按一下 [!UICONTROL **添加源**] 定義將卡導入工作流的源。 此時，唯一可用的源是 [!DNL Adobe Workfront]。
1. 添加篩選器以將任務和問題作為卡從Workfront導入。

   為工作流源添加篩選器與在基本面板或看板面板上為入口列添加篩選器相同。 有關詳細資訊，請參見 [向主板添加進氣柱](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md)。
