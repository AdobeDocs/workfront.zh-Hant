---
user-type: administrator
product-area: system-administration;user-management
keywords: 群組，偏好設定，任務，群組，問題，解鎖
navigation-topic: create-and-manage-groups
title: 設定群組的時程表和小時偏好設定
description: 在系統層級，Adobe Workfront管理員可以解鎖時程表和小時偏好設定區段一般偏好設定和預先填入時程表。 這可讓群組管理員為自己的群組獨立設定這些區段中的選項。
author: Becky
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 1ee9343e-9452-4e41-a9ff-a6c865d4813b
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '1336'
ht-degree: 1%

---

# 設定群組的時程表和小時偏好設定

Adobe Workfront管理員可以在系統層級解除鎖定時程表和小時偏好設定的以下區段，讓群組管理員可以獨立地為自己的群組設定這些區段：

* 一般喜好設定
* 使用者記錄時間的位置
* 預填時程表

如果您管理的群組之上有任何群組，其管理員也可以為您的群組執行此動作。 Workfront管理員也是如此（適用於任何群組）。

「時程表與時數偏好設定」頁面上的下列區段只能在系統層級設定，且無法為群組解除鎖定：

* 已刪除的專案、任務和問題

如需Workfront管理員如何解除鎖定時程表和小時偏好設定的相關資訊，請參閱[設定時程表和小時偏好設定](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md#lock)一文中的[解除鎖定群組的時程表和小時偏好設定](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md)小節。

>[!TIP]
>
>專案偏好設定、任務與問題偏好設定也可使用群組層級設定。 如需詳細資訊，請參閱[設定群組的專案偏好設定](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md)和[設定群組的任務和問題偏好設定](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md)。

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

## 群組時程表和小時偏好設定

請考量下列有關為群組設定未鎖定時程表或小時偏好設定的資訊：

* 如果您是群組管理員，並且為群組設定時程表或小時偏好設定，則會影響使用群組作為主群組的使用者。
* 通常，已解鎖的偏好設定會無限期地保持解鎖狀態。 如果Workfront管理員將其重新鎖定，系統設定將再次生效，並且群組管理員所做的偏好設定設定將遺失。
* 時程表會繼承為時程表擁有者的主群組設定的時程表和小時偏好設定。

  <!--
  Add example here?
  -->

* Workfront管理員在系統層級解除鎖定偏好設定，而您為群組設定該偏好設定後，您就可以鎖定該偏好設定，以確保在您下方的群組中的所有人都使用相同的設定。 此功能與Workfront管理員必須為系統中的每個人設定並鎖定偏好設定的功能平行。 如需詳細資訊，請參閱[鎖定或解除鎖定群組時程表和小時喜好設定](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-timesheet-hour-preference.md)。

## 設定群組的解鎖時程表或小時偏好設定

>[!TIP]
>
>如果您是Workfront管理員，可以前往「設定>時程表和時數>偏好設定」，然後在頁面頂端的方塊中搜尋群組名稱，略過步驟1至4。

{{step-1-to-setup}}

1. 在左側面板中，按一下&#x200B;**群組** ![群組](assets/groups-icon.png)。

1. 按一下要設定其時程表或小時偏好設定的群組名稱。
1. 在左側面板中，按一下&#x200B;**時程表和時數**。

1. 在顯示的頁面上，在&#x200B;**一般偏好設定**&#x200B;區段中，設定下列任一選項：

   >[!TIP]
   >
   >如果您將游標停留在偏好設定上，且顯示工具提示以告知您該偏好設定已鎖定，您可以要求Workfront管理員為組織中的所有群組解除鎖定該偏好設定。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">記錄未來日期的時間</td> 
      <td> <p>可讓使用者在整個系統記錄未來日期的時間，位置如下：</p> 
       <ul> 
       <li>他們有權記錄時間的任何專案、任務和問題，無論專案群組為何</li> 
       <li>他們的時程表作為一般時間</li>
       </ul> 
       <p>當使用者計畫離開辦公室並想要預先記錄該時間時，此功能會很有用。</p> 
       <p><b>注意</b>：您無法防止使用者在已關閉或已取消的任務或問題上記錄時間。 您只能防止使用者記錄完成或廢棄專案的時間。 建議您在任務和問題清單中使用篩選器，以排除已完成或取消的對使用者可見的任務和問題。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">從時程表新增費用</td> 
      <td> <p>讓使用者能在時程表中記錄時間和費用。</p> 
      <p>當為群組啟用此偏好設定，且群組設定為特定使用者的主群組時，費用圖示會顯示在這些使用者的時程表上的專案和任務旁。 使用者可以按一下此圖示來新增或編輯專案或任務的費用。</p>
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">手動指派工作角色到時數專案</td> 
      <td> <p>允許使用者手動選取在其使用者設定檔中指派或指派給物件的任何工作角色。</p> <p><b>重要</b>：  
        <ul> 
         <li>如果您在將工作角色指派給時數專案後停用此設定，使用者必須調整在專案、任務或問題的時數索引標籤上各種角色底下記錄的時數。</li> 
         <li>如果使用者未在其設定檔中指派工作角色，且在「進階指派」對話方塊中有指派為「任務所有者」的任務，則當使用者將時間記錄在任務時，將會顯示該工作角色。</li> 
        </ul> </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">限制只有所有者和管理員能編輯時間表</td> 
      <td> <p>限制時程表所有者的編輯，無論專案的群組和Workfront管理員為何。 停用此選項時，也可以由以下人員編輯時程表：</p> 
       <ul> 
        <li> <p>具有時程表管理存取許可權的使用者及其存取層級的時數</p> </li> 
        <li> <p>時程表核准者（如果時程表上啟用了「可編輯時數」）</p> </li> 
        <li> <p>時程表所有者的經理</p> </li> 
       </ul> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">限制所有者和管理員只能編輯小時</td> 
      <td>僅限輸入時數的使用者和Workfront管理員進行編輯。 此設定適用於專案或時數報表中的時數索引標籤。</td> 
     </tr> 
    </tbody> 
   </table>

1. 在&#x200B;**使用者可記錄時間**&#x200B;區段中，設定下列任一選項：

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader">直接在專案上記錄時間</td> 
      <td>允許使用者在專案上記錄時間（在更新索引標籤和時程表上）。 如果要限制使用者在專案層級錄製時間，請取消核取此選項。</td>
     </tr>
     <tr>
      <td role="rowheader">將時間記錄在完成的專案上</td>
      <td>允許使用者記錄已標示為完成的專案時間。 如果停用此選項，使用者將無法記錄他們在處於完成狀態的專案上完成的工作時間。</td>
     </tr>
     <tr>
      <td role="rowheader">將時間記錄在廢棄的專案上</td> 
      <td>當啟用此選項時，使用者可以在處於廢棄狀態的專案上記錄時數。</td>
     </tr>
    </tbody>
   </table>

   >[!NOTE]
   >
   >此偏好設定是根據使用者主群組偏好設定的設定套用。 如果在使用者的首頁群組偏好設定中啟用這些設定，則無論專案的群組偏好設定是否允許，他們都能直接在專案上記錄時間，包括已完成或廢棄的專案。

1. 在&#x200B;**預先填入時程表**&#x200B;區段中，設定下列任一選項：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">在時程表工作範圍&lt;number of weeks&gt;內的工作</td> 
      <td> <p>定義包含指派給使用者的任務和問題日期的時程表日期範圍之前和之後的周數。 預設值為1週，您可以將此範圍延長至4週。 也就是說，如果您為範圍選取4週，則時程表已預先填入日期在時程表日期範圍前4週至時程表日期範圍後4週之間的任何時間任務和問題。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">已完成的任務和問題</td> 
      <td>如果通常將多個資源指派給單一任務，建議您進行此設定。 這表示當一個資源針對任務記錄時間並標籤為完成時，指派給任務的其他資源仍然可以在其時程表中找到任務或問題以記錄其時數。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">計畫日期在時程表日期範圍內的任務和問題</td> 
      <td> <p>選取時，時程表包含其計劃開始日期或完成日期介於時程表日期範圍內的任務和問題。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> 計畫日期在時程表日期範圍內的任務</td> 
      <td> <p>選取時，時程表包含具有專案時間範圍內的預計開始日期或完成日期的任務，即使問題或任務的計畫日期不在時程表日期範圍內。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下「**儲存**」。
