---
product-area: resource-management
navigation-topic: resource-scheduling
title: 在「計畫」區域中管理用戶分配
description: 本文介紹如何使用「資源計畫」區域為分配給任務或問題的用戶更新每日每小時分配。
author: Alina
feature: Resource Management
exl-id: c8ddb250-145e-4321-8747-4f4967fcce41
source-git-commit: f150c57e8b83e73734b1cbeded7ef4c16d65097c
workflow-type: tm+mt
source-wordcount: '2944'
ht-degree: 0%

---

# 在「計畫」區域中管理用戶分配

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
> <span class="preview">The information in this article refers to the Adobe Workfront's Scheduling tools. The Scheduling areas have been removed from the Preview environment and will be removed from the Production environment in **January 2023**.  </span> 
> <span class="preview"> Instead, you can schedule resources in the Workload Balancer. </span> 
> 
>* <span class="preview"> For information about scheduling resources using the Workload Balancer, see the section [The Workload Balancer](../../resource-mgmt/workload-balancer/workload-balancer.md).</span> 
> 
>* <span class="preview"> For more information about the deprecation and removal of the Scheduling tools, see [Deprecation of Resource Scheduling tools in Adobe Workfront](../../resource-mgmt/resource-mgmt-overview/deprecate-resource-scheduling.md).</span> 

-->

用戶分配是指用戶應花在某一指定日完成工作項的時間的小時數。 它們包含在工作項目的「計畫小時數」中。

本文介紹如何使用「資源計畫」區域為分配給任務或問題的用戶更新每日每小時分配。 有關管理用戶的總體分配和任務角色的資訊，請參閱 [管理任務上的用戶和角色分配時數](../../manage-work/tasks/assign-tasks/manage-allocation-hours-on-tasks.md). 您無法更新用戶和作業角色的整體分配以解決問題。

您可以在Adobe Workfront的下列區域顯示使用者配置：

* 在「資源」區域的「計畫」部分。
* 在專案的「排程」區段上（在排程單一專案的資源時）。
* 在團隊的「排程」區段上（為團隊排程資源時）。

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
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>工作或更高</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級*</td> 
   <td> <p>查看或更高程度地訪問項目、任務和問題</p> <p><b>附註</b>

如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何變更您的存取層級的詳細資訊，請參閱 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>為專案、工作和問題貢獻權限</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 在「排程」區域中的使用者分配

開始依本文所述將時間分配給使用者之前，請先熟悉資源排程在Workfront中的運作方式，如 [開始使用資源計畫](../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md).

您可以為您所屬的單個團隊、您是項目團隊成員的單個項目或您是資源管理器的多個項目安排資源以處理任務和問題。

以下幾節說明如何在Workfront中啟用和管理使用者分配：

