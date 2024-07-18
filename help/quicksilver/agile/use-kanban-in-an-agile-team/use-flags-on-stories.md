---
product-area: agile-and-teams;projects
navigation-topic: use-kanban-in-an-agile-team
title: 在Kanban展示板上的劇本上使用旗標
description: 在 [!DNL Kanban] 展示板上，旗標提供內文準備移至下一個狀態的視覺指示。 這可讓Kanban團隊在跨狀態移動故事時使用「提取」方法，而非「推送」方法。
author: Lisa
feature: Agile
exl-id: e19a007d-737c-42d4-aa69-771d8a9e9fd8
source-git-commit: 33daf0633701a1c271552e796ffe22a58645c561
workflow-type: tm+mt
source-wordcount: '530'
ht-degree: 0%

---

# 在[!UICONTROL Kanban]展示板上的劇本上使用旗標

在[!DNL Kanban]展示板上，旗標可提供劇本何時準備好移至下一個狀態的視覺指示。 這可讓[!UICONTROL Kanban]團隊在跨狀態移動劇本時，使用「提取」方法，而非「推送」方法。

**範例：**&#x200B;考慮下列使用「提取」方法的團隊範例：團隊的平面設計師Olivia完成工作，然後將劇本旗標設為&quot;[!UICONTROL 準備提取]&quot;。 這個旗標可為Tony （團隊的文案撰稿人）提供視覺化提示，表示該故事已準備好讓他進入下一個狀態。 然後Tony準備開始製作時，將故事移至下一個狀態。

在內文上使用標幟時，請考量下列事項：

* 旗標不是狀態，而是劇本已準備好由團隊其他成員移動到下一個狀態的視覺指示。
* 旗標不會出現在[!UICONTROL 待處理專案]資料行或[!UICONTROL 完成]資料行中的任何內文卡片上（或資料行狀態等於[!UICONTROL 完成]的任何資料行中）。

  如需內文狀態的詳細資訊，請參閱[在Kanban面板上的內文上使用旗標](#updating-the-status-of-stories-and-subtasks)

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 計畫*</strong></td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 授權*</strong></td> 
   <td> <p>[！UICONTROL Work]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>存取層級設定*</strong></td> 
   <td> <p>[！UICONTROL Worker]或更高版本</p> <p>注意：如果您還是沒有存取權，請詢問您的[!DNL Workfront]管理員是否對您的存取層級設定了其他限制。 如需[!DNL Workfront]管理員如何變更您的存取層級的詳細資訊，請參閱<a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的[!DNL Workfront]管理員。

## 在[!UICONTROL Kanban]展示板上的劇本上使用旗標

若要變更劇本上的旗標：

1. 按一下[!DNL Adobe Workfront]右上角的&#x200B;**[!UICONTROL 主要功能表]**&#x200B;圖示![](assets/main-menu-icon.png)，然後按一下&#x200B;**[!UICONTROL 團隊]**。

1. （選擇性）按一下&#x200B;**[!UICONTROL 切換團隊]**&#x200B;圖示![切換團隊圖示](assets/switch-team-icon.png)，然後從下拉式選單中選取新的[!UICONTROL Kanban]團隊，或在搜尋列中搜尋團隊。

1. 前往您想要變更劇本旗標的[!UICONTROL Kanban]面板。
1. 展開內文拼貼以檢視旗標。\
   每個內文的旗標預設為&#x200B;**[!UICONTROL 曲目]**。\
   ![看板卡](assets/agile-storycard-kanban-2021-350x308.png)

1. 按一下目前的旗標，然後從下列旗標選項中選取：

   * **[!UICONTROL 播放軌]：**&#x200B;劇本處於適當的狀態，目前不需要採取任何動作。\

     這是Kanban板上每個內文的預設標幟。\
      ![kanban_flag_ontrack.png](assets/kanban-flag-ontrack.png)

   * **[!UICONTROL 已封鎖]：**&#x200B;該劇本無法繼續進入下一個狀態。 當在劇本上設定此旗標時，該劇本不會計入WIP限制中。 (如需WIP限制的詳細資訊，請參閱文章[設定Kanban](../../agile/get-started-with-agile-in-workfront/configure-kanban.md)。\

     ![kanban_flag_blocked.png](assets/kanban-flag-blocked.png)

   * **[!UICONTROL 準備提取]：**&#x200B;劇本已準備好由團隊的其他成員移至下一個狀態。\

     ![kanban_flag_ready.png](assets/kanban-flag-ready.png)
