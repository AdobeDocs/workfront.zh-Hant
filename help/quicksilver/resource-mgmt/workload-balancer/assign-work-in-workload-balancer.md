---
product-area: resource-management
navigation-topic: the-workload-balancer
title: 工作負載平衡器中分配工作的概述
description: 作為資源管理器，您可以使用Adobe Workfront工作負載平衡器來查看尚未分配給用戶的工作項，並將這些項分配給它們。
author: Alina
feature: Resource Management
exl-id: 98779b67-b975-4501-8426-63e255b1d7df
source-git-commit: 8420f65e84edd42204d91aa503ff0b95153a1e67
workflow-type: tm+mt
source-wordcount: '1027'
ht-degree: 0%

---

# 工作負載平衡器中分配工作的概述

作為資源管理器，您可以使用Adobe Workfront工作負載平衡器來查看尚未分配給用戶的工作項，並將這些項分配給它們。

有關工作負載平衡器的一般資訊，請參見 [工作負載平衡器概述](../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

您可以將工作項目（工作和問題）指派給Workfront其他區域的使用者。 但是，通過使用工作負載平衡器，您可以輕鬆了解用戶的可用性，並清楚地查看他們分配給的所有其他項目，然後再為其分配更多工作。

如需在Workfront的其他區域指派工作項目的相關資訊，請參閱下列文章：

* [指派任務](../../manage-work/tasks/assign-tasks/assign-tasks.md)
* [指派問題](../../manage-work/issues/manage-issues/assign-issues.md)

## 工作負載平衡器中的用戶可用性

您可以在工作負載平衡器中分配工作以匹配用戶的可用時間。 為確保您分配正確的工作量，並且不要過度分配用戶，分配給用戶的工作項的計畫小時數總計必須與用戶的每日或每週分配相匹配。

您必須了解Workfront如何計算使用者的可用時間。

Workfront使用以下資訊在工作負載平衡器中計算用戶的容量：

* 資源管理首選項。 Workfront管理員通過在「設定」的「資源管理」區域中選擇使用以下選項之一，確定系統可用時間的計算方式：

   * Workfront系統的預設計畫和用戶的FTE。
   * 使用者的排程，如「使用者設定檔」區域所示。

      這會計算使用者的每日和每週可用性。 所選計畫上的任何計畫異常都反映在工作負載平衡器中用戶的容量中。
   如需詳細資訊，請參閱 [配置資源管理首選項](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

   如需排程的相關資訊，請參閱 [建立排程](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)

* 使用者的休息時間。 這表示使用者計畫離開的天數。

   如需詳細資訊，請參閱 [在Adobe Workfront中設定個人休假時間](../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/personal-time-overview.md).

* 使用者的工作時間。 這表示用戶可用於執行實際項目相關工作（不包括間接費用）的FTE時間百分比。 將「工作時間」值設定為1，表示用戶可用於與項目相關的整個全職工作。


## 在工作負載平衡器中分配工作

您可以分配尚未分配給用戶的工作項，或重新分配已分配給工作負載平衡器中用戶的工作項。

可以通過以下方式在工作負載平衡器中分配工作：

* 手動指派每個項目，一次一個項目。

   手動分配物料時，您可以執行「高級分配」，一次執行一次。

   如需詳細資訊，請參閱 [使用工作負載平衡器手動分配工作](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-manually.md).

* 將工作項目拖放給需要指派的使用者，一次只需一個項目。

   如需詳細資訊，請參閱 [通過拖放來分配工作負載平衡器中的工作](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-by-drag-and-drop.md).

* 使用「批量分配」選項，一次多個項目。 您可以定義規則，依此規則一次將項目指派給多個使用者。

   如需詳細資訊，請參閱 [使用工作負載平衡器批量分配工作](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-in-bulk.md).

有關取消分配工作的資訊，請參閱 [在工作負載平衡器中取消分配工作](../../resource-mgmt/workload-balancer/unassign-work-in-workload-balancer.md).

## 工作負載平衡器中的分配區域

您可以在資源區域、項目或團隊級別使用工作負載平衡器為用戶分配工作。 有關工作負載平衡器在Workfront中的位置的詳細資訊，請參見 [找到工作負載平衡器](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).

工作負載平衡器中有兩個區域，您可以在其中查看工作項：

* **未分配的工作**:顯示未指派給使用者的項目。
* **已分配的工作**:顯示指派給使用者的項目。

下表根據項目的分配說明了每個區域中顯示哪些項目：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>分配類型</strong> </td> 
   <td colspan="2"><strong>分配可見的區域</strong> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td>未指派的工作 </td> 
   <td>已指派的工作 </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span style="font-weight: normal;">未分配的項目</span> </td> 
   <td><span>✔</span> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>團隊</td> 
   <td>✔</td> 
   <td> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span data-mc-edit-date="2020-04-08T15:57:40.7175506-04:00" data-mc-editor="alinawilson" data-mc-comment="Drafted because role only is not displayed; first it will be displayed in Unassigned - 20.2 beta" data-mc-initials="AL" data-mc-creator="alinawilson" data-mc-create-date="2019-11-15T13:24:04.5189150-05:00">角色</span> </td> 
   <td><span>✔</span> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>角色和團隊</td> 
   <td>✔</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>使用者</td> 
   <td> </td> 
   <td>✔</td> 
  </tr> 
  <tr> 
   <td>使用者和團隊</td> 
   <td> <p> </p> </td> 
   <td>✔</td> 
  </tr> 
  <tr> 
   <td>用戶、角色和團隊</td> 
   <td>✔*</td> 
   <td>✔**</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>使用者和角色</p> </td> 
   <td><span data-mc-edit-date="2019-11-15T13:37:42.5435254-05:00" data-mc-editor="alinawilson" data-mc-comment="drafted because it's not in the Unassigned" data-mc-initials="AL" data-mc-creator="alinawilson" data-mc-create-date="2019-11-15T13:37:33.3097484-05:00">✔</span>*</td> 
   <td>✔**</td> 
  </tr> 
 </tbody> 
</table>

&#42;將工作項目分配給用戶和角色時，僅當角色是主要受託人時，它才會顯示在「未分配的工作」區域中。

&#42;&#42;當工作項被分配給用戶和另一個實體時，僅當用戶是主要受託人時，它才會顯示在「已分配的工作」區域中。

有關工作負載平衡器的「未分配」和「已分配」區域的詳細資訊，請參見 [導航工作負載平衡器](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## 指派給工作角色、團隊和使用者的多項考量事項

為工作項分配多個資源時，請考慮以下事項：

* 使用者可以有多個與其設定檔相關聯的工作角色。 有關將用戶與作業角色關聯的資訊，請參閱 [編輯使用者的設定檔](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* 通常會先將任務或問題指派給一個或多個作業角色或團隊。 當專案準備好開始時，也可能需要將其指派給使用者。\
   如果將任務或問題指派給一或多個角色，然後您又指派一個使用者，Adobe Workfront會根據下列規則決定要與其他使用者建立關聯的作業角色（如果有的話）:

   * 如果只分配了一個作業角色，並且該角色與用戶的主角色匹配，則該任務或問題僅分配給完成其主角色的用戶。
   * 如果分配了多個角色，且至少有一個角色與用戶的輔助角色匹配，則任務或問題將分配給履行其中一個「其他角色」(如果有多個匹配，則Workfront會隨機選擇)的用戶，以及已分配的任何其他角色。
   * 如果分配了一個或多個作業角色，並且沒有與用戶角色匹配的角色，則將任務或問題分配給該角色或角色以及該用戶。

* 如果將任務或問題分配給某個團隊，並且您也分配了某個用戶，則任務或問題將同時分配給該團隊和該用戶。

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2 data-mc-conditions="QuicksilverOrClassic.Quicksilver"> Manually assign one item at a time</h2>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Moved manual assignment and drag-and-drop to their own articles) </p>
<ol>
<li value="1">Go to the Workload Balancer.</li>
<li value="2"> <p>Go to the <strong>Unassigned Work</strong> area and apply a filter to view work items</p> <p>Or</p> <p>Go to the <strong>Assigned Work</strong> area and expand the name of a user to view the work items assigned to them.</p> <note type="important">
<span>You cannot view and assign issues from the Unassigned Work area. You can only reassign issues already assigned to users in the Assigned Work area. Otherwise,</span> you can assign issues from a list or at the issue level. For information, see
<a href="../../manage-work/issues/manage-issues/assign-issues.md" class="MCXref xref">Assign issues</a>.
</note> </li>
<li value="3"> <p>Click the <strong>More menu</strong> <img src="assets/qs-more-menu.png"> on the bar of a work item, then click <strong>Assign this to</strong>. </p> <p> <img src="assets/workload-balancer-assign-this-to-link-from-task-350x117.png" style="width: 350;height: 117;"> </p> <note type="tip">
<p><span>You can also use the following shortcuts to assign tasks or issues:</span> </p>
<ul>
<li><span>In Windows: CTRL+click the task or issue bar.</span> </li>
<li><span>In&nbsp;Mac: CMD+click the task or issue bar.</span> </li>
</ul>
</note> </li>
<li value="4"> <p>Start typing the name of a user, job role, or team that you want to assign to the item in the <strong>Search people, role or teams</strong> field, select it when it displays in the list, then click&nbsp;<strong>Save</strong>. </p> <p> <img src="assets/assignments-box-wb.png"> </p> <p>This assigns or reassigns the work item to the specified assignees.</p> <p>If you assign an item to just a team or a job role, the item displays only in the Unassigned Work area. You must assign work items to users in order to display them in the Assigned Work area of the Workload Balancer.</p> <note type="tip">
<p>You can assign multiple users or job roles, and you can assign only one team. <span>You can assign only active users, <span>job roles</span>, and teams.</span></p>
<p><span>If a user, <span>job role</span>, or a team was assigned before they were deactivated, they remain assigned to the work item. In this case, we recommend the following:</span> </p>
<ul>
<li> <p><span>Reassign the work item to active resources.</span> </p> </li>
<li> <p><span>Associate the users in a deactivated team with an active team and reassign the work item to the active team.</span> </p> </li>
</ul>
</note> </li>
<li value="5"> <p>(Optional) Click the <strong>Show allocations icon</strong> <img src="assets/show-allocations-icon-small.png">, then click the <strong>More menu</strong> <img src="assets/qs-more-menu.png"> > <strong>Edit allocations</strong>.</p> <p>Or</p> <p>Double-click a daily or weekly allocation to modify the amount of time the user is allocated to the work item.</p> <p>For information about modifying user allocations in the Workload Balancer, see the "Modify user allocations"&nbsp;section in the article <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">Manage user allocations in the Workload Balancer</a>.</p> </li>
</ol>
<div data-mc-conditions="QuicksilverOrClassic.Quicksilver">
<h2>Assign an item by dragging and dropping</h2>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: consider retitling this to "Assign one item at a time by dragging and dropping" when bulk assignments will come???)&nbsp;</p>
<p>You can assign an item from the Unassigned Work area to a user, or you can reassign an already assigned item to another user in the Assigned Work area.</p>
<ol>
<li value="1">Go to the Workload Balancer.</li>
<li value="2"> <p>Go to the <strong>Unassigned Work</strong> area and apply a filter to view work items.</p> <note type="important">
<span>You cannot view and assign issues from the Unassigned Work area.</span>
</note> </li>
<li value="3"> <p>Click the bar of a work item that indicates either the planned or the projected timeline and drag it over the name of a user in the <strong>Assigned</strong> area.</p> <p>The user you hover over to drop the work item to is highlighted.</p> <note type="tip">
The Planned Hours for the user you're hovering over update in real time with the number of daily Planned Hours from the work item, to indicate what the impact of adding a new item might be to their overall allocation.
</note> <p> <img src="assets/drag-drop-item-from-unassigned-to-assigned-wb-nwe-350x152.png" style="width: 350;height: 152;"> </p> </li>
<li value="4"> <p>When you are ready, drop the selected work item in the same line as the user's name in the Assigned Area. The item is assigned and the allocated Planned Hours are updated for the user with the new hours from the work item.</p> <note type="tip">
<p>If you enabled Group by Project in the Settings area, the assigned task displays under the corresponding project. If the setting is disabled, the assigned task displays in the user area. </p>
<p>The item displays according to the Workload Balancer criteria for sorting work items.&nbsp;For more information, see <a href="../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md" class="MCXref xref">Navigate the Workload Balancer</a>.</p>
</note> </li>
<li value="5"> <p>(Optional) Click the <strong>Show allocations icon</strong> <img src="assets/show-allocations-icon-small.png">, then click the <strong>More menu</strong> <img src="assets/qs-more-menu.png"> > <strong>Edit allocations</strong>. (NOTE: make sure these are still called this, and that the icon has not changed)</p> <p>Or</p> <p>Double-click a daily or weekly allocation to modify the amount of time the user is allocated to the work item.</p> <p>For information about modifying user allocations in the Workload Balancer, see the "Modify user allocations"&nbsp;section in the article <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">Manage user allocations in the Workload Balancer</a>.</p> </li>
</ol> 
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Assign items in bulk</h2>
<p>(NOTE: This is also a separate article. Should we keep this section or the separate article?) </p>
</div>
<p>&nbsp;</p>
</div>
</div>
-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Unassign work items in the Workload Balancer</h2>
<p>(NOTE: moved this section to a new article. Draft here at release to preview) </p>
<p>You can either unassign items from users and move them to the Unassigned Work area, or reassign them to other users. </p>
<p>To unassign work items from users: </p>
<ol>
<li value="1">In the Workload Balancer, go to the <strong>Assigned Work</strong> area and expand a user.</li>
<li value="2">Do 
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
one of
</MadCap:conditionalText>
the following:
<ul>
<li class="preview" data-mc-conditions="QuicksilverOrClassic.Draft mode"><p>Find the item you want to unassign in a user's area, click it, drag and drop it in the Unassigned area or in another user's area. </p></li>
<li><p>Click the <strong>More</strong> icon <img src="assets/more-icon-task-list.png"> to the right of the name of a work item, click&nbsp;<strong>Assign this to</strong> , then remove the name of the entities assigned to the work item or enter another name and click&nbsp;<strong>Save</strong>.</p><p><img src="assets/workload-balancer-assign-this-to-link-from-task-350x117.png" style="width: 350;height: 117;"></p></li>
</ul><p>The item displays in the Unassigned Work area if it matches the filtering criteria for that area and it is not assigned to any users or it displays in the user area if it is assigned to that user. </p><note type="tip">
Unassigned issues do not display in the Unassigned area.
</note><p>For information about filtering information in the Workload Balancer, see <a href="../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md" class="MCXref xref">Manage filters in the Workload Balancer</a>. </p></li>
</ol>
</div>
-->
