---
product-area: resource-management
navigation-topic: the-workload-balancer
title: 使用工作負載平衡器大量指派工作
description: 您可以使用Adobe Workfront工作負載平衡器大量指派資源給多個任務和問題。
author: Lisa
feature: Resource Management
exl-id: fb0f80d3-7da4-4f5f-857d-3fb518ba12e2
TQID: https://experienceleague.adobe.com/6QlIfRh94tpLTZF6x5LU2BueTjShzNsaKxb45CEylqA
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
subfeature_v2:
  - id: c33d85a1-be85-4290-854c-87408c10aa80
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 4008f50a332371ac468cc8abb79b4e7a24541067
workflow-type: tm+mt
source-wordcount: 1242
ht-degree: 3%

---

# 使用工作負載平衡器大量指派工作

<!--Audited: 07/2024-->

您可以使用Adobe Workfront工作負載平衡器大量指派資源給多個任務和問題。

如需使用工作負載平衡器指派工作給使用者的一般資訊，請參閱在工作負載平衡器[&#128279;](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md)中指派工作的總覽。

## 存取權要求

+++ 展開以檢視這篇文章中所述功能的存取權要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront 封裝</td> 
   <td><p>任何</p></td>
  </tr>
  <tr> 
   <td>Adobe Workfront授權</td> 
   <td><p>標準</p>
       <p>計畫：在資源區域使用工作負載平衡器；工作，使用團隊或專案的工作負載平衡器</p></td>
  </tr>
  <tr> 
   <td>存取層級設定</td> 
   <td> <p>編輯下列專案的存取權：</p> 
    <ul> 
     <li>資源管理</li> 
     <li>專案</li> 
     <li>任務</li> 
     <li>問題</li> 
    </ul>
   </td> 
  </tr> 
  <tr> 
   <td>物件許可權</td> 
   <td>包含進行指派的專案、任務和問題的貢獻許可權或更高</td> 
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 在工作負載平衡器中進行大量指派的注意事項

* 您可以快速管理一個或多個專案中多個任務和問題的資源指派。 指派中的變更會立即顯示在工作負載平衡器中。
* 您無法將資源指派給已完成的工作專案，或指派給已完成專案上的專案。
* 大量指派工作角色和使用者時，您可以進行下列工作：

   * 取代所有有效組合中使用者和角色之間的指派。
   * 從使用者的所有工作專案解除指派使用者。

**範例**

* 您負責為多個新專案進行使用者指派。 專案原本是從範本建立的，工作角色已指派給專案內的各種任務。 您想要將特定使用者Jackie Simms指派給目前指派給工作角色的所有任務。 您可以使用Replace函式將這些工作指派給Jackie Simms。
* 3個不同專案中的45個任務指派給Jackie Simms。 Jackie離開了組織，現在您需要將其任務重新指派給其他使用者。 您可以使用「取代」功能，將這些工作指派給新人員。
* 2個不同專案中的10個任務指派給另一位使用者Rick Kuvec。 您意識到這些任務錯誤地指派了Rick，但您不確定此時需要指派給誰。 您需要同時將Rick解除指派給所有工作。 您可以使用「取消指派」功能將Rick從這些工作中移除。

## 在工作負載平衡器中大量指派工作

1. 前往您要指派工作的工作負載平衡器。

   您可以使用資源區域、專案或團隊層級的工作負載平衡器將工作指派給使用者。 如需有關工作負載平衡器在Workfront中的位置的詳細資訊，請參閱[找到工作負載平衡器](../../resource-mgmt/workload-balancer/locate-workload-balancer.md)。


1. 按一下工作負載平衡器頂端的&#x200B;**大量指派** ![大量指派](assets/bulk-assignments-wb.png)。

   「批次任務」面板將在工作負載平衡器的右側開啟。

1. （視條件而定）如果您要從「資源」區域或團隊存取「工作負載平衡器」，請展開「**專案：名稱**」下拉式功能表，並使用篩選修飾元來選取要指派給您的一或多個專案。 您可以依名稱（此為預設選項）或狀態來選取專案。

   如需Workfront篩選修飾元的資訊，請參閱[篩選和條件修飾元](../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md)。

   >[!NOTE]
   >
   >存取專案的工作負載平衡器時，預設會選取專案名稱。

   ![大量指派中的專案名稱](assets/project-name-status-dropdown-bulk-assignments-wb.png)

1. （選擇性）按一下&#x200B;**選取專案任務**&#x200B;以選取要指派給您的任務，然後在&#x200B;**任務：名稱**&#x200B;下拉式功能表中，依名稱（此為預設選項）或狀態選取任務，並使用篩選修飾元來搜尋特定任務。

   如需Workfront篩選修飾元的資訊，請參閱[篩選和條件修飾元](../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md)。

   >[!NOTE]
   >
   >您無法選取處於完成狀態的任務。

   ![大量指派中的任務狀態](assets/task-name-status-dropdown-bulk-assignments-wb.png)

   >[!TIP]
   >
   >如果您想要對問題和任務進行批次指派，請將此選取項保留空白。

1. （選擇性）按一下其中一個選取條件旁的&#x200B;**刪除**&#x200B;圖示![刪除圖示](assets/delete.png)

   或

   按一下「大量任務」面板右上角的「全部清除&#x200B;**&#x200B;**」以移除所有選取專案。

1. 選取下列其中一個選項，然後繼續下列步驟：

   * [取代資源](#replace-user)
   * [取消指派資源](#unassign-user)

   >[!TIP]
   >
   >如果沒有符合所選篩選條件的專案，這些選項將會變暗。

<!--

### Assign user {#assign-user}

When you assign a user using Bulk Assignments in the Workload Balancer, the following things occur:

* A user is assigned to all work items currently assigned to a specified role within the selected projects.
* The user is not assigned to the following types of work items:

   * Items that are already assigned to a user.
   * Completed items.

* If the user you selected is not associated with the specified role, the role is replaced by the user in the user's Primary Role.

To assign a user to work items previously assigned to job roles:

1. Start assigning work items using Bulk Assignments in the Workload Balancer as described above and select **Assign**. 

1. In the **Role assignment** field, click the drop-down arrow to choose from a list of roles. Only roles currently assigned within the specified projects are displayed. This is a required field. 

   ![Role assignment](assets/bulk-assignments-workload-balancer-assign-selected.png)

1. In the **User to assign** field, click the drop-down arrow to choose from a list of suggested users or to type another user's name.

   Select users from the following areas:

   * **Suggested Assignments**: Users who can fulfill the selected role and who match the criteria for Smart Assignments. For more information, see [Smart assignments overview](../../manage-work/tasks/assign-tasks/smart-assignments.md).
   * **Other Assignments**: All users in the system who can fulfill the selected role. 
   
      >[!TIP]
      >
      >Only the first 50 users are listed in the Other Assignments area.


   After selecting a user, Workfront displays a note about the number of items where the user you specified will be assigned and what job role they will replace.

   >[!TIP]
   >
   >All the roles of the user display in the list, under the user's name.


1. Click **Assign**.

   The specified roles are replaced with the users that you selected.

   You receive a confirmation about how many work items have had the selected role replaced with the selected user.

   ![Bulk assignment confirmation](assets/bulk-assign-user-confirmation-before-assigning-nwe-350x83.png)

-->

### 取代資源 {#replace-user}

您可以使用所選專案中的其他資源來取代已指派給工作專案的資源。

資源取代可以是：

* 角色與角色
* 具有使用者的使用者
* 使用者角色
* 具有使用者的角色

當您在工作負載平衡器使用批次指派將資源替換為另一個資源時，會發生以下情況：

* 取代資源會指派給目前指派給所選專案中原始資源的所有工作專案。
* 新資源未指派給任何已標示為「完成」的工作專案。
* 對於使用者對使用者的替換，如果與第一個使用者關聯的角色與第二使用者的任何角色都不相符，則會將第二個使用者指派為其主要角色。

以其他資源取代資源：

1. 如上所述，在工作負載平衡器大量指派區域中選取工作專案，並選取&#x200B;**取代資源**。
1. 在&#x200B;**目前指派的資源**&#x200B;欄位中，按一下下拉箭頭，從資源清單中選擇。 僅顯示指定專案內目前指派給未完成工作專案的資源。 這是必填欄位。

   ![取代資源](assets/bulk-assignments-workload-balancer-replace-selected.png)

1. 在&#x200B;**要指派的資源**&#x200B;欄位中，按一下下拉箭頭，從建議資源清單中選擇，或輸入另一個工作角色或使用者名稱。 依預設，第一個列出的資源符合智慧指派的條件。 如需詳細資訊，請參閱[智慧指派總覽](../../manage-work/tasks/assign-tasks/smart-assignments.md)。

   Workfront會顯示一個附註，說明目前指派的資源將取代第二個資源的專案數量。

1. 按一下&#x200B;**取代**。

   所選專案或任務的所有工作專案中的第一個資源會由第二個資源取代。

   您會收到確認，確認有多少工作專案已將原始指派取代為所選的第二個資源。

### 取消指派資源 {#unassign-user}

您可以在所選專案中，將資源從所有工作專案取消指派。

當您使用工作負載平衡器中的大量指派從使用者的所有指派中取消指派使用者時，會發生以下情況：

* 指定的使用者會從指派給該使用者的所有工作專案中移除。
* 如果未指派的使用者與工作角色相關聯，則移除使用者後，工作角色仍會指派給工作專案。

* 如果將指定的使用者指派給已完成的工作專案，則該使用者仍會指派給這些工作專案。

如需有關使用者和工作角色指派的詳細資訊，請參閱[在工作負載平衡器](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md)中指派工作的總覽。

若要從所選專案中的工作專案或針對已指派使用者的所選任務或問題取消指派使用者：

1. 如上所述，在工作負載平衡器大量指派區域中選取工作專案，並選取&#x200B;**取消指派資源**。

1. 在&#x200B;**要取消指派的使用者**&#x200B;欄位中，按一下下拉箭頭，從使用者清單中選擇。 只有目前指派給指定專案中未完成工作專案的使用者才會顯示。 這是必填欄位。

   ![取消指派使用者](assets/bulk-assignments-workload-balancer-unassign-selected.png)

   Workfront會顯示附註，說明目前指派的使用者將被取消指派的專案數量。

1. 按一下&#x200B;**取消指派**。\
   您會收到有關指定的使用者被移除的工作專案數目的確認。



