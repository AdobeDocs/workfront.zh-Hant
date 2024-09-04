---
content-type: overview
product-area: resource-management
navigation-topic: resource-planning
title: 開始使用資源規劃
description: 您可以使用資源計畫工具來管理您的職務角色、其可用性，以及根據此可用性的一般專案配置。
author: Lisa
feature: Resource Management
exl-id: 0db9fbb3-4e94-47bd-b272-00b3ca4decaf
source-git-commit: a5317e3126939d4c648977635af2dbc6add02780
workflow-type: tm+mt
source-wordcount: '555'
ht-degree: 0%

---

# 開始使用資源規劃

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(**** THIS WILL BE LINKED TO THE PRODUCT UI IN THE PLANNER AREA***DO NOT DELETE OR CHANGE URL FOR THIS ARTICLE****) </p>
<p>(Alina ***Keep the pink blurb for all articles in this NEW section.***More prerequisites for Users (with later releases): - users have an accurate number for their FTE field; The Prerequisites section: (this is linked to other articles, do not change name and link/ anchor))</p>
</div>
-->

您可以使用Adobe Workfront資源管理工具來預測資源的配置，以便準確知道專案是否準時及符合預算。 如需Workfront的資源管理概觀，請參閱[開始使用資源管理](../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md)。

您可以使用資源計畫工具來管理您的職務角色、其可用性，以及根據此可用性的一般專案配置。

預算使用者對專案的一般配置不會將其指派給實際工作（任務和問題）。 您必須使用工作負載平衡器指派您的資源以進行工作。

如需使用工作負載平衡器在Workfront中排程資源的詳細資訊，請參閱[工作負載平衡器概覽](../workload-balancer/overview-workload-balancer.md)。

## Workfront中的資源規劃工具

若要針對您計畫指派給專案的資源，編列其預算時間，您可以使用下列工具：

* 若要在系統層次編列多重專案的預算分配，並設定其優先順序：請使用系統層次「資源規劃工具」。

  您可以前往「資源」區域中的規劃工具區段來存取資源規劃工具。

  如需資源規劃工具的相關資訊，請參閱[資源規劃工具概觀](../../resource-mgmt/resource-planning/get-started-resource-planner.md)。

* 針對單一專案的預算分配：使用專案之業務案例的「資源預算」區域中的專案層次資源規劃工具。 如需為一個專案編列預算資源的相關資訊，請參閱文章[商業案例中的預算資源](../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md)。

  若要根據共同技能或部門結構來管理使用者，並將他們組織到集區，然後管理他們指派給專案的配置，您必須建立資源集區。 如需有關建立資源集區的詳細資訊，請參閱[建立資源集區](../../resource-mgmt/resource-planning/resource-pools/create-resource-pools.md)。

  >[!TIP]
  >
  >專案的資源預算區域是專案層次的資源規劃工具。 當您在專案的「業務案例」中編列資源預算時，資訊也會反映在系統層次「資源規劃工具」中。

* 若要在高層級、跨多個行動方案管理資源，並依照組織的策略調整您的工作，請使用Adobe Workfront情境規劃工具。 Scenario Planner需要額外的授權。 如需Workfront Scenario Planner的相關資訊，請參閱[Scenario Planner概觀](../../scenario-planner/scenario-planner-overview.md)。

  您可以在系統層級、多個專案中使用「資源規劃工具」，以及在業務案例的「資源預算」區域中，為單一專案預算資源。 如需商務案例中專案預算資源的詳細資訊，請參閱商務案例中的[預算資源](../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md)。

## 資源規劃工具的用途

* 您可以使用資源規劃工具執行下列作業：

   * 排定專案的優先順序，以決定哪些專案應先接收資源。 （僅於資源規劃工具）
   * 根據使用者的排程，瞭解資源的可用性。
   * 針對資源（使用者和職位角色）指派給他們的專案，為其分配預算小時、FTE或成本分攤。

  如需有關在資源規劃工具中工作的資訊，請參閱文章[資源規劃工具概觀](../../resource-mgmt/resource-planning/get-started-resource-planner.md)。

