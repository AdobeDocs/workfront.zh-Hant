---
product-area: portfolios;projects
navigation-topic: create-and-manage-portfolios
title: 將專案新增至Portfolio
description: 我們建議您在啟動專案時，將專案新增至專案組合。 不過，您可以在產品組合期限內的任何時間將其新增至產品組合。
author: Alina
feature: Work Management, Strategic Planning
exl-id: 97f36c18-3ac8-45ac-b5bc-dfe8b1363faf
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: fee6b71eeb0ca79703a2a9e29a14040b91cb7387
workflow-type: tm+mt
source-wordcount: '514'
ht-degree: 2%

---

# 將專案新增至投資組合

<!--Audited: 08/2025-->

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers after a week from the Preview release. </span>   

<span class="preview">For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md). </span>
-->

我們建議您在啟動專案時，將專案新增至專案組合。 不過，您可以在產品組合期限內的任何時間將其新增至產品組合。

將專案新增至投資組合時，請考量下列事項：

* 您只能將一個投資組合與一個專案建立關聯。
* 專案會保留在投資組合中，直到被移除或與另一個投資組合相關聯為止。
* 投資組合可包含不限數量的專案。

>[!CAUTION]
>
>   在大量子物件中使用繼承的許可權時，可能無法正確套用。
>   
>   為協助避免繼承許可權問題，我們建議以下事項：
>
>   * 限制單一父項（投資組合或方案）下的子物件（專案）數量。 我們建議每個投資組合或計畫不超過10,000個專案。
>   * 在較低層級的物件上套用許可權，以降低繼承深度。
>
>     例如，直接在專案層級套用許可權，而不是依賴從專案組合繼承到方案，然後繼承到專案的許可權。
>   * 分割計畫以包含較少的專案，這會降低許可權的複雜性。


## 存取權要求

+++ 展開以檢視這篇文章中所述功能的存取權要求。 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 封裝</td> 
   <td> <p>任何</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權</td> 
   <td><p>標準</p> 
   <p>[!UICONTROL 計畫] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>[!UICONTROL Edit]存取權投資組合</p> <p>[!UICONTROL Edit]專案的存取權</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>投資組合的[!UICONTROL Manage]許可權</p> <p>[!UICONTROL Manage] permissions to the projects</p>  </td> 
  </tr> 
 </tbody> 
</table>

*For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--
Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> <p>Any</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td><p>New: Standard</p> 
   <p>Current: [!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level</td> 
   <td> <p>[!UICONTROL Edit] access Portfolios</p> <p>[!UICONTROL Edit] access to Projects</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>[!UICONTROL Manage] permissions to the portfolio</p> <p>[!UICONTROL Manage] permissions to the projects</p>  </td> 
  </tr> 
 </tbody> 
</table>
-->

## Add a project to a portfolio

1. Go to a portfolio, then click **[!UICONTROL Projects]** in the left panel.

   ![Portfolio with projects](assets/qs-portfolio-with-projects-350x90.png)

1. Click **[!UICONTROL New Project]** and select a method for adding a project.

   >[!TIP]
   >
   >You cannot add a project when you view the list of projects in the [!UICONTROL Milestone] view.

   從下列選項中選取：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Existing Project]</td> 
      <td> <p>Add a project that has already been created.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL New Project]</td> 
      <td> <p>Add a new project. </p> <p>For more information about creating a new project, see <a href="../../../manage-work/projects/create-projects/create-project.md" class="MCXref xref">Create a project</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Import a Project from [!DNL MS Project]] </td> 
      <td> <p>Add a project that you previously exported from [!DNL MS Project] and have saved on your computer. </p> <p>For more information about creating a new project by importing it from [!DNL Microsoft Project], see <a href="../../../manage-work/projects/create-projects/import-project-from-ms-project.md" class="MCXref xref">Import a project from [!DNL Microsoft Project]</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Request Project]</td> 
      <td> <p>Request that a project is approved.</p> <p>For information about requesting projects, see <a href="../../../manage-work/projects/create-projects/request-project.md">Requesting a Project</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL New from Template]</td> 
      <td> <p>Add a new project using an existing template. </p> <p>For more information about creating a project from a template, see <a href="../../../manage-work/projects/create-projects/create-project-from-template.md" class="MCXref xref">Create a project using a template</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

   ![新專案下拉式清單](assets/new-project-dropdown-expanded-from-portfolio-nwe-350x376.png)

1. (Conditional) If you selected to add an existing project, the **Add Projects** box opens. <!--check this after UI changes-->

   ![Add existing project](assets/add-existing-projects-to-portfolios-box.png) <!--check this after UI changes-->

1. Start typing the name of a project in the **[!UICONTROL Add Projects to this Portfolio]** field, then click them when they appear in the list.  <!--check this after UI changes-->

   You can add more than one project.

1. (Optional) Click the **X** icon to the right of the project name to remove it from the list, if you decide not to add it to the portfolio.

   <!--replace last step with this, for unshim: 1. (Optional) Click the **Delete** icon ![Delete icon](assets/delete-icon.png) next to the name of a project if you decide not to add it to the portfolio.-->

1. Click **[!UICONTROL Add Projects]**. <!--check this after UI changes-->

   The project or projects you selected are now associated with the portfolio.
