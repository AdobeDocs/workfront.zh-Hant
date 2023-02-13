---
content-type: overview
product-area: resource-management
navigation-topic: resource-planning
title: 資源計畫員概覽
description: 您可以估計和預算資源分配給分配給它們的項目，並使用資源計畫器預測其可用性以供將來工作使用。
author: Alina
feature: Resource Management
exl-id: 06cd2226-f94d-4b6a-8692-6d35210782f2
source-git-commit: ec49a7d3adeb24c1b8df0ff5fafe650d18d92280
workflow-type: tm+mt
source-wordcount: '2077'
ht-degree: 0%

---

# 資源計畫員概覽

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(Alina: this used to be the beginning of Planning in the Resource Planner - consider restructuring it further? Merging some of this information with information about Understanding Navigation in the RP?!)</p>
-->

您可以估計和預算資源分配給分配給它們的項目，並使用資源計畫器預測其可用性以供將來工作使用。

如需Adobe Workfront中資源規劃的一般概覽，請參閱文章 [開始使用資源規劃](../../resource-mgmt/resource-planning/get-started-resource-planning.md).

## 資源計畫員概覽

您可以使用資源計畫員輕鬆了解用戶和職務角色的可用性，以及完成項目工作所需的計畫時間。 然後，您可以決定如何根據使用者的可用時間，在指派給的專案上分配使用者及其工作角色。

