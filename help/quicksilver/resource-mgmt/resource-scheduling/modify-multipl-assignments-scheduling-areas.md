---
product-area: resource-management
navigation-topic: resource-scheduling
title: 修改調度區域中任務的多個用戶分配
description: 修改調度區域中任務的多個用戶分配。
author: Alina
feature: Resource Management
exl-id: 545a5033-a09e-4019-a10e-c388cf977ae4
source-git-commit: f150c57e8b83e73734b1cbeded7ef4c16d65097c
workflow-type: tm+mt
source-wordcount: '2213'
ht-degree: 0%

---

# 修改調度區域中任務的多個用戶分配


>[!IMPORTANT]
>  
><span class="preview">自2023年1月的23.1版開始，本文所述的排程功能已遭取代，並已從Adobe Workfront中移除。   </span>
>  
> <span class="preview"> 2023年初，23.1版發行後不久，也將移除本文。 此時，建議您據以更新任何書籤。 </span>
> 
><span class="preview"> 您現在可以使用工作負載平衡器來調度資源的工作。 </span>
>  
> <span class="preview">有關使用工作負載平衡器調度資源的資訊，請參見一節 [工作負載平衡器](../../resource-mgmt/workload-balancer/workload-balancer.md). </span>

<!--   

>[!CAUTION] 
> 
> 
> <span class="preview">The information in this article refers to the Adobe Workfront's Scheduling tools. The Scheduling areas have been removed from the Preview environment and will be removed from the Production environment in **January 2023**. </span> 
> <span class="preview"> Instead, you can schedule resources in the Workload Balancer. </span> 
> 
>* <span class="preview"> For information about scheduling resources using the Workload Balancer, see the section [The Workload Balancer](../../resource-mgmt/workload-balancer/workload-balancer.md).</span> 
> 
>* <span class="preview"> For more information about the deprecation and removal of the Scheduling tools, see [Deprecation of Resource Scheduling tools in Adobe Workfront](../../resource-mgmt/resource-mgmt-overview/deprecate-resource-scheduling.md).</span> 

This article refers to modifying user assignments for multiple tasks using the Scheduling area of Adobe Workfront. Also see the following articles for modifying assignments on multiple tasks in other areas:

* For information about modifying assignments on multiple tasks in a task list, see [Modify multiple user assignments in a task list](../../manage-work/tasks/assign-tasks/modify-multiple-assignments-in-task-list.md). 
* For information about scheduling resources using the new Workload Balancer, see the section [The Workload Balancer](../../resource-mgmt/workload-balancer/workload-balancer.md).
-->
使用資源調度程式時，可以同時將用戶分配給多個任務。

>[!NOTE]
>
>只有在為多個專案排程資源時（從「排程」區段），或為單一專案（從「排程」區段），才適用本文；在計畫團隊的資源時（從「計畫」部分），無法按本節所述管理多個任務的用戶分配。

## 存取需求

您必須具備下列條件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權概述*</td> 
   <td> <p>工作或更高</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級*</td> 
   <td> <p>查看或更高程度地訪問項目、任務和問題</p> <p><b>注意</b> 如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何變更您的存取層級的詳細資訊，請參閱 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>將權限或更高版本提供給項目、任務和問題，以更新分配</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 在計畫區域中進行多個分配的注意事項

您可以快速管理一或多個專案中多個工作和問題的使用者指派（變更會反映在排程時間軸上）。

您可以將用戶分配給當前分配給作業角色的所有任務、在用戶之間交換用戶分配，或從所有任務中取消分配用戶。

例如：

* 資源管理器負責在新項目上分配用戶。 項目最初建立為模板，而作業角色已分配給項目內的各種任務。 資源管理器希望將特定用戶分配給當前分配給作業角色的所有任務。
* 3個不同項目的45項任務被分配給Jackie Simms。 Jackie離開了組織，現在，資源經理需要將她的任務重新分配給其他用戶。

>[!NOTE]
>
>管理多個任務的用戶分配時，請考慮以下限制：
>
>* 為多個項目計畫資源時，您管理的項目必須處於以下狀態之一（或與以下狀態之一相等的狀態）:計畫、當前或已批准。 如需專案狀態的詳細資訊，請參閱 [建立或編輯狀態](../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).
>* 在計畫單個項目的資源時，項目狀態不會影響此功能的可用性。
>* 您可以為具有下列授權的使用者進行資源變更：計畫、工作和審核。 您無法為具有請求許可證的用戶進行資源更改。
>


## 管理一個或多個項目的用戶分配

1. 前往多個專案或個別專案的排程時間表：

   * **適用於多個專案**:  按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Workfront的右上角，按一下 **資源配置>工作負載平衡器**，然後選取 **排程** 的下拉式功能表。
   * **針對個別專案**:前往專案，按一下 **工作負載平衡器** 區段，然後選取 **排程** 從左上角的下拉式功能表。

