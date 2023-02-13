---
content-type: overview
product-area: resource-management
navigation-topic: resource-management-overview
title: 開始使用資源管理
description: Oracle Resource Management允許您配置系統，以根據資源的可用性準確預測資源的使用情況，以便按時和按預算完成必須完成的工作。
author: Alina
feature: Resource Management
exl-id: b10ef503-60ea-4450-b63e-b2918e9bcc11
source-git-commit: f150c57e8b83e73734b1cbeded7ef4c16d65097c
workflow-type: tm+mt
source-wordcount: '1171'
ht-degree: 0%

---

# 開始使用資源管理

<!--
<p>(NOTE: DO NOT DELETE THIS ARTICLE. MANY ARTICLES MENTIONING RES MANAGEMENT ARE AND STILL SHOULD / WILL BE LINKED TO IT.) </p>
<p>(NOTE: Alina: ***As functionality is removed from Legacy and added to Res Planning - this will be continually updated: remove the Legacy Res Planning when that functionality is removed from the system.) </p>
</div>
-->

Oracle Resource Management允許您配置系統，以根據資源的可用性準確預測資源的使用情況，以便按時和按預算完成必須完成的工作。

## Adobe Workfront資源管理概述

資源管理指由Adobe Workfront管理員、資源管理器和項目所有者執行的所有活動，以規劃（資源或方案規劃）和計畫（工作負載平衡器）組織的資源，並將其分配給需要完成的工作，同時考慮其可用性。 此外，資源管理還指在報告視圖（利用率報告）中查看有關計畫和實際資源分配的資訊。

Workfront提供數套管理資源的工具。 每個工具都有個別的範圍。 目前，您可以在Workfront中使用以下資源管理工具，具體取決於您處於哪個資源管理階段：

* 要在項目的實際工作開始之前計畫如何在更高級別分配資源，請使用以下工具：

   * **資源計畫員**:您可以在資源管理的第一階段使用資源計畫器，根據資源的計畫可用性來預算資源的項目時間。 在資源階段的規劃期間，您可以在資源池中組織用戶，並為項目分配多個資源池。

      有關資源計畫的詳細資訊，請參見 [Adobe Workfront資源規劃](../../resource-mgmt/resource-planning/resource-planning-overview.md).

   * **方案計畫員**:這是一個更高級別的資源規劃，允許您跨多個計畫管理這些資源，這些計畫可跨一年、三年或五年計畫，並包括多個項目。 您可以使用最佳方案來充分利用其可用性和預算。

      除了Workfront許可證外，方案規劃器還需要單獨的許可證。 有關Workfront方案計畫器的資訊，請參閱 [方案計畫員概覽](../../scenario-planner/scenario-planner-overview.md).

      <!--   
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: when more functionality is added, maybe we add that we recommend to start here if this is available for them?!) </p>   
     -->

* 要計畫或分配資源給實際工作（任務和問題），請使用以下工具：

   * **工作負載平衡器**:這屬於資源管理的較低級別，您可以根據完成這些任務所需的小時數及其可用性，將資源分配給必須完成的實際工作（任務和問題）。 使用工作負載平衡器，可以將用戶分配給當前未分配或分配給作業角色的實際工作。

      有關Workfront平衡器的資訊，請參見 [工作負載平衡器](../../resource-mgmt/workload-balancer/workload-balancer.md).

<!--

  * **Scheduling** (deprecated <span class="preview">and removed from the Preview environment</span>): Refers to assigning actual work to users by matching the job roles assigned to the tasks and issues with the job roles they can fulfill, or assigning actual work to users on tasks and issues which are currently unassigned. This happens at a lower-level in the process of managing resources, where you can assign your resources to the actual work (tasks and issues) that they must fulfill, according to the hours needed in the project plan to fulfill them.  

     For more information about resource scheduling, see the section [Resource Scheduling](../../resource-mgmt/resource-scheduling/resource-scheduling-overview.md).

    >[!CAUTION]
    >
    >
    >We are no longer supporting the Resource Scheduling tools and they will be removed from Workfront in **January 2023**. We recommend that you use the Workload Balancer for scheduling your resources. 
    >
    >
    >* For information about scheduling resources using the Workload Balancer, see the section [The Workload Balancer](../../resource-mgmt/workload-balancer/workload-balancer.md).
    >
    >
    >* For more information about the timeline for removing the Resource Scheduling tools and replacing them with the Workload Balancer, see [Deprecation of Resource Scheduling tools in Adobe Workfront](../../resource-mgmt/resource-mgmt-overview/deprecate-resource-scheduling.md).

