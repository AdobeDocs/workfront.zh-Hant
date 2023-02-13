---
content-type: overview
product-area: resource-management
navigation-topic: resource-scheduling
title: 排程區域概觀
description: 以下小節說明您可在何處存取Adobe Workfront內的排程區域，以及排程區域中可用的功能。
author: Alina
feature: Resource Management
exl-id: ed6f1db9-917d-4a19-9fd4-1ed5d2ca95fb
source-git-commit: f150c57e8b83e73734b1cbeded7ef4c16d65097c
workflow-type: tm+mt
source-wordcount: '1790'
ht-degree: 0%

---

# 排程區域概觀

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

-->


以下小節說明您可在何處存取Adobe Workfront內的排程區域，以及排程區域中可用的功能。

## Workfront區域，可讓您排程資源

您可以在Workfront中排程以下區域的資源：

* **對於您擔任資源管理員的任何項目** (從 **排程** 區域)Workfront中的「計畫」區域使資源管理器能夠在多個項目之間進行資源分配。

* **當您是專案團隊的成員時，針對個別專案** (從 **排程** 項目區域):

   項目內的「計畫」(Scheduling)區域使項目組成員能夠將項目中的工作分配給項目組中的用戶。

* **對於個別團隊，您是** (從 **排程** 小組的部分)團隊中的「計畫」部分允許團隊成員將已從多個項目分配給團隊的工作分配給各個團隊成員。

## 「排程」區域中可用的功能

計畫區域顯示任務和問題以及當前資源分配。\
![resource_scheduling_overview.png](assets/resource-scheduling-overview-350x237.png)

