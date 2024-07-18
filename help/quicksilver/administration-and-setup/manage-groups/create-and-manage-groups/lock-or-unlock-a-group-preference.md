---
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: create-and-manage-groups
title: 鎖定或解除鎖定子群組的專案、任務或問題偏好設定
description: 身為群組管理員，您可以設定專案、任務或問題偏好設定，然後加以鎖定(如果Workfront管理員在系統層級將其解除鎖定)。
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 05c32b6f-52e1-46a7-9011-633713422f3d
source-git-commit: 02191d80ea58f80de2e7be2ff55f43663e415e31
workflow-type: tm+mt
source-wordcount: '600'
ht-degree: 0%

---

# 鎖定或解除鎖定子群組的專案、任務或問題偏好設定

身為群組管理員，您可以設定專案、任務或問題偏好設定，然後加以鎖定(如果Workfront管理員在系統層級將其解除鎖定)。

鎖定已在層級設定的專案、任務或問題偏好設定，可確保群組及其子群組中的每個人都使用該偏好設定的相同設定。 雖然您仍然可以重新設定您為群組鎖定的喜好設定，但群組管理員無法為群組重新設定它。

反之，解鎖專案、任務或問題偏好設定可讓群組管理員擁有更大的彈性，可管理其群組處理這些專案的方式。 解鎖偏好設定後，群組管理員可以為其重新設定這些子群組。

此功能與Workfront管理員必須鎖定或解除鎖定系統中每個人的偏好設定的功能平行。

如需Workfront管理員如何鎖定或解除鎖定系統中所有群組的偏好設定的相關資訊，請參閱[鎖定或解除鎖定系統中所有群組的專案偏好設定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/lock-or-unlock-project-preferences-for-groups-system.md)。

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Unlike other Lock/Unlock articles that start just like this one, we need the steps here. In other areas, the lock/unlock step is part of the article about setting preferences or creating statuses.</p>
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
>

## 存取需求

您必須具備下列專案才能執行本文所述的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront計畫*</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>計劃 </p> <p>您必須是群組的群組管理員或Workfront管理員。 如需詳細資訊，請參閱<a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">群組管理員</a>和<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授與使用者完整管理存取權</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;如果您需要瞭解您擁有的計畫或授權型別，請連絡您的Workfront管理員。

## 鎖定或解除鎖定群組專案、任務或問題偏好設定

1. 按一下Adobe Workfront右上角的&#x200B;**主要功能表**&#x200B;圖示![](assets/main-menu-icon.png)，然後按一下&#x200B;**設定** ![](assets/gear-icon-settings.png)。

1. 在左側面板中，按一下&#x200B;**群組**。
1. 按一下您要鎖定或解除鎖定專案偏好設定的群組名稱。
1. 在左側面板中，按一下&#x200B;**專案偏好設定**&#x200B;或&#x200B;**任務與問題偏好設定**。

1. 在出現的頁面上，針對系統層級上已解鎖的偏好設定或群組上方的群組執行下列任一動作：

   * 如果您希望群組下方的群組管理員能夠設定其群組的偏好設定，請解除鎖定![](assets/unlock-toggle-button.png)。
   * 如果您希望下方的所有群組都使用您的設定進行偏好設定，請確定它已鎖定![](assets/lock-toggle-button.png)。

     >[!IMPORTANT]
     >
     >請務必與您下方群組中的管理員和使用者溝通，以確保以您設定鎖定偏好設定的方式考慮到所有需求。 鎖定時，其設定會由下方的任何子群組繼承。 如果偏好設定已解除鎖定任何時間段，您的設定會取代較低子群組中的群組管理員可能進行的設定。

1. 按一下「**儲存**」。
