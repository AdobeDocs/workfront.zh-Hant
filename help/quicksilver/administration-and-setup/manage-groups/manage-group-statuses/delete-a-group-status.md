---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: 刪除組狀態
description: 作為組管理員，如果組未在系統級別上配置為必需或鎖定狀態，或在層次結構中為較高組配置，則可以刪除您管理的組的狀態。
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: bfce0325-fe6e-459f-96ca-9a5c94c61ed3
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '572'
ht-degree: 0%

---

# 刪除組狀態

作為組管理員，如果組未在系統級別上配置為必需或鎖定狀態，或在層次結構中為較高組配置，則可以刪除您管理的組的狀態。

如果您管理的群組上方有任何群組，其管理員也可以對您的群組執行此動作。 Workfront管理員（適用於任何群組）也是如此。

>[!NOTE]
>
>您無法刪除下列項目：
>
>* 內置狀態Planning、Current和Complete。 您可以更新其名稱、編輯其顏色，以及鎖定或解除鎖定，但無法刪除它們。
>* 處於待批准狀態的狀態，至少與組或其子組相關聯的一個對象。


## 存取需求

您必須具備下列條件才能執行本文所述步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront計畫*</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>計劃 </p> <p>您必須是群組的群組管理員或Workfront管理員。 如需詳細資訊，請參閱 <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">群組管理員</a> 和 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予使用者完整的管理存取權</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;如果您需要了解您擁有的計畫或授權類型，請聯絡Workfront管理員。

## 刪除組狀態

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **設定** ![](assets/gear-icon-settings.png).

1. 在左側面板中，按一下 **群組**.
1. 按一下頂層群組的名稱。
1. 在左側面板中，按一下 **狀態**.
1. 在顯示的狀態清單中，暫留在您要刪除的狀態上，然後按一下 **刪除** 在最右邊。

   ![](assets/hover-click-delete.jpg)

1. 在顯示的框中，選擇一個狀態以指定使用您正在刪除的狀態的對象（項目、任務、問題和審批流程）的替換狀態。

   只有與您要刪除的狀態等同的狀態才可用。 例如，如果您刪除等於「目前」的狀態，則只能看到等於「目前」的狀態。

   此外，顯示的狀態取決於您刪除的狀態是解鎖還是鎖定：

   * **如果沒鎖**:可使用非隱藏的鎖定和解除鎖定狀態。

      除了為子組建立的狀態外，還包括從系統級和上級組繼承的狀態。

   * **如果鎖定了**:下列其中一項為true:

      * 如果有其他鎖定、非隱藏的狀態，則只有這些狀態可用。
      * 如果沒有鎖定的非隱藏狀態，即使預設的Workfront狀態已隱藏或已解除鎖定，仍可使用。

         如需預設Workfront狀態的詳細資訊，請參閱 [訪問系統項目狀態清單](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md), [訪問系統任務狀態清單](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/task-statuses.md)，以及 [訪問系統問題狀態清單](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md).

1. 按一下 **刪除狀態**.

   如果刪除狀態是組中該類型的預設狀態，則替換狀態將取而代之。

   如果刪除的狀態被設定為項目首選項中的預設項目狀態，則首選項現在將設定為替換狀態。

## 刪除群組時

刪除某組並替換成另一組時，所刪除的組具有的所有唯一狀態都會添加到替換組的狀態中。 如需詳細資訊，請參閱 [移動或刪除的群組中的自訂狀態](../../../administration-and-setup/manage-groups/manage-group-statuses/custom-statuses-in-group-moved-or-deleted.md).
