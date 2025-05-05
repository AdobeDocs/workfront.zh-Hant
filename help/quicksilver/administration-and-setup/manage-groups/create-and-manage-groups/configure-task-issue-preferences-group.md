---
title: 設定群組的任務和問題偏好設定
user-type: administrator
product-area: system-administration;user-management;setup
keywords: 群組，偏好設定，任務，問題，解除鎖定
navigation-topic: create-and-manage-groups
description: 如果貴組織中的群組需要以獨立於系統層級設定方式設定任務或問題偏好設定，Adobe Workfront管理員可以解鎖偏好設定。 然後，作為群組管理員，您可以設定群組的偏好設定，這將會影響與群組相關的所有任務或問題。
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 6889b94a-1be6-4be9-8397-c38f890f9103
source-git-commit: d2ca099e78d5adb707a0a5a53ccb2e6dd06698f8
workflow-type: tm+mt
source-wordcount: '2189'
ht-degree: 2%

---

# 設定群組的任務和問題偏好設定

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

如果貴組織中的群組需要以獨立於系統層級設定方式設定任務或問題偏好設定，Adobe Workfront管理員可以解鎖偏好設定。 然後，作為群組管理員，您可以設定群組的偏好設定，這將會影響與群組相關的所有任務或問題。

如果您管理的群組之上有任何群組，其管理員也可以為您的群組執行此動作。 Workfront管理員也是如此（適用於任何群組）。

如需Workfront管理員如何解除鎖定偏好設定的相關資訊，請參閱[鎖定或解除鎖定系統中所有群組的專案偏好設定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/lock-or-unlock-project-preferences-for-groups-system.md)。

>[!TIP]
>
>專案偏好設定也可以使用群組層級設定。 如需詳細資訊，請參閱[設定群組的專案偏好設定](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md)。

