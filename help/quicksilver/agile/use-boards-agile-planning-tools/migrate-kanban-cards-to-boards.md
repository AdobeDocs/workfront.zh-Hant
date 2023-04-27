---
content-type: reference
navigation-topic: boards
title: 將敏捷團隊看板卡遷移至Workfront展示板
description: 您可以將工作項從敏捷的小組看板板遷移到新的或現有的Workfront看板。
author: Lisa
exl-id: c40b6453-5869-437b-a1e0-f20dd833d2b8
source-git-commit: f6bee61bbfbac98595d737fa002bbe01c0c573dc
workflow-type: tm+mt
source-wordcount: '375'
ht-degree: 0%

---

# 將敏捷團隊看板卡遷移至Workfront展示板

您可以將工作項從敏捷的小組看板板遷移到新的或現有的Workfront看板。 運行遷移時，看板板上的所有卡都將複製到Workfront板。 您無法選擇特定卡片。

在Workfront展示板上放置資訊卡是根據欄政策。 (例如，策略可將狀態為「正在進行」的所有卡移至特定欄。 有關列策略的詳細資訊，請參見 [管理展示板欄](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md).) 如果沒有策略，或者卡與策略不匹配，則這些卡會放在展示板上最左邊的列中。 目前，舊版展示板上「積壓」欄中的資訊卡不會新增至Workfront展示板。

卡不會從敏捷的小組看板板中刪除，並且卡狀態更改將同步到兩個看板。 您可以讓兩個展示板保持作用中，直到您準備好切換至Workfront展示板為止。

>[!NOTE]
>
>只有透過Workfront展示板的早期功能選擇，才能使用此功能。

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

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的 [!DNL Workfront] 管理員。

## 將看板卡遷移到新板

{{step1-to-team}}

1. 訪問看板板。
1. 按一下 [!UICONTROL **新增至展示板**] 選取 [!UICONTROL **新展示板**].
1. 在 [!UICONTROL 添加到新展示板] 對話框，鍵入新展示板的名稱(當前的名稱 [!UICONTROL 看板] 展示板)，然後按一下 [!UICONTROL **新增**].

   ![將看板卡添加到新板](assets/add-kanban-cards-to-new-board-dialog.png)

1. （選用）在顯示的成功訊息上，按一下連結以開啟新展示板。

## 將看板卡遷移到現有看板板

{{step1-to-team}}

1. 訪問看板板。
1. 按一下 [!UICONTROL **新增至展示板**] 選取 [!UICONTROL **現有主板**].
1. 在 [!UICONTROL 添加到現有展示板] 對話方塊，搜尋並選取要移轉資訊卡的展示板。 然後，按一下 [!UICONTROL **新增**].

   ![將看板卡添加到現有看板](assets/add-kanban-cards-to-existing-board-dialog.png)

1. （選用）在顯示的成功訊息上，按一下連結以開啟展示板。
