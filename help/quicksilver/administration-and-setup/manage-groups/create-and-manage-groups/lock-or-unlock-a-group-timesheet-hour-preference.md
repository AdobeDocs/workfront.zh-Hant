---
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: create-and-manage-groups
title: 鎖定或解除鎖定群組時程表和小時喜好設定
description: 如果您是群組管理員，可以在Workfront管理員在系統層級解除鎖定您的群組後，設定並鎖定該群組的時程表和小時偏好設定。
author: Becky
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 5b36106f-d521-4cc1-9f1f-647415c282b4
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '600'
ht-degree: 0%

---

# 鎖定或解鎖群組時程表和小時偏好設定

如果您是群組管理員，可以在Workfront管理員在系統層級解除鎖定您的群組後，設定並鎖定該群組的時程表和小時偏好設定。

鎖定Adobe Workfront偏好設定可確保群組及其子群組中的每個人都使用該偏好設定的相同設定。 雖然您仍然可以重新設定您鎖定的偏好設定，但群組管理員無法對較低子群組這麼做。

反之，在群組層級解鎖偏好設定，可讓子群組管理員更靈活地管理其群組處理這些專案的方式。 解鎖偏好設定後，群組管理員可以為其重新設定這些子群組。

此功能與Workfront管理員必須鎖定或解除鎖定系統中每個人的偏好設定的功能平行。

如需Workfront管理員如何鎖定或解除鎖定系統中所有群組的時程表和小時偏好設定的相關資訊，請參閱[設定時程表和小時偏好設定](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md)。

如需有關設定群組的時程表和小時喜好設定的資訊，請參閱[設定群組的時程表和小時喜好設定](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-timesheet-hour-preferences-group.md)。

<!--
Unlike other Lock/Unlock articles that start just like this one, we need the steps here. In other areas, the lock/unlock step is part of the article about setting preferences or creating statuses.</p>
-->

>[!NOTE]
>
>* 設定群組的解除鎖定偏好設定不會影響群組底下任何子群組的該偏好設定。
>
>  但是，建立新的子群組時，它會繼承其上方群組的偏好設定和鎖定或解除鎖定狀態。
>
>* 如果您將群組移到具有鎖定偏好設定的群組下，則移動的群組會繼承該偏好設定，而且會為移動的群組鎖定該偏好設定。
>* 如果您將群組移動到具有已解除鎖定偏好設定的群組下，則已移動的群組不受該偏好設定影響。
>
>  如果移動時鎖定了已移動群組中的偏好設定，則該偏好設定會維持鎖定狀態，但群組管理員現在可以將其解鎖，因為已為父群組解除鎖定。

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
   <td>您必須是群組的群組管理員或系統管理員。</td>
  </tr>
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 鎖定或解鎖群組時程表和小時偏好設定

>[!TIP]
>
>如果您是Workfront管理員，可以前往「設定>時程表和時數>偏好設定」，然後在頁面頂端的方塊中搜尋群組名稱，略過步驟1至4。

{{step-1-to-setup}}

1. 在左側面板中，按一下&#x200B;**群組**。
1. 按一下您要鎖定或解除鎖定時程表和時數偏好設定的群組名稱。
1. 在左側面板中，按一下&#x200B;**時程表和時數偏好設定**。

1. 在出現的頁面上，執行下列任一項作業：

   * 如果您希望群組下方的群組管理員能夠設定其群組的偏好設定，請將其解除鎖定![解除鎖定切換](assets/unlock-toggle-button.png)。
   * 如果您希望下方的所有群組都使用您的設定進行偏好設定，請確定已將其鎖定![鎖定切換](assets/lock-toggle-button.png) （此為預設值）。

     >[!IMPORTANT]
     >
     >請務必與您下方群組中的管理員和使用者溝通，以確保以您設定鎖定偏好設定的方式考慮到所有需求。 鎖定時，其設定會由下方的任何子群組繼承。 如果偏好設定已解除鎖定任何時間段，您的設定會取代較低子群組中的群組管理員可能進行的設定。

1. 按一下「**儲存**」。
