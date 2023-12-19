---
product-area: projects;templates
navigation-topic: plan-a-project
title: 指定專案或範本的資源管理員
description: 您可以指定專案的資源管理員，以指出誰負責管理專案上的資源。
author: Alina
feature: Work Management
exl-id: ae2a89e7-8049-4ee6-9b28-ce247d3f2a6f
source-git-commit: 59c3a57e334d1660e3e59da480a90060b1ba81b7
workflow-type: tm+mt
source-wordcount: '826'
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

<!--drafted for P&P:

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
   <td> <p>Current license: Standard </p> 
   Or
   <p>Legacy license: Plan </p>
   </td> 
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
</table>
-->

您必須具有下列存取權才能執行本文中的步驟：

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
   <td> <p>計劃 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>編輯專案和範本的存取權</p> <p><b>附註</b>

如果您還是沒有存取權，請詢問您的Workfront管理員，他們是否在您的存取層級中設定其他限制。 如需有關Workfront管理員如何修改您的存取層級的資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>管理專案或範本的許可權</p>

<p><b>附註</b>

新增為專案或範本的資源管理員的使用者會立即獲得專案或範本的管理許可權</p> <p>如需請求其他存取許可權的詳細資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">要求物件的存取權 </a>.</p> </td>
</tr> 
 </tbody> 
</table>

*若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的Workfront管理員。

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

  如需有關專案團隊的資訊，請參閱 [管理專案團隊](../../../manage-work/projects/planning-a-project/manage-project-team.md).

* 您可以指定專案或專案範本的資源管理員。 當您在專案範本上指定「資源管理員」時，您在範本上指定為「資源管理員」的任何使用者，都會自動成為使用該範本建立之任何專案的資源管理員。
* 您可以在下列區域中檢視Resource Manager欄位：

   * 編輯專案時，如本文所述。
   * 編輯範本時，如本文所述。
   * 建立專案或範本報表時。 如需有關建立報表的資訊，請參閱 [建立自訂報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
   * 建立或自訂清單的專案或範本檢視時。 如需詳細資訊，請參閱 [Adobe Workfront中的檢視概觀](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

* 您可以快速在多個專案或範本上新增或移除資源管理員，方法是將資源管理員欄位新增到清單或專案的檢視中，並使用內嵌編輯來編輯此欄位。

## 指定專案的資源管理員

1. 執行下列任一項作業：

   * 若要將資源管理員新增至單一專案，請移至您要指定一或多個資源管理員的專案，然後按一下 **更多選單** 在專案名稱旁，然後 **編輯。**

   * 若要同時新增資源管理員至多個專案，請瀏覽至專案清單，選取您要指定一或多個資源管理員的專案，然後按一下 **編輯**.

     不會從您編輯的專案中移除現有的資源管理員；您以這種方式新增的任何使用者都會新增為專案上的資源管理員，以及任何現有的資源管理員。

   * 若要將資源管理員新增至新專案，請開始建立新專案。

     如需有關建立專案的資訊，請參閱 [建立專案](../../../manage-work/projects/create-projects/create-project.md).

1. 在 **概觀** 區段編輯專案對話方塊中，按一下 **資源管理員** 欄位。
1. 開始輸入您想要新增為專案資源管理員的使用者名稱，然後按一下出現在清單中的名稱。

   重複此步驟，為專案新增多個資源管理員。

1. 按一下「**儲存變更**」。

## 指定範本的資源管理員

1. 按一下 **主要功能表** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角。

1. 按一下 **範本**.

1. 執行下列任一項作業：

   * 若要將資源管理員新增至單一範本，請移至您要指定一或多個資源管理員的範本，然後按一下 **更多選單** 在範本名稱旁，然後 **編輯。**

   * 若要同時將「資源管理員」新增至多個範本，請移至範本清單，並選取您要指定一或多個資源管理員的範本，然後按一下 **編輯**.

     不會從您編輯的範本中移除現有的資源管理員；您以這種方式新增的任何使用者都會新增為範本上的資源管理員，以及任何現有的資源管理員。

   * 若要將資源管理員新增至新範本，請按一下 **建立範本**，然後按一下 **更多選單** 在範本名稱旁，然後 **編輯。**

1. 在 **概觀** 區段，按一下 **資源管理員** 欄位。
1. 開始輸入您想要新增為範本資源管理員的使用者名稱，然後按一下出現在清單中的名稱。

   重複此步驟，將多個資源管理員新增至範本。

1. 按一下「**儲存變更**」。
