---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: 設定系統範圍的任務和問題偏好設定
description: 您可以設定任務和問題的全系統偏好設定。 這些偏好設定會影響使用者在Workfront中建立任務和問題的方式。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 8b99f939-12fe-4470-9dc8-f8a92c6db334
source-git-commit: 51b8e474cefe63b4db8c42e480990ca0ba431a4d
workflow-type: tm+mt
source-wordcount: '2075'
ht-degree: 0%

---

# 設定整個系統的任務和問題偏好設定

<!-- Audited: 2/2024 -->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.
Linked to Converting Issues.-->

作為[!DNL Adobe Workfront]管理員，您可以設定任務和問題的全系統偏好設定。 這些偏好設定會影響您的使用者在[!DNL Workfront]中建立任務和問題的方式。

依照預設，任務和問題偏好設定會鎖定，群組管理員無法在群組層級修改它們，除非您為整個系統的所有群組解除鎖定它們。 如需詳細資訊，請參閱本文章的[鎖定群組](#lock-task-and-issue-preferences-for-groups)的任務和問題偏好設定。


## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具有下列存取權才能執行本文中的步驟：

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
   <td><p>新增：[！UICONTROL Standard]</p>
   或
   <p>目前： [！UICONTROL計畫]</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>您必須是[!DNL Workfront]管理員。</p> </td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 為[!DNL Workfront]中的每個人設定任務和問題偏好設定

{{step-1-to-setup}}

1. 在左側面板中，按一下&#x200B;**[!UICONTROL 專案偏好設定]** >**[!UICONTROL 任務和問題]。**

1. 在出現的頁面上，繼續下列的5個區段之一，以設定[!UICONTROL 新任務預設值]、[!UICONTROL 問題]、[!UICONTROL 刪除]、[!UICONTROL 實際日期]和[!UICONTROL 存取]的設定：

   * [[!UICONTROL 新任務預設值]](#new-task-defaults)
   * [[!UICONTROL 問題]](#issues)
   * [[!UICONTROL 刪除]](#deletion)
   * [[!UICONTROL 實際日期]](#actual-dates)
   * [[!UICONTROL 委派]](#delegation)

   <!--
<li class="preview" data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#work-on-it" class="MCXref xref">處理它</a> </li>
  —&gt;

* [[!UICONTROL 存取]](#access)

### [!UICONTROL 新任務預設值] {#new-task-defaults}

<table style="table-layout:auto"> 
  <col> 
  <col> 
  <tbody> 
    <tr> 
    <td role="rowheader">[！UICONTROL開始日期]</td> 
    <td> <p>決定專案經理新任務的預設開始日期。 新任務的開始日期可以是專案的計劃開始日期，也可以是建立任務的日期。</p> </td> 
    </tr> 
    <tr> 
    <td role="rowheader"> <p>[！UICONTROL期間型別] </p> </td> 
    <td> <p>決定資源數（及其配置百分比）與工期或任務總付出之間的關係。 如需詳細資訊，請參閱<a href="../../../manage-work/tasks/taskdurtn/task-duration-duration-type.md" class="MCXref xref">任務期間與期間型別</a></p> </td> 
    </tr> 
    <tr> 
    <td role="rowheader">[！UICONTROL收入型別]</td> 
    <td> <p>計算任務的計畫和實際收入預估。 當<strong>[！UICONTROL收入型別]</strong>設為<strong>[！UICONTROL不可記帳]</strong>時，計畫時數和實際記錄時數不會產生任務的收入預估，且任務上的工作不會貢獻專案層級的收入。</p> </td> 
    </tr> 
    <tr> 
    <td role="rowheader">[！UICONTROL成本型別]</td> 
    <td> <p>計算任務的計畫和實際成本預估。 設定為<strong>[！UICONTROL無成本]</strong>時，計畫時數與實際記錄時數不會產生任務的計畫或實際成本預估，且任務上的工作不會貢獻專案層級的成本。</p> </td> 
    </tr> 
  </tbody> 
</table>

### 問題 {#issues}

<table style="table-layout:auto"> 
  <col> 
  <col> 
  <tbody> 
    <tr> 
    <td role="rowheader">[！UICONTROL當解析物件的狀態變更時，自動更新可解析問題狀態]</td> 
    <td> <p>當有人將問題轉換為專案或任務時，原始問題和轉換的專案或任務都會成為解決物件。 此設定可讓您將原始問題的解決方案與其可解析物件的解決方案相關聯。 如需解析物件的詳細資訊，請參閱<a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">解析和可解析物件概述</a>。</p> <p>為了讓此設定生效，必須選取<strong>[！UICONTROL保留原始問題並將其解決方案連結至任務]</strong>的選項。</p> 
      <ul> 
      <li>啟用此設定後，您可以針對問題和專案或任務使用相同的鍵值建立自訂狀態。 當專案或任務（作為可解析物件）變成自訂狀態時，變更也會反映在問題的狀態上。 問題和專案或任務狀態的狀態索引鍵必須相同。</li> 
      <li>停用此設定時，解析物件狀態會自動設定為預設狀態，而非自訂狀態。 如需預設狀態的詳細資訊，請參閱<a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref">存取系統問題狀態清單</a>。</li> 
      </ul> </td> 
    </tr> 
    <tr> 
    <td role="rowheader">[！UICONTROL將問題轉換為任務時]</td> 
    <td> <p>本節中的設定會決定從問題轉換為任務期間會發生什麼情況：</p> 
      <ul> 
      <li> <p><strong>[！UICONTROL保留原始問題並將其解決方案連結至任務]</strong>：當您轉換問題時，在任務完成之前，它仍會被視為問題。 任務完成後，問題的狀態會自動變更為[！UICONTROL已關閉]。 取消選取時，問題即被刪除。</p> <p><b>附註</b>：  <p>無論此設定的狀態為何，沒有存取許可權或刪除問題的使用者在轉換問題時都將無法刪除問題。 如需問題的存取和許可權資訊，請參閱：</p> 
        <ul> 
          <li> <p><a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">授與問題的存取權</a> </p> </li> 
          <li> <p><a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">共用問題</a> </p> </li> 
        </ul> </p> </li> 
      <li><strong>[！UICONTROL允許主要連絡人存取任務]</strong>：給予主要連絡人（問題建立者）檢視任務的存取權以檢閱任務、隨時瞭解其進度，以及在任務的[更新]區段上發表評論。</li> 
      <li> <p><strong>[！UICONTROL允許在轉換期間變更這些設定]</strong>：允許轉換問題的使用者在轉換問題至任務期間變更這些選項。</p></li> 
      </ul> </td> 
    </tr> 
    <tr> 
    <td role="rowheader">[！UICONTROL將問題轉換為專案時]</td> 
    <td> <p>本節中的設定會決定從問題轉換至專案的流程中會發生什麼情況：</p> 
      <ul> 
      <li> <p><strong>[！UICONTROL保留原始問題並將其解決方案連結至專案]</strong>：當您轉換問題時，在專案完成之前，它仍會被視為問題。 專案完成時，問題的狀態會自動變更為[！UICONTROL已關閉]。 取消選取時，問題即被刪除。 </p> <p><b>附註</b>：  <p>無論此設定的狀態為何，沒有存取許可權或刪除問題的使用者在轉換問題時都將無法刪除問題。 如需問題的存取和許可權資訊，請參閱：</p> 
        <ul> 
          <li> <p><a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">授與問題的存取權</a> </p> </li> 
          <li> <p><a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">共用問題</a> </p> </li> 
        </ul> </p> </li> 
      <li><strong>[！UICONTROL允許主要連絡人存取專案]</strong>：授予主要連絡人（問題建立者）檢視專案的存取權，以檢閱專案、隨時瞭解其進度，並在專案的更新區段上發表評論。</li> 
      <li><strong>[！UICONTROL允許在轉換期間變更這些設定]</strong>：允許轉換問題的使用者在問題轉換為專案期間變更列出的選項。</li> 
      </ul> </td>
    </tr> 
  </tbody> 
  </table>

### [!UICONTROL 刪除] {#deletion}

**[!UICONTROL 允許使用者刪除具有記錄時數的任務和問題]**：讓您決定是否允許刪除具有記錄時數的任務或問題。 依預設，會選取此選項。

>[!TIP]
>
>此設定也適用於刪除有任務或問題且已記錄時數的專案。 此設定不適用於直接為專案記錄時間的刪除專案。

* 選取後，當您刪除任務或問題時，會收到資訊性警告。 警告會提醒您，如果任務或問題已記錄時數，則會將其移至專案或刪除。 您可以在[!UICONTROL 設定]的[!UICONTROL 時程表和時數偏好設定]區域中設定是否要刪除時數或將其移至專案。 確認您已看到警告後，該任務或問題即被刪除。 如需有關設定時程表和時數偏好設定的詳細資訊，請參閱[設定時程表和時數偏好設定](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md)。

  >[!TIP]
  >
  >當您刪除具有已記錄時數的任務和問題的專案時，會刪除已記錄時數，或根據[!UICONTROL 設定]的[!UICONTROL 時程表和時數偏好設定]區域中的設定保留已記錄時數。 刪除專案時未顯示警告訊息。

* 取消選取此選項時，當您刪除具有記錄時數的任務或問題時，或是當您刪除具有記錄其任務或問題的時數的專案時，會收到禁止性警告。 警告指定管理員不允許刪除記錄時數的任務或問題。 無法刪除為任務和問題記錄時數的任務、問題或專案。

### [!UICONTROL 實際日期] {#actual-dates}

<table style="table-layout:auto"> 
  <col> 
  <col> 
  <tbody> 
    <tr> 
    <td role="rowheader">[！UICONTROL當任務或問題從「新增」移至「進行中」時，將實際開始日期設定為]</td> 
    <td> <p>當任務或問題從<strong>[！UICONTROL新增]</strong>移至<strong>[！UICONTROL進行中]</strong>時，為[!DNL Workfront]中記錄實際開始日期選取下列其中一個選項：</p> 
      <ul> 
      <li><strong>[！UICONTROL現在]：</strong>實際開始日期已設定為目前日期。</li> 
      <li><strong>[！UICONTROL計劃開始日期]：</strong>實際開始日期已設為任務或問題的計劃開始日期。</li> 
      </ul> </td> 
    </tr> 
    <tr> 
    <td role="rowheader">[！UICONTROL任務或問題完成時，將實際完成日期設定為]</td> 
    <td> <p>當任務或問題完成時，選擇實際完成日期記錄在[!DNL Workfront]中的以下選項之一：</p> 
      <ul> 
      <li><strong>[！UICONTROL現在]：</strong>實際完成日期已設定為目前日期。</li> 
      <li> <p><strong>[！UICONTROL計畫完成日期]：</strong>實際完成日期已設為任務或問題的計畫完成日期。</p> </li> 
      </ul> </td> 
    </tr> 
  </tbody> 
</table>

### 委派

啟用&#x200B;**[!UICONTROL 允許使用者委派其任務和問題]**&#x200B;設定可讓中的所有使用者暫時將其工作委派給其他人。

啟用此設定時，使用者可以看到下列內容：

* [!UICONTROL 代理人]連結位於其[!UICONTROL 首頁]區域。 他們可以從這裡委派核准，或任務和問題指派。
* 表示任務或問題已委派給任務或問題標題中[!UICONTROL 指派和委派]區域中的其他使用者。

  如果您停用[!UICONTROL 允許使用者委派其任務和問題]設定，目前排程的委派將停止，且委派的使用者將收到委派已停止的電子郵件通知。

如需將工作委派給其他人的相關資訊，請參閱下列文章：

* [委派工作概覽](../../../manage-work/delegate-work/delegate-work-overview.md)
* [管理任務和問題](../../../manage-work/delegate-work/how-to-delegate-work.md)

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
    <td role="rowheader">[！UICONTROL將某人指派給任務時]</td> 
    <td> 
      <ul> 
      <li><strong>[！UICONTROL授予他們……任務的存取權]</strong>：定義使用者對其所指派任務的預設許可權。 如需有關工作許可權的詳細資訊，請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">授予使用者存取權</a>。</li> 
      <li> <p><strong>[！UICONTROL也授與他們……專案的存取權]</strong>：定義使用者對其任務指派給他們的專案具有的預設許可權。 如需有關專案許可權的詳細資訊，請參閱<a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">設定全系統的專案偏好設定</a>。</p> </li> 
      </ul> </td> 
    </tr> 
    <tr> 
    <td role="rowheader">[！UICONTROL將某人指派給問題時]</td> 
    <td> 
      <ul> 
      <li><strong>[！UICONTROL授予他們……任務的存取權]</strong>：定義使用者對其所指派任務的預設許可權。 如需有關工作許可權的詳細資訊，請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">授予使用者存取權</a>。</li> 
      <li> <p><strong>[！UICONTROL也授與他們……專案的存取權]</strong>：定義使用者對其任務指派給他們的專案具有的預設許可權。 如需有關專案許可權的詳細資訊，請參閱<a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">設定全系統的專案偏好設定</a>。</p> </li> 
      </ul> </td> 
    </tr> 
    <tr> 
    <td role="rowheader">[！UICONTROL某人提交請求時]</td> 
    <td> 
      <ul> 
      <li><strong>[！UICONTROL授予他們……問題的存取權]</strong>：定義使用者對其所提交之要求的預設許可權。 如需詳細資訊，請參閱<a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">共用問題</a>。</li> 
      <li> <p><strong>[！UICONTROL來自相同公司的人員將會為所有要求繼承相同的許可權]</strong>：允許使用者檢視由他們來自相同公司的其他使用者提交的要求。 他們對於這些請求具有的許可權，與他們本身提交的請求相同。</p> </li> 
      </ul> </td> 
    </tr> 
  </tbody> 
</table>

1. 按一下「**[!UICONTROL 儲存]**」。

## 鎖定群組的任務和問題偏好設定 {#lock-task-and-issue-preferences-for-groups}

如果貴組織中的群組需要為其獨特工作流程設定不同的任務或問題偏好設定，您可以解鎖整個組織中所有群組的偏好設定，以便他們可自行設定。 當偏好設定已解除鎖定且群組管理員修改時，與群組相關聯的工作或問題會受偏好設定的群組層級設定（而非系統層級設定）影響。

有關群組管理員如何設定群組的任務和問題偏好設定的資訊，請參閱[設定群組的任務和問題偏好設定](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md)。

>[!NOTE]
>
>在[!DNL Workfront]管理員在系統層級解除鎖定偏好設定後，任何群組管理員都可以對其進行設定，然後將其鎖定，以確保其群組中的所有人和下面的子群組都使用相同的設定。 此功能與[!DNL Workfront]管理員必須設定並鎖定系統中每個人的偏好設定功能平行。 如需詳細資訊，請參閱[設定群組的專案偏好設定](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md)以及[鎖定或解除鎖定子群組的專案、任務或問題偏好設定](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-preference.md)。

若要鎖定或解除鎖定任務或問題偏好設定，讓群組可以設定它：

{{step-1-to-setup}}

1. 按一下&#x200B;**[!UICONTROL 專案偏好設定]** > **[!UICONTROL 任務和問題]**。

1. 執行下列任一項作業：

   * 如果您希望群組下方的群組管理員能夠設定其群組的偏好設定，請解除鎖定![](assets/unlock-toggle-button.png)。
   * 如果您希望您的群組及其下方的所有群組使用您設定的偏好設定，請確定已鎖定該群組（此為預設值）。

     >[!IMPORTANT]
     >
     >我們建議您與整個系統群組內的管理員和使用者溝通，以確保以您設定鎖定偏好設定的方式考慮所有需求。 當您鎖定時，系統中的所有群組都會繼承您的設定。 如果偏好設定已解除鎖定任何時間段，您的設定會取代群組管理員可能已進行的設定。

1. 按一下「**[!UICONTROL 儲存]**」。
