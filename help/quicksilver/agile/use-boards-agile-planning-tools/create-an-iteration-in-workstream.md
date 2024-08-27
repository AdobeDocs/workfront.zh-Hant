---
content-type: reference
product-area: agile-and-teams
navigation-topic: boards
title: 在工作串流中建立反複專案
description: 反複專案是完成工作所保留的時間設定。 某些敏捷團隊可能會將反複專案稱為衝刺。
author: Lisa
feature: Agile
exl-id: 37b8810d-8439-4a7a-89d5-7c2560422ace
source-git-commit: df4c2a73b5eb2498564bbf27aa92a297388562cd
workflow-type: tm+mt
source-wordcount: '412'
ht-degree: 0%

---

# 在工作串流中建立反複專案

>[!IMPORTANT]
>
>工作串流僅適用於特定客戶群組。

反複專案是完成工作所保留的時間設定。 某些敏捷團隊可能會將反複專案稱為衝刺。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront]</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權</td> 
   <td> 
   <p>新增：[！UICONTROL Contributor]或以上</p> 
   <p>或</p>
   <p>目前： [！UICONTROL Request]或以上</p>
   </td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 在工作串流中建立反複專案

{{step1-to-boards}}

1. 開啟您要新增反複專案的工作流。 若要開啟工作流程，請按一下[檢視工作流程]。[!UICONTROL ****]
1. 使用下列其中一種方法建立反複專案：

   * 在[卡片清單]索引標籤上的反複專案檢視中，按一下[建立反複專案]。[!UICONTROL ****]
   * 在[卡片清單]索引標籤上，按一下[清單檢視]中的[建立反複專案]。[!UICONTROL ****]
   * 在[展示板]索引標籤上，按一下[新增展示板&#x200B;**]]並選取[反複專案程式][!UICONTROL **&#x200B;做為展示板範本。 [!UICONTROL ****]&#x200B;然後，開啟反複專案板並按一下&#x200B;[!UICONTROL **設定反複專案**]。

1. 在「版序詳細資訊」對話方塊中，新增下列資訊：

   <table style="table-layout:auto"> 
    <tbody> 
     <tr> 
      <td><strong>[！UICONTROL反複專案名稱]</strong></td> 
      <td>反複運算的名稱，例如「Sprint 1」。</td> 
     </tr> 
     <tr> 
      <td><strong>[！UICONTROL反複專案長度]</strong></td> 
      <td>反複專案長度，以天、周或月為單位。</td> 
     </tr>
     <tr> 
      <td><strong>[！UICONTROL開始日期]</strong></td> 
      <td>反複專案開始的日期。 系統會根據反複專案長度自動輸入結束日期。</td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下「[!UICONTROL **儲存**]」。

   反複專案現在會出現在卡片清單的反複專案檢視中，以及反複專案板上的量度區域中。

   若要將卡片新增至反複專案，請參閱[使用卡片清單](/help/quicksilver/agile/use-boards-agile-planning-tools/use-card-list.md)。

## 編輯現有反複專案

1. 若要開啟工作流程，請按一下[檢視工作流程]。[!UICONTROL ****]
1. 使用下列其中一種方法開啟反複專案：

   * 在[卡片清單]索引標籤上的反複專案檢視中，按一下&#x200B;[!UICONTROL **反複專案詳細資料**]&#x200B;圖示![反複專案詳細資料](assets/iteration-details-button.png)。
   * 在反複專案展示板上，按一下右上角量度區域中的&#x200B;[!UICONTROL **反複專案詳細資料**]&#x200B;圖示![反複專案詳細資料](assets/iteration-details-button.png)。

1. 在[!UICONTROL 反複專案組態]面板中，視需要編輯反複專案。
1. 若要變更反複專案名稱，請展開&#x200B;[!UICONTROL **反複專案詳細資料**]。

   反複專案開始後，您只能變更反複專案名稱，不能變更日期或反複專案長度。

<!--   

1. <span class="preview">To add goals to the iteration, expand [!UICONTROL **Goals**].</span>
1. <span class="preview">Click [!UICONTROL **Add goal**], and type the goal name.</span>

   <span class="preview">As goals are completed during the iteration, you can select the check box to mark them complete, or click the **Delete** icon ![Delete icon](assets/delete.png) to delete a goal. The metrics area on the top right of the iteration shows how many goals exist and how many have been completed.</span>

<div class="preview">

## Assign cards to the next iteration

Use the [!UICONTROL Next Iteration] column to move cards from the current iteration to the next iteration, without sending them to the backlog first.

1. Move a card to the [!UICONTROL **Next Iteration**] column, or add a new card directly in the column.
1. Access the next iteration by clicking the [!UICONTROL **Next Iteration**] column title, or by clicking the up-pointing arrow next to the iteration name on the top of the screen.

   The cards that you marked to come over to the next iteration are placed in the columns that correspond with their status.

</div>
-->

## 刪除反複專案

1. 按一下工作流程上的&#x200B;[!UICONTROL **卡片清單**]&#x200B;索引標籤，然後開啟反複專案檢視。
1. 按一下反複專案旁的&#x200B;**刪除**&#x200B;圖示![刪除圖示](assets/delete.png)。
1. 按一下確認訊息上的&#x200B;[!UICONTROL **刪除反複專案**]。