* [篩選和交換工具](#filter-and-swap-tools)
* [日期選擇](#date-selection)
* [未分配區域](#unassigned-area)
* [使用者和角色](#users-and-roles)
* [排程時間表](#scheduling-timeline)

### 篩選和交換工具 {#filter-and-swap-tools}

* **篩選工具：** 可讓您篩選顯示在排程時間軸上的內容。 如需使用篩選工具的詳細資訊，請參閱 [篩選「排程」區域中的資訊](../../resource-mgmt/resource-scheduling/filter-scheduling-area.md).
* **交換工具：** （僅當從「計畫」頁簽或「人員配備」頁簽為項目計畫資源時可用）使您能夠在多個項目中快速分配、交換或取消分配用戶的任務。 如需詳細資訊，請參閱 [在「計畫」區域中手動分配未分配的任務和問題](../../resource-mgmt/resource-scheduling/manually-assign-items-scheduling-areas.md).

### 日期選擇 {#date-selection}

您可以調整在排程時間軸上顯示資料的日期範圍。 依預設，從當天開始的日期範圍是2週（連續14天，包括週末）。

### 未分配區域 {#unassigned-area}

* [將資源作為資源管理器進行計畫時（用於「計畫」區域中的多個項目）](#when-scheduling-resources-as-the-resource-manager-for-multiple-projects-in-the-scheduling-area)
* [將資源作為項目團隊的成員（來自項目）進行計畫時](#when-scheduling-resources-as-a-member-of-the-project-team-from-a-project)
* [將資源安排為團隊成員時（來自團隊）](#when-scheduling-resources-as-a-team-member-from-a-team)

#### 將資源作為資源管理器進行計畫時（用於「計畫」區域中的多個項目） {#when-scheduling-resources-as-the-resource-manager-for-multiple-projects-in-the-scheduling-area}

此 **未指派** 排程時間軸上的區域只會顯示符合下列所有條件的任務和問題：

* 未指派給使用者。
* 未指派給團隊。\
   如果將任務或問題指派給團隊，則任務或問題仍顯示在 **未指派** 區域（如果除了團隊分配外，任務或問題也被分配給角色）。\
   如果任務或問題具有用戶未履行的附加任務角色分配，則也會顯示這些任務或問題。\
   例如，將任務分配給3個作業角色：設計人員、產品經理和開發人員。 將此任務分配給具有設計師職務角色的用戶A和具有產品經理職務角色的用戶B。 在此情境中，任務仍顯示在計畫時間線上的「未分配」區域中，因為未將開發人員作業角色分配給用戶。

#### 將資源作為項目團隊的成員（來自項目）進行計畫時 {#when-scheduling-resources-as-a-member-of-the-project-team-from-a-project}

此 **未指派** 排程時間表頂端的區域會顯示符合下列條件的任務和問題：

* 與項目關聯，但未分配給項目團隊中的任何用戶。\
   與項目關聯並分配給項目團隊中某個用戶的任務將顯示在分配給任務的用戶行中。
* 與項目關聯，但分配給不在項目組的成員。

   <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;[! Is it even possible to have the task assigned to a member who is not part of the project team? If so, then would this end up in the Unassigned area?])</p>
  -->

#### **將資源安排為團隊成員時（來自團隊）** {#when-scheduling-resources-as-a-team-member-from-a-team}

此 **未指派** 排程時間表頂端的區域會顯示符合下列條件的任務和問題：

* 已分配給團隊，並且沒有分配給團隊中的其他用戶。\
   同時分配給團隊和團隊中某個用戶的任務將顯示在分配給任務的用戶行中。
* 同時分配給組和非組成員的用戶。

### 使用者和角色 {#users-and-roles}

* [將資源作為資源管理器進行計畫時（用於「計畫」區域中的多個項目）](#when-scheduling-resources-as-the-resource-manager-for-multiple-projects-in-the-scheduling-area)
* [將資源作為項目團隊的成員（來自項目）進行計畫時](#when-scheduling-resources-as-a-member-of-the-project-team-from-a-project)
* [將資源安排為團隊成員時（來自團隊）](#when-scheduling-resources-as-a-team-member-from-a-team)

#### 將資源作為資源管理器進行計畫時（用於「計畫」區域中的多個項目） {#when-scheduling-resources-as-the-resource-manager-for-multiple-projects-in-the-scheduling-area-1}

任何有資格被分配其中一個未分配任務的用戶位於 **未指派** 的上界。 在以下情況下，計畫時間表上的用戶可分配任務或問題：

* 預設情況下，僅當在系統中定義了作業角色（主作業角色或輔助作業角色），並且該作業角色與分配給當前可見的任務或問題的作業角色匹配時，用戶才顯示在調度時間軸上 **未指派** 排程時間表上的區域。 您可以禁用此功能，以便允許將任務和問題分配給任何用戶，而不管該用戶在其用戶配置檔案上是否定義了與任務的角色分配相匹配的角色，還是分配給任務的問題。 如需詳細資訊，請參閱 [在「排程」區域中，無論角色和群組成員資格為何，都允許指派使用者](../../resource-mgmt/resource-scheduling/assignments-regardless-of-role-or-group-scheduling-areas.md).\
   如果使用者在Workfront系統中指定多個工作角色，則使用者和使用者指派的工作可能會在排程時間軸上出現多次。\
   在分配任務或問題後，即使沒有剩餘任務或問題具有匹配角色分配，用戶仍停留在計畫時間線上。 這可讓您在指派後進行任何必要的變更。\
   如果未將任務分配給作業角色，則會顯示符合篩選要求的所有用戶。 如需篩選器的詳細資訊，請參閱 [篩選「排程」區域中的資訊](../../resource-mgmt/resource-scheduling/filter-scheduling-area.md).

* 已在 **使用者** 欄位 **篩選** 標籤。\
   如需篩選器的詳細資訊，請參閱 [篩選「排程」區域中的資訊](../../resource-mgmt/resource-scheduling/filter-scheduling-area.md).\
   在計畫團隊的資源時（在「工作日」頁簽上），也會顯示團隊分配。

分配給這些用戶的任何其他任務或問題也會顯示在時間軸上。

您可以查看在指定日期分配使用者的層級，如 [在「計畫」區域中管理用戶分配](../../resource-mgmt/resource-scheduling/manage-allocations-scheduling-areas.md). 您至少沒有Contribute權限的工作，會在排程時間軸上顯示為灰色列。

#### 將資源作為項目團隊的成員（來自項目）進行計畫時 {#when-scheduling-resources-as-a-member-of-the-project-team-from-a-project-1}

無論用戶的作業角色分配和「未分配」區域中任務的角色分配如何，團隊的每個成員都始終顯示在計畫時間表上。

如果用戶在系統中定義了多個作業角色，則當滿足以下條件之一時，用戶在計畫時間軸上出現多次：

* 在 **未指派** 分配給與用戶關聯的作業角色的區域。
* 項目上存在已分配作業角色的任務或問題，這些任務或問題將分配給在系統中定義了該作業角色的用戶。

#### 將資源安排為團隊成員時（來自團隊） {#when-scheduling-resources-as-a-team-member-from-a-team-1}

無論用戶的作業角色分配和「未分配」區域中任務的角色分配如何，團隊的每個成員都始終顯示在計畫時間表上。

您可以查看在指定日期分配使用者的層級，如 [在「計畫」區域中管理用戶分配](../../resource-mgmt/resource-scheduling/manage-allocations-scheduling-areas.md). 您至少沒有Contribute權限的工作，會在排程時間軸上顯示為灰色列。

### 排程時間表 {#scheduling-timeline}

* **預設內容：** 依預設，符合區段中定義之要求的所有工作 [任務和問題先決條件](../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md#task-and-issue-prerequisites) 在 [開始使用資源計畫](../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md) 所有狀態為「目前」(Current)的項目的相關文章將顯示在計畫時間表上。

   <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  (NOTE: [! true for teams? - Yes, but really we're focusing on tasks, and the team assignment.])
  </MadCap:conditionalText>
  -->

   若要自訂排程時間表上顯示的內容（包括顯示問題和狀態不同的專案），請使用篩選器，如 [篩選「排程」區域中的資訊](../../resource-mgmt/resource-scheduling/filter-scheduling-area.md).

   指定使用者每天最多會顯示10個工作。 您可以展開清單以檢視目前指派給該使用者的所有工作。

* **父任務：** 時間軸上是否顯示父任務取決於多個設定。 如需詳細資訊，請參閱 [在排程區域中配置設定](../../resource-mgmt/resource-scheduling/configure-settings-scheduling-areas.md) 文章。

* **顏色編碼：** 排程時間軸上的任務和問題會根據其所屬專案以色彩編碼。 您無法自訂與特定專案相關聯的顏色。

   排程團隊的工作時（從「人員配備」頁簽），只有在 **顯示所有用戶任務** 選項。 如需詳細資訊，請參閱 [在排程區域中配置設定](../../resource-mgmt/resource-scheduling/configure-settings-scheduling-areas.md) 文章。

* **任務持續時間：** 任務持續時間在每個任務的時間軸上表示（任務實際跨越的天數等於持續時間）。 無法從計畫時間軸調整任務持續時間。

* **關閉時間：** 在調度時間線上，在為給定用戶調度時間的日期的列中，以淺灰色指示器表示時間的關閉。\
   系統會根據下列資訊為每個使用者設定休息時間：

   使用者的個人逾時日曆。 有關個人休假日曆的詳細資訊，請參閱 [在Adobe Workfront中設定個人休假時間](../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/personal-time-overview.md).

   指派給使用者的排程。 這可能是預設排程或自訂排程。 如需排程的詳細資訊，請參閱 [建立排程](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

* **週末：** 週末在排程時間軸上以星期六和星期日的淺灰色陰影表示。 在排程時間軸上設定為週末的一週天數無法設定。 您可以排程使用者在週末工作。
