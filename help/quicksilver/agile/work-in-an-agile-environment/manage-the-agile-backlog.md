---
product-area: agile-and-teams
navigation-topic: work-in-an-agile-environment
title: 管理敏捷積壓
description: 任務和問題可以指派給敏捷團隊，並根據團隊使用的敏捷方法，以故事形式新增至該團隊的積壓工作中。
author: Lisa
feature: Agile
exl-id: 59660840-7ab8-482e-8b43-96b4a1ecc538
source-git-commit: b855f032b24079ff27435fb833cd3ed8a382a77c
workflow-type: tm+mt
source-wordcount: '1376'
ht-degree: 0%

---

# 管理敏捷積壓

可根據團隊使用的敏捷方法，將下列工作項目指派給敏捷團隊，並以動態形式添加到該團隊的積壓工作中：

* **[!UICONTROL 敏捷戰鬥隊]:** 可將任務和問題指派給敏捷團隊，並新增至積壓工作。
* **[!UICONTROL 看板敏捷團隊]:** 可將任務分配給敏捷團隊，並添加到積壓工作中。 使用者可以直接從敏捷故事板檢視積壓，如 [[!UICONTROL 添加積壓] 看板板](../../agile/use-kanban-in-an-agile-team/view-the-backlog-on-the-kanban-board.md). 該團隊使用此積壓工作來優先處理和管理其工作隊列。

可以從以下位置將任務或問題指派給團隊（並隨後新增至團隊積壓）: [!DNL Adobe Workfront]. 例如，單個團隊可能被從多個項目中分配工作分配。

>[!NOTE]
>
>如果向積壓物料添加多個團隊，則任務或問題僅顯示在主要團隊的積壓上。 主要團隊是先指派的團隊。

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
   <td> <p>[!UICONTROL工作]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>訪問級別配置*</strong></td> 
   <td> <p>[!UICONTROL Worker]或更高版本</p> <p>注意：如果您仍無法存取，請詢問您的 [!DNL Workfront] 管理員。 若要了解 [!DNL Workfront] 管理員可修改您的存取層級，請參閱 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>物件權限</strong></td> 
   <td> <p>[!UICONTROL管理]對文章所在項目的訪問</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的 [!DNL Workfront] 管理員。

## 建立和管理積壓工作的動態

