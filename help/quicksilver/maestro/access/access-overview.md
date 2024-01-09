---
title: 存取權總覽
description: 組織中的所有使用者都可以存取Adobe大師。 目前，沒有與使用者或Maestro中的資訊相關聯的存取層級或許可權。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 99fac041-a235-4991-b826-d19944164bc9
source-git-commit: 4e3449e7c31d29e1a289a7866ba98f873e62922c
workflow-type: tm+mt
source-wordcount: '359'
ht-degree: 1%

---

<!--update the metadata with real things when making this public; also update the description with something like this: Not all users in the organization have the same access and permissions to use Adobe Maestro. This article describes the levels of access that users could have to Adobe Maestro. -->

# 存取權總覽

>[!IMPORTANT]
>
>本文資訊是指Adobe Maestro，這是Adobe Workfront的新產品。
>
>目前，Adobe大師是測試版計畫的一部分，向有限數量的客戶開放。 您必須是Workfront客戶才能存取Maestro。
>
>如需加入Maestro測試版計畫的詳細資訊，請聯絡您的客戶代表。
>
>如需詳細資訊，請參閱 [Adobe大師概觀](../maestro-overview.md).

Adobe大師(Maestro)沒有存取層級限制。

您組織中的所有使用者都可以存取Maestro，無論其存取層級為何。

<!-- the table will change after we implement access levels/ permissions for Maestro-->
<!-- fix the formatting on the table - some lines are way too spaced out-->

## 存取需求

您必須具備下列專案才能使用Adobe大師：

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> 產品</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront合約</p></td>
   <td>
<p>貴組織必須註冊AdobeMaestro封閉測試版計畫。  </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront計畫</p></td>
   <td>
<p>任何</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront授權</p></td>
   <td>
   <p>任何</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>存取層級</p></td>
   <td> <p>任何</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>版面配置範本</p></td>
   <td> <p>您的Workfront管理員必須新增主功能表中的Maestro區域到您的版面配置範本。</p> 
   <p>如需詳細資訊，請參閱 <a href="../../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md">使用版面配置範本自訂主功能表</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

<!--After we enable permissions, replace the section content above with this:

There are license and sharing permission restrictions to use Adobe Maestro capabilities. (*********** this should be the intro right under the title; also update the metadata with this when live*******)

You must have the following settings to use Adobe Maestro: 

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Product</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the Adobe Maestro closed beta program. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license*</p></td>
   <td>
   <p>Any</p>
   To create workspaces, users must have the following license: 
   <ul><li><p>New: Standard</p> </li>
   <li><p>Current: Worker or higher</p> </li></ul>
  </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Access level configuration</p></td>
   <td> <p>There are no access level controls for Maestro objects</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Object permissions</p></td>
   <td>
   <p>Contribute or higher permissions to workspaces and views that you did not create to edit, delete, and share them</p>
    <p>System Administrators can manage workspaces and views they did not create </p>
   <p>For information about sharing permissions for Maestro objects, see  
   <a href="../access/sharing-permissions-overview.md">Overview of sharing permissions in Adobe Maestro</a> 
  </td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your system administrator must add the Maestro area in the Main Menu to your layout template.</p> 
   <p>For information, see <a href="../../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md">Customize the Main Menu using a layout template</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

*For more information about the new and current pricing models, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).  

-->

## 與其他共用主功能表中的Maestro區域

<!--First, contact your account manager to obtain access to the current Maestro closed beta program.-->

貴組織註冊Maestro測試版計畫後，您可以使用版面配置範本將Maestro區域新增到所有使用者的主功能表中。

1. 登入 **Workfront** Workfront管理員。

1. 新增 **大師** 圖示 ![](assets/maestro-icon.png) 至 **主要功能表** 使用 **版面配置範本**.

   如需詳細資訊，請參閱 [使用版面配置範本自訂主功能表](../../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md).

1. 將版面配置範本指派給您要存取Maestro的使用者。

   如需詳細資訊，請參閱 [將使用者指派至版面配置範本](../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md).

   所有指派給範本的使用者現在可以在他們的主功能表中存取Maestro。

   使用者可以開始建立工作區、記錄型別、記錄和欄位。

## 授予存取權

Maestro沒有存取控制。

擁有任何授權型別的使用者都可以存取Maestro。

## 授予許可權

沒有與Maestro物件關聯的許可權。

所有在其環境中啟用Maestro的使用者都可以檢視、編輯和刪除任何其他使用者新增到Maestro的所有資訊。

<!--
Take out the text above and replace with this: 

For more information, see [Sharing permissions overview in Adobe Maestro](/help/quicksilver/maestro/access/sharing-permissions-overview.md).-->