1. 按一下 **動作**.\
   ![resource_scheduling.png](assets/resource-scheduling.png)

1. 在 **選擇項目** 欄位，視您是在查看多個項目的計畫時間表（從「計畫」頁簽），還是單個項目（從「人員配置」頁簽），執行以下任一操作：

   * **對於多個專案：** 開始鍵入要更改分配的項目名稱，然後在下拉清單中顯示名稱時按一下該名稱。 或者，按一下下拉式箭頭，從專案清單中選擇。 重複此過程，在多個項目之間進行分配更改。\
      將此欄位留空，以便對您擔任資源管理器的所有項目進行分配更改。

      >[!NOTE]
      >
      >只有符合以下條件時，才能選取專案：
      >
      >   
      >   
      >   * 您被指定為項目上的資源管理器\
         >     如需詳細資訊，請參閱 [為項目或模板指定資源管理器](../../manage-work/projects/planning-a-project/designate-resource-managers-for-projects-and-templates.md).
      >   
      >   * 項目處於以下狀態之一（或與以下狀態之一相等的狀態）:計畫、當前或已批准\
         >     如需專案狀態的詳細資訊，請參閱 [建立或編輯狀態](../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).
      >   
      >   * 您是具有計畫許可證的用戶。


   * **針對個別專案：** 此 **選擇項目** 欄位無法修改。 此 **選擇項目** 欄位一律包含您檢視之專案的名稱。

