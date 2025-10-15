---
product-area: user-management;portfolios
navigation-topic: grant-and-request-access-to-objects
title: 移除物件的許可權
description: 您可以移除其他使用者對您有權共用之物件的許可權。 從物件中移除許可權對於所有可共用的物件來說都是相同的。
author: Alina
feature: Get Started with Workfront
exl-id: 8e191b5e-31df-4291-8b9d-9ca69be27561
source-git-commit: 4ae96f67b15838403ffce32317d871d6904d6d95
workflow-type: tm+mt
source-wordcount: '767'
ht-degree: 0%

---

# 移除物件的許可權

<!--Audited: 01/2024-->

您可以移除其他使用者對您有權共用之物件的許可權。 從物件中移除許可權對於所有可共用的物件來說都是相同的。

與共用物件類似的考量適用於從物件移除許可權。 如需詳細資訊，請參閱文章[共用物件許可權總覽](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md#consider)中的[共用物件的考量事項](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md)一節

## 存取需求

+++ 展開以檢視本文中功能的存取需求。 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront套件</td> 
   <td> <p>任何 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td> <p>投稿人或以上</p> 
   <p>要求或更高版本</p>
   <p><strong>注意</strong>：某些物件需要比要求更高的存取許可權。</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>檢視您要共用之物件的存取許可權或以上許可權</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>檢視您要共用之物件的許可權或更高的許可權</p> <p>管理移除物件繼承許可權的許可權</p>  </td> 
  </tr>
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 從物件的共用清單中移除實體 {#remove-entities-from-the-sharing-list-of-an-object}

您可以從物件的共用清單中移除實體（使用者、工作角色、團隊、群組、公司）。 這會移除使用者對物件的許可權。

1. 移至您要移除許可權的物件。

   如需哪些物件可以共用的資訊，請參閱[物件共用許可權簡介](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md)。

1. （視條件而定）針對計畫、投資組合和檔案，執行下列動作：

   1. 按一下物件名稱旁的&#x200B;**更多**&#x200B;圖示![更多](assets/more-icon.png)，然後按一下&#x200B;**共用**&#x200B;或&#x200B;**共用**。

      ![共用](assets/share-a-document-350x160.png)

   1. 按一下使用者、團隊、群組、公司、工作角色名稱旁的&#x200B;**x**，在物件存取方塊中移除這些專案。

      ![移除許可權](assets/remove-permissions-on-portfolio.png)

   1. 在&#x200B;**[使用者名稱]的Workfront存取權將從此**&#x200B;下拉式功能表中移除，請選取是否要從您選取的物件移除其存取權，還是從與其關聯的所有子物件移除其存取權。

1. （視條件而定）對於專案、任務和問題，請執行以下作業：

   1. 按一下物件名稱右邊的&#x200B;**共用**。

      ![共用](assets/new-share-button.png)
   1. 尋找要從物件中移除的使用者、角色、團隊、群組或公司。
   1. 按一下&#x200B;**移除**。
在&#x200B;**「從**&#x200B;移除&lt;使用者名稱>」下拉式功能表中，選取是否要從選取的物件移除其存取權，或是從與其關聯的所有子物件移除其存取權。

      ![移除](assets/remove-permissions-on-project-nwe-350x479.png)

   存在下列情況：

   * 如果您只從物件中移除實體，則該實體會失去其對物件的許可權，以及其對子物件的繼承許可權。 如果先前已個別授予子專案的許可權，當您選取此選項時，它們會保留與其相關聯之所有子物件的相同許可權。
   * 如果您將實體從物件及所有子物件中移除，該實體會失去其對該物件及所有子物件的許可權，即使先前已授予他們個別對各個子物件的許可權。

1. 按一下「**儲存**」。

<!--
## Remove permissions from several objects in bulk

You can remove entities (users, job roles, teams, groups, companies) from several objects at a time when you bulk select them in a list.

>[!NOTE]
>
>You cannot view what access entities have for all the objects selected when you select them in bulk. You must know which entity you want to remove from the sharing of the objects selected before removing their permissions.

1. Go to the list of objects that you want to share.

   For information about which objects can be shared, see [Overview of sharing permissions on objects](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

1. Select several objects in the list, then click the **Share** icon ![share icon](assets/share-icon.png)at the top of the list. 
1. Type the name of the user, role, team, group, or company for which you want to remove the access in the **Edit `<Object Name>` access to** field. 
1. From the access drop-down menu, select **No Access**.

   ![remove in bulk](assets/no-access-option-removing-permissions-bulk-tasks-nwe-350x166.png)

1. In the `<User Name>`'s Workfront access will be removed from this drop-down menu, select whether you want their access to be removed just from the objects that you have selected, or from all other children objects associated with it.  
   The following scenarios exist:

   * If you remove the entity only from the object, that entity loses their permissions on the object, and their inherited permissions to the children objects. If they were previously granted permissions to the children items individually, they retain the same permissions on all children objects associated with it when you select this option.&nbsp;
   * If you remove the entity from the object and all the children objects, that entity loses their permissions to the object as well as all children objects, even when they were previously given individual permission on each child object.

   **Example:** Select whether to remove permissions to just the tasks you selected in a list, or to the issues and documents attached to the tasks as well.

   ![access](assets/remove-permissions-bulk-drop-down-for-attached-objects-nwe-350x96.png)

1. (Optional) To change permissions in bulk for several objects, select another level of sharing for the selected entity.

   For example, if they have Manage permissions, select Contribute or View instead. 

1. Click **Save**.

-->

## 移除繼承的許可權

繼承的許可權可以從物件中移除，讓擁有者能夠明確識別誰將取得子物件的存取權，無論使用者是否取得父物件的存取權。

>[!IMPORTANT]
>
>只有具有「管理」許可權的使用者才能移除繼承的許可權。

若要移除繼承的許可權：

1. 移至您擁有管理許可權的物件。 例如，前往任務。
1. 依照本文中[從物件](#remove-entities-from-the-sharing-list-of-an-object)的共用清單移除實體一節中的說明，移至物件存取方塊。
1. 選取&#x200B;**繼承的許可權**&#x200B;旁的&#x200B;**關閉**&#x200B;以停用。

   這可確保授予父系物件（例如專案）許可權的任何人都不會預設擁有此任務的許可權。 您必須在任務共用清單中列出個別實體，才能授與任務許可權。

   >[!TIP]
   >
   >您無法從繼承的許可權清單中移除個別實體。 您只能對列出的所有實體停用繼承許可權。

1. 按一下&#x200B;**儲存**。 

## 將物件設為私人

如果您已在系統範圍內共用物件，或透過將其設為公開而與外部使用者共用物件，則可移除系統範圍或公開許可權，使其再次成為私人物件。 

如需有關讓物件在整個系統內或公開使用的詳細資訊，請參閱[共用物件](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md)。

將物件設為私人：

1. 移至您要設為私用的物件。\
   例如，導覽至報表。
1. 按一下&#x200B;**報告動作**，然後按一下&#x200B;**共用**。

   ![設為私人](assets/report-permissions-make-private-nwe-350x477.png)

1. 按一下齒輪圖示，然後取消勾選&#x200B;**將此專案公開給外部使用者**。
1. 在&#x200B;**擁有存取權**&#x200B;下拉式功能表中，按一下&#x200B;**只有受邀者才能存取**&#x200B;以停止與所有Workfront使用者共用。
1. 按一下「**儲存**」。
