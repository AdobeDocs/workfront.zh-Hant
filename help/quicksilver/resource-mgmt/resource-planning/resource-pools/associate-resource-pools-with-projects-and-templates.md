---
product-area: resource-management
navigation-topic: resource-pools
title: 將資源集區與專案和範本建立關聯
description: 資源集區是使用者的集合，可協助您管理Adobe Workfront中的資源。
author: Alina
feature: Resource Management
exl-id: bbfe8257-ff02-4f06-9763-3f2ae4871c9d
source-git-commit: 171ccfe5d2bc9825c9cdb195df1a97a32e515646
workflow-type: tm+mt
source-wordcount: '644'
ht-degree: 0%

---

# 將資源集區與專案和範本建立關聯


<!-- drafted for bulk editing projects: keep this in yellow till this releases to ALL customers - May 1, 2023

Also - take out all the references to Preview and Prod at prod final
-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available for all customers in the Preview environment and for a select group of customers in the Production environment.</span>-->


<!--
<p>The sections about how to add resource pools to templates, projects are duplicated from the articles listed in those sections (Editing Projects, Creating a Template, etc).</p>
<p>***I decided to keep these steps here, though, because it's hard to parse through those much lunger articles for just updating this one field.)</p>
-->

資源集區是使用者的集合，可協助您管理Adobe Workfront中的資源。

建立資源集區後，您可以將其與專案或範本建立關聯，以便稍後在專案上編列資源預算。

我們建議您預先建立資源集區、將其與專案建立關聯，並在專案開始前為資源編列預算。

如需有關資源集區的資訊，請參閱[資源集區概觀](../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md)。

如需有關建立資源集區的資訊，請參閱[建立資源集區](../../../resource-mgmt/resource-planning/resource-pools/create-resource-pools.md)。

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
   <td> <p>計劃 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>編輯對資源管理的存取權，包括管理資源集區的存取權</p> <p>編輯專案、範本和使用者的存取權</p> <p>注意：如果您還是沒有存取權，請詢問您的Workfront管理員，他們是否在您的存取層級中設定其他限制。 如需Workfront管理員如何變更存取層級的詳細資訊，請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>管理您與資源集區建立關聯的專案、範本和使用者的許可權</p> <p>如需請求其他存取權的資訊，請參閱<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求物件</a>的存取權。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的Workfront管理員。

## 將資源集區與一個專案或範本建立關聯

您可以使用與將資源集區與專案建立關聯相同的方法，將資源集區與範本建立關聯。 本文說明如何將資源集區與專案建立關聯。

1. 前往專案，按一下專案名稱旁的&#x200B;**更多**&#x200B;圖示![](assets/more-icon.png)，然後按一下&#x200B;**編輯**。

1. 按一下&#x200B;**專案設定**。

1. 開始在&#x200B;**資源集區**&#x200B;欄位中輸入資源集區的名稱，然後在其出現時從清單中選取它。\
   您可以將多個資源集區與一個專案或範本建立關聯。

   ![](assets/nwe-project-settings-in-edit-project-box-350x380.png)

1. 按一下「**儲存**」。

如需有關如何編輯專案並將其與資源集區關聯的詳細資訊，請參閱[編輯專案](../../../manage-work/projects/manage-projects/edit-projects.md)。

如需有關如何編輯範本並將其與資源集區關聯的詳細資訊，請參閱[編輯專案範本](../../../manage-work/projects/create-and-manage-templates/edit-templates.md)。

## 將資源集區與數個專案或範本大量關聯

您可以大量編輯多個專案或範本，並同時將相同的資源集區與它們全部相關聯。

您可以透過將資源集區與專案建立關聯的相同方式，將資源集區與範本建立關聯。

若要將資源集區與數個專案大量關聯，請執行下列動作：

1. 前往專案清單。
1. 選取多個專案，然後按一下清單頂端的&#x200B;**編輯**&#x200B;圖示![](assets/edit-icon.png)。

1. 按一下&#x200B;**設定**。
1. 開始在&#x200B;**資源集區**&#x200B;欄位中輸入資源集區的名稱，然後在其出現時從清單中選取它。\
   您可以將多個資源集區與專案或範本建立關聯。

   >[!NOTE]
   >
   >* 當您大量編輯範本時，此欄位只會顯示所有選定範本通用的資源集區。 如果選取的範本沒有共用資源集區，則此欄位為空白。 您在此處指定的資源集區會覆寫專案或範本的個別資源集區。
   >
   >* 大量編輯專案時，如果所選專案具有不同的資源集區，則會顯示「多個值」指示器。 如果您為專案大量新增資源集區，所有集區都會新增至選取的專案，並覆寫原始資源集區。

   ![add_resource_pools_to_multiple_projects.png](assets/add-resource-pools-to-multiple-projects-350x358.png)

1. 按一下「**儲存變更**」。\
   當您的資源集區與您的專案或範本相關聯時，您可以在資源規劃工具內為專案編列使用者配置的預算。\
   如需資源規劃工具的詳細資訊，請參閱[資源規劃工具概觀](../../../resource-mgmt/resource-planning/get-started-resource-planner.md)。

如需有關如何大量編輯專案的詳細資訊，請參閱[編輯專案](../../../manage-work/projects/manage-projects/edit-projects.md)中的「大量編輯專案」一節。

如需有關如何大量編輯範本的詳細資訊，請參閱[編輯專案範本](../../../manage-work/projects/create-and-manage-templates/edit-templates.md)中的「大量編輯範本」一節。
