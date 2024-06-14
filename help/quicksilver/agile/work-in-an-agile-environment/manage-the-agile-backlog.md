---
product-area: agile-and-teams
navigation-topic: work-in-an-agile-environment
title: 管理敏捷待處理專案
description: 任務和問題可以指派給敏捷團隊，並根據團隊使用的敏捷方法以該團隊的待辦專案為單位新增。
author: Lisa
feature: Agile
exl-id: 59660840-7ab8-482e-8b43-96b4a1ecc538
source-git-commit: 8769637342ab65f1e627107f7bfb41f9a3f61cca
workflow-type: tm+mt
source-wordcount: '1371'
ht-degree: 0%

---

# 管理敏捷待處理專案

以下工作專案可指派給敏捷團隊，並根據團隊使用的敏捷方法，以劇本形式新增到該團隊的待辦專案中：

* **[!UICONTROL Scrum敏捷團隊]：** 可以將任務和問題指派給敏捷團隊並新增到待辦專案中。
* **[!UICONTROL Kanban敏捷團隊]：** 任務可以指派給敏捷團隊並新增到待辦專案中。 使用者可以直接從敏捷故事板檢視待處理專案，如所述 [[!UICONTROL 新增待處理專案] 至Kanban面板](../../agile/use-kanban-in-an-agile-team/view-the-backlog-on-the-kanban-board.md). 團隊使用此待處理專案來排定優先順序並管理其工作佇列。

任務或問題可以從中的任何位置指派給團隊（並隨後新增到團隊待辦專案中）。 [!DNL Adobe Workfront]. 例如，一個團隊可能被指派來自多個專案的工作指派。

