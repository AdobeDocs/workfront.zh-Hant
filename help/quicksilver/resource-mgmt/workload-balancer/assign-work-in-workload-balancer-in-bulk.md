---
product-area: resource-management
navigation-topic: the-workload-balancer
title: 使用工作負載平衡器批量分配工作
description: 您可以使用Adobe Workfront Workload Balancer手動將工作項目指派給使用者。
author: Alina
feature: Resource Management
exl-id: fb0f80d3-7da4-4f5f-857d-3fb518ba12e2
source-git-commit: 57ca3b58f3ef39eaea82acf609135b1e5ae8e631
workflow-type: tm+mt
source-wordcount: '1543'
ht-degree: 2%

---

# 使用工作負載平衡器批量分配工作

<!--drafted
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment.</span> 
-->

您可以使用Adobe Workfront Workload Balancer手動將工作項目指派給使用者。

有關使用工作負載平衡器為用戶分配工作的一般資訊，請參見 [工作負載平衡器中分配工作的概述](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md).

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>任何 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>在資源區中使用工作負載平衡器時進行計畫</p>
   <p>使用團隊或項目的工作負載平衡器時工作</p>

</td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級*</td> 
   <td> <p>編輯對以下項目的存取權：</p> 
    <ul> 
     <li> <p>資源管理</p> </li> 
     <li> <p>專案</p> </li> 
     <li> <p>任務</p> </li> 
     <li> <p>問題</p> </li> 
    </ul> <p><b>附註</b>

如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何變更您的存取層級的詳細資訊，請參閱 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>將權限或更高版本貢獻給包括「進行分配」的項目、任務和問題</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 在工作負載平衡器中進行批量分配的注意事項

* 您可以快速管理一或多個專案中多個工作和問題的使用者指派。 工作負載平衡器中會立即顯示分配中的更改。
* 不能將資源分配給已完成的工作項或已完成項目上的項。
* 大量指派使用者時，您可以執行下列操作：

   * 將用戶分配給當前分配給作業角色的所有工作項。
   * 替換用戶之間的用戶分配。
   * 從其所有工作項目中取消指派使用者。

**範例**

* 您負責在多個新專案中指派使用者。 項目最初是從模板建立的，而作業角色已分配給項目中的各種任務。 您想要將特定用戶Jackie Simms分配給當前分配給工作角色的所有任務。 您可以使用「指定」功能將這些任務指定給Jackie Simms。
* 3個不同項目的45項任務被分配給Jackie Simms。 傑姬離開了組織，現在你需要將她的任務重新分配給其他用戶。 您可以使用「替換」功能將這些任務分配給新人員。
* 2個不同專案中的10個工作會指派給另一個使用者Rick Kuvec。 您意識到Rick錯誤地被分配給了這些任務，但您不確定此時需要分配給誰。 您需要同時取消將Rick分配給所有任務。 您可以使用Unassign函式從這些任務中刪除Rick。

## 在工作負載平衡器中批量分配工作

1. 轉到要分配工作的工作負載平衡器。

   您可以在資源區域、項目或團隊級別使用工作負載平衡器為用戶分配工作。 有關工作負載平衡器在Workfront中的位置的詳細資訊，請參見 [找到工作負載平衡器](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).


1. 按一下 **大量指派** ![](assets/bulk-assignments-wb.png) 工作負載平衡器的頂端。

   「Bulk Assignments（批量分配）」面板將開啟到工作負載平衡器的右側。

1. （條件性）如果要從「資源配置」區域或團隊訪問「工作負載平衡器」，請展開 **專案：名稱** 下拉式功能表，並使用篩選修改量來選取您要指派的專案或專案。 您可以依名稱（此為預設選項）或依狀態選取專案。

