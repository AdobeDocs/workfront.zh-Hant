---
product-area: agile-and-teams
navigation-topic: create-and-manage-teams
title: 停用團隊
description: 您可以停用保留相關歷史資料時不再使用的團隊。 Adobe Workfront管理員可以隨時從「設定」的「團隊」區域重新啟用團隊。
author: Lisa
feature: People Teams and Groups
exl-id: 634e4c0f-aa1d-4197-92e3-54f414344ac0
source-git-commit: 24bb9b5c0836196a1c6e15f828eb47bbd489ef25
workflow-type: tm+mt
source-wordcount: '338'
ht-degree: 0%

---

# 停用團隊

您可以停用保留相關歷史資料時不再使用的團隊。 [!DNL Adobe Workfront] 管理員可以隨時從「設定」的「團隊」區域重新啟用團隊。 如果停用團隊，則團隊不再顯示於下列區域：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> 
    <ul> 
     <li> <p>自訂表單中的預先輸入欄位</p> </li> 
    </ul> 
    <ul> 
     <li> <p>對象共用對話框</p> </li> 
     <li> <p>[!UICONTROL用戶配置檔案]*</p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL團隊]區域中的主選擇下拉菜單</p> </li> 
     <li> <p>[!UICONTROL分配]類型</p> </li> 
     <li> <p>項目中的[!UICONTROL添加到看板]板對話框</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

當您搜尋團隊時，已停用的團隊不會出現，但仍會顯示在 [!UICONTROL 主隊] 和「其他團隊」(Other Teams)。

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
   <td> <p>計劃</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫或授權類型，請連絡您的 [!DNL Workfront] 管理員。

## 停用團隊

在停用前分配給該團隊的任何工作仍被分配。 建議您先重新指派工作，然後再停用團隊。

>[!TIP]
>
>您可以建立報表以篩選任何仍指派停用之團隊的工作或問題。

使用請求隊列時，如果禁用路由規則中指定為預設團隊的團隊，則團隊將保持不變，請求仍被路由到停用的團隊。 建議您先與作用中團隊更新路由規則，然後再停用團隊。

1. 按一下 **[!UICONTROL 主菜單]** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **[!UICONTROL 團隊]**.
1. 按一下 **[!DNL Switch team]** 表徵圖，然後從下拉菜單中選擇新團隊，或在搜索欄中搜索團隊。
1. 按一下 **[!UICONTROL 更多]** ，然後選取 **[!UICONTROL 編輯]**.

   ![](assets/edit-team-settings-350x205.png)

1. 清除 **[!UICONTROL 活動]** 框。
1. 按一下 **[!UICONTROL 儲存變更]**.

## 已知限制

已停用的團隊會顯示在下列區域：

* 中的「擁有者」欄位 [!DNL Workfront Goals]. 這需要額外的授權 [!DNL Adobe Workfront Goals]. 如需詳細資訊，請參閱 [開始使用 [!DNL Adobe Workfront Goals]](../../workfront-goals/goal-management/getting-started-with-wf-goals.md).
