---
product-area: resource-management;user-management
navigation-topic: resource-scheduling
title: 在「計畫」區域中手動分配未分配的任務和問題
description: 使用計畫時間軸，除了指定每個用戶為工作項分配的時間長度之外，您還可以管理用戶分配。
author: Alina
feature: Resource Management
exl-id: 627e4442-767a-41a2-9700-76f2ad2dc9cf
source-git-commit: f150c57e8b83e73734b1cbeded7ef4c16d65097c
workflow-type: tm+mt
source-wordcount: '1110'
ht-degree: 0%

---

# 在「計畫」區域中手動分配未分配的任務和問題

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

使用計畫時間軸，除了指定每個用戶為工作項分配的時間長度之外，您還可以管理用戶分配。

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

## 指派任務和排程時間表中問題的先決條件

開始如本節所述管理使用者指派之前，請先熟悉資源排程在Workfront中的運作方式，如 [開始使用資源計畫](../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md).

若要依照本節所述成功管理使用者指派，您必須先確定您、您的專案以及工作和問題符合 [使用Workfront中排程工具的必要條件](../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md#prerequisites) 文章一節 [開始使用資源計畫](../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md).

以下幾節說明如何手動、自動或按用戶或角色交換分配來修改用戶分配。

## 手動將未指派的任務或問題指派給使用者

排程時間表可提供所需的可見度，讓使用者能夠完成工作或問題。\
如需排程時間軸的詳細資訊，請參閱 [開始使用資源計畫](../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md).

您可以從Workfront的下列區域，在排程時間軸上將個別工作和問題指派給使用者：

* 「資源調度」下的「調度」部分（當為多個項目調度資源時）。
* 專案下的「排程」區段（在排程單一專案的資源時）。
* 團隊下的「排程」區段（為團隊排程資源時）。

排程時間軸頂端「未指派」區域中顯示的資訊會因您使用資源排程的Workfront區域(與「排程」區段（當為多個專案排程資源時）、「排程」區段（當為單一專案排程資源時）或「排程」區段（當為團隊排程資源時）而有所不同。 如需詳細資訊，請參閱 [「排程」區域中可用的功能](../../resource-mgmt/resource-scheduling/overview-scheduling-areas.md#functionality-available-in-the-scheduling-area) 在文章中 [排程區域概觀](../../resource-mgmt/resource-scheduling/overview-scheduling-areas.md).

根據您檢視排程時間軸的Workfront區域，可能只有部分使用者符合獲派工作的資格。 如需詳細資訊，請參閱 [排程區域概觀](../../resource-mgmt/resource-scheduling/overview-scheduling-areas.md).

要將未分配的任務或問題分配給調度時間表上的用戶，請執行以下操作：

1. 前往多個專案、個別專案或團隊的排程時間軸：

   * **適用於多個專案**:  按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Workfront的右上角，按一下 **資源配置>工作負載平衡器**，然後選取 **排程** 的下拉式功能表。
   * **針對個別專案**:前往專案，按一下 **工作負載平衡器** 區段，然後選取 **排程** 從左上角的下拉式功能表。
   * **團隊**:按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Workfront的右上角，然後按一下 **團隊**，選取團隊，按一下 **工作負載平衡器** 在左側面板中，選取 **排程** 從左上角的下拉式功能表。

   ![scheduling_contours.png](assets/scheduling-contours-350x139.png)

1. （選用）建立篩選器以自訂排程時間軸上顯示的內容，如 [篩選「排程」區域中的資訊](../../resource-mgmt/resource-scheduling/filter-scheduling-area.md) . [篩選「排程」區域中的資訊](../../resource-mgmt/resource-scheduling/filter-scheduling-area.md). 例如，對於要在排程時間軸上顯示的問題，您必須建立篩選器。

1. （可選）修改計畫時間表上顯示的日期範圍，如 [調整計畫區域的日期範圍](../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md#adjusting-the-date-range-for-which-data-is-displayed) in [開始使用資源計畫](../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md).

1. 執行以下操作以分配未分配的任務或問題：

   * 將任務或問題拖到要分配的用戶行。\
      指定使用者每天最多會顯示10個工作。 您可以展開清單以檢視目前指派給該使用者的所有工作。 （在排程時間軸上進行指派後，可能會暫時顯示超過10個任務。）\
      拖動項目時，在釋放任務或問題並完成分配之前將顯示以下資訊：

   * 如果在計畫時間表上啟用了用戶分配，則如果完成分配會導致用戶被過度分配，則會顯示紅色的過度分配指示符。\
      如需超額分配指標的詳細資訊，請參閱區段 [分配指標](../../resource-mgmt/resource-scheduling/manage-allocations-scheduling-areas.md#understanding-allocation-indicators) 在文章中 [在「計畫」區域中管理用戶分配](../../resource-mgmt/resource-scheduling/manage-allocations-scheduling-areas.md).

      若 **將分配限制為具有匹配角色的用戶** 「設定」區域中啟用「 」選項，但無資格接收指派的使用者將呈現灰色。 如果禁用此選項，則所有用戶都可接收分配。 依預設會啟用選項。\
      如需此選項的詳細資訊，請參閱 [](../../resource-mgmt/resource-scheduling/assignments-regardless-of-role-or-group-scheduling-areas.md#allowing-assignmennts-to-users-regardless-of-role) in [在「排程」區域中，無論角色和群組成員資格為何，都允許指派使用者](../../resource-mgmt/resource-scheduling/assignments-regardless-of-role-or-group-scheduling-areas.md)

      下拉指示器顯示在用戶的行中。 這使您能夠在進行分配之前查看物料的分配位置。

      展開要指派的任務或問題，按一下 **分配** 欄位中，開始輸入要指派的使用者名稱，然後在下拉式清單中按一下該使用者的名稱。\
      ![schedule_task_expanded.png](assets/schedule-task-expanded-350x170.png)

1. （條件性）在將未分配的任務或問題分配給用戶後，您可能希望調整調度時間表上用戶之間的任務和問題的現有分配。 在計畫項目資源時（在「計畫」頁簽或「人員配備」頁簽上），只有具有相同任務角色的用戶才能接收分配。\
   要將任務或問題重新分配給其他用戶，請將任務從一個用戶的行拖到另一個用戶的行。
1. （選用）設定每個指派的使用者分配給任務或問題的小時數，如 [在「計畫」區域中管理用戶分配](../../resource-mgmt/resource-scheduling/manage-allocations-scheduling-areas.md) .
