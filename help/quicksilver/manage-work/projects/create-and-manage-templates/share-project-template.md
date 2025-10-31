---
product-area: templates
navigation-topic: templates-navigation-topic
title: 共用專案範本
description: 您可以在範本層級使用下列共用選項，與使用者共用範本，或定義將如何使用範本與使用者共用從範本建立的專案。
author: Alina
feature: Work Management
exl-id: 99c6b241-a2c9-4b6c-b605-177bbbc3f21a
source-git-commit: 76379d5433cc13ee412c8c1045316ef253b3ee7d
workflow-type: tm+mt
source-wordcount: '730'
ht-degree: 3%

---

# 共用專案範本

您可以在範本層級使用下列共用選項，與使用者共用範本，或定義將如何使用範本與使用者共用從範本建立的專案。

在Adobe Workfront中共用物件時，您可以允許其他使用者檢視、貢獻或編輯該物件。

如需Workfront許可權的相關資訊，請參閱[物件共用許可權總覽](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md)。

如需共用範本時您可以授與使用者的許可權相關資訊，請參閱[共用範本](../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md)。

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
   <td> <p>標準</p>
   <p>規劃</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>編輯範本的存取權</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>管理範本的許可權</p> </td> 
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
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Templates</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a template</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## 共用範本 {#share-a-template}

您可以使用「範本共用」與其他使用者共用您的範本。 此動作會定義誰擁有範本的許可權。

>[!NOTE]
>
>當您指定作用中的使用者作為範本擁有者時，該使用者會自動收到範本的管理許可權。 如需將某人指定為範本擁有者的詳細資訊，請參閱[編輯專案範本](../../../manage-work/projects/create-and-manage-templates/edit-templates.md)。

共用範本：

1. 從&#x200B;**主功能表**&#x200B;圖示![主功能表圖示](assets/main-menu-icon.png)，按一下&#x200B;**範本**。

1. 執行下列其中一項：\
   按一下範本名稱以開啟，然後按一下&#x200B;**更多**&#x200B;功能表![更多圖示](assets/more-icon.png)，然後按一下&#x200B;**範本共用**。

   或

   從清單中選取範本，按一下[共用]圖示![](assets/share-icon.png)，然後按一下&#x200B;**範本。**

   >[!TIP]
   >
   >您只能與作用中使用者、團隊、角色或公司共用物件。

1. 在「**範本存取**」方塊中，選取您要共用範本的人員、團隊、角色、群組或公司。

   您也可以按一下&#x200B;**選項**&#x200B;圖示，讓範本在整個系統內可用：

1. 從與您共用之每個實體的下拉式選單中，選取下列選項：

   * **檢視**：具有這些許可權的使用者可以檢視範本並使用它建立專案，或將其附加至現有的專案。

     >[!TIP]
     >
     >您的Workfront管理員必須授予您專案的編輯存取權才能建立專案。

   * **管理**：具有這些許可權的使用者可以編輯或刪除範本。

     如需此處可用的進階設定![](assets/gear-icon-in-access-levels.png)的相關資訊，請參閱[共用範本](../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md#template-permissions)一文中的[範本共用的進階設定](../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md)小節。

1. 按一下「**儲存**」。

## 從範本共用專案 {#share-a-project-from-a-template}

使用範本專案共用，您可以在範本層級定義誰對從範本建立的專案擁有許可權。

若要與使用者共用從範本建立的未來專案：

1. 執行下列其中一項：\
   按一下範本名稱以開啟，然後按一下&#x200B;**更多**&#x200B;功能表![更多圖示](assets/more-icon.png)，然後按一下&#x200B;**範本共用**。

   ![從範本共用專案](assets/project-sharing-on-template-nwe-2022-350x172.png)

   或

   從清單中選取範本，按一下&#x200B;**共用**，然後按一下&#x200B;**專案**。

1. 在&#x200B;**專案存取**&#x200B;方塊中，選取與範本共用的人員、團隊、角色、群組或公司。

   >[!TIP]
   >
   >您只能與作用中使用者、團隊、角色或公司共用物件。

1. 從每個實體的下拉式功能表中，選取下列專案：

   * **沒有存取權**：您可以指定哪些使用者沒有範本的存取權。\
     此選項僅在從範本大量共用專案時可用。 
   * **檢視**：具有這些許可權的使用者可以檢視從範本建立的專案。
   * **參與**：擁有這些許可權的使用者可以參與由範本建立的專案 
   * **管理**：具有這些許可權的使用者可以管理或刪除從這個範本建立的專案。

1. （選擇性）按一下&#x200B;**選項**&#x200B;圖示，讓專案在整個系統內都可用。
1. 按一下「**儲存**」。

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h3>Overview of project sharing from other sources</h3>
<p>You may already have been assigned access to projects from other areas of Workfront. <br>You may have been assigned access to projects from the following areas: </p>
<ul>
<li>When a project is created<br>For more information about sharing projects when the project is created, see the "Access" section in <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">Edit projects</a>.</li>
<li>When your Workfront administrator sets user access levels<br>For more information about setting access levels, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</li>
<li>When using the project access template</li>
</ul>
<p>When using the Template Project Sharing feature, if a user's access to a project is View, but you set the access permissions for Template Project Sharing to Manage, the user will have Manage permission for every project created using this specific template. The user will only have View permission for the other projects they are on.</p>
</div>
-->

## 大量共用範本中的範本和專案

您可以同時共用多個範本以及從多個範本共用專案。

>[!NOTE]
>
>選取多個範本時，您無法檢視誰已有個別範本的許可權。

1. 前往範本清單。
1. 選取多個範本，然後按一下[共用]。![](assets/share-icon.png)

   ![大量共用範本或專案](assets/share-templates-projects-in-bulk-link-in-toolbar-nwe-2022.png)

   >[!TIP]
   >
   >您只能與作用中使用者、團隊、角色或公司共用物件。

1. 按一下&#x200B;**範本**&#x200B;以共用選取的範本。

   或

   按一下&#x200B;**專案**，共用將從選取的範本建立的專案。

1. 繼續共用範本或專案，如本文中以下章節所述：

   * [共用範本](#share-a-template)
   * [從範本共用專案](#share-a-project-from-a-template)