* 使用「情境規劃工具」，您可以跨多個行動方案建立企業級計畫，概述公司的整體策略結果。 如需詳細資訊，請參閱[開始使用Scenario Planner](../../scenario-planner/get-started-with-scenario-planning.md)。

  Scenario Planner需要額外的授權。 如需Workfront Scenario Planner的相關資訊，請參閱[Scenario Planner概觀](../../scenario-planner/scenario-planner-overview.md)。

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode">Prerequisites for resource planning</h2>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(This section drafted because it was moved to the "Resource Planner overview" article instead. But this used to be true: THIS SECTION IS LINKED TO ALL RES PLANNING ARTICLES. DO NOT RENAME OF DELETE THIS!)</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">To successfully use the Resource Planner for budgeting your resources, you must first ensure that you, your projects, and your tasks meet a set of prerequisites. These prerequisites are mandatory to display the correct information in the Resource Planner and to accurately manage your resources. </p>
-->

<!--
<note type="important">  If any of the following prerequisites are missing, you might find that some of the information about the allocation or the availability of the resources is missing or has a zero value.
<br>For more information understanding why fields are missing data or have zero values, hover over the fields.
</note>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no-users-with-this-role-in-the-res-pool-350x57.png" style="width: 350;height: 57;"> </p>
-->

<!--
<note type="note">
The following prerequisites are required only when viewing the Resource Planner by project or by job role or when budgeting resources in the Business Case of a project.
<br>For more information about the views in the Resource Planner, see the "Project/ Role/ User view" selection section in the article
<a href="../../resource-mgmt/resource-planning/get-started-resource-planner.md" class="MCXref xref">Resource Planner overview</a>.
<br>
</note>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">The following types of prerequisites are required for the correct functionality of the Resource Planner: </p>
-->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#user-prerequisites" class="MCXref xref">User prerequisites</a> </li>
  -->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#project-prerequisites" class="MCXref xref">Project prerequisites</a> </li>
  -->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#tasks-and-issues-prerequisites" class="MCXref xref">Tasks and issues prerequisites</a> </li>
  -->

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode" id="user-prerequisites">User prerequisites</h3>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Ensure the following user setup exists before starting using the Resource Planner:</p>
<li>  <ul>   <li> <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You have the correct access to budget resources.</p><p data-mc-conditions="QuicksilverOrClassic.Draft mode">For information about the access needed to budget resources, see the article <a href="../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md" class="MCXref xref">Access needed to budget resources in&nbsp;Adobe Workfront</a>.</p>   </li>  </ul> </li>
-->

<!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Users who are assigned to tasks are added to the Resource Pools associated with the project.</p>
  -->

<!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For information about adding users to Resource Pools, see <a href="../../resource-mgmt/resource-planning/resource-pools/associate-resource-pools-with-users.md" class="MCXref xref">Associate resource pools with users </a> and <a href="../../resource-mgmt/resource-planning/resource-pools/create-resource-pools.md" class="MCXref xref">Create resource pools</a>.</p>
  -->

<!--
  >[!NOTE]
  >
  >
  >
  ><p data-mc-conditions="QuicksilverOrClassic.Draft mode">When users are not added to Resource Pools, the following scenarios may exist: </p>  >
  >
  >
  >   
  >   
  >   
  >     <li style="font-style: normal;" data-mc-conditions="QuicksilverOrClassic.Draft mode">The users do not appear in the Resource Planner although they might be assigned to tasks on the projects. </li>  >   
  >     <li style="font-style: normal;" data-mc-conditions="QuicksilverOrClassic.Draft mode">If the tasks they are associated with have Planned Hours, those hours do not appear for the project in the Resource Planner, unless the user is also associated with a job role on those tasks. </li>  >   
  >     <li style="font-style: normal;" data-mc-conditions="QuicksilverOrClassic.Draft mode">If the users are associated with a job role on a task on the project, the Planned Hours display in the Resource Planner for the job role, but the job role cannot be budgeted. </li>  >
  -->

<!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Users who are assigned to work and Resource Pools must have Schedules and Job Roles associated with their profile.</p>
  -->

<!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For information about associating Schedules and Job Roles with users, see the article <a href="../../administration-and-setup/add-users/create-and-manage-users/add-users.md" class="MCXref xref">Add users</a></p>
  -->

