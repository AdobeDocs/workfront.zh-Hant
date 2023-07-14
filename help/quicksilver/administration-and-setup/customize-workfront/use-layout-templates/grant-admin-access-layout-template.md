---
title: 授予配置範本的管理存取權
user-type: administrator
product-area: system-administration;templates;user-management
navigation-topic: layout-templates
description: 作為Adobe Workfront管理員，您可以授予配置範本的管理存取權給特定群組的群組管理員，以便他們能夠編輯範本。 這不會將範本指派給群組中的使用者。
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: 066a55ef-1904-4678-8866-c59428f78bc1
source-git-commit: 7ee96045e5673c51c3ce348f395226857686a923
workflow-type: tm+mt
source-wordcount: '429'
ht-degree: 0%

---

# 授予配置範本的管理存取權

作為Adobe Workfront管理員，您可以授予配置範本的管理存取權給特定群組的群組管理員，以便他們能夠編輯範本。 這不會將範本指派給群組中的使用者。

如需將使用者指派至版面配置範本的相關資訊，請參閱 [將使用者指派至版面配置範本](../../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md).

如需版面配置範本的詳細資訊，請參閱 [建立和管理版面範本](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

如需有關群組版面配置範本的資訊，請參閱 [建立和修改群組的版面配置範本](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td>計劃</td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td><p>系統管理員存取層級</p><p><b>注意</b>：如果您還是沒有存取權，請洽詢Workfront管理員，瞭解他們是否對您的存取層級設定其他限制。 如需有關Workfront管理員如何修改您的存取層級的資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 授予配置範本的管理存取權

1. 開始使用版面範本，如所述 [建立和管理版面範本](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
1. 按一下 **授予存取許可權** 在頁面的頂端區段中。
1. 在出現的方塊中，按一下 **新增群組**，開始輸入群組名稱，在群組出現時按一下名稱，然後按一下 **完成**.

   任何指定為您指定之群組的群組管理員的使用者都可以管理配置範本。 不過，範本並未指派給群組的成員以供其使用。 如需將版面配置範本指派給群組的相關資訊，請參閱 [指派配置範本給使用者](../../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md#assign) 本文章內容。

   >[!NOTE]
   >
   >* 當群組管理員建立版面配置範本時，必須指派管理存取權。 版面配置範本是指定給的，只有指定的群組可以看到。 如需詳細資訊，請參閱 [編輯使用者的設定檔](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md). 如需群組管理員的相關資訊，請參閱 [群組管理員](../../../administration-and-setup/manage-groups/group-roles/group-administrators.md).
   >   
   >* 如果您未授予管理許可權給特定群組中的群組管理員，則所有可以編輯使用者帳戶的使用者都會擁有版面配置範本的管理許可權。 有些Workfront管理員故意選擇不授予配置範本的管理存取權，以便使其成為系統層級的配置範本。

1. 您可以隨時按一下「儲存」以儲存進度，然後繼續稍後修改範本。
