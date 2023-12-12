---
content-type: overview
product-area: resource-management
navigation-topic: resource-management-overview
title: 開始使用資源管理
description: 「資源管理」可讓您設定系統，以根據資源的可用性來準確預測資源的使用，使必須完成的工作能準時且按預算完成。
author: Alina
feature: Resource Management
exl-id: b10ef503-60ea-4450-b63e-b2918e9bcc11
source-git-commit: dfd8dd07e1a88da872550163051e703f6aea5f74
workflow-type: tm+mt
source-wordcount: '1175'
ht-degree: 0%

---

# 開始使用資源管理

<!--
<p>(NOTE: DO NOT DELETE THIS ARTICLE. MANY ARTICLES MENTIONING RES MANAGEMENT ARE AND STILL SHOULD / WILL BE LINKED TO IT.) </p>
<p>(NOTE: Alina: ***As functionality is removed from Legacy and added to Res Planning - this will be continually updated: remove the Legacy Res Planning when that functionality is removed from the system.) </p>
</div>
-->

「資源管理」可讓您設定系統，以根據資源的可用性來準確預測資源的使用，使必須完成的工作能準時且按預算完成。

## Adobe Workfront中的資源管理概觀

「資源管理」是指由Adobe Workfront管理員、資源管理員和專案所有者執行的所有活動，以計畫（資源或案例計畫）和排程（工作負載平衡器）組織的資源，並將它們指派給需要完成的工作，同時考慮到它們的可用性。 此外，資源管理也指在報表檢視（「使用率報表」）中檢視有關計畫資源配置與實際資源配置的資訊。

Workfront有幾組用於管理資源的工具。 每個工具都有個別的範圍。 目前，您可以根據自己所處的資源管理階段，在Workfront中使用下列資源管理工具：

* 若要在專案的實際工作開始之前，計畫如何在較高層次配置資源，請使用下列工具：

   * **資源規劃工具**：您可以在資源管理的第一個階段中使用資源規劃工具，根據資源的已排程可用性來預算資源的專案時間。 在資源規劃階段中，您可以組織資源集區中的使用者，並將多個資源集區指定給專案。

     如需有關「資源規劃」的詳細資訊，請參閱區段 [Adobe Workfront中的資源規劃](../../resource-mgmt/resource-planning/resource-planning-overview.md).

   * **情境規劃工具**：這是資源的較高層級計畫，可讓您跨多個方案管理資源，這些方案可跨越一、三或五年計畫，並包含多個專案。 您可以善用最佳情境，以充分利用其可用性和預算。

     除了Workfront授權外，Scenario Planner還需要單獨的授權。 如需Workfront Scenario Planner的相關資訊，請參閱 [情境規劃工具概觀](../../scenario-planner/scenario-planner-overview.md).

     <!--   
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: when more functionality is added, maybe we add that we recommend to start here if this is available for them?!) </p>   
     -->

* 若要排程或指派資源給實際工作（任務和問題），請使用下列工具：

   * **工作負載平衡器**：這屬於資源管理的較低層級階段，您可以在此處根據完成資源所需的時數及其可用性，將資源指派給必須完成的實際工作（任務和問題）。 您可以使用工作負載平衡器將使用者指派給目前未指派或指派給工作角色的實際工作。

     如需Workfront平衡器的相關資訊，請參閱區段 [工作負載平衡器：文章索引](../../resource-mgmt/workload-balancer/workload-balancer.md).

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
* 若要分析多個專案的預算、計畫和實際配置，請使用以下工具：

   * **使用率報告**：此報表可檢視專案的資源使用率。 您可以比較專案的預算、計畫和實際分配，以及其對專案成本和收入的影響。

     如需「使用率報表」的相關資訊，請參閱 [檢視資源使用率資訊](../../resource-mgmt/resource-utilization/view-utilization-information.md).

## 資源管理程式的元件

>[!NOTE]
>
>在Workfront中，資源管理絕非停滯不前的程式。 隨著專案的排程、使用者的可用性或其角色變更，您必須持續調整有關資源、其指定以及其配置給專案、任務和問題的資訊。

在Workfront中管理資源的程式包括下列階段：

