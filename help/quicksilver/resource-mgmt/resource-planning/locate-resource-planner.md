---
product-area: resource-management
navigation-topic: resource-planning
title: 找到資源規劃工具
description: '(本文是這樣產生的：當此為即時狀態時，草稿文章中的內容： /Content/Resource Mgmt/Resource Planning/get-started-resource-planner.html)'
author: Alina
feature: Resource Management
exl-id: 0de749df-5af9-4124-8539-06b82dca2ec4
source-git-commit: d3172a681ef6ac8b7bde44c680ad7febc3f26121
workflow-type: tm+mt
source-wordcount: '512'
ht-degree: 0%

---

# 找到資源規劃工具

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(This came off this article: draft that content in the article when this comes live: /Content/Resource Mgmt/Resource Planning/get-started-resource-planner.html)</p>
-->

您可以使用資源規劃工具來管理專案的資源配置。 您可以同時存取多個專案的資源規劃工具，或是從專案的「業務案例」區域存取一個專案的資源規劃工具。

## 存取需求

您必須具備下列條件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>專業及更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>評論或以上<!--
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
        (this seems to be the case in NWE only, not classic. Waiting on Vazgen's response for this)
      </MadCap:conditionalText>
     --></p> <p>計畫或以上以找出全域區域中的資源規劃工具</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>檢視對資源管理的存取權或以上許可權</p> <p><b>附註</b>

如果您還是沒有存取權，請詢問您的Workfront管理員，他們是否在您的存取層級中設定其他限制。 如需Workfront管理員如何修改存取層級的詳細資訊，請參閱<a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>。</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>檢視專案和使用者的許可權 </p> <p>如需請求其他存取權的資訊，請參閱<a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求物件</a>的存取權。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的Workfront管理員。

## 先決條件

在開始使用資源規劃工具之前，請確保滿足存取和使用資源規劃工具的所有先決條件。 如此一來，您就能在開始編列資源預算之前，確保資源規劃工具顯示正確的資訊。

如需有關資源規劃工具先決條件的資訊，請參閱[開始使用資源規劃](../../resource-mgmt/resource-planning/get-started-resource-planning.md)。

## 找到資源規劃工具

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(this was moved from the get-started-resource-planner article)</p>
-->

您可以在Workfront的兩個區域中找到資源規劃工具，這取決於您是要為多個專案還是僅一個專案預算資源。

* [將資源規劃工具用於多個專案](#use-the-resource-planner-for-multiple-projects)
* [針對一個專案使用資源規劃工具](#use-the-resource-planner-for-one-project)

### 將資源規劃工具用於多個專案 {#use-the-resource-planner-for-multiple-projects}

針對多個專案使用資源規劃工具時，資源的配置數字代表多個專案中的數字。

若要存取「資源」區域中的「規劃者」區段：

1. 按一下Adobe Workfront右上角的&#x200B;**主要功能表**&#x200B;圖示![](assets/main-menu-icon.png)。

1. 按一下「**資源**」。 「供需規劃員」預設會顯示。  如需有關資源規劃工具中預算資源的資訊，請參閱使用專案和角色檢視的資源規劃工具中的文章[預算資源](../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md)。

   ![](assets/qs-resource-management-area-with-planner-as-default-350x152.png)

1. 將滑鼠停留在左側面板，然後按一下&#x200B;**資源集區**。\
   如需有關建立資源集區的資訊，請參閱[建立資源集區](../../resource-mgmt/resource-planning/resource-pools/create-resource-pools.md)。

### 針對一個專案使用資源規劃工具 {#use-the-resource-planner-for-one-project}

針對一個專案使用資源規劃工具時，您資源的配置編號代表所選專案的編號。

1. 移至您要編列資源預算的專案。
1. 按一下左側面板中的&#x200B;**業務案例**。
1. 捲動至業務案例的&#x200B;**資源預算**&#x200B;區段。
1. 按一下&#x200B;**編輯資源預算**，將資源集區新增至專案，並開始為資源編列預算。

   >[!TIP]
   >
   >當專案沒有關聯的資源集區時，您只能在業務案例的資源預算區域新增資源集區。 當專案已有資源集區時，集區中的使用者及其工作角色依預設會顯示在「資源預算」區域中。

   ![](assets/resource-budgeting-area-on-project-350x70.png)

   如需為一個專案編列預算資源的相關資訊，請參閱文章[商業案例中的預算資源](../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md)。
