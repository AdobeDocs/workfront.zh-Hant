---
product-area: resource-management
navigation-topic: resource-pools
title: 將資源池與項目和模板關聯
description: 資源池是協助您在Adobe Workfront中管理資源的使用者集合。
author: Alina
feature: Resource Management
exl-id: bbfe8257-ff02-4f06-9763-3f2ae4871c9d
source-git-commit: 78de23b4d5814e5e2ead6bb61a80bba7bd2aed33
workflow-type: tm+mt
source-wordcount: '612'
ht-degree: 0%

---

# 將資源池與項目和模板關聯


<!-- drafted for bulk editing projects: make this live when we release edit projects in bulk and replace the screen shot below (marked) and make the shot in yellow showing adding resource pools to multiple projects:
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment.</span> 

-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>The sections about how to add resource pools to templates, projects are duplicated from the articles listed in those sections (Editing Projects, Creating a Template, etc).</p>
<p>***I decided to keep these steps here, though, because it's hard to parse through those much lunger articles for just updating this one field.)</p>
</div>
-->

資源池是協助您在Adobe Workfront中管理資源的使用者集合。

建立資源池後，可以將它們與項目或模板關聯，以便以後可以對項目上的資源進行預算。

建議您事先建立資源池，將其與項目關聯，並在項目開始前對資源進行預算。

有關資源池的資訊，請參見 [資源池概述](../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md).

有關建立資源池的資訊，請參見 [建立資源池](../../../resource-mgmt/resource-planning/resource-pools/create-resource-pools.md).

## 存取需求

您必須具備下列條件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>Pro及更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>計劃 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>編輯對資源管理的訪問，包括對管理資源池的訪問</p> <p>編輯專案、範本和使用者的存取權</p> <p>注意：如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何變更您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">物件權限</td> 
   <td> <p>管理與資源池關聯的項目、模板和用戶的權限</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 將資源池與一個項目或模板關聯

您可以按與項目關聯資源池的相同方式將資源池與模板關聯。 本文說明如何將資源池與項目關聯。

1. 前往專案，然後按一下 **更多** 圖示 ![](assets/more-icon.png)在專案名稱旁，按一下 **編輯**.

1. 按一下 **專案設定**.

1. 開始鍵入資源池的名稱 **資源池** 欄位，然後在出現時從清單中選取它。\
   您可以將多個資源池與一個項目或模板相關聯。

   ![](assets/nwe-project-settings-in-edit-project-box-350x380.png)

1. 按一下&#x200B;**儲存**。

有關如何編輯項目以及將其與資源池關聯的詳細資訊，請參見 [編輯專案](../../../manage-work/projects/manage-projects/edit-projects.md).

有關如何編輯模板並將其與資源池關聯的詳細資訊，請參見 [編輯專案範本](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

## 將資源池與多個項目或模板大量關聯

您可以批量編輯多個項目或模板，並將相同的資源池與所有項目或模板同時關聯。

您可以用與資源池與項目關聯的相同方式將資源池與模板關聯。

要批量將資源池與多個項目關聯：

1. 前往專案清單。
1. 選取多個專案，然後按一下 **編輯** 圖示 ![](assets/edit-icon.png) 清單頂端。

1. 按一下 **設定**.
1. 開始鍵入資源池的名稱 **資源池** 欄位，然後在出現時從清單中選取它。\
   您可以將多個資源池與項目或模板相關聯。

   >[!NOTE]
   >
   >批量編輯項目或模板時，此欄位中只會顯示所有選定項目或模板的共同資源池。 如果所選項目沒有共用資源池，則此欄位將為空。 您在此處指定的資源池將覆蓋項目或模板的單個資源池。

   <!--drafted note for bulk editing projects - update the screen shot below for Edit Projects with the new UI in bulk and add the preview tags to the picture for Preview-->

   ![add_resource_pools_to_multiple_projects.png](assets/add-resource-pools-to-multiple-projects-350x358.png)

1. 按一下 **儲存變更**.\
   當資源池與項目或模板相關聯時，您可以在資源計畫器中為項目預算用戶分配。\
   有關資源計畫員的詳細資訊，請參閱 [資源計畫員概覽](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

如需如何大量編輯專案的詳細資訊，請參閱 [編輯專案](../../../manage-work/projects/manage-projects/edit-projects.md).

如需如何大量編輯範本的詳細資訊，請參閱 [編輯專案範本](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).
