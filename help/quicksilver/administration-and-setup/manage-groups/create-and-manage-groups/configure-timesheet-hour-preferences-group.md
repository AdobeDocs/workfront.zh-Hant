---
user-type: administrator
product-area: system-administration;user-management
keywords: 組，首選項，任務，組，問題，解鎖
navigation-topic: create-and-manage-groups
title: 配置組的時間表和小時首選項
description: 在系統級別，Adobe Workfront管理員可以解鎖工時單和小時首選項部分「常規首選項」和「預填充工時單」。 這可讓群組管理員為自己的群組獨立設定這些區段中的選項。
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 1ee9343e-9452-4e41-a9ff-a6c865d4813b
source-git-commit: df55d6659fac7588610bc05ea0380a766b4277a2
workflow-type: tm+mt
source-wordcount: '1368'
ht-degree: 1%

---

# 配置組的時間表和小時首選項

Adobe Workfront管理員可以在系統層級解除鎖定下列時間表和小時偏好設定區段，讓群組管理員可以針對自己的群組獨立設定這些區段：

* 一般喜好設定
* 使用者記錄時間的位置
* 預填工時單

如果您管理的群組上方有任何群組，其管理員也可以對您的群組執行此動作。 Workfront管理員（適用於任何群組）也是如此。

「工時單」和「小時首選項」頁上的以下部分僅在系統級別可配置，並且無法為組解鎖：

* 已刪除的專案、任務和問題

