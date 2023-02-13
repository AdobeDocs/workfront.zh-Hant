---
product-area: projects;templates
navigation-topic: plan-a-project
title: 為項目或模板指定資源管理器
description: 您可以為項目指定資源經理，以指明誰負責管理項目上的資源。
author: Alina
feature: Work Management
exl-id: ae2a89e7-8049-4ee6-9b28-ce247d3f2a6f
source-git-commit: f150c57e8b83e73734b1cbeded7ef4c16d65097c
workflow-type: tm+mt
source-wordcount: '825'
ht-degree: 0%

---

# 為項目或模板指定資源管理器

<!--
<p This article might have to be deleted when the Resource Manager field/ requirement will be forever removed from the system; right now it's still a requirement for Scheduler - January 2023/p>
-->

<!-- remove Prod and Prev references with Prod release - Jan 2023-->

您可以為項目指定資源經理，以指明誰負責管理項目上的資源。 這是一個資訊欄位，它未連接到任何資源管理工具。

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

您必須具備下列存取權，才能執行本文中的步驟：

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
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>編輯專案和範本的存取權</p> <p><b>附註</b>

如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>管理專案或範本的權限</p>

<p><b>附註</b>

在項目或模板中添加為資源管理器的用戶會立即獲得項目或模板的管理權限</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td>
</tr> 
 </tbody> 
</table>

*若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 關於資源管理器的考量

>[!NOTE]
>
>資源管理器不是作業角色；此欄位是專案或範本上可用的欄位，您可以手動更新。

* 您可以為單個項目或模板指定最多30個用戶作為資源管理器。

<!--
* In the Production environment,designating Resource Managers on projects is a prerequisite to allowing users to schedule resources for work on the project when using the Scheduling tools.

  For information about resource scheduling, see [Resource Scheduling](../../../resource-mgmt/resource-scheduling/resource-scheduling-overview.md). 

  <span class="preview">Scheduling tools have been removed from the Preview environment.</span>

* Designating Resource Managers on projects is not a prerequisite to allowing users to schedule resources for work using the Workload Balancer.

  For information about the Workload Balancer, see [Overview of the Workload Balancer](../../../resource-mgmt/workload-balancer/overview-workload-balancer.md). 

 -->

* 不能將團隊或組指定為資源管理器。 您只能將用戶指定為資源管理器。

* 您在項目或模板上指定為資源管理器的用戶不會自動成為項目團隊的一部分。

   如需專案團隊的相關資訊，請參閱 [管理專案團隊](../../../manage-work/projects/planning-a-project/manage-project-team.md).

* 您可以為項目或項目模板指定資源管理器。 在項目模板上指定資源管理器時，在模板上指定為資源管理器的任何用戶將自動成為使用該模板建立的任何項目的資源管理器。
* 您可以在以下區域查看「資源管理器」欄位：

   * 編輯專案時，如本文所述。
   * 編輯範本時（如本文所述）。
   * 建立專案或範本報表時。 如需建立報表的相關資訊，請參閱 [建立自訂報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
   * 建立或自訂清單的專案或範本檢視時。 如需詳細資訊，請參閱 [Adobe Workfront中的檢視概觀](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

* 通過將「資源管理器」欄位添加到清單或項目的視圖，並使用行內編輯編輯此欄位，可以快速添加或刪除多個項目或模板上的資源管理器。

## 為項目指定資源管理器

1. 執行下列任一操作：

   * 要向單個項目添加資源管理器，請轉至要指定一個或多個資源管理器的項目，然後按一下 **更多功能表** 在專案名稱旁，然後 **編輯。**

   * 要同時將資源管理器添加到多個項目，請導航至項目清單，選擇要指定一個或多個資源管理器的項目，然後按一下 **編輯**.

      現有資源管理器不會從您正在編輯的項目中刪除；除了任何現有的資源管理器外，還會以此方式添加的任何用戶在項目上添加為資源管理器。

   * 要向新項目添加資源管理器，請開始建立新項目。

      如需建立專案的相關資訊，請參閱 [建立專案](../../../manage-work/projects/create-projects/create-project.md).

1. 在 **概述** 在「編輯項目」(Edit Project)對話框的部分上，按一下 **資源管理器** 欄位。
1. 開始鍵入要添加為項目資源管理器的用戶的名稱，然後在名稱出現在清單中時按一下該名稱。

   重複此步驟為項目添加多個資源管理器。

1. 按一下 **儲存變更**.

## 為模板指定資源管理器

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角。

1. 按一下 **範本**.

1. 執行下列任一操作：

   * 要將資源管理器添加到單個模板，請轉到要指定一個或多個資源管理器的模板，然後按一下 **更多功能表** 在範本名稱旁，然後 **編輯。**

   * 要同時將資源管理器添加到多個模板，請轉到模板清單並選擇要指定一個或多個資源管理器的模板，然後按一下 **編輯**.

      現有資源管理器不會從您正在編輯的模板中刪除；除了任何現有的資源管理器外，還會以此方式添加的任何用戶在模板上作為資源管理器添加。

   * 要將資源管理器添加到新模板，請按一下 **新範本**，然後按一下 **更多功能表** 在範本名稱旁，然後 **編輯。**

1. 在 **概述** 區段中，按一下 **資源管理器** 欄位。
1. 開始鍵入要添加為模板資源管理器的用戶的名稱，然後在該名稱出現在清單中時按一下該名稱。

   重複此步驟，將多個資源管理器添加到模板中。

1. 按一下 **儲存變更**.
