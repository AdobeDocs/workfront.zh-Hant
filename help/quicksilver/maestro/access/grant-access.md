---
title: 授與Adobe大師的存取權
description: 瞭解如何在Adobe Maestro中授與存取權和共用資訊。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 475a519d-d3bd-4461-8099-0e296d556d34
source-git-commit: 90c730bbab2e62bcc60bee37272edb1219b2afb4
workflow-type: tm+mt
source-wordcount: '301'
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

<!-- the table will change after we implement access levels/ permissions for Maestro-->
<!-- fix the formatting on the table - some lines are way too spaced out-->

目前，如果具備以下先決條件，您組織中的所有使用者都可以存取Maestro：

* 貴組織已註冊AdobeMaestro封閉測試版計畫。

  請聯絡您的客戶代表以查詢此新產品/服務。


如需有關使用Maestro時所需存取許可權的資訊，請參閱 [Adobe大師存取概觀](../access/access-overview.md).

>[!NOTE]
>
>沒有與使用者或Maestro中的資訊相關聯的存取層級或許可權。 所有在其環境中啟用Maestro的使用者都可以檢視、編輯和刪除任何其他使用者新增到Maestro的所有資訊。

## 為您的Workfront執行個體中的使用者啟用Maestro

<!--First, contact your account manager to obtain access to the current Maestro closed beta program.-->

貴組織註冊Maestro測試版計畫後，您可以使用版面配置範本為其他使用者新增Maestro區域。

若要使用版面配置範本共用主區域：

1. 登入 **Workfront** Workfront管理員。

1. 新增 **大師** 圖示 ![](assets/maestro-icon.png) 至 **主要功能表** 使用 **版面配置範本**.

   如需詳細資訊，請參閱 [使用版面配置範本自訂主功能表](../../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md).

1. 將版面配置範本指派給您要存取Maestro的使用者。

   如需詳細資訊，請參閱 [將使用者指派至版面配置範本](../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md).

   所有指派給範本的使用者現在可以在他們的主功能表中存取Maestro。

   使用者可以開始建立工作區、記錄型別、記錄和欄位。

<!--
## Share permissions to a workspace

1. Click the **Main Menu** icon ![](assets/dots-main-menu.png) in the upper-right or the **Main Menu** icon ![](assets/lines-main-menu.png) in the upper-left corner, if available, then click **Maestro**.
1. Open the workspace you want to share, then click **Share** in the upper-right corner of the screen. (*************add screen shot when UI is finalized and maybe edit the steps*********)
1. In the field provided, start typing the name of a user or a group, then click it when it displays in the list. 
1. Select one of the following permission levels from the drop-down menu: 
    * View
    * Contribute
    * Manage

        For information about permission levels and what actions users can perform for each level, see [Overview of sharing permissions in Adobe Maestro](../access/sharing-permissions-overview.md).
1. Click **Save**.


## Remove permissions to a workspace

1. Click the **Main Menu** icon ![](assets/dots-main-menu.png) in the upper-right or the **Main Menu** icon ![](assets/lines-main-menu.png) in the upper-left corner, if available, then click **Maestro**.
1. Open the workspace you want to share, then click **Share** in the upper-right corner of the screen. (********) add screen shot when UI is finalized and maybe edit the steps???****)
1. Click the drop-down menu at the right of a user or group name, then click **Remove**. 
    
    The user or the users that belong to the group removed no longer have access to the workspace or its objects. 
1. Click **Save**.

-->