<!--
  <note type="note">  Users who are not associated with a Schedule but are in the Resource Pool of the project cannot be budgeted in the Resource Planner.
  </note>
  -->

<!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For accurate Available Hours information, ensure that the schedules associated with your users have the schedule exceptions and time off updated.</p>
  -->

<!--
  <note type="note">  If a user is not associated with a Schedule, the Default Schedule of your Workfront system is associated with the user by default, for the purposes of the Resource Planner.
  </note>
  -->

<!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For information about creating schedules, see the article <a href="../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Create a schedule</a>.<br></p>
  -->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">If you want to budget your resources by Cost, you must associate Job Roles with Cost/Hr. rates. The cost associated with Job Roles assigned to users in your Resource Pools is used to calculate the Budgeted Labor Cost and the Budgeted Cost of the project.<br>For information about associating job roles with rates, see the article <a href="../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Create and manage job roles</a>.<br>For information about calculating Budgeted Labor Cost, see the article <a href="../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">Understand Budgeted Labor Cost and Budgeted Hours for projects</a>.<br>For information about calculating Budgeted Cost, see the article <a href="../../manage-work/projects/project-finances/budgeted-cost.md" class="MCXref xref">Calculate Budgeted Cost</a>.</li>
  -->

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode" id="project-prerequisites">Project prerequisites</h3>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Ensure the following project setup exists before starting using the Resource Planner:</p>
-->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> Your projects are associated with Resource Pools.<br>For more information about adding Resource Pools to projects, see <a href="../../resource-mgmt/resource-planning/resource-pools/associate-resource-pools-with-projects-and-templates.md" class="MCXref xref">Associate resource pools with projects and templates</a>.<br>
  <note type="important">  Projects without Resource Pools do not display Planned Hour or assignments information in the Resource Planner.
  </note>
  -->

<!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You have the correct access to budget resources.</p>
  -->

<!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For information about the access needed to budget resources, see the article <a href="../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md" class="MCXref xref">Access needed to budget resources in&nbsp;Adobe Workfront</a>.</p>
  -->

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode" id="tasks-and-issues-prerequisites">Tasks and issues prerequisites</h3>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Ensure the following tasks and issues setup exists before starting budgeting resources in the Resource Planner:</p>
-->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> The tasks or issues on the projects for which you are budgeting resources are assigned to one of these entities:<br>
  <ul>
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Users in the Resource Pools of the project who are also associated with Job Roles</li>
  <li>
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Job Roles</p>
  </li>  
  </ul>
  <note type="note">
  Teams assigned to tasks or issues do not display in the Resource Planner. The Planned Hours of tasks and issues assigned to job roles display in the Resource Planner, but these hours cannot be budgeted unless a user who is associated with the job role is listed in a Resource Pool associated with the project.
  </note>
  -->

<!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Parent tasks should not be assigned to users or roles. </p>
  -->

<!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">This will impact the value of Planned Hours for the project. </p>
  -->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Tasks and issues have a value for Planned Hours which is greater than zero. </li>
  -->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Tasks and issues have a value for their Duration which is greater than zero. </li>
  -->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">The Planned Dates of the issues are within the timeline of the project. </li>
  -->

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode">Access resource planning tools in&nbsp;Workfront</h2>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can access the Planner from the  People Planner section  of the Resourcing area. </p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">For information about accessing the Planner, see <a href="../../resource-mgmt/resource-planning/get-started-resource-planner.md" class="MCXref xref">Resource Planner overview</a>.</p>
-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Create Resource Pools</h2>
<p>(drafted because it's redundant with the user prerequisites above) </p>
<p>You can manage your user resources by adding users to Resource Pools. Having users organized in Resource Pools and associating the pools with your projects are prerequisites to Resource Planning.</p>
<p>For information about adding users to Resource Pools and associating them with projects, see <a href="../../resource-mgmt/resource-planning/resource-pools/create-resource-pools.md" class="MCXref xref">Create resource pools</a> and <a href="../../resource-mgmt/resource-planning/resource-pools/associate-resource-pools-with-users.md" class="MCXref xref">Associate resource pools with users </a>.</p>
</div>
-->
