---
title: 配置組的任務和問題首選項
user-type: administrator
product-area: system-administration;user-management;setup
keywords: 組，首選項，任務，問題，解鎖
navigation-topic: create-and-manage-groups
description: 如果您組織中的群組需要設定任務或問題偏好設定，而與在系統層級設定任務或問題偏好設定的方式無關，Adobe Workfront管理員可解除鎖定偏好設定。 然後，作為組管理員，您可以配置組的首選項，該首選項將影響與組關聯的所有任務或問題。
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 6889b94a-1be6-4be9-8397-c38f890f9103
source-git-commit: 7fa4791e19a84d7215e341e8bbde8dd4d4d8ccc6
workflow-type: tm+mt
source-wordcount: '1894'
ht-degree: 3%

---

# 配置組的任務和問題首選項

如果您組織中的群組需要設定任務或問題偏好設定，而與在系統層級設定任務或問題偏好設定的方式無關，Adobe Workfront管理員可解除鎖定偏好設定。 然後，作為組管理員，您可以配置組的首選項，該首選項將影響與組關聯的所有任務或問題。

如果您管理的群組上方有任何群組，其管理員也可以對您的群組執行此動作。 Workfront管理員（適用於任何群組）也是如此。

如需Workfront管理員如何解除鎖定偏好設定的相關資訊，請參閱 [鎖定或解鎖系統中所有組的項目首選項](../../../administration-and-setup/set-up-workfront/configure-system-defaults/lock-or-unlock-project-preferences-for-groups-system.md).

>[!TIP]
>
>項目首選項也可以使用組級配置。 如需詳細資訊，請參閱 [配置組的項目首選項](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md).

