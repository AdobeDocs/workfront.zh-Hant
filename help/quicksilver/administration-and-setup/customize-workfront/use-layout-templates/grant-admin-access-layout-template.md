---
title: 授予配置範本的管理存取權
user-type: administrator
product-area: system-administration;templates;user-management
navigation-topic: layout-templates
description: 作為Adobe Workfront管理員，您可以將版面配置範本的管理存取權授與特定群組的群組管理員，以便他們編輯範本。 這不會將範本指派給群組中的使用者。
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: 066a55ef-1904-4678-8866-c59428f78bc1
source-git-commit: a8214d9e10363881afbc2bd71f78f46cb6a25880
workflow-type: tm+mt
source-wordcount: '440'
ht-degree: 0%

---

# 授予配置範本的管理存取權

作為Adobe Workfront管理員，您可以將版面配置範本的管理存取權授與特定群組的群組管理員，以便他們編輯範本。 這不會將範本指派給群組中的使用者。

如需將使用者指派給配置範本的資訊，請參閱[將使用者指派給配置範本](../../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md)。

如需配置範本的詳細資訊，請參閱[建立和管理配置範本](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md)。

如需有關群組配置範本的資訊，請參閱[建立和修改群組的配置範本](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md)。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

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
   <td><p>系統管理員存取層級</p><p><b>注意</b>：如果您還是沒有存取權，請詢問您的Workfront管理員是否對您的存取層級設定了其他限制。 如需Workfront管理員如何修改存取層級的詳細資訊，請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## 授予配置範本的管理存取權

1. 開始使用版面配置範本，如[建立和管理版面配置範本](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md)中所述。
1. 按一下頁面頂端區段中的&#x200B;**授與**&#x200B;的存取權。
1. 在出現的方塊中，按一下&#x200B;**新增群組**，開始輸入群組的名稱，出現時按一下名稱，然後按一下&#x200B;**完成**。

   任何被指定為您指定之群組的群組管理員的使用者都可以管理配置範本。 但是，範本未指派給群組的成員以供其使用。 如需將配置範本指派給群組的相關資訊，請參閱本文中的[將配置範本指派給使用者](../../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md#assign)。

   >[!NOTE]
   >
   >* 當群組管理員建立版面配置範本時，必須指派管理存取權。 配置圖範本是指定給且僅對指定群組可見。 如需詳細資訊，請參閱[編輯使用者的設定檔](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)。 如需群組管理員的相關資訊，請參閱[群組管理員](../../../administration-and-setup/manage-groups/group-roles/group-administrators.md)。
   >   
   >* 如果您未將管理存取權授與特定群組的群組管理員，則所有可編輯使用者帳戶的使用者都會擁有版面配置範本的管理存取權。 有些Workfront管理員故意選擇不授予版面配置範本的管理存取權，以便使其成為系統層級的版面配置範本。

1. 您可以隨時按一下「儲存」以儲存進度，然後繼續修改範本。
