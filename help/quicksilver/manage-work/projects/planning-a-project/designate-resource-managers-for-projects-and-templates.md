---
product-area: projects;templates
navigation-topic: plan-a-project
title: 指定專案或範本的資源管理員
description: 您可以指定專案的資源管理員，以指出誰負責管理專案上的資源。
author: Alina
feature: Work Management
exl-id: ae2a89e7-8049-4ee6-9b28-ce247d3f2a6f
source-git-commit: 5bc7a1c00b72cfc07270cafee5bf753989b48d33
workflow-type: tm+mt
source-wordcount: '748'
ht-degree: 1%

---

# 指定專案或範本的資源管理員

<!--
<p This article might have to be deleted when the Resource Manager field/ requirement will be forever removed from the system; right now it's still a requirement for Scheduler - January 2023/p>
-->

<!-- remove Prod and Prev references with Prod release - Jan 2023-->

您可以指定專案的資源管理員，以指出誰負責管理專案上的資源。 此為資訊欄位，未連線至任何資源管理工具。

<!-- drafted for res scheduling deprecation blurb for preview release
Designating Resource Managers for a project is a prerequisite for using the Scheduling tools in Adobe Workfront, in the Production environment.
  
>[!CAUTION]  
>  
>  
> <span class="preview">Some of the information in this article refers to the Adobe Workfront's Scheduling tools. The Scheduling areas have been removed from the Preview environment and will be removed from the Production environment in **January 2023**. </span>  
> <span class="preview"> Instead, you can schedule resources in the Workload Balancer. </span>  
>  
>* <span class="preview"> For information about scheduling resources using the Workload Balancer, see the section [The Workload Balancer](../../../resource-mgmt/workload-balancer/workload-balancer.md).</span>  
>  
>* <span class="preview"> For more information about the deprecation and removal of the Scheduling tools, see [Deprecation of Resource Scheduling tools in Adobe Workfront](../../../resource-mgmt/resource-mgmt-overview/deprecate-resource-scheduling.md).</span> 
-->

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront套件</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td><p>標準</p> 
   <p>規劃</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>編輯專案和範本的存取權</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>管理專案或範本的許可權</p>

</td> 
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects and Templates</p> <p><b>NOTE</b> 
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions on the project or template</p> 
   
   <p><b>NOTE</b>
   
   Users who are added as Resource Managers to a project or a template immediately gain Manage permissions on the project or the template</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## 關於資源管理員的考量事項

>[!NOTE]
>
>資源管理員不是工作角色；它是專案或範本上可供手動更新的欄位。

* 您最多可以指定30位使用者作為個別專案或範本的資源管理員。

<!--
* In the Production environment,designating Resource Managers on projects is a prerequisite to allowing users to schedule resources for work on the project when using the Scheduling tools.

  For information about resource scheduling, see [Resource Scheduling](../../../resource-mgmt/resource-scheduling/resource-scheduling-overview.md). 

  <span class="preview">Scheduling tools have been removed from the Preview environment.</span>

* Designating Resource Managers on projects is not a prerequisite to allowing users to schedule resources for work using the Workload Balancer.

  For information about the Workload Balancer, see [Workload Balancer overview](../../../resource-mgmt/workload-balancer/overview-workload-balancer.md). 

 -->

* 您無法將專案團隊或群組指定為資源管理員。 您只能指定使用者作為資源管理員。

* 您在專案或範本上指定為資源管理員的使用者不會自動成為專案團隊的一部分。

  如需有關專案團隊的資訊，請參閱[管理專案團隊](../../../manage-work/projects/planning-a-project/manage-project-team.md)。

* 您可以指定專案或專案範本的資源管理員。 當您在專案範本上指定「資源管理員」時，您在範本上指定為「資源管理員」的任何使用者，都會自動成為使用該範本建立之任何專案的資源管理員。
* 您可以在下列區域中檢視Resource Manager欄位：

   * 編輯專案時，如本文所述。
   * 編輯範本時，如本文所述。
   * 建立專案或範本報表時。 如需建立報表的相關資訊，請參閱[建立自訂報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)。
   * 建立或自訂清單的專案或範本檢視時。 如需詳細資訊，請參閱[Adobe Workfront中的檢視總覽](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)。

* 您可以快速在多個專案或範本上新增或移除資源管理員，方法是將資源管理員欄位新增到清單或專案的檢視中，並使用內嵌編輯來編輯此欄位。

## 指定專案的資源管理員

1. 執行下列任一項作業：

   * 若要將資源管理員新增至單一專案，請移至您要指定一或多個資源管理員的專案，然後按一下專案名稱旁的&#x200B;**更多&#39;a5&#39;5c能表**，然後&#x200B;**編輯。**

   * 若要同時新增資源管理員至多個專案，請瀏覽至專案清單，選取您要指定一或多個資源管理員的專案，然後按一下[編輯]。**&#x200B;**

     不會從您編輯的專案中移除現有的資源管理員；您以這種方式新增的任何使用者都會新增為專案上的資源管理員，以及任何現有的資源管理員。

   * 若要將資源管理員新增至新專案，請開始建立新專案。

     如需有關建立專案的資訊，請參閱[建立專案](../../../manage-work/projects/create-projects/create-project.md)。

1. 在[編輯專案]對話方塊的&#x200B;**總覽**&#x200B;區段中，按一下&#x200B;**資源管理員**&#x200B;欄位。
1. 開始輸入您想要新增為專案資源管理員的使用者名稱，然後按一下出現在清單中的名稱。

   重複此步驟，為專案新增多個資源管理員。

1. 按一下「**儲存變更**」。

## 指定範本的資源管理員

1. 按一下Adobe Workfront右上角的&#x200B;**主功能表**&#x200B;圖示![主功能表圖示](assets/main-menu-icon.png)。

1. 按一下&#x200B;**範本**。

1. 執行下列任一項作業：

   * 若要將資源管理員新增至單一範本，請移至您要指定一或多個資源管理員的範本，然後按一下範本名稱旁的&#x200B;**更多功能表**，然後&#x200B;**編輯。**

   * 若要同時新增資源管理員到多個範本，請移至範本清單，並選取您要指定一或多個資源管理員的範本，然後按一下[編輯]。**&#x200B;**

     不會從您編輯的範本中移除現有的資源管理員；您以這種方式新增的任何使用者都會新增為範本上的資源管理員，以及任何現有的資源管理員。

   * 若要將資源管理員新增至新範本，請按一下[新增範本] **，然後按一下範本名稱旁的[其他]功能表**，再按一下[編輯] **。**&#x200B;**&#x200B;**

1. 在&#x200B;**總覽**&#x200B;區段中，按一下&#x200B;**資源管理員**&#x200B;欄位。
1. 開始輸入您想要新增為範本資源管理員的使用者名稱，然後按一下出現在清單中的名稱。

   重複此步驟，將多個資源管理員新增至範本。

1. 按一下「**儲存變更**」。