有關Workfront管理員如何解除工時表和小時首選項鎖定的資訊，請參閱 [解鎖組的工時單和小時首選項](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md#lock) 在文章中 [配置工時單和小時首選項](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

>[!TIP]
>
>項目首選項以及任務和問題首選項也可以進行組級配置。 如需詳細資訊，請參閱 [配置組的項目首選項](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md) 和 [配置組的任務和問題首選項](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

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

## 組時間表和小時首選項

請考慮以下有關配置組的未鎖定時間表或小時首選項的資訊：

* 如果您是組管理員，並且為組配置了時間表或小時首選項，則會影響將組用作其首頁組的人員。
* 通常，未鎖定首選項會無限期保持未鎖定狀態。 如果Workfront管理員重新鎖定，系統設定會再次生效，且群組管理員所做偏好設定的設定會遺失。
* 工時單繼承為工時單所有者的「主組」配置的工時單和小時首選項。

   <!--
  Add example here?
  -->

* 在Workfront管理員解除系統層級的偏好設定鎖定並為群組進行設定後，您就可以鎖定偏好設定，以確保下方群組中的每個人都使用相同的設定。 這與Workfront管理員必須為系統中的每個人設定和鎖定偏好設定的功能平行。 如需詳細資訊，請參閱 [鎖定或解除鎖定組時間表和小時首選項](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-timesheet-hour-preference.md).

## 配置組的未鎖定時間表或小時首選項

>[!TIP]
>
>如果您是Workfront管理員，可以前往「設定」>「時間表和小時」>「首選項」，然後在頁面頂端的方塊中搜尋群組名稱，以略過步驟1至4。

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **設定** ![](assets/gear-icon-settings.png).

1. 在左側面板中，按一下 **群組** ![](assets/groups-icon.png).

1. 按一下要配置其工時單或小時首選項的組的名稱。
1. 在左側面板中，按一下 **工時單和小時數**.

1. 在顯示的頁面上， **一般偏好設定** ，請配置以下任一選項：

   >[!TIP]
   >
   >如果您將滑鼠指標暫留在偏好設定上，系統會顯示工具提示來告知您該偏好設定已鎖定，您可以要求Workfront管理員為組織中的所有群組解除鎖定。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">日期記錄時間</td> 
      <td> <p>可讓使用者在下列位置記錄系統中未來日期的時間：</p> 
       <ul> 
       <li>任何項目、任務和問題，無論項目組如何，它們都有權訪問日誌時間</li> 
       <li>他們的工時單作為一般時間</li>
       </ul> 
       <p>當用戶計畫離開辦公室並想提前登錄該時間時，此功能非常有用。</p> 
       <p><b>注意</b>:您無法阻止用戶登錄已關閉或已取消的任務或問題。 您只能防止使用者登入已完成或已停用的專案。 建議您在任務和問題清單中使用篩選器，以排除已完成或已取消的任務和問題，使用者無法看到這些任務和問題。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">添加工時單的費用</td> 
      <td> <p>允許用戶在工時單中記錄時間和費用。</p> 
      <p>為組啟用此首選項，並將組設定為某些用戶的主組時，這些用戶的工時單上的項目和任務旁邊將顯示一個費用表徵圖。 用戶可以按一下此表徵圖來添加或編輯項目或任務的費用。</p>
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">手動將作業角色分配給小時條目</td> 
      <td> <p>允許用戶手動選擇在其用戶配置檔案中分配或分配給對象的任何作業角色。</p> <p><b>重要</b>:  
        <ul> 
         <li>如果在將作業角色分配給工時條目後禁用此設定，則用戶必須調整項目、任務或問題的「工時」頁簽上各種角色下記錄的工時。</li> 
         <li>如果用戶在其配置檔案中沒有分配作業角色，並且在「高級分配」對話框中存在分配為「任務所有者」的任務，則當用戶記錄任務的時間時，將顯示該作業角色。</li> 
        </ul> </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">將時間表編輯限制給所有者和管理員</td> 
      <td> <p>不論項目的組和Workfront管理員如何，都限制對時間表所有者進行編輯。 禁用此選項時，還可以通過以下方式編輯工時單：</p> 
       <ul> 
        <li> <p>在訪問級別具有對工時單和小時的管理訪問權限的用戶</p> </li> 
        <li> <p>如果工時單上啟用了「可以編輯工時」，則工時單批准者</p> </li> 
        <li> <p>工時單所有者的管理員</p> </li> 
       </ul> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">限制對所有者和管理員進行小時編輯</td> 
      <td>限制編輯給輸入小時數的使用者和Workfront管理員。 此設定適用於專案或「小時」報表中的「小時」索引標籤。</td> 
     </tr> 
    </tbody> 
   </table>

1. 在 **使用者可在此記錄時間** ，請配置以下任一選項：

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader">直接在專案上記錄時間</td> 
      <td>允許用戶登錄項目的時間（在「更新」頁簽和時間表上）。 如果您想要限制使用者在專案層級記錄時間，請保留此選項為未勾選狀態。</td>
     </tr>
     <tr>
      <td role="rowheader">登錄已完成的項目</td>
      <td>允許用戶記錄已標籤為完成的項目上的時間。 如果禁用此選項，則用戶無法以「完成」狀態記錄在項目上完成的工作的時間。</td>
     </tr>
     <tr>
      <td role="rowheader">對已停用的專案登入時間</td> 
      <td>啟用此選項後，使用者可以登入處於「無效」狀態的專案數小時。</td>
     </tr>
    </tbody>
   </table>

   >[!NOTE]
   >
   >此首選項根據用戶的「首頁組」首選項的配置而應用。 如果在用戶的「首頁組」首選項中啟用了這些設定，則無論項目的組首選項是否允許，它們都能夠直接登錄項目，包括已完成或已結束的項目。

1. 在 **預填工時單** ，請配置以下任一選項：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">內的工作 &lt;number of="" weeks=""&gt; 工時單的工作範圍</td> 
      <td> <p>定義時間表日期範圍前後的周數，該時間表包含分配給用戶的任務和問題日期。 預設設定為1週，您可將此範圍延長至4週。 這表示，如果您為範圍選擇4週，則時間表預先填充任務和問題，這些任務和問題的日期在時間表日期範圍之前四週之間，最多在時間表日期範圍之後四週。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">已完成的任務和問題</td> 
      <td>如果通常將多個資源指派給單一任務，建議使用此設定。 這意味著，當一個資源根據任務記錄時間並將其標籤為已完成時，分配給任務的其他資源仍可以在其時間表中查找任務或問題，以記錄其小時數。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">工時單日期範圍內具有計畫日期的任務和問題</td> 
      <td> <p>選定後，工時單將包括具有計畫起始日期或完成日期且落在工時單日期範圍內的任務和問題。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> 在工時單的日期範圍內具有預計日期的任務</td> 
      <td> <p>選定後，時間表包括具有在項目時間範圍內的預計起始日期或完成日期的任務，即使問題或任務的計畫日期超出時間表日期範圍也是如此。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下&#x200B;**儲存**。
