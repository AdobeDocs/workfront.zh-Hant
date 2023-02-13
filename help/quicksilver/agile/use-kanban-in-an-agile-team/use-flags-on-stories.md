---
product-area: agile-and-teams;projects
navigation-topic: use-kanban-in-an-agile-team
title: 在看板板上的動態上使用標籤
description: 在 [!DNL Kanban] 展示板，旗標提供動態何時準備好進入下一個狀態的視覺指示。 這使看板團隊在跨狀態移動動態時可以使用「拉」方法，而不是「推」方法。
author: Lisa
feature: Agile
exl-id: e19a007d-737c-42d4-aa69-771d8a9e9fd8
source-git-commit: 33daf0633701a1c271552e796ffe22a58645c561
workflow-type: tm+mt
source-wordcount: '536'
ht-degree: 0%

---

# 在 [!UICONTROL 看板] 展示板

在 [!DNL Kanban] 展示板，旗標提供動態何時準備好進入下一個狀態的視覺指示。 如此可啟用 [!UICONTROL 看板] 團隊可在跨狀態移動動態時使用「提取」方法，而非「推送」方法。

**範例：** 請考量下列使用「提取」方法的團隊範例：團隊中的平面設計師奧利維亞完成了她的工作，然後把故事標籤設定為「[!UICONTROL 準備提取].&quot; 此標幟可以透過視覺方式向團隊中的文案撰寫者Tony指出，故事已準備好讓他進入下一個狀態。 當托尼準備好開始做這件事時，他會把故事移到下一個狀態。

在動態上使用旗標時，請考量下列事項：

* 標幟不是狀態，而是可視的指示，說明該動態已準備好由團隊的其他成員移至下一個狀態。
* 旗標不會出現在 [!UICONTROL 積壓] 欄或 [!UICONTROL 完成] 欄(或列中的任何欄，其中列的狀態與 [!UICONTROL 完成])。

   如需有關動態狀態的詳細資訊，請參閱 [在看板板上的動態上使用標籤](#updating-the-status-of-stories-and-subtasks)

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
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
   <td> <p>[!UICONTROL Worker]或更高版本</p> <p>注意：如果您仍無法存取，請詢問您的 [!DNL Workfront] 管理員。 若要了解 [!DNL Workfront] 管理員可以更改您的訪問級別，請參閱 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的 [!DNL Workfront] 管理員。

## 在 [!UICONTROL 看板] 展示板

要更改文章的標幟：

1. 按一下 **[!UICONTROL 主菜單]** 圖示 ![](assets/main-menu-icon.png) 在 [!DNL Adobe Workfront]，然後按一下 **[!UICONTROL 團隊]**.

1. （選用）按一下 **[!UICONTROL 交換組]** 圖示 ![切換團隊表徵圖](assets/switch-team-icon.png)，然後選取新 [!UICONTROL 看板] 團隊（從下拉式功能表），或在搜尋列中搜尋團隊。

1. 前往 [!UICONTROL 看板] 要更改故事標誌的展示板。
1. 展開「文章」圖磚以檢視旗標。\
   標幟設為 **[!UICONTROL 在軌]** 依預設會針對每個動態。\
   ![看板卡](assets/agile-storycard-kanban-2021-350x308.png)

1. 按一下目前標幟，然後選取下列標幟選項：

   * **[!UICONTROL 在軌]:** 故事處於適當狀態，此時無需採取任何操作。\

      這是看板板上每個歷程的預設標誌。\
      ![kanban_flag_ontrack.png](assets/kanban-flag-ontrack.png)

   * **[!UICONTROL 已阻止]:** 故事無法繼續到下一狀態。 當動態上設定此旗標時，動態不會計入WIP限制。 (如需WIP限制的詳細資訊，請參閱文章 [配置看板](../../agile/get-started-with-agile-in-workfront/configure-kanban.md).\

      ![kanban_flag_blocked.png](assets/kanban-flag-blocked.png)

   * **[!UICONTROL 準備提取]:** 此動態已準備好由團隊的其他成員移至下一個狀態。\

      ![kanban_flag_ready.png](assets/kanban-flag-ready.png)
