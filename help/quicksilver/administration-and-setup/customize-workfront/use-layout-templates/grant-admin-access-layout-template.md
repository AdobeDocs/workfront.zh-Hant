---
title: 授予版面範本的管理存取權
user-type: administrator
product-area: system-administration;templates;user-management
navigation-topic: layout-templates
description: 身為Adobe Workfront管理員，您可以將配置範本的管理存取權授予特定群組的群組管理員，以便他們編輯範本。 這不會將範本指派給群組中的使用者。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 066a55ef-1904-4678-8866-c59428f78bc1
source-git-commit: e20934501c2117455ca7950834d868f78576dee7
workflow-type: tm+mt
source-wordcount: '429'
ht-degree: 0%

---

# 授予版面範本的管理存取權

身為Adobe Workfront管理員，您可以將配置範本的管理存取權授予特定群組的群組管理員，以便他們編輯範本。 這不會將範本指派給群組中的使用者。

有關將用戶分配到佈局模板的資訊，請參閱 [將使用者指派至版面範本](../../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md).

如需版面範本的詳細資訊，請參閱 [建立和管理版面範本](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

如需群組版面範本的相關資訊，請參閱 [建立和修改群組的版面範本](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

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
   <td role="rowheader">訪問級別配置</td> 
   <td><p>系統管理員訪問級別</p><p><b>注意</b>:如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 授予版面範本的管理存取權

1. 開始使用版面範本，如 [建立和管理版面範本](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
1. 按一下 **授予的存取權** 在頁面頂端的區段中。
1. 在出現的方塊中，按一下 **新增群組**，開始輸入群組名稱，在出現時按一下名稱，然後按一下 **完成**.

   任何指定為您指定之群組之群組管理員的使用者，皆可管理配置範本。 但是，該模板沒有分配給組的成員以供其使用。 有關為組分配佈局模板的資訊，請參閱 [將版面範本指派給使用者](../../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md#assign) 這篇文章。

   >[!NOTE]
   >
   >* 當群組管理員建立配置範本時，必須指派管理存取權。 版面模板被指定為，並且只對指定的組可見。 如需詳細資訊，請參閱 [編輯使用者的設定檔](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md). 如需群組管理員的相關資訊，請參閱 [群組管理員](../../../administration-and-setup/manage-groups/group-roles/group-administrators.md).
   >   
   >* 如果您未授予特定群組中群組管理員的管理存取權，所有可編輯使用者帳戶的使用者都可以管理配置範本的存取權。 有些Workfront管理員有目的地選擇不授予版面範本的管理存取權，以使其成為系統層級的版面範本。


1. 您可以隨時按一下「儲存」以儲存進度，然後稍後繼續修改範本。
