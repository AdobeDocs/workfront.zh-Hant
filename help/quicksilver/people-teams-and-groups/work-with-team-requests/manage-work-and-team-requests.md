---
content-type: reference
product-area: user-management;agile-and-teams
navigation-topic: people-teams-and-groups
title: 管理工作和團隊請求
description: 請求代表擱置任務或問題指派。 工作請求會向個人發出，而團隊請求則會向團隊發出。
author: Lisa
feature: People Teams and Groups, Work Management
exl-id: ef96e520-0d5f-4180-a27a-1fbbffff8f2b
source-git-commit: dd47158a4c2e1b7372af6c9450b2d277d1ca8c6f
workflow-type: tm+mt
source-wordcount: '486'
ht-degree: 0%

---

# 管理工作和團隊請求

請求代表擱置任務或問題指派。 工作請求會向個人發出，而團隊請求則會向團隊發出。

>[!NOTE]
>
>敏捷團隊沒有團隊請求。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Adobe Workfront套件</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td>
   <p>若要指派或處理請求，請執行下列步驟：
   <p>淺色或更高</p>
  <p>評論或以上</p>
   <p>若要重新指派請求，請執行下列步驟：
   <p>標準</p>
   <p>工作或更高</p></td>
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 將請求指派給團隊 {#assign-a-request-to-a-team}

當專案經理和問題請求者不知道哪一種資源適合做工作或誰完成工作並不重要時，可以將工作指派給團隊。

指派給團隊的任務會保留在[!UICONTROL 團隊請求]標籤上，直到團隊中的使用者自願處理請求為止。

當請求同時指派給團隊和非團隊成員的使用者時，該請求會顯示在[!UICONTROL 團隊請求]索引標籤和使用者的工作請求區域中。 如果不在團隊中的使用者自願處理該任務，則該任務仍保留在[!UICONTROL 團隊請求]索引標籤中，直到團隊中的使用者自願處理為止。

團隊可以透過以下任何方式指派給任務和問題：

* 透過[!UICONTROL 甘特圖]
* 從任務或問題清單（個別或大量）
* 建立或修改任務或問題時
* 透過請求的路由規則（僅限問題）

您可以從專案團隊頁面手動將請求指派給專案團隊，如本節所述。

若要從專案團隊頁面手動指派請求給專案團隊：

{{step1-to-team}}

1. 按一下&#x200B;**[!UICONTROL 切換群組]**&#x200B;圖示![切換群組圖示](assets/switch-team-icon.png)，然後從下拉式功能表中選取新群組或在搜尋列中搜尋群組。

1. 按一下&#x200B;**[!UICONTROL 更多]**&#x200B;圖示![](assets/more-icon.png)，然後選取&#x200B;**[!UICONTROL 傳送工作要求]**。

   ![](assets/edit-team-settings-350x205.png)

1. 在開啟的方塊中填入資訊。
1. 按一下&#x200B;**[!UICONTROL 傳送要求]**。\
   專案團隊現在會被指派新任務，該任務會顯示在「專案團隊請求」標籤上。 此任務目前未與專案關聯，但可以移動，如[移動任務](../../manage-work/tasks/manage-tasks/move-tasks.md)中所述。

## 重新指派請求 {#reassign-requests}

您可以重新指派已指派給團隊的要求：

{{step1-to-team}}

1. 按一下&#x200B;**[!UICONTROL 切換群組]**&#x200B;圖示![切換群組圖示](assets/switch-team-icon.png)，然後從下拉式功能表中選取新群組或在搜尋列中搜尋群組。
1. 在左側導覽面板中，選取&#x200B;**[!UICONTROL 團隊要求]**。
1. 按一下&#x200B;**[!UICONTROL 重新指派]**&#x200B;圖示。

1. 開始輸入您要重新指派請求的使用者、群組或團隊名稱，然後按一下[指派]。****\
   請求已重新指派。
