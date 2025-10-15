---
title: 設定自訂條件為任務和問題的預設值
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-conditions
description: 當使用者按一下處理它或將更新評論新增到他們被指派的新任務（不手動設定任務的條件），Adobe Workfront顯示任務的預設條件，這在「設定」中設定。 同樣的情況也適用於問題。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 40b426f4-0a9c-49a6-91c7-b5f8aa48bd37
source-git-commit: 366043a786c94f1bc40ad3b20af175bb84c94742
workflow-type: tm+mt
source-wordcount: '348'
ht-degree: 1%

---

# 設定自訂條件作為任務和問題的預設值

當使用者按一下處理它或將更新評論新增到他們被指派的新任務（不手動設定任務的條件），Adobe Workfront顯示任務的預設條件，這在「設定」中設定。 同樣的情況也適用於問題。

Workfront使用內建條件「順利進行」作為任務的預設條件，如果是問題，則另外使用。 身為Workfront管理員，您可以將這兩種物件型別的預設條件變更為您已建立的自訂條件。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront套件</td> 
   <td><p>任何</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront授權</td> 
   <td><p>標準</p>
       <p>規劃</p></td>
  </tr> 
  <tr> 
   <td>存取層級設定</td> 
   <td>系統管理員</td> 
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 將自訂條件設定為任務或問題的預設條件：

{{step-1-to-setup}}

1. 按一下&#x200B;**專案偏好設定** > **條件**。

1. 按一下「**任務**」或「**問題**」標籤。

1. 按一下&#x200B;**設定預設條件**。
1. 在下拉式功能表中，按一下您想要作為任務（或問題）預設條件的自訂條件。
1. 按一下「**儲存**」。

>[!NOTE]
>
>* 指派給任務或問題的使用者，或對其具有「管理」許可權的使用者，可以手動變更其條件。 如需詳細資訊，請參閱[更新任務和問題的條件](../../../manage-work/projects/updating-work-in-a-project/update-condition-for-tasks-and-issues.md)。
>* Workfront隨附的任務和問題的三個預設條件進行得很順利、有一些問題和主要障礙。 您無法隱藏或刪除這些條件，但可以變更其名稱和顏色。 或者，您可以建立新的條件來取代使用，如[建立或編輯自訂條件](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md)中所述。

如需將自訂條件設定為專案預設條件的詳細資訊，請參閱[將自訂條件設定為專案的預設值](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-projects.md)。