1. （選用）按一下 **指定任務** 修改單個任務的分配更改。 當您指定個別工作時，您在 **選擇項目** 欄位被忽略。\
   在 **選擇任務** 欄位中，開始鍵入要更改分配的任務的名稱。 重複此步驟，對其他任務進行分配更改。\
   如果將此欄位留空，則您在步驟3中選取的專案內的所有工作都會受到影響。\
   在對單個任務進行分配更改時，更改將應用於指定任務的所有子任務。 如果將問題配置為顯示在計畫時間表上，則更改也會應用於與任務相關的所有問題，如 [您可以配置各種設定，以自訂排程時間軸中資訊的顯示方式和內容。](../../resource-mgmt/resource-scheduling/configure-settings-scheduling-areas.md#configuring-issues-to-display-on-the-scheduling-timeline) in [在排程區域中配置設定](../../resource-mgmt/resource-scheduling/configure-settings-scheduling-areas.md).

1. 繼續下列任何小節：

   * [指派使用者](#assign-a-user)
   * [交換使用者](#swap-a-user)
   * [取消指派使用者](#unassign-a-user)

### 指派使用者 {#assign-a-user}

您可以將使用者指派給目前指派給所選專案內特定角色的所有工作。

以此方式指派使用者時，系統不會將使用者指派給下列類型的工作：

* 已分配給用戶的任務的分配
* 已完成的任務

要將用戶分配給整個所選項目或任務的任務，請執行以下操作：

1. 選擇 **指派使用者** 在 **選擇操作** 區段。\
   ![](assets/resource-scheduling-assign-350x678.png)

1. 在 **選擇角色** 欄位中，按一下下拉箭頭，從角色清單中選擇。 僅顯示當前分配給指定項目內任務的角色。\
   當您指派使用者時，使用者會取代您在此處選取的角色。

1. 在 **選擇要分配的用戶** 欄位中，按一下下拉箭頭，從使用者清單中選擇。\
   若 **將分配限制為具有匹配角色的用戶** 「設定」區域中啟用「 」選項時，只有在使用者在其使用者設定中（作為「主要角色」或「其他角色」）指派給他們時，使用者才可選取「 」。 如果禁用此選項，則可以開始鍵入要分配的另一個用戶的名稱，即使該用戶在系統中沒有定義匹配角色。 依預設會啟用選項。\
   如需此選項的詳細資訊，請參閱 [在「排程」區域中，無論角色和群組成員資格為何，都允許指派使用者](../../resource-mgmt/resource-scheduling/assignments-regardless-of-role-or-group-scheduling-areas.md). 預設情況下，只能對在其用戶配置檔案上定義了與指派給他們的任務或問題的角色分配相匹配的角色的用戶進行分配。

1. 按一下 **指派**.\
   在單一動作中，最多可以執行1,000個指派。 如果您所做的選擇將更改1,000個以上的分配，則必須重新調整您的選擇，然後重試。

### 交換使用者 {#swap-a-user}

您可以將用戶的任務分配與選定項目中另一個用戶的任務分配或選定任務的任務分配交換。

如本節所述，交換用戶的任務分配時，不會交換已標籤為「完成」的任何分配。

要將用戶的任務分配與另一個用戶的任務分配交換：

1. 選擇 **交換用戶** 在 **選擇操作** 區段。\
   ![](assets/resource-scheduling-swap-350x674.png)

1. 在 **選擇用戶** 欄位中，按一下下拉箭頭從用戶清單中選擇（或開始鍵入要交換的用戶的名稱，然後在下拉清單中顯示該名稱時按一下該名稱）。\
   只有在將使用者指派給指定專案內的一或多個未完成工作時，才會顯示。

1. （條件性） **選擇角色** 僅當所選用戶被分配給具有不同角色的多個任務時，才顯示欄位。 (要查看用戶在任務上設定的作業角色，請參閱 **受託人的角色** 欄，如 [建立高級分配](../../manage-work/tasks/assign-tasks/create-advanced-assignments.md))。\
   在 **選擇角色** 欄位，選擇角色以確定要交換的任務類型。 只有為用戶分配了此角色的任務才會分配給新用戶。\
   例如， Hanna Marin被指派給專案的5個工作。 在2項任務中，她的工作職責被定義為「工程師」。 在剩下的3項任務中，她的工作角色被定義為「設計師」。 如果在「選擇角色」欄位中選擇「設計器」，則表示要更改Hanna的所有3個任務上的分配，其中其職務角色定義為「設計器」。 將她的工作角色定義為「工程師」的2項任務保持不變。\
   ![](assets/resource-scheduling-swap-role.png)

1. 在 **選擇要分配的用戶** 欄位中，按一下下拉箭頭，從使用者清單中選擇。 只有當其角色（如其用戶設定中所定義）與分配給要替換的用戶的工作的角色匹配時，用戶才可分配。\
   若 **將分配限制為具有匹配角色的用戶** 選項在「設定」區域中啟用，則只有當其角色（如其用戶設定中定義）與分配給您替換的用戶的工作的角色匹配時，用戶才可以分配。 如果禁用此選項，則可以開始鍵入要分配的另一個用戶的名稱，即使該用戶在系統中沒有定義匹配角色。 依預設會啟用選項。\
   如需此選項的詳細資訊，請參閱 [在「排程」區域中，無論角色和群組成員資格為何，都允許指派使用者](../../resource-mgmt/resource-scheduling/assignments-regardless-of-role-or-group-scheduling-areas.md). 預設情況下，只能對在其用戶配置檔案上定義了與指派給他們的任務或問題的角色分配相匹配的角色的用戶進行分配。\
   如果您要替換的用戶在選定項目的任務上被分配到多個角色，並且您在 **選擇角色** 欄位， **選擇要分配的用戶** 欄位僅顯示具有所有指定角色的使用者。

1. 按一下 **交換**.\
   在單一動作中，最多可以執行1,000個指派。 如果您所做的選擇將更改1,000個以上的分配，則必須重新調整您的選擇，然後重試。

### 取消指派使用者 {#unassign-a-user}

您可以從選定項目或選定任務中分配給用戶的所有任務中取消分配用戶。 取消分配用戶時，分配給該用戶的任何任務在分配用戶之前都將還原為分配狀態。

如果用戶在系統中定義了主要角色，並且您取消分配了該用戶，則在取消分配該用戶時，該任務將自動分配給該用戶的主要角色。 或者，它被指派給在指派用戶之前被指派給的角色。

如果用戶在系統中未定義主角色，並且您取消分配了該用戶，則當您取消分配該用戶時，該任務將進入未分配狀態。

無法取消分配標籤為「完成」的任務。

要從整個選定項目或選定任務的任務中取消分配用戶，請執行以下操作：

1. 選擇 **取消分配用戶** 在 **選擇操作** 區段。\
   ![](assets/resource-scheduling-unassign-350x618.png)

1. 在 **選擇用戶** 欄位中，按一下下拉式箭頭以從使用者清單中選擇（或開始輸入您要取消指派的使用者名稱，然後在下拉式清單中出現名稱時按一下名稱）。 一次只能取消指派一個使用者。
1. （條件性） **選擇角色** 僅當所選用戶被分配給具有不同角色的多個任務時，才顯示欄位。 (要查看在用戶的任務上設定了哪些作業角色，請參閱 **受託人的角色** 欄，如 [建立高級分配](../../manage-work/tasks/assign-tasks/create-advanced-assignments.md))。\
   在 **選擇角色** 欄位，選擇角色以確定要取消分配的任務類型。 只有分配了此角色的用戶的任務才會被取消分配。\
   例如， Hanna Marin被指派給專案上的5個工作。 在2項任務中，她的工作職責被定義為工程師。 在剩餘的3個任務中，她的工作角色被定義為設計師。 如果在「選擇角色」欄位中選擇「設計器」，這意味著要取消分配Hanna的所有3個任務，其中其職務角色定義為「設計器」。 將其職務定義為工程師的兩項任務將保持不變。\
   ![](assets/resource-scheduling-unassign-role.png)

1. 按一下 **取消指派**.\
   在單一動作中，最多可以執行1,000個指派。 如果您所做的選擇將更改1,000個以上的分配，則必須重新調整您的選擇，然後重試。
