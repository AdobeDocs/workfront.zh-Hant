---
content-type: reference
product-area: agile-and-teams
navigation-topic: boards
title: 管理工作流
description: 工作流是一組可配置的展示板和卡片，用於協作工作。
author: Lisa
feature: Agile
source-git-commit: 16e96d55932116cb475eecbe8b6ebfd4661eb494
workflow-type: tm+mt
source-wordcount: '862'
ht-degree: 2%

---

# 管理工作流

{{highlighted-preview}}

>[!NOTE]
>
>您可以透過預先選擇加入的功能，在預覽環境和生產環境中使用工作流 [!UICONTROL [!DNL Workfront] 展示板]. 如需詳細資訊，請參閱 [搶先選擇加入Adobe Workfront展示板的功能](/help/quicksilver/agile/get-started-with-boards/boards-early-feature-opt-in.md).

工作流是一組可配置的展示板和卡片，用於協作工作。 工作流可包含從範本、 <span class="preview">和工作品的卡片清單。 在工作流中，您可以跟蹤小版本或sprint中的工作。</span>

<span class="preview">如需詳細資訊，請參閱 [使用卡片清單](/help/quicksilver/agile/use-boards-agile-planning-tools/use-card-list.md) 和 [建立小版本](/help/quicksilver/agile/use-boards-agile-planning-tools/create-an-iteration.md).</span>

工作流程會連同您可存取但不屬於工作流程的個別展示板一起顯示在控制面板上。 如需展示板控制面板的相關資訊，請參閱 [使用展示板控制面板](/help/quicksilver/agile/get-started-with-boards/use-boards-page.md). 您可以按一下控制面板上的任何展示板名稱以開啟它。

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
   <td> <p>[!UICONTROL Request]或更高版本</p> </td> 
  </tr> 
 </tbody> 
</table>

## 建立工作流

{{step1-to-boards}}

1. 按一下 **[!UICONTROL 新增工作流]** 在 [!UICONTROL 工作流] 的子文檔。
1. 輸入要替換的名稱 **[!UICONTROL 無標題工作流]** 按Enter鍵。

   您可以將展示板新增至工作流，或按一下 [!UICONTROL **所有展示板**] 返回控制面板。

## 在工作流中建立新展示板

1. 如果您尚未進入工作流，請按一下 [!UICONTROL **檢視工作流**] 開啟現有工作流。
1. 按一下 **[!UICONTROL 新增展示板]** 在 [!UICONTROL 展示板] 頁簽。
1. 為展示板選取範本。

| 範本 | 說明 |
|---------|----------|
| 基本展示板 | 展示板上提供三個預設欄。 您可以新增欄，並重新命名或刪除預設欄。 <p>未應用列策略。 |
| Kanban 展示板 | 展示板上提供下列欄：積壓、新建、正在進行、完成和暫掛。 您可以新增欄，並重新命名或刪除預設欄。<p>要使用積壓，必須為進氣列設定篩選器。 如需詳細資訊，請參閱 [向展示板新增進紙欄](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md). <p>要查看每列的預設策略，請按一下 [!UICONTROL **更多** 功能表] 在欄上選取 [!UICONTROL **編輯**]. 您可以變更任何這些預先設定的原則。 如需詳細資訊，請參閱 [管理展示板欄](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md). |
| 追溯展示板 | 展示板上提供下列欄：什麼進展順利？ 有哪些可以改進的地方? 我們應該為誰慶祝? 我們可以做些什麼來加快進度? 您可以新增欄，並重新命名或刪除預設欄。 <p>未應用列策略。 |
| <span class="preview">迭代過程</span> | <span class="preview">這是用於定義和運行迭代的板。 <p>展示板上提供下列欄：積壓、新建、正在進行、完成和暫掛。 您無法將任何欄新增至展示板。 <p>要查看每列的預設策略，請按一下 [!UICONTROL **更多**] 選單，然後選取 [!UICONTROL **編輯**]. 您可以變更任何這些預先設定的原則。 如需詳細資訊，請參閱 [管理展示板欄](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md).</span> |

如需設定展示板的詳細資訊，請參閱 [建立或編輯展示板](/help/quicksilver/agile/get-started-with-boards/create-edit-board.md).

## 篩選工作流上的展示板清單

當在展示板清單上套用預設值以外的篩選時，篩選圖示上會顯示指標 ![已套用篩選](assets/boards-filterapplied-30x30.png). 按一下 [!UICONTROL **全部清除**] 移除所有篩選器，然後按一下 [!UICONTROL **隱藏篩選器**] 來關閉篩選面板。

{{step1-to-boards}}

1. 在控制面板上，按一下 [!UICONTROL **檢視工作流**] 來開啟工作流。
1. 按一下 [!UICONTROL **展示板**] 標籤。
1. 按一下 [!UICONTROL **篩選**].
1. 依狀態（封存的展示板、使用中展示板或所有展示板）選取您要查看的展示板。
1. 依範本選取您要檢視的展示板。

## 將成員添加到工作流

必須將人員和團隊新增為工作流成員，才能檢視工作流及其內容。 工作流成員可以添加和移除工作流上的成員，並查看工作流中的哪些板。

>[!NOTE]
>
>工作流成員作為成員添加到該特定板之前無法開啟工作流上的板。

{{step1-to-boards}}

1. 在控制面板上，按一下 [!UICONTROL **檢視工作流**] 來開啟工作流。
1. 按一下 **[!UICONTROL 添加成員]** 圖示 ![添加成員](assets/boards-addmember-spectrum-25x25.png) 將成員和團隊添加到工作流。

   這是將成員新增至展示板的程式。 如需詳細資訊，請參閱 [從展示板新增或移除成員](/help/quicksilver/agile/get-started-with-boards/add-members-to-board.md).

<div class="preview">

## 設定工作流

{{step1-to-boards}}

1. 在控制面板上，按一下 [!UICONTROL **檢視工作流**] 來開啟工作流。
1. 按一下 [!UICONTROL **設定**] 開啟 [!UICONTROL 設定工作流] 中。
1. （選用）輸入工作流的說明。 此說明會顯示在控制面板上。

   「卡片清單」區段中會顯示卡片總數、指向的卡片數和迭代次數。 按一下 [!UICONTROL **檢視清單**] 以開啟清單並新增卡片。 如需詳細資訊，請參閱 [使用卡片清單](/help/quicksilver/agile/use-boards-agile-planning-tools/use-card-list.md).

   如果已定義小版本，則會顯示其開始日期、卡片數和點數。 按一下 [!UICONTROL **查看迭代板**] 來開啟展示板。 如需詳細資訊，請參閱 [建立小版本](/help/quicksilver/agile/use-boards-agile-planning-tools/create-an-iteration.md).

1. 按一下 [!UICONTROL **添加源**] 定義將卡導入工作流的源。 此時，唯一可用的來源為 [!DNL Adobe Workfront].
1. 新增篩選器以從Workfront匯入工作和問題，做為卡片。

   添加工作流源的篩選器與添加基本板或看板板上進料列的篩選器相同。 如需詳細資訊，請參閱 [向展示板新增進紙欄](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md).

</div>