>[!NOTE]
>
>* 通常，未鎖定首選項會無限期保持未鎖定狀態。 如果Workfront管理員重新鎖定，系統設定會再次生效，且群組管理員所做偏好設定的設定會遺失。
>* 為與項目關聯的組設定的首選項優先於為建立項目的用戶的「首頁組」設定的首選項。
>* 某些組級別首選項會影響您為組建立的項目模板。 如需詳細資訊，請參閱 [從「組」區域查看、使用和建立組的模板](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md#view) 在文章中 [建立和修改群組的專案範本](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md).
>
>* 在Workfront管理員解除系統級別偏好設定的鎖定後，您可以進行設定，然後將其鎖定，以確保群組及其子群組中的每個人都使用相同的設定。 這與Workfront管理員必須為系統中的每個人設定和鎖定偏好設定的功能平行。 如需詳細資訊，請參閱 [鎖定或解除鎖定子組的項目、任務或問題首選項](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-preference.md).
>


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

## 配置頂級組的解除鎖定任務和問題首選項

>[!TIP]
>
>如果您是Workfront管理員，可以前往「設定>專案偏好設定>工作與問題」 ，然後在頁面頂端的方塊中搜尋群組名稱，以略過步驟1至4。

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **設定** ![](assets/gear-icon-settings.png).

1. 在左側面板中，按一下 **群組** ![](assets/groups-icon.png).

1. 按一下要為其配置解鎖任務和問題首選項的組的名稱。
1. 在針對群組顯示的頁面上，按一下左側面板中的 **任務和問題首選項**.
1. 在顯示的頁面上，繼續以下步驟中列出的5個部分之一，以配置「新任務預設值」、「問題」、「刪除」、「實際日期」和「訪問」區域的設定，然後按一下 **儲存**.

   如果將滑鼠暫留在鎖定圖示上 ![](assets/lock-toggle-button-dimmed.png) 如需您需要設定的偏好設定，以及顯示工具提示來告知您已鎖定，您可以要求Workfront管理員為組織中的所有群組解除鎖定。

   解除鎖定後，您和其他群組管理員可以為您自己的群組個別設定它。 此外，您也可以將其鎖定在群組下方的子群組。

   * [新任務預設值](#new-task-defaults)
   * [問題](#issues)
   * [刪除](#deletion)
   * [實際日期](#actual-dates)

      <!--   
     <li><a href="#work-on-it" class="MCXref xref">Work On It</a> </li>   
     -->

   * [存取](#access)

### 新任務預設值 {#new-task-defaults}

<table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">新任務的開始日期</td> 
      <td> <p>確定項目管理員新任務的預設起始日期。 新任務的起始日期可以是項目的計畫起始日期或任務建立日期。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>期間類型 </p> </td> 
      <td> <p>確定資源數（及其分配百分比）與任務的持續時間或總工作量之間的關係。 如需詳細資訊，請參閱 <a href="../../../manage-work/tasks/taskdurtn/task-duration-duration-type.md" class="MCXref xref">任務持續時間和持續時間類型</a></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">收入類型</td> 
      <td> <p>計算任務的計畫和實際收入估計。 當 <strong>收入類型</strong> 設為<strong>不計費</strong>，計畫小時數和記錄的實際小時數不會生成任務的收入估計值，而任務上的工作不會對項目層收入作出貢獻。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">成本類型</td> 
      <td> <p>計算任務的計畫和實際成本估計。 設為時 <strong>無成本</strong>，計畫小時數和記錄的實際小時數不會生成任務的計畫成本或實際成本估計值，而任務上的工作不會對項目層成本產生貢獻。</p> </td> 
     </tr> 
    </tbody> 
   </table>

### 問題 {#issues}

<table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">當解決物件的狀態變更時，自動更新可解決問題狀態</td> 
      <td> <p>當某人將問題轉換為項目或任務時，原始問題和轉換的項目或任務都成為解決對象。 此設定可讓您將原始問題的解決方法與其可解析物件的解決方法建立關聯。 有關解析對象的詳細資訊，請參見 <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">解析和可解析對象概述 </a>.</p> <p>為了讓此設定有任何效果，請選取 <strong>保留原始問題，並將其解決方案與任務掛鈎</strong> 中指定的URL。</p> 
       <ul> 
        <li>啟用此設定時，您可以針對問題和專案或工作，以相同的鍵值建立自訂狀態。 當專案或任務（可解析的物件）變成自訂狀態時，變更也會反映問題的狀態。 對於問題和項目或任務狀態，狀態鍵必須相同。</li> 
        <li>禁用此設定時，解析對象狀態會自動設定為預設狀態，而不是自定義狀態。 如需預設狀態的詳細資訊，請參閱 <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref">訪問系統問題狀態清單</a>.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">將問題轉換為任務時</td> 
      <td> <p>本節中的設定會決定在從問題轉換至任務的過程中會發生什麼：</p> 
       <ul> 
        <li><strong>保留原始問題，並將其解決方案與任務掛鈎</strong>:轉換問題時，在任務完成之前，問題仍會顯示為問題。 任務完成時，問題狀態會自動變更為「已關閉」。</li> 
        <li><strong>允許主聯繫人訪問任務</strong>:為主要聯繫人（問題建立者）提供對任務的訪問權，以審核任務、進行更新並隨時了解其進度</li> 
        <li> <p><strong>允許在轉換期間變更這些設定</strong>:允許正在轉換問題的用戶在將問題轉換為任務期間更改這些選項。</p> <!--
          Screenshot when possible</p>
         --> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">將問題轉換為專案時</td> 
      <td> <p>本節中的設定會決定在從問題轉換至專案的過程中會發生什麼：</p> 
       <ul> 
        <li><strong>保留原始問題，並將其解決方案與項目掛鈎</strong>:轉換問題時，在專案完成前，問題仍會顯示為問題。 專案完成時，問題狀態會自動變更為「已關閉」。</li> 
        <li><strong>允許主要連絡人存取專案</strong>:提供主要連絡人（問題產生者）對專案的存取權，以檢閱專案、進行更新，並隨時了解其進度。</li> 
        <li><strong>允許在轉換期間變更這些設定</strong>:可讓正在轉換問題的使用者在將問題轉換為專案期間變更列出的選項。</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

### 刪除 {#deletion}

<table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">允許使用者刪除具有記錄時數的任務和問題</td> 
      <td> <p> 可讓您判斷是否允許刪除工作或記錄小時的問題。 預設會選取此選項。</p> 
       <div> 
        <p><b>筆尖</b>:此設定也適用於刪除有任務或記錄小時數問題的專案。 此設定不適用於直接為專案記錄時間的刪除專案。 </p> 
        <p>請考量下列事項：</p> 
        <ul> 
         <li> <p>選取此選項時，您會在刪除任務或問題時收到資訊性警告。 警告會提醒您，如果任務或問題已記錄小時數，則會將其移至專案或加以刪除。 您可以在「設定」的「工時單和工時首選項」區域中配置小時是否被刪除或移動到項目。 確認您看到警告後，會刪除該任務或問題。 有關配置時間表和小時首選項的詳細資訊，請參閱 <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md" class="MCXref xref">配置工時單和小時首選項</a>. </p> <p>提示： <span>如果刪除具有記錄小時的任務和問題的項目，則記錄的小時數將被刪除，或根據「設定」的「時間表和小時數首選項」區域中的設定保留</span>. </p> </li> 
         <li><span>取消選擇此選項時，您會在刪除任務或記錄小時問題時，或刪除記錄了任務或問題的小時的項目時，收到禁止性警告</span> <span>.</span> 警告指定管理員不允許刪除記錄小時的任務或問題。 任務、問題<span>，或記錄工作和問題數小時的專案</span> 無法刪除。 </li> 
        </ul> 
       </div> </td> 
     </tr> 
    </tbody> 
   </table>

### 實際日期 {#actual-dates}

<table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">當任務或問題從「新」變為「正在進行」時，將「實際開始日期」設定為</td> 
      <td> <p>選擇以下選項之一，以備任務或問題從 <strong>新增</strong> to <strong>進行中</strong>:</p> 
       <ul> 
        <li><strong>現在：</strong> 實際起始日期設定為當前日期。</li> 
        <li><strong>計劃開始日期：</strong> 實際起始日期設定為任務或問題的計畫起始日期。</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">任務或問題完成時，將實際完成日期設定為</td> 
      <td> <p>為任務或問題完成時在Workfront中記錄實際完成日期時選擇以下選項之一：</p> 
       <ul> 
        <li><strong>現在：</strong> 實際完成日期設定為當前日期。</li> 
        <li> <p><strong>計畫完成日期：</strong> 實際完成日期設定為任務或問題的計畫完成日期。</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

<!--
   This was a Ninja story in Summer/Fall 2020 that may never be implemented Leaving it here drafted in case Ninja decides to add it. Here's what Jeremy Flores says on 12/1/20:
   
   I have not had a chance to follow up with customers to verify if this is still a need. It has not come up organically. I can follow up with a few customers, but overall I would say that we're probably safe to move on and just mark what we've done to support this as complete. It could still come up but I don't want to push it unless customers really want it.
   You can replace the Work On It button with a Start button. When a user assigned to a task or issue clicks Start, the status and Actual Start Date of the work item update automatically, letting others know that the user started work.
   Workfront's default Work On It button also signals that a user started work on a task or issue, but it doesn't update the status and Actual Start Date.

   To switch to the Start button:
   
   Select Change the Work On It button to a Start button to automatically update the status of an item. 
   In the lists of check boxes that display below this option, select one or more statuses for each work item type. With multiple statuses selected here, when a user clicks Start on a work item, a drop-down menu lets the user choose a status for the item. 
     
   Making this change does not affect tasks and issues where the Actual Start Date was already updated. For these, the button displays as Work On It even if it is replaced with the Start button.
   If you select New as a status for a work item type (in step 2 above), the Actual Start Date does not update when a user clicks the Start button and then chooses New. This is because a Workfront item is not yet in progress (therefore not yet started) when New is its current status.
   This setting is not currently available in
   
   The Workfront Mobile App
   Workfront for Office 365
   Workfront email notifications
   
   This setting can be configured both at the system level and at the Team level. Enabling the Start button for everyone in the system automatically disables the same setting at the Team level.
   If the Work On It setting is enabled, then disabled, tasks and issues function with a Work On It button the way they did before.
   -->

### 存取 {#access}

<table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">將某人指派給任務時</td> 
      <td> 
       <ul> 
        <li><strong>授予他們……任務的存取權</strong>:定義用戶對其分配的任務具有的預設權限。 有關任務權限的詳細資訊，請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref"> 授予使用者存取權</a>.</li> 
        <li> <p><strong>同時授予他們……專案的存取權</strong>:定義用戶對其分配了任務的項目的預設權限。 如需專案權限的詳細資訊，請參閱 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">配置系統範圍的項目首選項</a>.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">將某人指派給問題時</td> 
      <td> 
       <ul> 
        <li><strong>授予他們……任務的存取權</strong>:定義用戶對其分配的任務具有的預設權限。 有關任務權限的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">授予使用者存取權</a>.</li> 
        <li> <p><strong>同時授予他們……專案的存取權</strong>:定義用戶對其分配了任務的項目的預設權限。 如需專案權限的詳細資訊，請參閱 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">配置系統範圍的項目首選項</a>.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">當某人提交請求</td> 
      <td> 
       <ul> 
        <li><strong>授予他們……問題的存取權</strong>:定義使用者在提交的請求上的預設權限。 如需詳細資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">共用問題</a>.</li> 
        <li> <p><strong>來自同一公司的人員將繼承所有請求的相同權限</strong>:可讓使用者查看來自與其相同公司的其他使用者提交的請求。 他們對這些請求擁有與對自己提交的請求相同的權限。</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>
