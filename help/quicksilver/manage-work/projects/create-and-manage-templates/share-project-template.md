---
product-area: templates
navigation-topic: templates-navigation-topic
title: 共用專案範本
description: 您可以與使用者共用範本，也可以使用範本層級的下列共用選項，定義從範本建立的專案與使用者共用的方式。
author: Alina
feature: Work Management
exl-id: 99c6b241-a2c9-4b6c-b605-177bbbc3f21a
source-git-commit: dd7f61fcd92a43303be356dd3209ec6da6a063dd
workflow-type: tm+mt
source-wordcount: '780'
ht-degree: 2%

---

# 共用專案範本

您可以與使用者共用範本，也可以使用範本層級的下列共用選項，定義從範本建立的專案與使用者共用的方式。

在Adobe Workfront中共用物件時，您可以讓其他使用者檢視、貢獻或編輯該物件。

如需Workfront權限的相關資訊，請參閱 [對象共用權限概述](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

如需在共用範本時可為使用者提供哪些權限的詳細資訊，請參閱 [共用範本](../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md).

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>任何 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>計劃 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>編輯範本的存取權</p> <p>注意：如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>管理範本的權限</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 共用範本 {#share-a-template}

您可以使用範本共用與其他使用者共用範本。 此動作會定義誰擁有範本的權限。

>[!NOTE]
>
>當您指定使用中使用者為範本擁有者時，該使用者會自動收到範本的管理權限。 有關指定某人為模板所有者的資訊，請參閱 [編輯專案範本](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

共用範本：

1. 從 **主菜單** 圖示 ![](assets/main-menu-icon.png)，按一下 **範本**.

1. 執行下列任一項作業：\
   按一下範本的名稱以開啟，然後按一下 **更多** 功能表 ![](assets/qs-more-icon-on-an-object.png)，然後 **範本共用**.

   或

   從清單中選取範本，按一下「共用」圖示 ![](assets/share-icon.png)，然後按一下&#x200B;**範本。**

   >[!TIP]
   >
   >您只能與作用中使用者、團隊、角色或公司共用物件。

1. 在 **範本存取** 框中，選擇要共用模板的人員、團隊、角色、組或公司。

   您也可以按一下 **選項** 表徵圖，使模板在系統範圍內可用：

1. 從您要共用之每個實體的下拉式功能表中，選取下列項目：

   * **檢視**:擁有這些權限的使用者可以檢視範本並使用範本建立專案，或將其附加至現有專案。

      >[!TIP]
      >
      >您的Workfront管理員必須授予您專案的「編輯」存取權，才能建立專案。

   * **管理**:具有這些權限的使用者可以編輯或刪除範本。

      如需進階設定的相關資訊， ![](assets/gear-icon-in-access-levels.png) 可在此取得，請參閱區段 [範本共用的進階設定](../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md#template-permissions) 在文章中 [共用範本](../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md).

1. 按一下&#x200B;**儲存**。

## 從範本共用專案 {#share-a-project-from-a-template}

透過範本專案共用，您可以定義誰擁有從範本層級建立之專案的權限。

若要與使用者共用從範本建立的未來專案：

1. 執行下列任一項作業：\
   按一下範本的名稱以開啟，然後按一下 **更多** 功能表 ![](assets/qs-more-icon-on-an-object.png)，然後 **範本共用**.

   ![從範本共用專案](assets/project-sharing-on-template-nwe-2022-350x172.png)

   或

   從清單中選取範本，按一下 **共用**，然後按一下&#x200B;**專案。**

1. 在 **專案存取** 框中，選擇與模板共用的人員、團隊、角色、組或公司。

   >[!TIP]
   >
   >您只能與作用中使用者、團隊、角色或公司共用物件。

1. 從每個實體的下拉式功能表中，選取下列項目：

   * **無權存取**:您可以指定哪些使用者將無法存取範本。\
      只有在從範本大量共用專案時，才可使用此選項。 
   * **檢視**:擁有這些權限的使用者可以檢視從範本建立的專案。
   * **Contribute**:擁有這些權限的使用者可以參與從範本建立的專案 
   * **管理**:擁有這些權限的使用者可以管理或刪除從此範本建立的專案。

1. （選用）按一下 **選項** 表徵圖，使項目在全系統可用。
1. 按一下&#x200B;**儲存**。

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

## 大量共用範本和專案

您可以同時共用多個範本和多個範本的專案。

>[!NOTE]
>
>當您選取多個範本時，無法檢視已擁有個別範本權限的人員。

1. 移至範本清單。
1. 選取多個範本，然後按一下 ![共用](assets/share-icon.png).

   ![大量共用範本或專案](assets/share-templates-projects-in-bulk-link-in-toolbar-nwe-2022.png)

   >[!TIP]
   >
   >您只能與作用中使用者、團隊、角色或公司共用物件。

1. 按一下 **範本** 共用所選範本。

   或

   按一下 **專案** 共用將從所選模板建立的項目。

1. 如本文的以下章節所述，繼續共用範本或專案：

   * [共用範本](#share-a-template)
   * [從範本共用專案](#share-a-project-from-a-template)
