---
product-area: agile-and-teams;projects
navigation-topic: use-kanban-in-an-agile-team
title: 將子任務添加到看板板上的現有物料
description: 請查看本文以了解如何為看板板上的現有動態建立子任務。
author: Lisa
feature: Agile
exl-id: c6610616-80e5-4ded-9d23-63f15536e45c
source-git-commit: 9da0c8234f563a0202cd15017b37a341476f7406
workflow-type: tm+mt
source-wordcount: '363'
ht-degree: 0%

---

# 將子任務添加到看板板上的現有物料

為現有動態建立子任務時，請記住以下事項：

**當 [!UICONTROL 摘要完成模式] 專案的設定設為 [!UICONTROL 手動]:**

* 您可以將含有子任務的父文章移至 [!UICONTROL 完成]，則父項動態會更新為100%，而 [!UICONTROL 狀態] to [!UICONTROL 完成]. 未更新子任務。
* 若要更新 [!UICONTROL 完成百分比] 對於故事，您必須從 [!UICONTROL 故事] 標籤或 [!UICONTROL 詳細資料] 頁。

**當 [!UICONTROL 摘要完成模式] 專案的設定設為 [!UICONTROL 自動]:**

* 你不能把父母的故事一概而論。 若要更新 [!UICONTROL 完成百分比] 為了講故事，您必須更新 [!UICONTROL 完成百分比] 的子任務。 此 [!UICONTROL 完成百分比] 根據 [!UICONTROL 完成百分比] 所有子任務。
* 將含有子任務的父文章移動到 [!UICONTROL 完成] 將父項動態更新為100%，且 [!UICONTROL 狀態] to [!UICONTROL 完成]. 子任務也會更新為100%，而 [!UICONTROL 狀態] 更新為 [!UICONTROL 完成].

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
  <tr> 
   <td role="rowheader"><strong>物件權限</strong></td> 
   <td> <p>[!UICONTROL Contribute]或[!UICONTROL Manage]對子任務所在任務的訪問</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的 [!DNL Workfront] 管理員。

## 將子任務新增至 [!UICONTROL 看板] 展示板

1. 前往 [!UICONTROL 看板] 包含您要新增子任務的案例的展示板。
1. 按一下文章圖磚上的任務名稱， [!UICONTROL 看板] 展示板。
1. 將子任務添加到任務中，如同在內的任何其他任務清單中一樣 [!DNL Workfront]，如 [建立子任務](../../manage-work/tasks/create-tasks/create-subtasks.md).
