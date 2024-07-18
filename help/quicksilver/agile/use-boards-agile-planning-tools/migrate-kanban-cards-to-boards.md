---
content-type: reference
navigation-topic: boards
title: 將敏捷團隊Kanban卡片移轉至Workfront展示板
description: 您可以將工作專案從敏捷團隊Kanban展示板移轉到新的或現有的Workfront展示板。
author: Lisa
feature: Agile
exl-id: 72e3902b-af9a-497c-817f-63630c4fb73b
source-git-commit: abb021a6857f8016d4f8b6bcf99fe818e47faea6
workflow-type: tm+mt
source-wordcount: '362'
ht-degree: 0%

---

# 將敏捷團隊Kanban卡片移轉至Workfront展示板

您可以將工作專案從敏捷團隊Kanban展示板移轉到新的或現有的Workfront展示板。 當您執行移轉時，Kanban展示板上的所有卡片都會複製到Workfront展示板。 您不得選擇特定卡片。

卡片在Workfront展示板上的放置是根據欄原則。 (例如，原則可將所有狀態為「進行中」的卡片移至特定欄。 如需資料行原則的詳細資訊，請參閱[管理面板資料行](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md)。 如果沒有原則或卡片不符合原則，卡片會放置在展示板最左側的欄。 目前，舊版展示板上「待處理專案」欄中的卡片未新增至Workfront展示板。

卡片不會從敏捷團隊Kanban面板中移除，卡片狀態變更將同步到兩個面板。 在準備切換至Workfront主機板之前，您可以讓兩個主機板都保持作用中。

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
  <tr>
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 計畫*</strong></td>
   <td> <p>任何</p> </td>
  </tr>
  <tr>
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 授權*</strong></td>
   <td> <p>[！UICONTROL Request]或更高版本</p> </td>
  </tr>
 </tbody>
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的[!DNL Workfront]管理員。

## 將Kanban卡片移轉至新面板

{{step1-to-team}}

1. 存取Kanban面板。
1. 按一下「[!UICONTROL **加入展示板**]」並選取「[!UICONTROL **新增展示板**]」。
1. 在[!UICONTROL 新增到新面板]對話方塊上，輸入新面板的名稱（會自動顯示目前[!UICONTROL Kanban]面板的名稱），然後按一下&#x200B;[!UICONTROL **新增**]。

   ![新增Kanban卡片至新展示板](assets/add-kanban-cards-to-new-board-dialog.png)

1. （選擇性）在出現的成功訊息上，按一下連結以開啟新展示板。

## 將Kanban卡片移轉至現有展示板

{{step1-to-team}}

1. 存取Kanban面板。
1. 按一下「[!UICONTROL **加入展示板**]」並選取「[!UICONTROL **現有展示板**]」。
1. 在[!UICONTROL 新增到現有展示板]對話方塊上，搜尋並選取要移轉卡片的目標展示板。 然後，按一下&#x200B;[!UICONTROL **新增**]。

   ![將Kanban卡片新增至現有展示板](assets/add-kanban-cards-to-existing-board-dialog.png)

1. （選用）在顯示的成功訊息上，按一下連結以開啟展示板。
