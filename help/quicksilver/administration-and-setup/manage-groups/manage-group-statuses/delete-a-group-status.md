---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: 刪除群組狀態
description: 作為群組管理員，您可以刪除您管理的群組的狀態（如果未在系統層級上設定為必要或鎖定狀態），或是刪除階層中較高群組的狀態。
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: bfce0325-fe6e-459f-96ca-9a5c94c61ed3
source-git-commit: 1554c067afcc548c7f7abd03dbc3a49404e3c89c
workflow-type: tm+mt
source-wordcount: '541'
ht-degree: 0%

---

# 刪除群組狀態

作為群組管理員，您可以刪除您管理的群組的狀態（如果未在系統層級上設定為必要或鎖定狀態），或是刪除階層中較高群組的狀態。

如果您管理的群組之上有任何群組，其管理員也可以為您的群組執行此動作。 Workfront管理員也是如此（適用於任何群組）。

>[!NOTE]
>
>您無法刪除下列專案：
>
>* 內建狀態為Planning、Current和Complete。 您可以更新其名稱、編輯其顏色、鎖定或解除鎖定，但無法刪除它們。
>* 至少有一個與群組或其子群組相關聯的物件處於未決核准狀態。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront套件</td> 
   <td><p>任何</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront授權</td> 
   <td><p>標準</p>
       <p>規劃</p></td>
  </tr>
  <tr> 
   <td>存取層級設定</td> 
   <td>您必須是群組的群組管理員或系統管理員。</td>
  </tr>
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 刪除群組狀態

{{step-1-to-setup}}

1. 在左側面板中，按一下&#x200B;**群組**。
1. 按一下最上層群組的名稱。
1. 在左側面板中按一下&#x200B;**狀態**。
1. 在顯示的狀態清單中，暫留在您要刪除的狀態上，然後在最右邊顯示&#x200B;**刪除**&#x200B;時按一下。

   ![刪除](assets/hover-click-delete.jpg)

1. 在顯示的方塊中，選取一個狀態，以指定使用您要刪除之狀態的物件（專案、任務、問題和核准流程）的取代狀態。

   您只能使用與您要刪除的狀態相同的狀態。 例如，如果您要刪除等同於「目前」的狀態，則只能看到等同於「目前」的狀態。

   此外，顯示的狀態取決於您要刪除的狀態是解除鎖定還是鎖定：

   * **如果已解除鎖定**：可以使用非隱藏的鎖定與解除鎖定狀態。

     除了為子群組建立的狀態外，也會包含從系統層級和上層群組繼承的狀態。

   * **若已鎖定**：下列其中一項true：

      * 如果有其他鎖定、非隱藏的狀態，則只能使用這些狀態。
      * 如果沒有鎖定的非隱藏狀態，則預設的Workfront狀態可供使用，即使該狀態為隱藏或未鎖定亦然。

        如需有關預設Workfront狀態的資訊，請參閱[存取系統專案狀態清單](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md)，[存取系統任務狀態清單](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/task-statuses.md)，以及[中有關4個必要問題狀態的資訊。存取系統問題狀態清單](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md)。

1. 按一下&#x200B;**刪除狀態**。

   如果刪除的狀態是群組中該型別的預設狀態，取代狀態會取代該狀態。

   如果刪除狀態在專案偏好設定中設定為預設專案狀態，則偏好設定現在會設定為取代狀態。

## 刪除群組時

當群組被刪除並被另一個群組取代時，已刪除群組之前的任何唯一狀態都會新增到取代群組的狀態。 如需詳細資訊，請參閱[已移動或刪除之群組中的自訂狀態](../../../administration-and-setup/manage-groups/manage-group-statuses/custom-statuses-in-group-moved-or-deleted.md)。
