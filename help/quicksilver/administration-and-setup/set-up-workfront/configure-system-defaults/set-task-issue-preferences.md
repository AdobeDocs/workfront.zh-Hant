---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: 配置全系統任務和問題首選項
description: 您可以為任務和問題配置全系統首選項。 這些偏好設定會影響使用者在Workfront中建立工作和問題的方式。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 8b99f939-12fe-4470-9dc8-f8a92c6db334
source-git-commit: 2fd772ffc667c4f32c6a7b0de9c87676ee6dd65b
workflow-type: tm+mt
source-wordcount: '2089'
ht-degree: 1%

---

# 配置全系統任務和問題首選項

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.
Linked to Converting Issues.-->

作為 [!DNL Adobe Workfront] 管理員，您可以配置任務和問題的全系統首選項。 這些偏好設定會影響使用者在 [!DNL Workfront].

預設情況下，任務和問題首選項被鎖定，除非您為整個系統中的所有組解鎖，否則組管理員無法在組級別修改它們。 如需詳細資訊，請參閱 [鎖定組的任務和問題首選項](#lock-task-and-issue-preferences-for-groups) 這篇文章。

<!--SPLIT OUT BOTTOM SECTION TO NEW ARTICLE?-->

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計劃</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權</td> 
   <td>[!UICONTROL計畫]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置</td> 
   <td> <p>您必須是 [!DNL Workfront] 管理員。</p> <p><b>注意</b>:如果您仍無法存取，請詢問您的 [!DNL Workfront] 管理員。 若要了解 [!DNL Workfront] 管理員可修改您的存取層級，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 為 [!DNL Workfront]

1. 按一下 **[!UICONTROL 主菜單]** 圖示 ![](assets/main-menu-icon.png) 在 [!DNL Adobe Workfront]，然後按一下 **[!UICONTROL 設定]** ![](assets/gear-icon-settings.png).

1. 在左側面板中，按一下 **[!UICONTROL 專案偏好設定]** >**[!UICONTROL 工作與問題].**

1. 在顯示的頁面上，繼續下列5個區段的其中一個，以配置 [!UICONTROL 新任務預設值], [!UICONTROL 問題], [!UICONTROL 刪除], [!UICONTROL 實際日期]，和 [!UICONTROL 存取].
1. 按一下&#x200B;**[!UICONTROL 儲存]**。

* [[!UICONTROL 新任務預設值]](#new-task-defaults)
* [[!UICONTROL 問題]](#issues)
* [[!UICONTROL 刪除]](#deletion)
* [[!UICONTROL 實際日期]](#actual-dates)
* [[!UICONTROL 委派]](#delegation)

   <!--
  <li class="preview" data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#work-on-it" class="MCXref xref">Work On It</a> </li>
  -->

* [[!UICONTROL 存取]](#access)

### [!UICONTROL 新任務預設值] {#new-task-defaults}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！新任務的開始日期]</td> 
   <td> <p>確定項目管理員新任務的預設起始日期。 新任務的起始日期可以是項目的計畫起始日期或任務建立日期。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL持續時間類型] </p> </td> 
   <td> <p>確定資源數（及其分配百分比）與任務的持續時間或總工作量之間的關係。 如需詳細資訊，請參閱 <a href="../../../manage-work/tasks/taskdurtn/task-duration-duration-type.md" class="MCXref xref">任務持續時間和持續時間類型</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL收入類型]</td> 
   <td> <p>計算任務的計畫和實際收入估計。 當 <strong>[!UICONTROL收入類型]</strong> 設為<strong>[!UICONTROL不計費]</strong>，計畫小時數和記錄的實際小時數不會生成任務的收入估計值，而任務上的工作不會對項目層收入作出貢獻。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL成本類型]</td> 
   <td> <p>計算任務的計畫和實際成本估計。 設為時 <strong>[!UICONTROL無成本]</strong>，計畫小時數和記錄的實際小時數不會生成任務的計畫成本或實際成本估計值，而任務上的工作不會對項目層成本產生貢獻。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 問題 {#issues}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL在解析對象的狀態更改時自動更新可解決的問題狀態]</td> 
   <td> <p>當某人將問題轉換為項目或任務時，原始問題和轉換的項目或任務都成為解決對象。 此設定可讓您將原始問題的解決方法與其可解析物件的解決方法建立關聯。 有關解析對象的詳細資訊，請參見 <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">解析和可解析對象概述 </a>.</p> <p>為了讓此設定有任何效果，請選取 <strong>[!UICONTROL保留原始問題並將其解決與任務關聯]</strong> 中指定的URL。</p> 
    <ul> 
     <li>啟用此設定時，您可以針對問題和專案或工作，以相同的鍵值建立自訂狀態。 當專案或任務（可解析的物件）變成自訂狀態時，變更也會反映問題的狀態。 對於問題和項目或任務狀態，狀態鍵必須相同。</li> 
     <li>禁用此設定時，解析對象狀態會自動設定為預設狀態，而不是自定義狀態。 如需預設狀態的詳細資訊，請參閱 <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref">訪問系統問題狀態清單</a>.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader" [!UICONTROL>將問題轉換為任務時]</td> 
   <td> <p>本節中的設定會決定在從問題轉換至任務的過程中會發生什麼：</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL保留原始問題並將其解決與任務關聯]</strong>:轉換問題時，在任務完成之前，問題仍會顯示為問題。 任務完成時，問題的狀態會自動更改為[!UICONTROL已關閉]。 取消選取此選項時，會刪除問題。</p> <p><b>附註</b>:  <p>無權存取或刪除問題的使用者在轉換問題時，無法刪除問題，無論此設定的狀態為何。 如需關於問題的存取權和權限的資訊，請參閱：</p> 
       <ul> 
        <li> <p><a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">授予問題的存取權</a> </p> </li> 
        <li> <p><a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">共用問題 </a> </p> </li> 
       </ul> </p> </li> 
     <li><strong>[!UICONTROL允許主要聯繫人訪問任務]</strong>:為主要聯繫人（問題建立者）提供對任務的訪問權，以審核任務、進行更新並隨時了解其進度</li> 
     <li> <p><strong>[!UICONTROL允許在轉換期間更改這些設定]</strong>:允許正在轉換問題的用戶在將問題轉換為任務期間更改這些選項。</p> <!--
       Screenshot when possible</p>
      --> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL將問題轉換為專案時]</td> 
   <td> <p>本節中的設定會決定在從問題轉換至專案的過程中會發生什麼：</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL保留原始問題，並將其解決方式與專案掛鈎]</strong>:轉換問題時，在專案完成前，問題仍會顯示為問題。 專案完成時，問題狀態會自動變更為[!UICONTROL已關閉]。 取消選取此選項時，會刪除問題。 </p> <p><b>附註</b>:  <p>無權存取或刪除問題的使用者在轉換問題時，無法刪除問題，無論此設定的狀態為何。 如需關於問題的存取權和權限的資訊，請參閱：</p> 
       <ul> 
        <li> <p><a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">授予問題的存取權</a> </p> </li> 
        <li> <p><a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">共用問題 </a> </p> </li> 
       </ul> </p> </li> 
     <li><strong>[!UICONTROL允許主要聯繫人訪問項目]</strong>:提供主要連絡人（問題產生者）對專案的存取權，以檢閱專案、進行更新，並隨時了解其進度。</li> 
     <li><strong>[!UICONTROL允許在轉換期間更改這些設定]</strong>:可讓正在轉換問題的使用者在將問題轉換為專案期間變更列出的選項。</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 刪除] {#deletion}

**[!UICONTROL 允許使用者刪除記錄小時的工作和問題]**:可讓您判斷是否允許刪除工作或記錄小時的問題。 預設會選取此選項。

>[!TIP]
>
>此設定也適用於刪除有任務或記錄小時數問題的專案。 此設定不適用於直接為專案記錄時間的刪除專案。

* 選取此選項時，您會在刪除任務或問題時收到資訊性警告。 警告會提醒您，如果任務或問題已記錄小時數，則會將其移至專案或加以刪除。 您可以設定小時是刪除，還是移至 [!UICONTROL 工時單和工時首選項] 區域 [!UICONTROL 設定]. 確認您看到警告後，會刪除該任務或問題。 有關配置時間表和小時首選項的詳細資訊，請參閱 [配置工時單和小時首選項](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

   >[!TIP]
   >
   >當您刪除包含已記錄小時的工作和問題的專案時，系統會刪除已記錄的小時，或根據 [!UICONTROL 工時單和工時首選項] 區域 [!UICONTROL 設定]. 刪除專案時不會顯示警告訊息。

* 取消選擇此選項時，您會在刪除任務或記錄小時問題時，或刪除記錄了任務或問題的小時的項目時，收到禁止性警告。 警告指定管理員不允許刪除記錄小時的任務或問題。 無法刪除記錄了任務和問題的工時的任務、問題或項目。

### [!UICONTROL 實際日期] {#actual-dates}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL當任務或問題從「新」到「正在進行」時，將「實際開始日期」設定為]</td> 
   <td> <p>選擇以下選項之一，以備實際開始日期記錄於 [!DNL Workfront] 任務或問題從 <strong>[!UICONTROL新]</strong> to <strong>[!UICONTROL正在進行中]</strong>:</p> 
    <ul> 
     <li><strong>[!UICONTROL Now]:</strong> 實際起始日期設定為當前日期。</li> 
     <li><strong>[!UICONTROL計畫的開始日期]:</strong> 實際起始日期設定為任務或問題的計畫起始日期。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL當任務或問題完成時，將實際完成日期設定為]</td> 
   <td> <p>選擇以下選項之一，以備實際完成日期記錄在 [!DNL Workfront] 完成任務或問題時：</p> 
    <ul> 
     <li><strong>[!UICONTROL Now]:</strong> 實際完成日期設定為當前日期。</li> 
     <li> <p><strong>[!UICONTROL計畫完成日期]:</strong> 實際完成日期設定為任務或問題的計畫完成日期。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 委派

啟用 [!UICONTROL 允許使用者委派其工作和問題] 設定可讓中的所有使用者暫時將其工作委派給其他人。

啟用此設定時，使用者會看到下列內容：

* 此 [!UICONTROL 委派] 連結 [!UICONTROL 首頁] 的上界。 他們可以從這裡委派核准或任務並發放指派。
* 將任務或問題委派給 [!UICONTROL 任務和委託] 區域。

如果您停用 [!UICONTROL 允許使用者委派其工作和問題] 設定時，目前排程的委派將停止，而委派的使用者將會收到電子郵件通知，告知委派已停止。

有關將工作委派給他人的資訊，請參閱以下文章：

* [委派工作概述](../../../manage-work/delegate-work/delegate-work-overview.md)
* [管理任務和問題委派](../../../manage-work/delegate-work/how-to-delegate-work.md)

<!--
<p><strong>Work On It</strong></p>
This was a Ninja story in Summer/Fall 2020 that may never be implemented Leaving it here drafted in case Ninja decides to add it.</p>
Here's what Jeremy Flores says on 12/1/20:</p>
I have not had a chance to follow up with customers to verify if this is still a need. It has not come up organically. I can follow up with a few customers, but overall I would say that we're probably safe to move on and just mark what we've done to support this as complete. It could still come up but I don't want to push it unless customers really want it.</p>
<p>You can replace the Work On It button with a Start button. When a user assigned to a task or issue clicks Start, the status and Actual Start Date of the work item update automatically, letting others know that the user started work.</p>
<p>Workfront's default Work On It button also signals that a user started work on a task or issue, but it doesn't update the status and Actual Start Date.</p>
<p>To switch to the Start button:</p>
<ol>
<li value="1"> <p>Select <strong>Change the Work On It button to a Start button to automatically update the status of an item</strong>.</p> </li>
<li value="2"> <p>In the lists of check boxes that display below this option, select one or more statuses for each work item type.</p> <p>With multiple statuses selected here, when a user clicks Start on a work item, a drop-down menu lets the user choose a status for the item.</p> </li>
</ol> <note type="note">
<ul class="preview">
<li>Making this change does not affect tasks and issues where the Actual Start Date was already updated. For these, the button displays as Work On It even if it is replaced with the Start button.</li>
<li>If you select New as a status for a work item type (in step 2 above), the Actual Start Date does not update when a user clicks the Start button and then chooses New. This is because a Workfront item is not yet in progress (therefore not yet started) when New is its current status.</li>
<li>This setting is not currently available in
<ul>
<li>The Workfront Mobile App</li>
<li>Workfront for Office 365</li>
<li>Workfront email notifications</li>
</ul></li>
<li>This setting can be configured both at the system level and at the Team level. Enabling the Start button for everyone in the system automatically disables the same setting at the Team level.</li>
<li>If the Work On It setting is enabled, then disabled, tasks and issues function with a Work On It button the way they did before.</li>
</ul>
</note>
-->

### [!UICONTROL 存取] {#access}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL當有人被分配給任務時]</td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL授予他們……對任務的訪問權]</strong>:定義用戶對其分配的任務具有的預設權限。 有關任務權限的詳細資訊，請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">授予使用者存取權</a>.</li> 
     <li> <p><strong>[!UICONTROL也授予他們……對專案的存取權]</strong>:定義用戶對其分配了任務的項目的預設權限。 如需專案權限的詳細資訊，請參閱 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">配置系統範圍的項目首選項</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL當有人被指派到問題時]</td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL授予他們……對任務的訪問權]</strong>:定義用戶對其分配的任務具有的預設權限。 有關任務權限的詳細資訊，請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">授予使用者存取權</a>.</li> 
     <li> <p><strong>[!UICONTROL也授予他們……對專案的存取權]</strong>:定義用戶對其分配了任務的項目的預設權限。 如需專案權限的詳細資訊，請參閱 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">配置系統範圍的項目首選項</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL當有人提交請求時]</td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL授予他們……對問題的存取權]</strong>:定義使用者在提交的請求上的預設權限。 如需詳細資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">共用問題 </a>.</li> 
     <li> <p><strong>[!UICONTROL來自同一公司的人員將繼承所有請求的相同權限]</strong>:可讓使用者查看來自與其相同公司的其他使用者提交的請求。 他們對這些請求擁有與對自己提交的請求相同的權限。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## 鎖定組的任務和問題首選項 {#lock-task-and-issue-preferences-for-groups}

如果組織中的組需要針對其唯一工作流配置的任務或問題首選項不同，您可以解鎖組織中所有組的首選項，以便他們可以自行配置。 當首選項被解除鎖定，並且組管理員修改它時，與組關聯的任務或問題會受到首選項的組級別設定（而不是系統級別設定）的影響。

有關組管理員如何配置任務和發佈組首選項的資訊，請參閱 [配置組的任務和問題首選項](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

>[!NOTE]
>
>之後 [!DNL Workfront] 管理員在系統級別解除對首選項的鎖定，任何組管理員都可以對其進行配置，然後將其鎖定，以確保組中的每個人以及下面的子組都使用相同的配置。 這與 [!DNL Workfront] 管理員必須配置並鎖定系統中每個人的首選項。 如需詳細資訊，請參閱 [配置組的項目首選項](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md) 和 [鎖定或解除鎖定子組的項目、任務或問題首選項](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-preference.md).

要鎖定或解除鎖定任務或問題首選項，以便組可以配置它

1. 按一下 **[!UICONTROL 主菜單]** 圖示 ![](assets/main-menu-icon.png) 在 [!DNL Adobe Workfront]，然後按一下 **[!UICONTROL 設定]** ![](assets/gear-icon-settings.png).

1. 按一下 **[!UICONTROL 專案偏好設定]** > **[!UICONTROL 工作與問題]**.

1. 執行下列任一操作：

   * 如果您希望群組下的群組管理員能夠設定其群組的偏好設定，請解除鎖定 ![](assets/unlock-toggle-button.png).
   * 如果您希望群組及其下方的所有群組針對偏好設定使用您的設定，請確定已鎖定（此為預設值）。

      >[!IMPORTANT]
      >
      >建議您與整個系統中群組的管理員和使用者通訊，以確保以您設定鎖定偏好設定的方式滿足所有需求。 當您鎖定它時，系統中的所有群組都會繼承您的設定。 如果首選項已在任意時間段內解除鎖定，則您的配置將替換組管理員可能所做的配置。

1. 按一下&#x200B;**[!UICONTROL 儲存]**。