>[!IMPORTANT]
>
>您不能使用資源規劃器將實際工作（任務和問題）分配給用戶。 您只能估計完成項目所需的用戶或作業角色時間，而不考慮其被分配的任務和問題。\
>要將實際工作分配給用戶，必須使用工作負載平衡器。 有關工作負載平衡器的詳細資訊，請參見 [工作負載平衡器概述](../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

您可以使用三個不同的視圖在資源計畫器中查看資訊。 您可以使用每個檢視來達成下列其中一個目的：

* 使用「項目」和「角色」視圖為需要完成的工作預算資源的時間或成本。 這是資源計畫員的主要用途。\
   有關資源計畫員中預算的詳細資訊，請參閱文章 [使用「項目」和「職責」視圖在資源計畫器中使用預算資源](../resource-planning/budget-resources-project-role-views-resource-planner.md).

* 要使用「用戶」視圖查看以下資訊：

   * 根據用戶的日程安排提供用戶
   * 根據項目計畫完成工作所需的計畫時間。
   * 用戶已登錄實際工作項的時間。

   有關查看資源計畫員中用戶的可用小時數、計畫小時數和實際小時數或FTE的詳細資訊，請參閱文章 [使用「用戶」視圖時，查看資源計畫員中的可用小時數、計畫小時數和實際小時數或FTE](../../resource-mgmt/resource-planning/view-hours-fte-user-view-resource-planner.md#using).

## 資源計畫員考量事項

* 您可以對正在處理的項目進行優先排序，並根據其優先順序對資源分配進行預算，以確保首先將資源分配給最重要的項目。

   有關在資源計畫器中排定項目優先順序的資訊，請參閱 [在資源計畫器中排列項目優先順序](../../resource-mgmt/resource-planning/prioritize-projects-resource-planner.md).

* 您可以顯示項目任務和問題中的小時數、FTE和成本資訊。

   >[!NOTE]
   >
   >任務和問題不會顯示在資源計畫器中。 但是，任務上資源分配的小時數、FTE和成本資訊在資源計畫器中顯示為項目的總數。

* 來自父任務的小時、FTE和成本資訊將從顯示在資源計畫器中的項目中排除。 如果要在資源規劃器中管理這些資源的時間或成本，建議僅將資源分配給子任務。

   如需上層工作的相關資訊，請參閱下列文章：

   * [任務概述](../../manage-work/tasks/task-information/tasks-overview.md)
   * [建立子任務](../../manage-work/tasks/create-tasks/create-subtasks.md)

   >[!TIP]
   >
   >父任務顯示子任務的總小時數和成本。 因此，從子任務和父任務計算小時數、FTE和成本將計算兩次這些金額。 這就是為什麼從資源計畫器中排除父任務資訊的原因。

* 您無法管理在資源計畫員中具有任務或問題的項目上的團隊分配。
* 您可以使用資源計畫員一次為多個項目預算資源，或使用業務案例的「資源預算」區域為單個項目預算資源。 您為一個項目預算的資訊也會顯示在資源計畫器中。

   如需如何為單一專案預算資源的相關資訊，請參閱文章 [業務案例中的預算資源](../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md).

   有關如何在資源計畫器中為一次多個項目預算資源的資訊，請參閱文章中的「資源計畫器中的預算資源」部分 [使用「項目」和「職責」視圖在資源計畫器中使用預算資源](../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md).

## 在資源規劃器中工作的先決條件 {#prerequisites-for-working-in-the-resource-planner}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(<b>THIS SECTION IS LINKED TO ALL RES PLANNING ARTICLES. DO NOT RENAME OF DELETE THIS!</b> - do NOT ADD the variable here, because it might break this link!)</p>
-->

要成功使用資源計畫器來對資源進行預算，您必須首先確保您、項目和任務符合一組先決條件。 這些先決條件是在資源規劃器中顯示正確資訊和準確管理資源的必備條件。

>[!IMPORTANT]
>
>如果缺少下列任一先決條件，您可能會發現缺少有關配置或資源可用性的某些資訊，或該資訊的值為零。\
>如需了解欄位為何遺失資料或有零值的詳細資訊，請將滑鼠移至欄位上。

![](assets/no-users-with-this-role-in-the-res-pool-350x57.png)

>[!NOTE]
>
>只有在按項目或任務職責查看資源計畫員時，或在項目的業務案例中預算資源時，才需要滿足以下先決條件。

按項目或按角色查看資源計畫器時，需要以下類型的必要條件，才能使資源計畫器的正確功能：

* [使用者必要條件](#user-prerequisites)
* [專案必要條件](#project-prerequisites)
* [工作和問題必要條件](#tasks-and-issues-prerequisites)
* [系統級先決條件](#system-level-prerequisites)

### 使用者必要條件 {#user-prerequisites}

開始使用資源計畫器之前，請確保存在以下用戶設定：

* 您有正確的預算資源存取權。

   如需存取預算資源所需權限的相關資訊，請參閱文章 [獲得Adobe Workfront預算資源所需資源](../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md).

* 分配給任務的用戶將添加到與項目關聯的資源池中。

   有關將用戶添加到資源池的資訊，請參見 [將資源池與用戶關聯](../../resource-mgmt/resource-planning/resource-pools/associate-resource-pools-with-users.md).

   >[!NOTE]
   >
   >當未將用戶添加到資源池時，可能存在以下情況：
   >
   >   
   >   
   >   * 雖然用戶可能被分配給項目上的任務，但這些用戶不會顯示在資源計畫器中。
   >   * 如果與之關聯的任務具有計畫小時數，則這些小時數不會在資源計畫員中顯示項目，除非用戶也與這些任務上的任務職責相關聯。
   >   * 如果用戶與項目上某個任務的任務職責相關聯，則「計畫小時數」將顯示在任務職責的「資源計畫員」中，但無法編入任務職責的預算。


* 分配給工作和資源池的用戶必須具有與其配置檔案關聯的調度和作業角色。

   有關將計畫和作業角色與用戶關聯的資訊，請參閱 [編輯使用者的設定檔](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

   >[!NOTE]
   >
   >未與計畫關聯但位於項目資源池中的用戶無法在資源計畫器中進行預算。

* 要獲得準確的「可用小時數」資訊，請確保與用戶關聯的計畫具有計畫例外和更新時間。

   >[!NOTE]
   >
   >如果用戶未與計畫關聯，則預設情況下，為了資源計畫員的目的，Workfront系統的預設計畫將與用戶關聯。

   如需建立排程的詳細資訊，請參閱文章 [建立排程](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

* 如果要按成本對資源進行預算，則必須將任務職責與成本/人力資源關聯。 比率。 與資源池中分配給用戶的職務職責關聯的成本用於計算項目的預算人工成本和預算成本。\
   有關將職務職責與費率關聯的資訊，請參閱文章 [建立和管理作業角色](../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).\
   有關計算預算人工成本的資訊，請參閱文章 [了解項目的預算人工成本和預算工時](../../manage-work/projects/project-finances/budgeted-labor-cost.md).\
   有關計算預算成本的資訊，請參閱文章 [計算預算成本](../../manage-work/projects/project-finances/budgeted-cost.md).

### 專案必要條件 {#project-prerequisites}

開始使用資源計畫員之前，請確保存在以下項目設定：

* 您的項目與資源池相關聯。\
   有關向項目添加資源池的詳細資訊，請參見 [將資源池與項目和模板關聯](../../resource-mgmt/resource-planning/resource-pools/associate-resource-pools-with-projects-and-templates.md).

   >[!IMPORTANT]
   >
   >沒有資源池的項目在資源計畫器中不顯示計畫小時或分配資訊。

### 工作和問題必要條件 {#tasks-and-issues-prerequisites}

雖然您不能在資源計畫員中顯示任務和問題，但它們的資訊將傳輸到顯示在資源計畫員中的項目。

在Oracle Resource Planner中啟動預算資源之前，請確保存在以下任務和問題設定：

* 要為其分配預算資源的項目的任務或問題將分配給以下實體之一：

   * 項目資源池中同時與作業角色關聯的用戶
   * 職務角色

   >[!NOTE]
   >
   >分配給任務職責的「計畫小時數」任務和問題顯示在「資源計畫員」中，但除非與任務職責關聯的用戶在與項目關聯的資源池中列出，否則無法預算這些小時數。

* 不應將父任務分配給用戶或角色。

   要在資源規劃器中顯示與父任務關聯的用戶或角色的小時資訊，您還必須將其分配給子任務。 資源計畫器不顯示父任務的資訊。

* 任務和問題的「計畫小時數」值大於零。
* 任務和問題的「持續時間」值大於零。
* 問題的計畫日期在項目時間表內。

### 系統級先決條件 {#system-level-prerequisites}

您必須了解Workfront實例如何根據系統中的資源管理首選項計算用戶可用性。 Workfront可使用使用者設定檔頁面中定義的使用者排程，或您系統的預設排程，來計算使用者可用性。

![](assets/resource-management-preferences-section-in-setup-350x89.png)

您的Workfront管理員將配置您的資源管理首選項。

如需詳細資訊，請參閱 [配置資源管理首選項](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

## 查找資源計畫員

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(This became another standalone article; drfat this section here when article is live.)</p>
-->

您可以在Workfront的兩個區域中查找資源計畫器，具體取決於您要為多個項目或僅一個項目預算資源。

有關查找資源計畫員的資訊，請參閱 [查找資源計畫員](../../resource-mgmt/resource-planning/locate-resource-planner.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(this is drafted and moved to its own article: locate-resource-planner) </p>
<p>Ensure that all prerequisites are met before starting to use the Resource Planner. This way, you ensure that the Resource Planner displays the correct information before you start budgeting your resources.<br>For information about the prerequisites that must be met before you can start using the Resource Planner, see the <a href="#prerequisites-for-working-in-the-resource-planner" class="MCXref xref">Prerequisites for working in the Resource Planner</a> section in this article. </p>
<p>You can locate the Resource Planner in two areas of Workfront, depending on whether you want to budget your resources for multiple projects, or for just one project.</p>
<ul>
<li><a href="#use-the-resource-planner-for-multiple-projects" class="MCXref xref">Use the Resource Planner for multiple projects</a> </li>
<li> <p><a href="#use-the-resource-planner-for-one-project" class="MCXref xref">Use the Resource Planner for one project</a> </p> </li>
</ul>
<p><strong>Use the Resource Planner for multiple projects</strong></p>
<p>When using the Resource Planner for multiple projects, the allocation numbers for your resources represent numbers across multiple projects. </p>
<p>To access the  Planner section  in the  Resourcing area: </p>
<ol>
<li value="1">  Click the <strong>Main Menu</strong> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of Adobe Workfront.  </li>
<li value="2"> <p>  Click <strong>Resourcing</strong>. The Resource Planner displays by default.  For information about budgeting resources in the Resource Planner, see the article <a href="../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md" class="MCXref xref">Budget resources in the Resource Planner using the Project and Role views</a>. </p> <p> <img src="assets/qs-resource-management-area-with-planner-as-default-350x152.png" style="width: 350;height: 152;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> </p> </li>
<li value="3">  Hover over the left panel, and click <strong>Resource Pools</strong>. <br>For information about creating new resource pools, see <a href="../../resource-mgmt/resource-planning/resource-pools/create-resource-pools.md" class="MCXref xref">Create resource pools</a>.</li>
</ol>
<p><strong>Use the Resource Planner for one project</strong></p>
<p>When using the Resource Planner for one project, the allocation numbers for your resources represent numbers for the selected project. </p>
<ol>
<li value="1"> <p>Go to a project you want to budget resources for.</p> </li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click <strong>Business Case</strong> in the left panel.</p> </li>
<li value="3"> <p>Scroll to the <strong>Resource Budgeting</strong> section of the Business Case.</p> </li>
<li value="4"> <p>Click <strong>Edit Resource Budgeting</strong> to add resource pools to your project and start budgeting your resources. </p> <note type="tip">
You can only add a resource pool in the Resource Budgeting area of the Business Case when the project has no resource pools associated with it. When the project already has a resource pool, the users in the pool and their job roles display in the Resource Budgeting area by default.
</note> <p> <img src="assets/resource-budgeting-area-on-project-350x70.png" style="width: 350;height: 70;"> </p> <p>For information about budgeting resources for one project, see the article <a href="../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md" class="MCXref xref">Budget resources in the Business Case</a>.</p> </li>
</ol>
</div>
-->

## 資源計畫員的區域

您可以在資源計畫員中查看以下資訊或執行以下活動：

* 有關在一般時間表中分配給資源計畫器中項目的資源的資訊。
* 在資源計畫器中資源的過度分配或利用率不足。
* 手動或自動為資源預算工作。

有關在資源規劃器中顯示哪些區域以及如何配置在這些區域中顯示哪些資訊的詳細資訊，請參閱文章 [資源計畫員導航概覽](../../resource-mgmt/resource-planning/resource-planner-navigation.md).

## 在資源計畫器中顯示資訊時的限制

為了改進效能，Workfront限制了可在資源計畫器中顯示的物料數量。

如需這些限制的詳細資訊，請參閱文章 [資源計畫器顯示限制](../../resource-mgmt/resource-planning/resource-planner-display-limitations.md) .

## 在資源計畫員中計算FTE

您可以按小時數、FTE或成本在資源計畫員中顯示可用性、分配和計畫值。

有關更改在資源計畫器中顯示的資訊的詳細資訊，請參閱：部分 [按小時、FTE或成本查看資訊](../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md#display-by-hour-or-fte-menu) 在文章中 [使用Adobe Workfront資源計畫器複查資源可用性和分配](../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md).

有關如何在Workfront中計算使用者和角色的小時數和FTE的詳細資訊，請參閱文章 [在資源計畫員中計算用戶和角色的小時數和FTE的概覽](../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md).

## 在資源計畫器中計算成本

您必須具有查看財務資料的訪問權限和查看項目的財務權限，才能按成本在資源計畫器中查看資訊。

除了以小時數和FTE在資源計畫員中顯示可用性、分配和計畫值外，您還可以按成本顯示它們。

>[!TIP]
>
>您必須將用戶和職務職責與每小時成本費率關聯，以便按成本在資源計畫器中顯示資訊。

有關將「每小時成本」費率與職務職責關聯的詳細資訊，請參閱文章 [建立和管理作業角色](../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).\
有關將「每小時成本」費率與用戶關聯的詳細資訊，請參閱文章 [編輯使用者的設定檔](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

在資源計畫器中按成本查看資訊時，請考慮以下事項：

* 每種類型的小時（計畫、可用、預算、用戶、角色或項目的實際）的成本使用不同的成本率計算。
* 計畫成本受項目任務的成本類型影響。
* 在將「用戶視圖」應用到資源計畫員時，您無法按成本顯示分配和可用性資訊。

有關如何在資源計畫器中計算用戶和職責的成本的詳細資訊，請參閱文章 [在資源計畫器中計算成本](../../resource-mgmt/resource-planning/calculate-costs-resource-planner.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Use the User View to view Available, Planned, and Actual Hours or FTE </h2>
<p>(this information is repeated from above where it exists in shorter form. Drafted to simplify the amount of info of this article.) </p>
<p>You can use the User View of the Resource Planner to display information about the Planned, Available, and Actual Hours or FTE values for projects and resources. </p>
<p>For information about using the Resource Planner to review the Available, Planned, and Actual Hours and FTE for resources, see the article <a href="../../resource-mgmt/resource-planning/view-hours-fte-user-view-resource-planner.md" class="MCXref xref">View Available, Planned, and Actual Hours or FTE in the Resource Planner when using the User view</a>.</p>
<p><strong>Use the Project and Role Views to budget resources </strong></p>
<p> The main function of the Resource Planner is to budget your resources for the work that needs to be completed on the projects that you can manage. </p>
<p> You can budget your resources only if you apply the <strong>View by Project</strong> or <strong>View by Role</strong> views to the Resource Planner.</p>
<p>For information about budgeting resources using the Project and Role views in the Resource Planner, see the article <a href="../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md"><a href="../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md" class="MCXref xref">Budget resources in the Resource Planner using the Project and Role views</a></a>.</p>
</div>
-->

## 在資源計畫器中篩選資訊

您可以通過建立篩選器來減少在資源計畫器中顯示的項目、角色或用戶數。\
如需詳細資訊，請參閱文章 [在資源計畫器中篩選資訊](../../resource-mgmt/resource-planning/filter-resource-planner.md).