* [使用計畫區域來分配工作](#use-the-scheduling-areas-to-assign-work)
* [在「編輯任務」或「編輯問題」框中設定的分配與在「計畫」區域中設定的分配](#allocations-set-on-the-edit-task-or-the-edit-issue-boxes-vs-in-the-scheduling-areas)
* [分配指標](#allocation-indicators)
* [計畫小時數的預設分配](#default-allocation-for-planned-hours)
* [誰可以查看和修改分配？](#who-can-view-and-modify-allocations)
* [排程區域中的時區考量事項](#time-zone-considerations-in-the-scheduling-areas)

### 使用計畫區域來分配工作 {#use-the-scheduling-areas-to-assign-work}

在計畫時間表上為用戶分配新工作時，您可以確定如何為任務或問題分配計畫小時數給用戶。\
如需「計畫小時數」的詳細資訊，請參閱 [計畫小時數概觀](../../manage-work/tasks/task-information/planned-hours.md).

「計畫小時數」可分為以下幾種：

* 在被指派給任務或問題的用戶中
* 任務或問題的整個期間\
   例如，與銷售相關的任務可能需要在任務持續時間結束前完成更多工作。 您可以在任務中規劃這種不均勻的小時分配。

>[!TIP]
>
>從「計畫」區域為多個項目計畫資源時，並非所有用戶和工作項都顯示在「計畫」時間軸上。 如需排程時間表上顯示哪些資訊的相關資訊，請參閱 [開始使用資源計畫](../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md).

### 在「編輯任務」或「編輯問題」框中設定的分配與在「計畫」區域中設定的分配 {#allocations-set-on-the-edit-task-or-the-edit-issue-boxes-vs-in-the-scheduling-areas}

您可以從Workfront內的以下位置修改任務或問題的用戶分配：

* 排程時間表\
   排程時間軸位於下列區域：

   * 在「資源」區域的「計畫」部分。
   * 在專案的「排程」區段上（在排程單一專案的資源時）。
   * 在團隊的「排程」區段上（為團隊排程資源時）。

   當您從計畫時間軸修改用戶分配時(如 [修改用戶分配](#modify-user-allocations) 部分)，您可以為每個用戶定義任務或問題的分配，以及任務或問題持續時間內的每一天。\
   ![scheduling_contours.png](assets/scheduling-contours-350x139.png)

* 編輯任務或編輯問題對話框。\
   從「編輯任務」或「問題」對話框修改用戶分配時(如 [管理任務上的用戶或角色分配百分比](../../manage-work/tasks/assign-tasks/manage-allocation-percentage-on-tasks.md))，您可以為任務定義分配，或僅為每個使用者定義整體分配。 如果要每天管理這些分配，則必須按 [修改用戶分配](#modify-user-allocations) 一節。

   >[!IMPORTANT]
   >
   >從「編輯任務」或「問題」對話框修改用戶分配時，將覆蓋以前在「計畫時間軸」中配置的分配。 此外，您對「計畫時間軸」中的分配所做的任何更改都不會反映在「編輯任務」或「問題」對話框中。

建議您從「排程」時間軸（而非「編輯任務」或「問題」）管理用戶分配，以便從以下優勢中受益：

* 您可以清楚了解使用者何時使用分配指標進行過度配置，如 [分配指標](#allocation-indicators) 區段。
* 您可以為一個使用者分配更多時間給另一個使用者。\
   分配指標提供如何比較分配的用戶與其他用戶的直觀表示，如 [分配指標](#allocation-indicators) 區段。

* 您可以為某一天的工作分配更多時間，而不是另一天。\
   分配指標提供分配使用者在指定日期的方式的視覺表示，如 [分配指標](#allocation-indicators).

* 您可以在「計畫」時間表的一個位置執行所有資源分配責任。

### 分配指標 {#allocation-indicators}

各種視覺指標可用於提供關於用戶被分配到某一天工作的級別的快速資訊。

您的系統管理員決定Workfront如何計算系統層級的使用者可用性（考慮小時數和FTE可用性）。 根據此系統範圍的設定，使用預設計畫或用戶的計畫來計算用戶可用性。 如需詳細資訊，請參閱 [配置Workfront如何計算計畫區域的資源小時數和FTE可用性](../../resource-mgmt/resource-scheduling/calculate-hours-fte-scheduling-area.md).

* **分配底紋**
以底紋形式在指派給使用者的工作上以視覺方式顯示配置。 深色底紋表示分配的小時數佔指定日分配用戶FTE（相當於全職）的百分比。 (如需如何在Workfront中設定FTE的詳細資訊，請參閱 [配置Workfront如何計算計畫區域的資源小時數和FTE可用性](../../resource-mgmt/resource-scheduling/calculate-hours-fte-scheduling-area.md).)\
   例如，將單個用戶分配給具有4個計畫小時和1天持續時間的任務。 用戶的FTE在系統中定義為1（這表示用戶被安排以全時狀態工作，或者每週40小時或每天8小時）。 指定日期上任務的底紋佔任務垂直空間的一半，這表示用戶在該日被分配了其FTE（4小時）的一半。\
   ![](assets/scheduling-shading-allocation.png)\
   任務或問題將顯示分配給工作項的所有用戶的累計分配。 您可以展開工作項目以查看更多詳細資訊，包括分配給該工作項目的人員以及每個用戶被分配的小時數。\
   底紋不會顯示在 **未指派** 排程時間軸上的區域。\
   ![resource_allocation_expanded.png](assets/resource-allocation-expanded-350x192.png)

* **每位使用者的每日總計：** 您可以顯示每天分配給指定用戶的總計畫時數。 此資訊會顯示在排程時間軸上每個使用者列的頂端。 預設不會顯示此資訊。 您可以依照 [啟用用戶分配](#enable-user-allocations). 決定每日總計時，會納入下列任何狀態之專案的工作：當前、計畫或已批准。\
   ![resource_daily_totas.png](assets/resource-daily-totals-350x55.png)

* **超額分配指標**
當指定日分配給用戶的計畫小時數總數超過用戶一天中工作的小時數（跨所有任務）時，該用戶在該日被視為被過度分配。\
   當使用者被過度配置時，會顯示紅色列，概述當天的每個任務。\
   決定使用者的超額分配時，會納入下列任何狀態之專案的工作：當前、計畫或已批准。\
   用戶一天中的工作小時數通過每個用戶配置檔案中的FTE欄位定義，如中所述 [配置Workfront如何計算計畫區域的資源小時數和FTE可用性](../../resource-mgmt/resource-scheduling/calculate-hours-fte-scheduling-area.md).\
   ![resource_over_allocation.png](assets/resource-over-allocation-350x72.png)\
   當您啟用 **顯示每日計畫小時數總計** 和 **顯示資源分配突出顯示** 選項，當使用者被過度分配時，每日總計計畫小時數會以紅色顯示。 預設會將小時數顯示為最接近的十（例如1.3）。\
   ![RS_planned_hours_in_red_with_decimals__1_.png](assets/rs-planned-hours-in-red-with-decimals--1--350x56.png)

### 計畫小時數的預設分配 {#default-allocation-for-planned-hours}

Workfront會嘗試在指派的使用者和天數之間分配計畫小時數，如下所示：

* 將多個使用者指派給任務或問題時，小時數會平均分配給使用者。\
   分配將反映已對任務進行的任何高級分配。\
   有關高級分配的詳細資訊，請參閱 [建立高級分配](../../manage-work/tasks/assign-tasks/create-advanced-assignments.md).

* 當任務或問題的持續時間跨越多天時，計畫小時數在各天之間以及根據用戶的計劃分配給任務的所有用戶之間平均分配。
* 當任務的「計畫小時數」跨越多天時，從不同時區查看任務的用戶可能會看到任務持續時間或計畫起始日期或計畫完成日期中的差異。

小時數預設會顯示為最接近的百位數（例如1.33）。 您可以捲動至右側以查看更多資訊。\
![RS_Planned_Hours_with_two_decimals_in_contour_screen__1___1_.png](assets/rs-planned-hours-with-two-decimals-in-contour-screen--1---1--350x252.png)

### 誰可以查看和修改分配？ {#who-can-view-and-modify-allocations}

下列類型的使用者可在Workfront中檢視或修改使用者配置：

* **資源管理器：** 您可以查看和修改任何項目上任務和問題的用戶分配，而您是其資源管理員。 您可以在「人員」區域的「計畫時間軸」或項目的「人員配置」頁簽中執行此操作。\
   有關資源管理器如何對各個項目的任務和問題進行更改的資訊，請參見 [在「計畫」區域中手動分配未分配的任務和問題](../../resource-mgmt/resource-scheduling/manually-assign-items-scheduling-areas.md).

* **計畫和工作用戶：** 通過使用新的「我的工作日曆」或您所屬團隊的「工作日曆」，您可以查看分配給您的任何任務和問題的分配。\
   除了查看分配外，如果您具有任務和問題的Contribute訪問權限，則可以修改分配。

   <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  (NOTE: Article is conditioned to classic.)
  </MadCap:conditionalText>
  -->

### 排程區域中的時區考量事項  {#time-zone-considerations-in-the-scheduling-areas}

在少數情況下，檢視排程時間軸的使用者可能會看到不一致的情況，即任務的計畫小時數不等於個別天的分配總小時數。 當一個用戶的作業系統時區設定使得「計畫起始日期」或「計畫完成日期」與另一個用戶不同時，就會發生這種情況。

例如，如果任務的「計畫完成日期」在11/3/18, MST設定為上午11:00，則澳大利亞的查看任務的用戶將在11/4/18的上午1:00看到計畫完成日期，即第二天。 如果澳大利亞的用戶在11/4/18上分配小時，則MST上的用戶將看不到這些分配小時。 不過，這些小時一律會納入專案的「計畫小時數」中。

## 啟用用戶分配 {#enable-user-allocations}

預設會在排程時間軸上停用使用者分配功能。 您必須先啟用，才能使用本節所述的使用者分配功能。

>[!NOTE]
>
>只有在將計畫時間表配置為使用計畫日期時，才能啟用用戶分配。 如果將計畫時間表配置為使用預計日期，則無法顯示用戶分配。 有關配置計畫時間軸以使用計畫日期或預計日期的詳細資訊，請參閱： [在排程區域中配置設定](../../resource-mgmt/resource-scheduling/configure-settings-scheduling-areas.md).

要在計畫時間表上啟用用戶分配，請執行以下操作：

1. 前往多個專案、個別專案或團隊的排程時間軸：

   * **適用於多個專案**:  按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Workfront的右上角，按一下 **資源配置>工作負載平衡器**，然後選取 **排程** 的下拉式功能表。
   * **針對個別專案**:前往專案，按一下 **工作負載平衡器** 區段，然後選取 **排程** 從左上角的下拉式功能表。
   * **團隊**:按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Workfront的右上角，然後按一下 **團隊**，選取團隊，按一下&#x200B;**工作負載平衡器** 在左側面板中，選取&#x200B;**排程** 從左上角的下拉式功能表。

   ![](assets/scheduling-tab-global-resourcing-area-nwe-350x145.png)

1. 按一下 **設定** 圖示。\
   ![scheduling_settings_icon.png](assets/scheduling-settings-icon-350x169.png)\
   將顯示「資源計畫設定」對話框。\
   ![RS_scheduling_tab_all_settings__4_.png](assets/rs-scheduling-tab-all-settings--4--350x348.png)

1. 啟用以下一個或兩個選項，以在計畫時間表上顯示用戶分配：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">顯示資源配置醒目提示</td> 
      <td> <p>在排程時間軸上顯示任務和問題的使用者配置底紋。 </p> <p>預設會停用此選項。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">顯示每日計畫時數總計</td> 
      <td>顯示在計畫時間表上分配給每個用戶的每天計畫小時總數。 「計畫時數」會顯示到最接近的十分（例如1.3）。<br>預設會停用此選項。</td> 
     </tr> 
    </tbody> 
   </table>

1. （選用）在 **包含問題** 區段，選擇是否要在計畫時間表上顯示問題。\
   預設會停用此選項。

1. 按一下 **返回計畫**.\
   使用者分配現在會顯示在排程時間表上。\
   ![RS_daily_planned_totals_and_allocation_highlighting__1_.png](assets/rs-daily-planned-totals-and-allocation-highlighting--1--350x123.png)

## 修改用戶分配 {#modify-user-allocations}

您可以從「計畫時間軸」（如本節所述）或從「編輯任務」或「問題」對話框修改任務或問題的用戶分配。 如需詳細資訊，請參閱 [在「編輯任務」或「編輯問題」框中設定的分配與在「計畫」區域中設定的分配](#allocations-set-on-the-edit-task-or-the-edit-issue-boxes-vs-in-the-scheduling-areas).

依預設，使用者會平均分配給受分配者以及持續時間內的各天，如 [計畫小時數的預設分配](#default-allocation-for-planned-hours).

要從計畫時間表修改任務或問題的用戶分配，請執行以下操作：

1. 前往多個專案、個別專案或團隊的排程時間軸：

   * **適用於多個專案**:  按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Workfront的右上角，按一下 **資源配置>工作負載平衡器**，然後選取 **排程** 的下拉式功能表。
   * **針對個別專案**:前往專案，按一下 **工作負載平衡器** 區段，然後選取 **排程** 從左上角的下拉式功能表。
   * **團隊**:按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Workfront的右上角，然後按一下 **團隊**，選取團隊，按一下&#x200B;**工作負載平衡器** 在左側面板中，選取&#x200B;**排程** 從左上角的下拉式功能表。

   ![scheduling_contours.png](assets/scheduling-contours-350x139.png)

1. 確保在排程時間表上啟用使用者分配，如 [啟用用戶分配](#enable-user-allocations) 一節。
1. 展開您要管理使用者分配的任務。\
   預設情況下，「計畫小時數」在分配的用戶和任務持續時間的天數之間平均分配。 週末（星期六和星期日）不增加小時數。 如需詳細資訊，請參閱 [計畫小時數的預設分配](#default-allocation-for-planned-hours) 一節。

1. 按一下您要在指定日調整其小時數的使用者欄位。

   >[!NOTE]
   >
   >要在修改小時後維護原始分配，請按一下 **取消**.

1. 指定調整後的小時數。
1. 按一下&#x200B;**儲存**。\
   僅當任務的總小時數等於原始計畫小時數時，才能保存更改。 此數字會顯示在 **計畫小時數** 欄位。 當總計不等於總計畫小時數時，數字會以紅色顯示。\
   ![resource_allocation_expanded_modified.png](assets/resource-allocation-expanded-modified-350x226.png)

## 重設用戶分配的條件

Workfront會在任務或專案上發生許多動作時，重設您在排程時間軸中手動編輯的使用者分配。 一般而言，只要重新計算專案時間表時，如果此程式中的任務和問題的「計畫小時數」已變更，Workfront就會重設使用者分配。\
如需重新計算專案時間軸的詳細資訊，請參閱 [重新計算項目時間表](../../manage-work/projects/manage-projects/recalculate-project-timeline.md).

可能會在排程時間軸中重設使用者配置的一些最常見條件如下：

* 將任務添加到小版本。\
   由於迭代具有固定日期，因此會重新計算任務和分配的日期。\
   有關迭代如何影響任務日期的資訊，請參閱 [將動態添加到現有小版本](../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md).

* 將任務的「持續時間類型」更改為「工作驅動」。
* 將任務的「持續時間類型」更改為「計算分配」（當分配了1個以上人員時）。\
   有關任務持續時間的資訊，請參閱 [任務持續時間和持續時間類型概覽](../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

* 更改項目計劃開始日期和計畫完成日期。\
   有關項目計畫日期的資訊，請參閱 [項目計劃開始日期概覽](../../manage-work/projects/planning-a-project/project-planned-start-date.md) 和 [設定項目計畫完成日期](../../manage-work/projects/planning-a-project/project-planned-completion-date.md).

   有關任務計畫完成日期的資訊，請參閱 [任務計畫完成日期概覽](../../manage-work/tasks/task-information/task-planned-completion-date.md).

* 如果「任務約束」是彈性約束，則更改前置任務的日期。\
   例如，盡快或盡快。\
   有關任務約束的資訊，請參閱 [任務約束概覽](../../manage-work/tasks/task-constraints/task-constraint-overview.md).

* 更改計畫小時數的任務或問題數量。

   如需Workfront中「計畫小時數」的相關資訊，請參閱 [計畫小時數概觀](../../manage-work/tasks/task-information/planned-hours.md).
