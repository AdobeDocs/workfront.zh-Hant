---
product-area: resource-management
navigation-topic: resource-pools
title: 將資源池與用戶關聯
description: 將資源池與用戶關聯
author: Alina
feature: Resource Management
exl-id: 0816a2d6-2a45-4e01-8ca2-6d0d190b2568
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '494'
ht-degree: 0%

---

# 將資源池與用戶關聯

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: The info about how to add resource pools to users, are duplicated from the articles listed in those sections (Creating Users, etc). I decided to keep the steps here because those articles are too long to rummage through for updating just this one field.)</p>
-->

資源池是協助您在Adobe Workfront中管理資源的使用者集合。

您必須先建立資源池，才能將其與用戶關聯。

建立資源池時，可以將用戶與資源池關聯。

如果您建立資源池時沒有用用戶填充資源池，則以後可以在編輯或建立新用戶時將它們與用戶關聯。

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

## 將資源池與一個用戶關聯

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角。

1. 按一下 **使用者**.
1. 勾選清單中使用者名稱旁的方塊，然後按一下 **編輯**.
1. 按一下 **資源規劃**.
1. 開始鍵入要與中的用戶關聯的資源池的名稱 **資源池** 欄位，然後在出現時從清單中選取它。\
   您可以將多個資源池與一個用戶關聯。\
   ![add_resource_pool_to_user.png](assets/add-resource-pool-to-user-350x307.png)

1. 按一下 **儲存變更**.

如需編輯使用者的詳細資訊，請參閱 [編輯使用者的設定檔](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

如需建立新使用者的詳細資訊，請參閱 [新增使用者](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

## 將資源池與用戶大量關聯

您可以批量編輯多個用戶，並將相同的資源池與所有用戶同時關聯。

要將資源池與多個用戶大量關聯，請執行以下操作：

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角。

1. 按一下 **使用者**.
1. 在清單中選取數個使用者，然後按一下 **編輯**.
1. 按一下 **資源規劃**.
1. 開始鍵入要與中的用戶關聯的資源池的名稱 **資源池** 欄位，然後在出現時從清單中選取它。\
   您可以將多個資源池與多個用戶關聯。

   >[!NOTE]
   >
   >此欄位中只會顯示所有所選使用者的共同資源池。 如果所選用戶沒有共用資源池，則此欄位為空。 如果此欄位為空，則在此處指定的資源池將覆蓋其各個資源池。

1. 按一下 **儲存變更**.

如需如何大量編輯使用者的詳細資訊，請參閱 [大量編輯使用者設定檔](../../../administration-and-setup/add-users/create-and-manage-users/edit-user-profiles-in-bulk.md).
