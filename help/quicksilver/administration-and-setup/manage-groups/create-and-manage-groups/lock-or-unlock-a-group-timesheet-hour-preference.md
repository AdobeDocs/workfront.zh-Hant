---
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: create-and-manage-groups
title: 鎖定或解除鎖定組時間表和小時首選項
description: 如果您是組管理員，則可以配置並鎖定組的時間表和小時首選項，在Workfront管理員在系統級別上解鎖組後。
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 5b36106f-d521-4cc1-9f1f-647415c282b4
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '627'
ht-degree: 0%

---

# 鎖定或解除鎖定組時間表和小時首選項

如果您是組管理員，則可以配置並鎖定組的時間表和小時首選項，在Workfront管理員在系統級別上解鎖組後。

鎖定Adobe Workfront偏好設定可確保組及其子組中的每個人使用該偏好設定的相同設定。 雖然您仍可以重新配置您所鎖定的首選項，但組管理員不能為較低的子組重新配置。

相反，在組級別解鎖首選項使子組管理員能夠更靈活地管理其組處理這些項目的方式。 當首選項解除鎖定時，組管理員可以為這些子組重新配置它。

這與Workfront管理員必須鎖定或解除鎖定系統中每個人的偏好設定功能平行。

有關Workfront管理員如何鎖定或解除鎖定系統中所有組的時間表和小時首選項的資訊，請參閱 [配置工時單和小時首選項](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

有關配置組的時間表和小時首選項的資訊，請參閱 [配置組的時間表和小時首選項](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-timesheet-hour-preferences-group.md).

<!--
Unlike other Lock/Unlock articles that start just like this one, we need the steps here. In other areas, the lock/unlock step is part of the article about setting preferences or creating statuses.</p>
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

## 鎖定或解除鎖定組時間表和小時首選項

>[!TIP]
>
>如果您是Workfront管理員，可以前往「設定」>「時間表和小時」>「首選項」，然後在頁面頂端的方塊中搜尋群組名稱，以略過步驟1至4。

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **設定** ![](assets/gear-icon-settings.png).

1. 在左側面板中，按一下 **群組**.
1. 按一下要鎖定或解鎖工時單和工時首選項的組的名稱。
1. 在左側面板中，按一下 **工時單和工時首選項**.

1. 在顯示的頁面上，執行下列任一操作：

   * 如果您希望群組下的群組管理員能夠設定其群組的偏好設定，請解除鎖定 ![](assets/unlock-toggle-button.png).
   * 如果您希望下面的所有群組使用您的設定來設定偏好設定，請確定已鎖定 ![](assets/lock-toggle-button.png) （此為預設值）。

      >[!IMPORTANT]
      >
      >請務必與您下方群組的管理員和使用者通訊，以確保以您設定鎖定偏好設定的方式滿足所有需求。 當您鎖定它時，下面的任何子組將繼承您的配置。 如果首選項已在任意時間段內解除鎖定，則您的配置將替換下層子組中的組管理員可能所做的配置。

1. 按一下&#x200B;**儲存**。
