---
content-type: overview
product-area: agile-and-teams
navigation-topic: agile-navigation-topic
title: 管理面板上的進行中工作(WIP)限制
description: 您可以為展示板上的每個欄設定進行中工作(WIP)限制。
author: Courtney
feature: Agile
exl-id: 7901c6e7-75a4-41e4-b288-d527c4a6d031
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: 'https://experienceleague.adobe.com/jOCQTCkNgEZfE8O4-KyKVjEluncwWx0vh5NdrKHC9vg'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
    internal-label: Work management
subfeature_v2:
  - id: be65ef36-43e4-48e1-a062-caa3778e15be
    internal-label: Agile
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 4c642a8ef31f3b9a03288f2d74e704be6ee86c55
workflow-type: tm+mt
source-wordcount: '242'
ht-degree: 7%
---
# 管理展示板上的[!UICONTROL 進行中工作] (WIP)限制

您可以為展示板上的每個欄設定[!UICONTROL 進行中工作] (WIP)限制。

WIP限制只是視覺上的警告，不會限制您在每一欄中擁有的料號超過您設定的限制。

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

## 設定欄位的在製品限制

{{step1-to-boards}}

1. 存取展示板。 如需詳細資訊，請參閱[建立或編輯展示板](../../agile/get-started-with-boards/create-edit-board.md)。
1. 找到您要新增WIP限制的欄。

   若要新增欄，請參閱[管理面板欄](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md)。

1. 按一下欄上的&#x200B;**[!UICONTROL 更多]**&#x200B;功能表，然後選取&#x200B;**[!UICONTROL 編輯]**&#x200B;以開啟[設定]區域。
1. 在[!UICONTROL 資料行原則]下，啟用&#x200B;**[!UICONTROL 進行中工作]限制**&#x200B;原則以限制可新增至資料行的卡片數目。
1. 在&#x200B;**[!UICONTROL 設定限制]**&#x200B;欄位中輸入限制數字。

   ![欄](assets/boards-wip-limit-in-column.png)的WIP限制

   卡片的數量和限制會顯示在欄的最上方。 如果欄包含超過限制的卡片，計數器會變成紅色。

   ![在製品限制計數器](assets/boards-wip-limit-counter.png)

1. 按一下&#x200B;**[!UICONTROL 關閉]**&#x200B;以結束[!UICONTROL 設定]區域並檢視資料行及其卡片。