>[!NOTE]
>
>如果您將多個團隊新增至待處理專案，則任務或問題僅會顯示在主要團隊的待處理專案中。 主要團隊是先指派的團隊。

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
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 計劃</strong></td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 授權</strong></td> 
   <td> <p>新增：[！UICONTROL Standard]</p><p>或</p><p>目前： [！UICONTROL Work]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>存取層級設定</strong></td> 
   <td> <p>新增：[！UICONTROL Standard]</p><p>或</p><p>目前： [！UICONTROL Worker]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>物件許可權</strong></td> 
   <td> <p>[！UICONTROL Manage]內文所在專案的存取權</p>  </td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱 [Workfront檔案中的存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## 建立和管理待處理專案上的劇本

* [重新排序劇本](#reorder-stories)
* [[!UICONTROL 劃分] 劇本](#break-down-stories)
* [編輯劇本](#edit-stories)

### 重新排序劇本 {#reorder-stories}

您可以使用拖放方式，重新排序待處理專案清單中的劇本。

1. 前往您要重新排序劇本的敏捷待辦專案。
1. 在 **[!UICONTROL 檢視]** 下拉式功能表，選取 **[!UICONTROL 待處理專案]** 檢視或包含 **[!UICONTROL 訂購]** 欄。

   >[!NOTE]
   >
   >如果任務或問題指派給敏捷團隊，且專案未處於等於目前狀態，則它們不會顯示在待辦專案中。 不過，它們仍會影響「訂單」欄中的待處理專案計數。

1. 選取一或多個劇本，然後將這些劇本拖曳到您要它們顯示在待處理專案中的順序。\
   ![拖放待處理專案](assets/agile-backlog-drag-and-drop.png)

### 劃分劇本 {#break-down-stories}

由於待處理專案中的內文大小不一，因此使用者可以將內文細分為可供反複專案使用的大小。 分解內文會在內文所代表的任務上建立子任務，並取代待處理專案中的原始任務。 您可以將父項任務或其子任務指派給敏捷專案團隊，但您不能將兩者同時指派給專案團隊。

>[!NOTE]
>
>劃分本文時，請考量下列限制：
>
>* 只能劃分代表任務的劇本。 您無法劃分代表問題的劇本。
>* 內文必須與專案相關聯時，才能加以劃分。


若要劃分劇本，請執行下列動作：

1. 移至包含您要劃分之劇本的待處理專案。
1. 選取您要劃分的內文，然後按一下 **[!UICONTROL 分解劇本]**.\
   此 [!UICONTROL 分解劇本] 對話方塊隨即顯示。\
   ![分解內文對話方塊](assets/backlog-breakdown-dialog.png)

1. 指定內文的名稱和預估，然後選取內文是否準備就緒。
1. 按一下 **[!UICONTROL 新增劇本]** 從原始劇本建立另一個劇本。
1. 按一下「**[!UICONTROL 儲存]**」。

### 編輯劇本 {#edit-stories}

您可以直接從編輯劇本 [!UICONTROL 劇本] 或 [!UICONTROL 問題] 如要大量編輯專案中的任何任務或問題，位於待處理專案索引標籤上，如所述 [大量編輯任務](../../manage-work/tasks/manage-tasks/edit-tasks.md#edit-tasks-in-bulk) 在 [編輯任務](../../manage-work/tasks/manage-tasks/edit-tasks.md)、和 [編輯問題](../../manage-work/issues/manage-issues/edit-issues.md).

## 在待處理專案上建立新劇本 {#create-new-stories-on-the-backlog}

您可以直接從待處理專案建立內文，或將現有任務或問題指派給敏捷團隊，來建立待處理專案上的新內文。

* [從待處理專案建立劇本](#create-a-story-from-the-backlog)
* [將任務或問題指派給敏捷團隊](#assign-a-task-or-issue-to-an-agile-team)

### 從待處理專案建立劇本 {#create-a-story-from-the-backlog}

當您從待處理專案建立內文時，內文會建立為專案內的任務或問題。 您無法從待處理專案中將劇本建立為問題。

若要從待處理專案建立劇本，請執行下列動作：

1. 按一下 **[!UICONTROL 主要功能表]** 圖示 ![主要功能表](/help/_includes/assets/main-menu-icon.png) 在Adobe Workfront的右上角，或（如果有的話）按一下 **[!UICONTROL 主要功能表]** 圖示 ![主要功能表](/help/_includes/assets/main-menu-icon-left-nav.png) 然後按一下「 」 **[!UICONTROL 團隊]**.

1. （可選）按一下 **[!UICONTROL 切換群組]** 圖示 ![切換群組圖示](assets/switch-team-icon.png)，然後從下拉式選單中選取新的Scrum團隊，或在搜尋列中搜尋團隊，並在團隊出現時加以選取。

1. 選取 **[!UICONTROL 待處理專案]** 從左側面板。
1. 根據您想要建立任務還是問題，執行下列任一操作：

   * **若要建立任務：** 按一下 **[!UICONTROL 劇本]**.

   * **若要建立問題：** 按一下 **[!UICONTROL 問題]**.

1. 按一下 **[!UICONTROL 新增劇本]** 或 **[!UICONTROL 新問題]**.

1. 指定下列資訊：

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>[！UICONTROL劇本名稱]</strong></td>
      <td> 輸入劇本的名稱。</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[！UICONTROL說明]</strong></td>
      <td>（選擇性）輸入劇本的說明。</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[！UICONTROL就緒]</strong></td>
      <td> 選取內文是否準備好新增至反複專案。 此設定僅供參考。 無論此設定的狀態為何，內文都可以新增至反複專案。</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[！UICONTROL估計]</strong></td>
      <td>指定劇本的點數或每小時預估。 預估會影響待執行工作圖表。 只有當每個內文都包含正確的估計時，疊代的待執行工作圖表才會準確。 （如果您提供點數預估，則必須在專案團隊設定中指定每個點代表的時數。）</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[！UICONTROL父專案]</strong></td>
      <td>開始輸入將建立此劇本的專案名稱，然後在名稱出現在下拉式清單中時按一下該名稱。<br>專案狀態必須設定為[！UICONTROL目前]。 如果專案狀態不是[！UICONTROL目前]，則不會顯示在下拉式功能表中。</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[！UICONTROL父系任務]</strong></td>
      <td>（選擇性）開始輸入此內文所屬之父系工作的名稱，然後在名稱出現在下拉式清單中時按一下該名稱。</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[！UICONTROL自訂Forms]</strong></td>
      <td> （選擇性）選取您要新增至本文的任何自訂表格。</td>
     </tr>
    </tbody>
   </table>

1. 按一下 **[!UICONTROL 儲存劇本]**.

### 將任務或問題指派給敏捷團隊 {#assign-a-task-or-issue-to-an-agile-team}

您可以將任務或問題指派給敏捷團隊。 指派後，任務或問題會在團隊待辦專案中顯示為新劇本。

若要將任務或問題指派給敏捷團隊：

1. 移至包含您要指派之任務的專案。
1. 選擇清單中的任務或問題。
1. 按一下 **[!UICONTROL 編輯]**.
1. 按一下 **[!UICONTROL 指定任務]**.
1. （選用）刪除任何現有的受指派人。
1. 按一下 **[!UICONTROL 新增被指定者]**.
1. 開始輸入您要指派給任務或問題的敏捷團隊名稱，然後按一下出現在下拉清單中的團隊名稱。
1. 按一下「**[!UICONTROL 儲存變更]**」。\
   團隊待處理專案現在提供任務或問題。

## 將劇本移入或移出待處理專案

{#move-stories-from-the-backlog-to-an-iteration-or-kanban-board}

* [將內文從待處理專案移至反複專案或+展示板](#move-stories-from-the-backlog-to-an-iteration-or--board)
* [將現有劇本移至待處理專案](#move-existing-stories-to-the-backlog)
* [從待處理專案匯出劇本](#export-stories-from-the-backlog)

### 將內文從待處理專案移至反複專案或+展示板

1. 前往敏捷團隊的待辦專案。
1. 選取您要移至反複專案或Kanban展示板的劇本，然後按一下 **[!UICONTROL 更多]** > **[!UICONTROL 移至]**.\
   如果移動本文至 [!UICONTROL Kanban] 展示板， [!UICONTROL 將劇本移至Kanban] 顯示展示板。\
   如果移動本文至反複專案，則 [!UICONTROL 移動本文至反複專案] 對話方塊隨即顯示。\
   ![移動內文對話方塊](assets/agile-backlog-addtoiteration.png)

1. 執行下列任一項作業：

   * **對於Scrum團隊：** 在 **[!UICONTROL 選取反複專案]** 欄位，選取您要移動內文的疊代。

   * **對於Kanban團隊：** 在 **[!UICONTROL 選取Kanban面板]** 欄位，選取您的團隊 [!UICONTROL Kanban] 展示板。 (Kanban團隊只能有一個 [!UICONTROL Kanban] 展示板。)

1. 按一下 **[!UICONTROL 移動劇本]**.

### 將現有劇本移至待處理專案 {#move-existing-stories-to-the-backlog}

如果您決定您的團隊尚未準備好處理劇本，您可以將劇本移至待處理專案。

如需詳細資訊，請參閱 [移動敏捷劇本](../../agile/work-in-an-agile-environment/move-an-agile-story.md).

### 從待處理專案匯出劇本 {#export-stories-from-the-backlog}

您可以直接從待處理專案匯出一或多個劇本（包括任務和問題）。

從待處理專案匯出劇本的方式與匯出其他資料的方式相同 [!DNL Workfront]，如所述 [匯出資料](../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md).
