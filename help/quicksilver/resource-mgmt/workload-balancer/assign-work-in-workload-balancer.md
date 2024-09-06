---
product-area: resource-management
navigation-topic: the-workload-balancer
title: 在工作負載平衡器中指派工作的總覽
description: 身為資源管理員，您可以使用Adobe Workfront工作負載平衡器來檢視尚未指派給使用者的工作專案，並將這些專案指派給使用者。
author: Lisa
feature: Resource Management
exl-id: 98779b67-b975-4501-8426-63e255b1d7df
source-git-commit: db0aab0e6e7e896a8e7c0afe2da709de7c3c2a4e
workflow-type: tm+mt
source-wordcount: '1033'
ht-degree: 1%

---

# 在工作負載平衡器中指派工作的總覽

身為資源管理員，您可以使用Adobe Workfront工作負載平衡器來檢視尚未指派給使用者的工作專案，並將這些專案指派給使用者。

如需工作負載平衡器的一般資訊，請參閱[工作負載平衡器總覽](../../resource-mgmt/workload-balancer/overview-workload-balancer.md)。

您可以將工作專案（任務和問題）指派給Workfront其他區域中的使用者。 但是，透過使用工作負載平衡器，您可以輕鬆瞭解使用者的可用性，並在指派他們更多工作之前清楚檢視他們指派給他們的所有其他專案。

如需在Workfront其他區域指派工作專案的相關資訊，請參閱下列文章：

* [指派任務](../../manage-work/tasks/assign-tasks/assign-tasks.md)
* [指派問題](../../manage-work/issues/manage-issues/assign-issues.md)

## 工作負載平衡器中的使用者可用性

您可以在工作負載平衡器中指派工作以符合使用者的可用時間。 為了確保您指派正確的工作量且不會過度配置使用者，指派給使用者的工作專案計畫時數總計必須符合使用者每日或每週配置。

您必須瞭解Workfront如何計算使用者的可用時間。

Workfront使用下列資訊在工作負載平衡器中計算使用者的容量：

* 資源管理喜好設定。 Workfront管理員在「設定」的「資源管理」區域中選取使用下列其中一項，以決定系統可用時間的計算方式：

   * Workfront系統的預設排程和使用者的FTE。
   * 使用者的排程，如使用者設定檔區域中所示。

     這會計算使用者的每日和每週可用性。 所選排程的任何排程例外都會反映在工作負載平衡器的使用者容量中。

  如需詳細資訊，請參閱[設定資源管理喜好設定](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md)。

  如需排程的相關資訊，請參閱[建立排程](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)

* 使用者的休假。 這表示使用者計畫起飛的日期。

  如需詳細資訊，請參閱[設定個人休假](../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/personal-time-overview.md)。

* 使用者的工作時間。 這表示使用者可用於執行實際專案相關工作（不包括管理費用）的FTE時間百分比。 將「工作時間」值設為1，表示使用者可用於專案相關工作的整個全職同等工作。


## 在工作負載平衡器中指派工作

您可以在工作負載平衡器中指派尚未指派給使用者的工作專案，或重新指派已指派給使用者的專案。

您可以透過以下方式在工作負載平衡器中指派工作：

* 手動指定每個專案，一次一個專案。

  您可以在手動指派專案時進行「進階指派」，一次一個。

  如需詳細資訊，請參閱[使用工作負載平衡器](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-manually.md)手動指派工作。

* 一次一個專案，方法是拖放工作專案給需要指派的使用者。

  如需詳細資訊，請參閱[透過拖放在工作負載平衡器中指派工作](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-by-drag-and-drop.md)。

* 使用「大量指派」選項，一次可指派多個專案。 您可以定義一次將專案指派給多個使用者的規則。

  如需詳細資訊，請參閱[使用工作負載平衡器](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-in-bulk.md)大量指派工作。

如需有關取消指派工作的資訊，請參閱[在工作負載平衡器](../../resource-mgmt/workload-balancer/unassign-work-in-workload-balancer.md)中取消指派工作。

## 工作負載平衡器中的指派區域

您可以使用資源區域、專案或團隊層級的工作負載平衡器將工作指派給使用者。 如需有關工作負載平衡器在Workfront中的位置的詳細資訊，請參閱[找到工作負載平衡器](../../resource-mgmt/workload-balancer/locate-workload-balancer.md)。

工作負載平衡器中有兩個區域可供您檢視工作專案：

* **未指派的工作**：顯示未指派給使用者的專案。
* **指派的工作**：顯示指派給使用者的專案。

下表說明哪些專案會根據其指定顯示在每個區域中：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>指派型別</strong> </td> 
   <td colspan="2"><strong>顯示指派的區域</strong> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td>未指派的工作 </td> 
   <td>已指派的工作 </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span style="font-weight: normal;">未指派的專案</span> </td> 
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
   <td>角色與團隊</td> 
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
   <td>使用者、角色和團隊</td> 
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

&#42;將工作專案指派給使用者和角色時，只有當角色是主要受指派人時，它才會顯示在「未指派的工作」區域中。

&#42;&#42;將工作專案指派給使用者和另一個實體時，只有當使用者是主要受指派人時，它才會顯示在「已指派的工作」區域中。

如需有關工作負載平衡器的未指派和已指派區域的詳細資訊，請參閱[瀏覽工作負載平衡器](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md)。

## 對工作角色、團隊和使用者的多個指派的考量事項

將多個資源指派給工作專案時，請考量下列事項：

* 使用者可以有多個與其設定檔相關聯的工作角色。 如需將使用者與工作角色建立關聯的資訊，請參閱[編輯使用者的設定檔](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)。

* 任務或問題通常會先指派給一或多個工作角色或團隊。 當專案準備開始時，也需要將其指派給使用者。\
  如果將任務或問題指派給一個或多個角色，然後您也指派了使用者，Adobe Workfront會根據以下規則決定要將哪個工作角色與其他使用者（如果有）相關聯：

   * 如果僅指派了一個工作角色，並且該工作角色與使用者的主要角色匹配，則任務或問題僅指派給履行其主要角色的使用者。
   * 如果有指派的多個角色，且至少有一個角色符合使用者的次要角色，則會將任務或問題指派給履行其中一個其他角色(如果有多個符合專案，則Workfront會隨機選取該角色)的使用者，以及任何已指派的其他角色。
   * 如果有指派的一或多個工作角色，但沒有匹配的使用者角色，則會將任務或問題指派給該角色或角色以及使用者。

* 如果將任務或問題指派給團隊且您也指派了使用者，則該任務或問題仍會同時指派給團隊和使用者。

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
