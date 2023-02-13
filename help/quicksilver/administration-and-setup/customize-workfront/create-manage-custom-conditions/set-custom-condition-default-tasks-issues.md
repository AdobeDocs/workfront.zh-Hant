---
title: 將自訂條件設為工作和問題的預設值
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-conditions
description: 當用戶按一下「工作」或將更新注釋添加到已分配給的新任務時（無需手動設定任務的條件）,Adobe Workfront將顯示任務的預設條件，該條件在「設定」中配置。 問題也是如此。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 40b426f4-0a9c-49a6-91c7-b5f8aa48bd37
source-git-commit: a3cb3d9d340d377e301c98480324bfe8bf507382
workflow-type: tm+mt
source-wordcount: '407'
ht-degree: 0%

---

# 將自訂條件設為工作和問題的預設值

當用戶按一下「工作」或將更新注釋添加到已分配給的新任務時（無需手動設定任務的條件）,Adobe Workfront將顯示任務的預設條件，該條件在「設定」中配置。 問題也是如此。

Workfront會使用內建條件「順利進行」作為工作的預設條件，以及個別用於問題。 身為Workfront管理員，您可以將這兩種物件類型的預設條件變更為您建立的自訂條件。

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
   <td> <p>您必須是Workfront管理員。</p> <p><b>注意</b>:如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 將自訂條件設為工作或問題的預設條件：

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **設定** ![](assets/gear-icon-settings.png).

1. 按一下 **專案偏好設定** > **條件**.

1. 按一下 **工作** 或 **問題** 標籤。

1. 按一下 **設定預設條件**.
1. 在下拉式功能表中，按一下您想要的自訂條件，作為工作（或問題）的預設條件。
1. 按一下&#x200B;**儲存**。

>[!NOTE]
>
>* 已指派給任務或問題的使用者，或擁有該任務或問題的「管理」權限的使用者，可以手動變更其條件。 如需詳細資訊，請參閱 [更新任務和問題的條件](../../../manage-work/projects/updating-work-in-a-project/update-condition-for-tasks-and-issues.md).
>* 隨Workfront一起出現的任務和問題的三個預設條件是：進展順利、一些擔憂和主要障礙。 您無法隱藏或刪除這些條件，但可以變更其名稱和顏色。 或者，您可以建立新的使用項目，如 [建立或編輯自訂條件](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).
>


如需將自訂條件設定為專案預設條件的相關資訊，請參閱 [將自訂條件設為專案的預設值](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-projects.md).

如需自訂條件的相關資訊，請參閱 [自訂條件](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/custom-conditions.md).