>[!NOTE]
>
>* 通常，已解鎖的偏好設定會無限期地保持解鎖狀態。 如果Workfront管理員將其重新鎖定，系統設定將再次生效，並且群組管理員所做的偏好設定設定將遺失。
>* 為與專案關聯的群組設定的偏好設定優先於為建立專案之使用者的「首頁」群組設定的偏好設定。
>* 有些群組層級偏好設定會影響您為群組建立的專案範本。 如需詳細資訊，請參閱文章[建立及修改群組的專案範本](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md)中的「群組」區域[&#128279;](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md#view)，一節「檢視、使用及建立群組的範本」。
>
>* Workfront管理員在系統層級解除鎖定偏好設定後，您可以對其進行設定，然後將其鎖定，以確保您的群組及其子群組中的每個人都使用相同的設定。 此功能與Workfront管理員必須為系統中的每個人設定並鎖定偏好設定的功能平行。 如需詳細資訊，請參閱[鎖定或解除鎖定子群組的專案、任務或問題偏好設定](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-preference.md)。
>

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td><p>新增：標準</p>
       <p>或</p>
       <p>目前：計畫</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td>您必須是群組的群組管理員或系統管理員。</td>
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 設定頂層群組的解除鎖定任務和問題偏好設定

>[!TIP]
>
>如果您是Workfront管理員，可以略過步驟1至4，方法是前往「設定>專案偏好設定>任務和問題」，然後在頁面頂端的方塊中搜尋群組名稱。

{{step-1-to-setup}}

1. 在左側面板中，按一下&#x200B;**群組** ![群組圖示](assets/groups-icon.png)。

1. 按一下您要為其設定解除鎖定任務和問題偏好設定的群組名稱。
1. 在顯示的群組頁面上，在左側面板中按一下&#x200B;**任務和問題偏好設定**。
1. 在出現的頁面上，繼續這些步驟下列出的5個區段之一，以設定[新增任務預設值]、[問題]、[刪除]、[實際日期]和[存取]區域的設定，然後按一下[儲存]。**&#x200B;**

   如果您將滑鼠游標停留在鎖定圖示![鎖定圖示](assets/lock-toggle-button-dimmed.png)上以取得需要設定的偏好設定，且顯示工具提示以告知您已鎖定，您可以要求Workfront管理員為組織中的所有群組解除鎖定。

   解鎖後，您和其他群組管理員可以單獨為您自己的群組設定它。 此外，您也可以為群組及群組下方的任何子群組鎖定它。

   * [新任務預設值](#new-task-defaults)
   * [問題](#issues)
   * [刪除](#deletion)
   * [移動](#move)
   * [實際日期](#actual-dates)
   * [委派](#delegation)
   * [存取](#access)

### 新任務預設值 {#new-task-defaults}

<table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">新任務的開始日期</td> 
      <td> <p>決定專案經理新任務的預設開始日期。 新任務的開始日期可以是專案的計劃開始日期，也可以是建立任務的日期。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>期間類型 </p> </td> 
      <td> <p>決定資源數（及其配置百分比）與工期或任務總付出之間的關係。 如需詳細資訊，請參閱<a href="../../../manage-work/tasks/taskdurtn/task-duration-duration-type.md" class="MCXref xref">工作期間與期間型別：文章索引</a></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">收入類型</td> 
      <td> <p>計算任務的計畫和實際收入預估。 當<strong>收入型別</strong>設為<strong>不可記帳</strong>時，計畫時數與實際記錄時數不會產生任務的收入預估，且任務上的工作不會貢獻專案層級的收入。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">成本類型</td> 
      <td> <p>計算任務的計畫和實際成本預估。 設定為<strong>無成本</strong>時，計畫時數與實際記錄時數不會產生任務的計畫或實際成本預估，且任務上的工作不會貢獻專案層級的成本。</p> </td> 
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
      <td> <p>當有人將問題轉換為專案或任務時，原始問題和轉換的專案或任務都會成為解決物件。 此設定可讓您將原始問題的解決方案與其可解析物件的解決方案相關聯。 如需解析物件的詳細資訊，請參閱<a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">解析和可解析物件概述</a>。</p> <p>為了讓此設定生效，必須選取<strong>保留原始問題並將其解決方案連結至任務</strong>的選項。</p> 
       <ul> 
        <li>啟用此設定後，您可以針對問題和專案或任務使用相同的鍵值建立自訂狀態。 當專案或任務（作為可解析物件）變成自訂狀態時，變更也會反映在問題的狀態上。 問題和專案或任務狀態的狀態索引鍵必須相同。</li> 
        <li>停用此設定時，解析物件狀態會自動設定為預設狀態，而非自訂狀態。 如需預設狀態的詳細資訊，請參閱<a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref">存取系統問題狀態清單</a>。</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">將問題轉換為任務時</td> 
      <td> <p>本節中的設定會決定從問題轉換為任務期間會發生什麼情況：</p> 
       <ul> 
        <li><strong>保留原始問題並將其解決方案連結至任務</strong>：當您轉換問題時，在任務完成之前，它仍會被視為問題。 任務完成後，問題的狀態會自動變更為「已關閉」。</li> 
        <li><strong>允許主要連絡人存取任務</strong>：讓主要連絡人（問題建立者）存取任務，以檢閱任務、更新並隨時瞭解其進度</li> 
        <li> <p><strong>允許在轉換期間變更這些設定</strong>：允許轉換問題的使用者在轉換問題至任務期間變更這些選項。</p> <!--
          Screenshot when possible</p>
         --> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">將問題轉換為專案時</td> 
      <td> <p>本節中的設定會決定從問題轉換至專案的流程中會發生什麼情況：</p> 
       <ul> 
        <li><strong>保留原始問題，並將其解決方案連結至專案</strong>：當您轉換問題時，在專案完成之前，它仍會顯示為問題。 專案完成時，問題的狀態會自動變更為「已關閉」。</li> 
        <li><strong>允許主要連絡人存取專案</strong>：給予主要連絡人（問題建立者）存取專案的許可權，以檢閱專案、進行更新並隨時瞭解其進度。</li> 
        <li><strong>允許在轉換期間變更這些設定</strong>：允許轉換問題的使用者在轉換問題至專案期間變更列出的選項。</li> 
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
      <td> <p> 可讓您確定您是否允許刪除記錄時數的任務或問題。 依預設，會選取此選項。</p> 
       <div> 
        <p><b>秘訣</b>：此設定也適用於刪除有任務或問題且有記錄時數的專案。 此設定不適用於直接為專案記錄時間的刪除專案。 </p> 
        <p>請考量下列事項：</p> 
        <ul> 
         <li> <p>選取後，當您刪除任務或問題時，會收到資訊性警告。 警告會提醒您，如果任務或問題已記錄時數，則會將其移至專案或刪除。 您可以在「設定」的「時程表和時數」偏好設定區域中，設定是否要刪除時數或將其移至專案。 確認您已看到警告後，該任務或問題即被刪除。 如需有關設定時程表和時數偏好設定的詳細資訊，請參閱<a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md" class="MCXref xref">設定時程表和時數偏好設定</a>。 </p> <p>提示： <span>當您刪除包含已記錄時數的任務與問題的專案時，會刪除記錄時數，或根據設定</span>的「時程表與時數偏好設定」區域中的設定保留記錄時數。 </p> </li> 
         <li><span>當您取消選取此選項時，當您刪除具有記錄時數的任務或問題時，或是當您刪除具有記錄其任務或問題的時數的專案時，會收到禁止性警告</span> <span>。</span>警告指定管理員不允許刪除記錄時數的任務或問題。 無法刪除任務、問題<span>或為任務和問題</span>記錄時數的專案。 </li> 
        </ul> 
       </div> </td> 
     </tr> 
    </tbody> 
   </table>


### 移動

<table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">允許使用者移動具有時數記錄的任務和問題</td> 
      <td> <p> 可讓您確定您是否允許移動記錄時數的任務或問題。 依預設，會選取此選項。</p> 
       <p>請考量下列事項：</p> 
        <ul> 
         <li> 選取後，您可以移動已記錄時間的任務和問題。 小時也會隨著任務或問題移動。 </li>
      <li>取消選取此選項時，當您移動具有記錄時數的任務或問題時，會收到禁止性警告。 警告指定管理員不允許移動記錄時數的任務或問題。 無法將記錄時數的任務或問題移至其他專案。 即使取消選取此選項，您也可以在相同專案中移動具有記錄時數的任務。  </li></ul>
      </td> 
     </tr> 
    </tbody> 
   </table>

### 實際日期 {#actual-dates}

<table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">將任務或問題從「新增」移至「進行中」時，將實際開始日期設定為</td> 
      <td> <p>選取下列其中一個選項，當任務或問題從<strong>新增</strong>移至<strong>進行中</strong>時，實際開始日期記錄在Workfront中：</p> 
       <ul> 
        <li><strong>現在：</strong>實際開始日期設定為目前日期。</li> 
        <li><strong>計劃開始日期：</strong>實際開始日期已設為任務或問題的計劃開始日期。</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">任務或問題完成時，將實際完成日期設為</td> 
      <td> <p>選取下列其中一個選項，以用於任務或問題完成時，實際完成日期在Workfront中的記錄：</p> 
       <ul> 
        <li><strong>現在：</strong>實際完成日期設定為目前日期。</li> 
        <li> <p><strong>計畫完成日期：</strong>實際完成日期設定為任務或問題的計畫完成日期。</p> </li> 
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

### 委派

啟用&#x200B;**[!UICONTROL 允許使用者委派他們的任務和問題]**&#x200B;設定可讓群組中的所有使用者暫時將其工作委派給其他人。

啟用此設定時，群組使用者可以看到下列內容：

* 在[!UICONTROL 首頁]區域的[!UICONTROL 我的工作]、[!UICONTROL 我的任務]或[!UICONTROL 我的問題]介面工具中的&#x200B;[!UICONTROL **代理人**]&#x200B;連結。 他們可以從那裡委派任務和問題指派。

  >[!NOTE]
  >
  >  [!UICONTROL **委派核准**]&#x200B;連結一律在[!UICONTROL 首頁]區域中啟用。

* 表示任務或問題已委派給任務或問題標題中[!UICONTROL 指派和委派]區域中的其他使用者。
* 表示任務或問題已委派給其他使用者（位於[!UICONTROL 首頁]的[!UICONTROL 我的工作] Widget）。

  如果您停用[!UICONTROL 允許使用者委派其任務和問題]設定，目前排程的委派將停止，且委派的使用者將收到委派已停止的電子郵件通知。

如需將工作委派給其他人的相關資訊，請參閱下列文章：

* [委派工作概覽](../../../manage-work/delegate-work/delegate-work-overview.md)
* [委派任務和問題](../../../manage-work/delegate-work/how-to-delegate-work.md)

### 存取 {#access}

<table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">將某人指派給任務時</td> 
      <td> 
       <ul> 
        <li><strong>授予他們……任務的存取權</strong>：定義使用者對其所指派之任務的預設許可權。 如需有關工作許可權的詳細資訊，請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">授予使用者存取權</a>。</li> 
        <li> <p><strong>同時授與他們……專案的存取權</strong>：定義使用者對其任務指派給他們的專案具有的預設許可權。 如需有關專案許可權的詳細資訊，請參閱<a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">設定全系統的專案偏好設定</a>。</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">將某人指派給問題時</td> 
      <td> 
       <ul> 
        <li><strong>授予他們……任務的存取權</strong>：定義使用者對其所指派之任務的預設許可權。 如需有關工作許可權的詳細資訊，請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">授予使用者存取權</a>。</li> 
        <li> <p><strong>同時授與他們……專案的存取權</strong>：定義使用者對其任務指派給他們的專案具有的預設許可權。 如需有關專案許可權的詳細資訊，請參閱<a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">設定全系統的專案偏好設定</a>。</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">某人提交請求時</td> 
      <td> 
       <ul> 
        <li><strong>授予他們……問題的存取權</strong>：定義使用者對其所提交之要求的預設許可權。 如需詳細資訊，請參閱<a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">共用問題</a>。</li> 
        <li> <p><strong>來自相同公司的人員將會為所有要求繼承相同的許可權</strong>：允許使用者檢視來自相同公司的其他使用者所提交的要求。 他們對於這些請求具有的許可權，與他們本身提交的請求相同。</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>
