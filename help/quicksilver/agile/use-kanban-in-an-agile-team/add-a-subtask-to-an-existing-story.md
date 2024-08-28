---
product-area: agile-and-teams;projects
navigation-topic: use-kanban-in-an-agile-team
title: 將子任務新增至Kanban面板上的現有劇本
description: 請檢閱本文，瞭解如何為Kanban面板上的現有內文建立子任務。
author: Lisa
feature: Agile
exl-id: c6610616-80e5-4ded-9d23-63f15536e45c
source-git-commit: 452f8ddc5268a0d67e32090d166199f2fad7dbc7
workflow-type: tm+mt
source-wordcount: '328'
ht-degree: 0%

---

# 將子任務新增至Kanban面板上的現有劇本

建立現有內文的子任務時，請牢記以下事項：

**專案的[!UICONTROL 摘要完成模式]設定設為[!UICONTROL 手動]：**&#x200B;時

* 您可以將具有子任務的父級本文移動到[!UICONTROL 完成]，這樣會將父級本文更新為100%，並將[!UICONTROL 狀態]更新為[!UICONTROL 完成]。 子任務未更新。
* 若要更新內文的[!UICONTROL 完成百分比]，您必須從[!UICONTROL 內文]索引標籤或物件的[!UICONTROL 詳細資料]頁面進行更新。

**專案的[!UICONTROL 摘要完成模式]設定設為[!UICONTROL 自動]：**&#x200B;時

* 您無法將父內文移到其他地方。 若要更新內文的[!UICONTROL 完成百分比]，您必須更新任何子任務的[!UICONTROL 完成百分比]。 內文的[!UICONTROL 完成百分比]是根據所有子工作的[!UICONTROL 完成百分比]計算的。
* 將具有子任務的父本文移動到[!UICONTROL 完成]會將父本文更新為100%，並將[!UICONTROL 狀態]更新為[!UICONTROL 完成]。 子任務也更新為100%，且[!UICONTROL 狀態]更新為[!UICONTROL 完成]。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計劃</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權</td> 
   <td> <p>新增：[！UICONTROL Standard]</p> 
   或
   <p>目前： [！UICONTROL Work]或更高版本</p> </td> 
  </tr>
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td>[！UICONTROL Contribute]或[！UICONTROL Manage]子任務所在任務的存取權</td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 將子任務新增至[!UICONTROL Kanban]展示板上的現有劇本

1. 前往包含您要新增子任務之劇本的[!UICONTROL Kanban]面板。
1. 按一下[!UICONTROL Kanban]展示板上劇本拼貼上工作的名稱。
1. 新增子任務至任務，就像您在[!DNL Workfront]內的任何其他任務清單中新增子任務一樣，如[建立子任務](../../manage-work/tasks/create-tasks/create-subtasks.md)中所述。