* [重新排序動態](#reorder-stories)
* [[!UICONTROL 插播] 故事](#break-down-stories)
* [編輯動態](#edit-stories)
* [建立關於積壓的新動態](#create-new-stories-on-the-backlog)
* [將物料從積壓移至小版本或看板板](#move-stories-from-the-backlog-to-an-iteration-or-kanban-board)

### 重新排序動態 {#reorder-stories}

您可以使用拖放方法，重新排序積壓清單中的動態。

1. 轉至要重新排序動態的敏捷積壓工作。
1. 在 **[!UICONTROL 檢視]** 下拉式功能表，選取 **[!UICONTROL 積壓]** 檢視或包含 **[!UICONTROL 順序]** 欄。

   >[!NOTE]
   >
   >如果任務或問題已分配一個敏捷的團隊，並且項目的狀態不等於「當前」，則它們不會顯示在積壓工作上。 但是，它們仍會影響「訂單」列中的積壓數量。

1. 選取一或多個動態，然後將動態拖曳至您希望動態在積壓中顯示的順序。\
   ![拖放積壓項目](assets/agile-backlog-drag-and-drop.png)

### 劃分故事 {#break-down-stories}

因為積壓工作中的故事大小不同，所以用戶可以將它們分解為迭代的可操作大小。 分解動態將建立動態所代表的任務的子任務，並替換積壓工作中的原始任務。 您可以將父任務或其子任務分配給敏捷團隊，但不能同時將兩者分配給團隊。

>[!NOTE]
>
>劃分動態時，請考量下列限制：
>
>* 只能劃分代表任務的故事。 您無法劃分代表問題的故事。
>* 只有當動態與專案相關聯時，才能加以劃分。



要分解故事：

1. 轉到包含要分解的故事的積壓。
1. 選取您要劃分的動態，然後按一下 **[!UICONTROL 劃分動態]**.\
   此 [!UICONTROL 劃分動態] 對話框。\
   ![劃分動態對話方塊](assets/backlog-breakdown-dialog.png)

1. 指定動態的名稱和估計，並選取動態是否已就緒。
1. 按一下 **[!UICONTROL 添加動態]** 從原始故事中創作另一個故事。
1. 按一下&#x200B;**[!UICONTROL 儲存]**。

### 編輯動態 {#edit-stories}

您可以直接從 [!UICONTROL 故事] 或 [!UICONTROL 問題] 按一下「積壓」頁簽，即可批量編輯項目中的任何任務或問題，如 [大量編輯任務](../../manage-work/tasks/manage-tasks/edit-tasks.md#editing-tasks-in-bulk) in [編輯任務](../../manage-work/tasks/manage-tasks/edit-tasks.md) 和 [編輯問題](../../manage-work/issues/manage-issues/edit-issues.md#bulk-editing-issues) in [編輯問題](../../manage-work/issues/manage-issues/edit-issues.md).

## 建立關於積壓的新動態 {#create-new-stories-on-the-backlog}

您可以直接從積壓工作中建立積壓工作，或將現有任務或問題指派給敏捷團隊，從而建立積壓工作的新動態。

* [從積壓工作中建立故事](#create-a-story-from-the-backlog)
* [將任務或問題指派給敏捷團隊](#assign-a-task-or-issue-to-an-agile-team)

### 從積壓工作中建立故事 {#create-a-story-from-the-backlog}

當您從積壓工作中建立動態時，該動態將作為任務或項目中的問題建立。 您不能從積壓工作中建立一個問題。

要從積壓工作中建立工作流，請執行以下操作：

1. 按一下 **[!UICONTROL 主菜單]** 圖示 ![](assets/main-menu-icon.png) 在 [!DNL Adobe Workfront]，然後按一下 **[!UICONTROL 團隊]**.

1. （選用）按一下 **[!UICONTROL 交換組]** 圖示 ![切換團隊表徵圖](assets/switch-team-icon.png)，然後從下拉式選單中選取新的Scrum團隊，或在搜尋列中搜尋團隊。

1. 選擇 **[!UICONTROL 積壓]** 從左側面板。
1. 根據您要建立任務還是問題，執行下列任一操作：

   * **要建立任務，請執行以下操作：** 按一下 **[!UICONTROL 故事]**.

   * **建立問題：** 按一下 **[!UICONTROL 問題]**.

1. 按一下 **[!UICONTROL 新動態]** 或 **[!UICONTROL 新問題]**.

1. 指定下列資訊：

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL文章名稱]</strong></td>
      <td> 輸入動態名稱。</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL描述]</strong></td>
      <td>（選用）輸入動態說明。</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL就緒]</strong></td>
      <td> 選擇文章是否準備好添加到小版本。 此設定僅提供資訊。 無論此設定的狀態如何，文章都可以新增至小版本。</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL估計]</strong></td>
      <td>指定動態的點數或每小時預估。 估計值會影響燃耗圖。 只有每個文章包含準確的估計時，迭代的燃耗圖才準確。 （如果您提供點估計值，則必須已在團隊設定中指定每個點代表的小時數。）</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL父項項目]</strong></td>
      <td>開始輸入要建立此動態的專案名稱，然後在下拉式清單中出現時按一下名稱。<br>項目的狀態必須設定為[!UICONTROL當前]。 如果專案的狀態為[!UICONTROL目前]以外的任何值，則下拉式功能表中不會顯示它。</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL父任務]</strong></td>
      <td>（可選）開始鍵入此動態所屬的父任務的名稱，然後在下拉清單中顯示該名稱時按一下該名稱。</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL自訂Forms]</strong></td>
      <td> （選用）選取您要新增至此動態的任何自訂表單。</td>
     </tr>
    </tbody>
   </table>

1. 按一下 **[!UICONTROL 儲存動態]**.

### 將任務或問題指派給敏捷團隊 {#assign-a-task-or-issue-to-an-agile-team}

您可以將任務或問題指派給敏捷團隊。 分配任務或問題後，該任務或問題將以新的動態形式顯示在團隊積壓工作上。

要將任務或問題分配給敏捷團隊，請執行以下操作：

1. 轉到包含要重新分配的任務的項目。
1. 在清單中選擇任務或問題。
1. 按一下 **[!UICONTROL 編輯]**.
1. 按一下 **[!UICONTROL 分配]**.
1. （可選）刪除任何現有受分配者。
1. 按一下 **[!UICONTROL 新增受託人]**.
1. 開始鍵入要分配給任務或問題的敏捷團隊的名稱，然後在下拉清單中出現團隊名稱時按一下該團隊名稱。
1. 按一下 **[!UICONTROL 儲存變更]**.\
   該任務或問題現在可用於團隊積壓。

## 將積壓工作中的動態移到迭代或+展示板 {#move-stories-from-the-backlog-to-an-iteration-or-kanban-board}

* [將現有動態移到積壓工作](#move-existing-stories-to-the-backlog)
* [從積壓中導出故事](#export-stories-from-the-backlog)

1. 去處理敏捷團隊的積壓問題。
1. 選擇要移至小版本或看板板的動態，然後按一下 **[!UICONTROL 更多]** > **[!UICONTROL 移至]**.\
   如果把故事 [!UICONTROL 看板] 董事會， [!UICONTROL 將動態移至看板] 顯示展示板。\
   如果將文章移到迭代，則 [!UICONTROL 將文章移動到迭代] 對話框。\
   ![移動文章對話框](assets/agile-backlog-addtoiteration.png)

1. 執行下列任一操作：

   * **Scrum團隊：** 在 **[!UICONTROL 選擇迭代]** 欄位中，選擇要移動文章的小版本。

   * **看板小組：** 在 **[!UICONTROL 選擇看板板]** 欄位，選取您的團隊 [!UICONTROL 看板] 展示板。 (看板小組只能有一個 [!UICONTROL 看板] 展示板。)

1. 按一下 **[!UICONTROL 移動動態]**.

### 將現有動態移到積壓工作 {#move-existing-stories-to-the-backlog}

如果您決定您的團隊尚未準備好處理動態，您可以將動態移至積壓工作。

如需詳細資訊，請參閱 [敏捷的故事](../../agile/work-in-an-agile-environment/move-an-agile-story.md).

### 從積壓中導出故事 {#export-stories-from-the-backlog}

您可以直接從積壓工作中匯出一或多個動態（包括任務和問題）。

從積壓工作中匯出動態的方式與將其他資料匯出至 [!DNL Workfront]，如 [匯出資料](../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md).
