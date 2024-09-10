---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: 檢視和管理子群組成員
description: 當您檢視您管理的群組時，可以檢視和管理群組子群組中的所有使用者。
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 8f7b0183-6035-4dd4-8e42-fd65485449bf
source-git-commit: 63c2206905f4ebbc35cb162ae6e895b98b5d20eb
workflow-type: tm+mt
source-wordcount: '384'
ht-degree: 0%

---

# 檢視和管理子群組成員

當您檢視您管理的群組時，可以檢視和管理群組子群組中的所有使用者。

如果您管理的群組之上有任何群組，其管理員也可以為您的群組執行此動作。 Workfront管理員也是如此（適用於任何群組）。

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
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td><p>新增：標準</p>
       <p>或</p>
       <p>目前：計畫</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>您必須具備下列其中一項：</p> 
    <ul> 
     <li> <p>系統管理員存取層級。 </li> 
     <li> <p>您的存取層級中的<b>使用者</b>設定已設定為<b>編輯</b>存取權，其中<b>建立</b>以及在<b>微調您的設定</b> <img src="assets/gear-icon-settings.png">下啟用的兩個<b>使用者管理員</b>選項中的至少一個。 </p> <p>在這兩個選項中，如果已啟用<b>使用者管理員（群組使用者）</b>，您必須是使用者所屬群組的群組管理員。</p> </li> 
    </ul> </td> 
  </tr>  
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 檢視和管理群組下子群組的成員

{{step-1-to-setup}}

1. 按一下&#x200B;**群組**。

   在顯示的清單中，您可以看到您管理的群組及其擁有的任何子群組。 Adobe Workfront管理員可檢視所有群組。

1. 按一下您要檢視或管理子群組成員的群組名稱。
1. 在左側面板中，按一下&#x200B;**子群組成員**。

   此左側面板專案僅在群組具有子群組時才可用。

1. 執行下列任一項作業：

   * 選取清單中的成員，然後按一下[編輯![](assets/edit-icon.png)]以修改該使用者的使用者設定檔。

     如需詳細資訊，請參閱[編輯使用者的設定檔](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)或[大量編輯使用者的設定檔](../../../administration-and-setup/add-users/create-and-manage-users/edit-user-profiles-in-bulk.md)。

   * 選取清單中任意數量的成員，然後按一下[更新![](assets/comment-icon.png)]，將註解新增至其使用者設定檔。

     使用者會收到應用程式內通知以及包含您評論的電子郵件通知。 註解會顯示在使用者設定檔的更新區域中。

   * 選取清單中任意數量的成員，然後按一下[停用![](assets/deactivate-user.png)]或[啟用![](assets/activate-user.png)]。

     如需詳細資訊，請參閱[停用或重新啟用使用者](../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md)。

   * 匯出![](assets/export.png)成員清單。