* **設定**：作為系統管理員、資源管理員或專案所有者，您必須在管理資源之前設定Workfront執行個體中的特定欄位和物件。 如需在Workfront中開始管理資源所需先決條件的詳細資訊，請參閱 [精確資源管理的先決條件](#prerequisites-for-accurate-resource-management) 一節。\
  除了讓專案包含工作專案之外，您還必須在Workfront中設定下列專案：

   * 使用者\
     如需建立使用者的詳細資訊，請參閱文章 [新增使用者](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

   * 職務角色\
     如需有關建立工作角色的詳細資訊，請參閱文章 [建立和管理職位角色](../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

   * 排程\
     如需建立排程的詳細資訊，請參閱文章 [建立排程](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

   * 專案偏好設定

     >[!TIP]
     >
     >只有系統或群組管理員才能修改您系統或您的群組的「專案偏好設定」。

     如需有關定義專案偏好設定的詳細資訊，請參閱文章 [設定全系統專案偏好設定](../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

   * 資源集區

     如需有關建立資源集區的詳細資訊，請參閱 [建立資源集區](../../resource-mgmt/resource-planning/resource-pools/create-resource-pools.md).

   * 資源管理喜好設定

     作為系統，您必須決定Workfront如何計算系統層級的使用者可用性，不論是使用使用者的排程還是您系統的「預設排程」。

     如需詳細資訊，請參閱 [設定資源管理喜好設定](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

* **資源配置**：身為資源管理員或專案所有者，您可以為專案定義資源配置並指派工作。 對於此步驟，您可以使用資源規劃工具或案例規劃工具管理資源的估計配置，並在工作負載平衡器中將實際工作指派給使用者。

  如需資源規劃與指派工作的詳細資訊，請參閱下列章節：

   * [Adobe Workfront中的資源規劃](../../resource-mgmt/resource-planning/resource-planning-overview.md)
   * [Adobe Workfront情境規劃工具](../../scenario-planner/scenario-planning.md)
   * [工作負載平衡器：文章索引](../../resource-mgmt/workload-balancer/workload-balancer.md)

<!--
* **Resource scheduling**: After generally planning for resources to use on your projects at a high level, you can start assigning work items (tasks and issues) to users based on their job roles using the Workload Balancer.

  For more information, see [Overview of the Workload Balancer](../workload-balancer/overview-workload-balancer.md). 
-->

* **分析**：身為資源管理員、專案所有者或人員管理員，請檢閱使用率報表，以瞭解資源的預算及計畫配置與實際配置的比較情形。 依時數、成本或收入複查資訊。 如需「使用率」報表的相關資訊，請參閱 [檢視資源使用率資訊](../../resource-mgmt/resource-utilization/view-utilization-information.md).

## 使用Workfront中的資源管理工具檢視和管理資源所需的存取權

下列使用者可以存取Workfront中的資源管理工具：

您必須是下列使用者之一，且具備下列存取許可權才能存取資源管理工具：

* 系統管理員。
* 擁有Plan授權的使用者。

  擁有工作授權的使用者可以使用專案的工作負載平衡器並管理指派和配置。

  除了擁有工作或更高的授權，您還必須具備下列專案才能使用特定的資源管理工具：

   * 編輯對資源管理的存取權（在工作負載平衡器中進行指派時不需要）
   * 編輯財務資料的存取權以在資源規劃工具中顯示成本資訊
   * 檢視財務資料的存取權，以檢視使用率報表中的成本與收入資訊（僅限擁有計畫授權的使用者）

* Contribute或更高的許可權，包括針對您想要管理資源的專案進行「工作分派」。

<!--
* Designated as a Resource Manager for projects to use the Scheduling tool (the Scheduling tool is deprecated).

  >[!TIP]
  >
  >You do not have to be a Resource Manager to use the Resource Planner, Scenario Planner, or the Workload Balancer. 
-->

如需有關預算資源所需存取權的資訊，請參閱文章 [預算資源所需的存取權](../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md).

如需有關管理工作負載平衡器中的資源所需存取許可權的資訊，請參閱 [管理工作負載平衡工具中的資源所需的存取權](../../resource-mgmt/workload-balancer/access-needed-manage-resources-balancer.md).

## 精確資源管理的先決條件  {#prerequisites-for-accurate-resource-management}

您必須符合一組需求，才能在Workfront中有效使用資源管理工具。

如需Workfront中每個資源管理工具的需求相關資訊，請參閱下列內容：

* 文章中「在資源規劃工具中工作的先決條件」一節 [資源規劃工具概觀](../../resource-mgmt/resource-planning/get-started-resource-planner.md).
  <!--remove this at production: * The section "Prerequisites" in the article [Get started with Resource Scheduling](../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md).-->
* 文章中「使用工作負載平衡器的最佳實務」小節 [工作負載平衡器概覽](../../resource-mgmt/workload-balancer/overview-workload-balancer.md).
* [在Adobe Workfront中預算資源所需的存取權](../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md).
* [管理工作負載平衡工具中的資源所需的存取權](../../resource-mgmt/workload-balancer/access-needed-manage-resources-balancer.md).

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
