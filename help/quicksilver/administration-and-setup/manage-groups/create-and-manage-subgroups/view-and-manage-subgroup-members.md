---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: 檢視和管理子群組成員
description: 當您檢視您管理的群組時，可以檢視和管理群組子群組中的所有使用者。
author: Becky
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 8f7b0183-6035-4dd4-8e42-fd65485449bf
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '382'
ht-degree: 0%

---

# 檢視和管理子群組成員

當您檢視您管理的群組時，可以檢視和管理群組子群組中的所有使用者。

如果您管理的群組之上有任何群組，其管理員也可以為您的群組執行此動作。 Workfront管理員也是如此（適用於任何群組）。

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
   <td> <p>您必須具備下列其中一項：</p> 
    <ul> 
     <li> <p>系統管理員存取層級。 </li> 
     <li> <p>您的存取層級中的<b>使用者</b>設定已設定為<b>編輯</b>存取權，其中<b>建立</b>以及在<b>微調您的設定</b> <b>下啟用的兩個</b>使用者管理員<img src="assets/gear-icon-settings.png">選項中的至少一個。 </p> <p>在這兩個選項中，如果已啟用<b>使用者管理員（群組使用者）</b>，您必須是使用者所屬群組的群組管理員。</p> </li> 
    </ul> </td> 
  </tr>  
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 檢視和管理群組下子群組的成員

{{step-1-to-setup}}

1. 按一下&#x200B;**群組**。

   在顯示的清單中，您可以看到您管理的群組及其擁有的任何子群組。 Adobe Workfront管理員可檢視所有群組。

1. 按一下您要檢視或管理子群組成員的群組名稱。
1. 在左側面板中，按一下&#x200B;**子群組成員**。

   此左側面板專案僅在群組具有子群組時才可用。

1. 執行下列任一項作業：

   * 在清單中選取成員，然後按一下[編輯] ![ [編輯]圖示](assets/edit-icon.png)以修改該使用者的使用者設定檔。

     如需詳細資訊，請參閱[編輯使用者的設定檔](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)或[大量編輯使用者的設定檔](../../../administration-and-setup/add-users/create-and-manage-users/edit-user-profiles-in-bulk.md)。

   * 選取清單中任意數量的子群組成員，然後按一下&#x200B;**傳送更新給使用者**，將註解新增至其使用者設定檔。

     使用者會收到應用程式內通知以及包含您評論的電子郵件通知。 註解會顯示在使用者設定檔的更新區域中。

     如需詳細資訊，請參閱[傳送直接訊息給其他使用者](/help/quicksilver/people-teams-and-groups/work-directly-with-others/send-direct-messages-to-other-users.md)。

   * 選取清單中任意數量的成員，然後按一下[停用![停用使用者](assets/deactivate-user.png)]或[啟用![啟用使用者](assets/activate-user.png)]。

     如需詳細資訊，請參閱[停用或重新啟用使用者](../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md)。

   * 匯出![匯出](assets/export.png)成員清單。