-->
* 要分析多個項目的預算分配、計劃分配和實際分配，請使用以下工具：

   * **利用率報告**:使用此報告可以查看項目的資源利用率。 您可以比較項目的預算、計畫和實際分配及其對項目成本和收入的影響。

      有關「利用率報告」的資訊，請參閱 [查看資源利用資訊](../../resource-mgmt/resource-utilization/view-utilization-information.md).

## 資源管理流程的元件

>[!NOTE]
>
>在Workfront，資源管理從來不是一個停滯的過程。 隨著項目的計畫、用戶的可用性或角色的更改，您必須不斷調整有關資源、其分配和對項目、任務和問題的分配的資訊。

在Workfront中管理資源的程式包括下列階段：

* **設定**:作為系統管理員、資源管理器或項目所有者，您必須先在Workfront實例中配置某些欄位和對象，然後才能管理資源。 如需開始在Workfront中管理資源所需必要條件的詳細資訊，請參閱 [準確資源管理的先決條件](#prerequisites-for-accurate-resource-management) 一節。\
   除了有包含工作項目的專案外，您還必須在Workfront中設定下列項目：

   * 使用者\
      如需建立使用者的詳細資訊，請參閱文章 [新增使用者](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

   * 職務角色\
      如需建立工作角色的詳細資訊，請參閱文章 [建立和管理作業角色](../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

   * 排程\
      如需建立排程的詳細資訊，請參閱文章 [建立排程](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

   * 專案偏好設定

      >[!TIP]
      >
      >只有系統或組管理員可以修改系統或組的項目首選項。

      如需定義專案偏好設定的詳細資訊，請參閱文章 [配置系統範圍的項目首選項](../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

   * 資源集區

      有關建立資源池的詳細資訊，請參見 [建立資源池](../../resource-mgmt/resource-planning/resource-pools/create-resource-pools.md).

   * 資源管理首選項

      作為系統，您必須決定Workfront如何計算系統層級的使用者可用性，無論是使用者排程或系統的預設排程。

      如需詳細資訊，請參閱 [配置資源管理首選項](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

* **資源分配**:作為資源管理員或項目責任人，您可以為項目定義資源分配並分配工作。 對於此步驟，您可以使用資源計畫器或方案計畫器管理資源分配的估計值，並在工作負載平衡器中將實際工作分配給用戶。

   有關資源規劃和分配工作的詳細資訊，請參閱以下各節：

   * [Adobe Workfront資源規劃](../../resource-mgmt/resource-planning/resource-planning-overview.md)
   * [Adobe Workfront方案規劃器](../../scenario-planner/scenario-planning.md)
   * [工作負載平衡器](../../resource-mgmt/workload-balancer/workload-balancer.md)

<!--
* **Resource scheduling**: After generally planning for resources to use on your projects at a high level, you can start assigning work items (tasks and issues) to users based on their job roles using the Workload Balancer.

  For more information, see [Overview of the Workload Balancer](../workload-balancer/overview-workload-balancer.md). 
-->

* **分析**:作為資源經理、項目責任人或人員經理，請複查「利用率報表」，以了解資源的預算分配和計劃分配與實際資源分配的比較情況。 按小時數、成本或收入來查看資訊。 有關「利用率」報告的資訊，請參見 [查看資源利用資訊](../../resource-mgmt/resource-utilization/view-utilization-information.md).

## 使用Workfront中的資源管理工具查看和管理資源所需的訪問權

以下用戶可以訪問Workfront中的資源管理工具：

您必須是以下用戶之一，並且具有以下訪問權限和訪問資源管理工具的權限：

* 系統管理員。
* 具有計畫許可證的用戶。

   具有工作許可證的用戶可以使用項目的工作負載平衡器，並管理分配和分配。

   除了具有工作或更高的許可證外，您還必須具備以下條件才能使用特定資源管理工具：

   * 編輯對資源管理的訪問（在工作負載平衡器中進行分配時不需要）
   * 編輯對財務資料的訪問以在資源計畫器中顯示成本資訊
   * 查看對財務資料的訪問，以查看利用率報告中的成本和收入資訊（僅具有計畫許可證的用戶）

* 貢獻或更高權限，包括對您要管理資源的專案進行指派。

<!--
* Designated as a Resource Manager for projects to use the Scheduling tool (the Scheduling tool is deprecated).

  >[!TIP]
  >
  >You do not have to be a Resource Manager to use the Resource Planner, Scenario Planner, or the Workload Balancer. 
-->

如需存取預算資源所需權限的相關資訊，請參閱文章 [預算資源所需的訪問](../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md).

有關在工作負載平衡器中管理資源所需的訪問權限的資訊，請參見 [在工作負載平衡器中管理資源所需的訪問](../../resource-mgmt/workload-balancer/access-needed-manage-resources-balancer.md).

## 準確資源管理的先決條件  {#prerequisites-for-accurate-resource-management}

您必須先滿足一組需求，才能高效地使用Workfront中的資源管理工具。

有關Workfront中每個資源管理工具的要求的資訊，請參閱以下內容：

* 文章中的「在資源規劃器中工作的先決條件」部分 [資源計畫員概覽](../../resource-mgmt/resource-planning/get-started-resource-planner.md).

<!--remove this at production: * The section "Prerequisites" in the article [Get started with Resource Scheduling](../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md).-->
* 文章中的「使用工作負載平衡器的最佳做法」部分 [工作負載平衡器概述](../../resource-mgmt/workload-balancer/overview-workload-balancer.md).
* [獲得Adobe Workfront預算資源所需資源](../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md).
* [在工作負載平衡器中管理資源所需的訪問](../../resource-mgmt/workload-balancer/access-needed-manage-resources-balancer.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: drafted and replaced with the links to each prerequisites instead) </p>
<p> We recommend that the following settings exist before starting to manage resources for your organization: </p>
<ul>
<li> You must have users in the system who have active accounts. </li>
<li> You must assign a Plan or a Worker license to the users whose work allocation you want to manage. <note type="note">
Although you can assign work to a Reviewer or a Requestor, they cannot complete it.
<br>We recommend against assigning work to Reviewers or Requestors. For information about access levels in Workfront, see
<a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md" class="MCXref xref" xrefformat="{para}">Access levels overview</a>.
</note></li>
<li> You must have job roles configured in the system.<br>For information about adding job roles to Workfront, see the article <a href="../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref" xrefformat="{para}">Create and manage job roles</a>.</li>
<li> (Optional) If you want to budget cost for your work, your job roles and your users must also have rates associated with them.<br></li>
<li> You must associate at least one job role with your users. </li>
<li> You must specify a valid value for the FTE field of all users when you use the User's Schedule instead of The Default Schedule in your Resource Management system preferences. <br>For information about editing users to ensure they have a job role, FTE, or cost associated with them, see the article <a href="../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref" xrefformat="{para}">Edit a user's profile</a>. For information about editing the Resource Management preferences in your system, see <a href="../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref" xrefformat="{para}">Configure Resource Management preferences</a>.</li>
<li>You must associate accurate schedules with your users and they should include schedule exceptions.<br>For information about creating and editing schedules, see the article <a href="../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref" xrefformat="{para}">Create a schedule</a>.</li>
<li>The Time Off calendar of the users must be up to date. </li>
<li> <p>The following is recommended for the Resource Planner when applying the Project and Role views: </p>
<ul>
<li> <p>You must associate projects with Resource Pools.<br>For information about associating projects with Resource Pools, see <a href="../../resource-mgmt/resource-planning/resource-pools/associate-resource-pools-with-projects-and-templates.md" class="MCXref xref" xrefformat="{para}">Associate resource pools with projects and templates</a>.</p> </li>
</ul> </li>
<li> <p>Your must designate a Resource Manager on your projects and they must have the correct access to budget resources when using the Scheduling tools. </p> <p>For information about the access needed to budget resources, see the article <a href="../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md" class="MCXref xref" xrefformat="{para}">Access needed to budget resources in&nbsp;Adobe Workfront</a>.</p> </li>
<li> <p>You must assign the tasks and issues in your system to job roles, teams, or users.</p> </li>
<li>You must specify a valid value for Planned Hours and Duration for all tasks in your system.<br>For information about Planned Hours, see the article <a href="../../manage-work/tasks/task-information/planned-hours.md" class="MCXref xref" xrefformat="{para}">Planned Hours overview</a>.<br>For information about Duration, see the article <a href="../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref" xrefformat="{para}">Overview of Task Duration and Duration Type</a>.</li>
</ul>
</div>
-->
