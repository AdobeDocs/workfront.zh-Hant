---
title: 授與Adobe大師的存取權
description: 瞭解如何在Adobe Maestro中授與存取權和共用資訊。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 475a519d-d3bd-4461-8099-0e296d556d34
source-git-commit: 937498a68a994d19b0005d518d7e313c48961672
workflow-type: tm+mt
source-wordcount: '316'
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

Only system administrators can access all workspaces in Maestro. As a system administrator, you must share a workspace with other users for them to view, manage, or contribute to it. 

To share a workspace with others: 

1. Click the **Main Menu** icon ![](assets/dots-main-menu.png) in the upper-right or the **Main Menu** icon ![](assets/lines-main-menu.png) in the upper-left corner, if available, then click **Maestro**.
1. Open the workspace you want to share, then click **Share** in the upper-right corner of the screen. (*************add screen shot when UI is finalized and maybe edit the steps*********)
1. In the field provided, start typing the name of a user or a group (******ensure you can share with groups*******), then click it when it displays in the list. 
1. Select one of the following permission levels from the drop-down menu: 
    * View
    * Contribute
    * Manage

        For information about permission levels and what actions users can perform for each level, see [Overview of sharing permissions in Adobe Maestro](../access/sharing-permissions-overview.md).
1. Click **Save**.


## Remove permissions to a workspace

1. Click the **Main Menu** icon ![](assets/dots-main-menu.png) in the upper-right or the **Main Menu** icon ![](assets/lines-main-menu.png) in the upper-left corner, if available, then click **Maestro**.
1. Open the workspace you want to share, then click **Share** in the upper-right corner of the screen. (********add screen shot when UI is finalized and maybe edit the steps???****)
1. Click the drop-down menu at the right of a user or group name, then click **Remove**. 
    
    The user or the users that belong to the group removed no longer have access to the workspace or its objects. 
1. Click **Save**.

-->