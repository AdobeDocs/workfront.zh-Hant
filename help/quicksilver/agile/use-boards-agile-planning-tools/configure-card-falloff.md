---
filename: configure-card-falloff.md
content-type: reference
navigation-topic: boards
title: 設定卡片縮減
description: 您可以設定展示板，讓卡片可以依排程封存或掉出展示板。
author: Courtney
feature: Agile
exl-id: 0e4f6b3c-75aa-4314-9cb0-737e5a9d3bda
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/iSsqfrcgbod28qez5XkHDP-nDSQO-UKDGm13zPeeBZ0
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: e458b7274f0f80c8be395bdc8ad91eaf6cfd0876
workflow-type: tm+mt
source-wordcount: 228
ht-degree: 7%

---

# 設定卡片縮減

您可以設定展示板，讓卡片可依排程封存或「脫落」展示板。 您可以在特定欄中設定卡片，讓卡片在幾天或幾週內從展示板上掉下來。

卡片從展示板掉落時封存。 您可以使用篩選器顯示已封存的卡片。 如需詳細資訊，請參閱[在展示板中篩選和搜尋](/help/quicksilver/agile/get-started-with-boards/filter-search-in-board.md)。

## 存取權要求

+++ 展開以檢視這篇文章中所述功能的存取權要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 封裝</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td> 
   <p>投稿人或以上</p> 
   <p>要求或更高版本</p>
   </td> 
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 設定卡片縮減

{{step1-to-boards}}

1. 存取展示板。 如需詳細資訊，請參閱[建立或編輯展示板](../../agile/get-started-with-boards/create-edit-board.md)。
1. 按一下主機板右側的&#x200B;**[!UICONTROL [設定]]**&#x200B;以開啟[設定]面板。
1. 展開&#x200B;**[!UICONTROL 卡片]**。
1. 開啟&#x200B;**[!UICONTROL 自動從展示板封存卡片]**。

   ![卡片遞減設定](assets/card-falloff-switch.png)

1. 選取何時從展示板封存卡片。 您可以選擇最多8週或最多60天。

   日期是從上次修改卡片時開始決定的。

1. 選取要移除卡片的來源欄。
1. 在確認訊息上按一下&#x200B;**[!UICONTROL 儲存]**。
1. 按一下&#x200B;**[!UICONTROL 隱藏設定]**&#x200B;以關閉[!UICONTROL 設定]面板。 當您重新整理主機板時，組態設定會自動套用。
