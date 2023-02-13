---
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: create-and-manage-groups
title: 鎖定或解除鎖定子組的項目、任務或問題首選項
description: 作為組管理員，如果Workfront管理員在系統級別解除了項目、任務或問題首選項的鎖定，則可以進行配置。
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 05c32b6f-52e1-46a7-9011-633713422f3d
source-git-commit: 02191d80ea58f80de2e7be2ff55f43663e415e31
workflow-type: tm+mt
source-wordcount: '600'
ht-degree: 0%

---

# 鎖定或解除鎖定子組的項目、任務或問題首選項

作為組管理員，如果Workfront管理員在系統級別解除了項目、任務或問題首選項的鎖定，則可以進行配置。

鎖定您在級別配置的項目、任務或問題首選項可確保組及其子組中的每個人使用該首選項的相同設定。 雖然您仍可以重新設定您為群組鎖定的偏好設定，但群組管理員無法重新設定群組的偏好設定。

反之，解鎖項目、任務或問題首選項使組管理員能夠更靈活地管理其組處理這些項目的方式。 當首選項解除鎖定時，組管理員可以為這些子組重新配置它。

這與Workfront管理員必須鎖定或解除鎖定系統中每個人的偏好設定功能平行。

有關Workfront管理員如何鎖定或解鎖系統中所有組的首選項的資訊，請參見 [鎖定或解鎖系統中所有組的項目首選項](../../../administration-and-setup/set-up-workfront/configure-system-defaults/lock-or-unlock-project-preferences-for-groups-system.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Unlike other Lock/Unlock articles that start just like this one, we need the steps here. In other areas, the lock/unlock step is part of the article about setting preferences or creating statuses.</p>
-->

>[!NOTE]
>
>* 為組配置未鎖定首選項不會影響組下任何子組的該首選項。
>
>  但是，建立新子組時，它會繼承首選項設定，並且會繼承組上方的鎖定或解鎖狀態。
>
>* 如果在具有鎖定首選項的組下移動組，則移動的組會繼承該首選項，並且會為移動的組鎖定該首選項。
>* 如果在具有未鎖定首選項的組下移動組，則移動的組不受該首選項的影響。
>
>  如果移動組中的首選項在移動時被鎖定，則它仍然被鎖定，但組管理員可以立即將其解鎖，因為它已為父組解鎖。

## 存取需求

您必須具備下列條件才能執行本文所述步驟：

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
   <td> <p>計劃 </p> <p>您必須是群組的群組管理員或Workfront管理員。 如需詳細資訊，請參閱 <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">群組管理員</a> 和 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予使用者完整的管理存取權</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;如果您需要了解您擁有的計畫或授權類型，請聯絡Workfront管理員。

## 鎖定或解除鎖定組項目、任務或問題首選項

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **設定** ![](assets/gear-icon-settings.png).

1. 在左側面板中，按一下 **群組**.
1. 按一下要鎖定或解除鎖定項目首選項的組的名稱。
1. 在左側面板中，按一下 **專案偏好設定** 或 **任務和問題首選項**.

1. 在顯示的頁面上，對於在系統級別上已解鎖的首選項，或對於組上方的組，執行以下任一操作：

   * 如果您希望群組下的群組管理員能夠設定其群組的偏好設定，請解除鎖定 ![](assets/unlock-toggle-button.png).
   * 如果您希望下面的所有群組使用您的設定來設定偏好設定，請確定已鎖定 ![](assets/lock-toggle-button.png).

      >[!IMPORTANT]
      >
      >請務必與您下方群組的管理員和使用者通訊，以確保以您設定鎖定偏好設定的方式滿足所有需求。 當您鎖定它時，下面的任何子組將繼承您的配置。 如果首選項已在任意時間段內解除鎖定，則您的配置將替換下層子組中的組管理員可能所做的配置。

1. 按一下&#x200B;**儲存**。