如需Workfront篩選修飾元的詳細資訊，請參閱 [篩選條件修飾元](../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

>[!NOTE]
>
>訪問項目的工作負載平衡器時，預設會選擇項目名稱。

![](assets/project-name-status-dropdown-bulk-assignments-wb-nwe-350x133.png)

1. （選用）按一下 **選擇項目任務** 要選擇要為其分配的任務或任務，請在 **任務：名稱** 下拉菜單，按名稱選擇任務（此為預設選項）或狀態，然後使用篩選修改符搜索特定任務。

如需Workfront篩選修飾元的詳細資訊，請參閱 [篩選條件修飾元](../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

>[!NOTE]
>
>不能選擇處於「完成」狀態的任務。

![](assets/task-name-status-dropdown-bulk-assignments-wb-nwe-350x102.png)

>[!TIP]
>
>如果要為問題和任務進行批量分配，請將此選項留空。

1. （選用）按一下 **刪除** 圖示 ![](assets/delete.png) 在其中一個選取的條件旁

   或

   按一下 **全部清除** 位於「批量分配」面板的右上角，以刪除所有選項。

1. 選取下列其中一個選項，然後繼續下列步驟：

   * [指派使用者](#assign-user)
   * [取代使用者](#replace-user)
   * [解除指派使用者](#unassign-user)

   >[!TIP]
   >
   >如果沒有項目與選取的篩選器相符，這些選項會呈現暗灰色。

### 指派使用者 {#assign-user}

在工作負載平衡器中使用批量分配來分配用戶時，將發生以下情況：

* 用戶被分配給當前分配給選定項目內指定角色的所有工作項。
* 未將用戶分配給以下類型的工作項：

   * 已指派給使用者的項目。
   * 已完成的項目。

* 如果您選擇的用戶未與指定的角色關聯，則該角色將由用戶的主角色中的用戶替換。

要將用戶分配給先前分配給作業角色的工作項，請執行以下操作：

1. 如上所述，在工作負載平衡器中使用批量分配開始分配工作項，並選擇 **指派**.

1. 在 **角色分配** 欄位中，按一下下拉箭頭，從角色清單中選擇。 只顯示當前在指定項目中分配的角色。 這是必填欄位。

   ![](assets/bulk-assignments-workload-balancer-assign-selected.png)

1. 在 **要指派的使用者** 欄位中，按一下下拉箭頭，從建議的使用者清單中選擇或鍵入其他使用者的名稱。

   從以下區域選擇用戶：

   * **建議的分配**:能夠完成所選角色的用戶以及符合智慧分配標準的用戶。 如需詳細資訊，請參閱 [智慧分配概述](../../manage-work/tasks/assign-tasks/smart-assignments.md).
   * **其他分配**:系統中能夠完成所選角色的所有用戶。

      >[!TIP]
      >
      >「其他分配」區域中只列出前50個用戶。
   選取使用者後，Workfront會顯示附註，說明您指定的使用者將被指派的項目數量，以及將取代的工作角色。

   >[!TIP]
   >
   >使用者的所有角色都會顯示在清單中，位於使用者名稱下。


1. 按一下 **指派**.

   指定的角色將替換為所選用戶。

   您會收到確認函，確認有多少工作項目已將選取的角色取代為選取的使用者。

   ![](assets/bulk-assign-user-confirmation-before-assigning-nwe-350x83.png)

### 取代使用者 {#replace-user}

您可以將已指派給工作項目的使用者，取代為所選專案中的其他使用者。

使用工作負載平衡器中的「批量分配」將用戶替換為另一個用戶時，會發生以下情況：

* 替換用戶被分配給當前分配給選定項目中原始用戶的所有工作項。

* 未將新用戶分配給已標籤為「完成」的任何工作項。
* 如果與第一用戶相關聯的角色與第二用戶的任何角色不匹配，則第二用戶被分配到其主角色中。

要將用戶替換為其他用戶：

1. 如上所述，開始在工作負載平衡器中分配工作項並選擇 **取代**.
1. 在 **當前分配的用戶** 欄位中，按一下下拉箭頭，從使用者清單中選擇。 僅顯示當前分配給指定項目中未完成工作項的用戶。 這是必填欄位。

   ![](assets/bulk-assignments-workload-balancer-replace-selected-350x345.png)

1. 在 **要指派的使用者** 欄位中，按一下下拉箭頭，從建議的使用者清單中選擇或鍵入其他使用者名稱。 依預設，清單中列出的用戶符合智慧分配的條件。 如需詳細資訊，請參閱 [智慧分配概述](../../manage-work/tasks/assign-tasks/smart-assignments.md).

   Workfront會顯示有關目前指派的使用者將取代第二個使用者的項目數，以及將取代哪些角色的附註。

   ![](assets/bulk-replace-user-confirmation-before-replacing-nwe-350x49.png)

1. 按一下 **取代**.

   所選項目的所有工作項中的第二用戶將替換所選的第一用戶。

   您會收到確認函，確認有多少工作項目已將原始使用者指派取代為選取的第二位使用者。

### 解除指派使用者 {#unassign-user}

您可以從使用者在所選專案中被指派的所有工作項目中取消指派使用者。

使用工作負載平衡器中的「批量分配」從其所有分配中取消分配用戶時，將發生以下情況：

* 指定的用戶將從分配給它們的所有工作項中刪除。
* 如果未分配的用戶與作業角色相關聯，則刪除該用戶後，作業角色仍被分配給工作項。

* 如果指定的用戶被分配給已完成的工作項，則用戶仍被分配給這些工作項。

有關用戶和作業角色分配的詳細資訊，請參閱 [工作負載平衡器中分配工作的概述](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md).

要從選定項目中的工作項目或為選定任務或分配任務或問題取消分配用戶，請執行以下操作：

1. 如上所述，開始在工作負載平衡器中分配工作項並選擇 **取消指派**.

1. 在 **要取消分配的用戶** 欄位中，按一下下拉箭頭，從使用者清單中選擇。 僅顯示當前分配給指定項目內未完成工作項的用戶。 這是必填欄位。

   ![](assets/bulk-assignments-workload-balancer-unassign-selected-350x318.png)

   Workfront會顯示有關將取消指派目前指派使用者的項目數的附註。

   ![](assets/bulk-unassign-user-confirmation-before-assigning-nwe-350x45.png)

1. 按一下 **取消指派**.\
   您會收到指定使用者被移除之工作項目數量的確認函。

 
