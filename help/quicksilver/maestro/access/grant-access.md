---
title: 授與Adobe大師的存取權
description: 瞭解如何在Adobe Maestro中授與存取權和共用資訊。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 475a519d-d3bd-4461-8099-0e296d556d34
source-git-commit: 85f499a429d4223c62b7b13dc0b1d10e8e79e9ed
workflow-type: tm+mt
source-wordcount: '403'
ht-degree: 0%

---

<!--update the metadata and description when we turn this article live; also, update title after Bob adds Maestro as a product-->

# 授與Adobe大師的存取權

>[!IMPORTANT]
>
>本文資訊是指Adobe Maestro，這是Adobe Workfront的新產品。
>
>目前，Adobe大師是測試版計畫的一部分，向有限數量的客戶開放。 您必須是Workfront客戶才能存取Maestro
>
>如需加入Maestro測試版計畫的詳細資訊，請聯絡您的客戶代表。
>
>如需詳細資訊，請參閱 [Adobe大師概觀](../maestro-overview.md).

貴組織的所有使用者都可以存取Maestro，前提為具備下列必要條件：

<!--the first requisite will be removed when we go to GA-->

* 貴組織已註冊AdobeMaestro封閉測試版計畫。
* 作為系統管理員，您必須使用版面配置範本將Maestro區域新增到「主功能表」。

  Maestro預設不會顯示在任何使用者的主功能表中，包括系統管理員。

  如需詳細資訊，請參閱 [使用版面配置範本自訂主功能表](../../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md).

<!-- take out the note below when we release permissions-->

>[!NOTE]
>
>沒有與使用者或Maestro中的資訊相關聯的存取層級或許可權。 所有在其環境中啟用Maestro的使用者都可以檢視、編輯和刪除任何其他使用者新增到Maestro的所有資訊。

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Adobe產品</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront合約</p></td>
   <td>
<p>貴組織必須註冊AdobeMaestro封閉測試版計畫。 請聯絡您的客戶代表以查詢此新產品/服務。 </p>
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
   <td> <p>任何使用Maestro</p>
   <p>系統管理員或計畫在版面配置範本中共用大師</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>版面配置範本</p></td>
   <td> <p>您的Workfront或群組管理員必須將Maestro區域新增至您的版面配置範本。 </p>  
</td>
  </tr>
 </tbody>
</table>

<!--
When permissions is released:

* leave as is for Access levels (I think)
* Add a new row for Permissions: System admin or Manage access to the workspace to share a workspace with others
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

<!--

## Share permissions to a workspace

The following users can share a workspace with other users:

* System administrators can share all workspaces, including the ones that they did not create.
* All other users can share only workspaces for which they have Manage permissions to. 

To share a workspace with others: 

1. Click the **Main Menu** icon ![](assets/dots-main-menu.png) in the upper-right or the **Main Menu** icon ![](assets/lines-main-menu.png) in the upper-left corner or Workfront, if available, then click **Maestro**.
1. Open the workspace you want to share, then click **Share** in the upper-right corner of the screen. (*************add screen shot when UI is finalized and maybe edit the steps*********)
1. In the field provided, start typing the name of a user or a group (******ensure you can share with groups*******), then click it when it displays in the list. 
1. Select one of the following permission levels from the drop-down menu: 
    * View
    * Contribute
    * Manage

        For information about permission levels and what actions users can perform for each level, see [Overview of sharing permissions in Adobe Maestro](../access/sharing-permissions-overview.md).
1. Click **Save**.


## Remove permissions to a workspace

1. Click the **Main Menu** icon ![](assets/dots-main-menu.png) in the upper-right or the **Main Menu** icon ![](assets/lines-main-menu.png) in the upper-left corner of Workfront, if available, then click **Maestro**.
1. Open the workspace you want to remove permissions to, then click **Share** in the upper-right corner of the screen. (********add screen shot when UI is finalized and maybe edit the steps???****)
1. Click the drop-down menu to the right of a user or group name, then click **Remove**. 
1. Click **Save**.

    The user or the users that belong to the group removed no longer have access to the workspace or its objects. 

-->