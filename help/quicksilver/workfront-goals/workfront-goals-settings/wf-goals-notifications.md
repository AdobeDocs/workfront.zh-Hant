---
content-type: reference
product-previous: workfront-goals
navigation-topic: workfront-goals-settings
title: 啟用Adobe Workfront目標通知
description: Adobe Workfront目標隨附一組預先定義的事件通知，您可以為您的帳戶啟用這些通知。 每次符合事件定義的條件時，這些事件通知都會觸發電子郵件通訊。
author: Alina
feature: Workfront Goals
exl-id: 40f9b9a3-c829-480b-9897-099b68389cd4
source-git-commit: 45c71a8106bdb8eeaa38f2fb83ff0312e48183d0
workflow-type: tm+mt
source-wordcount: '226'
ht-degree: 0%

---

# 啟用Adobe Workfront目標通知

>[!IMPORTANT]
>
>您的組織必須具備下列專案，才能使用本文所述的功能：
>
>* 對於新計畫和授權結構：
>
>   * Ultimate Workfront計畫
>    
>* 對於目前的計畫與授權結構：
>
>   * Pro或更高版本Workfront計畫
>   * 除了Adobe Workfront授權之外，還有Workfront目標授權。
>
>請連絡您的Workfront客戶經理，以瞭解Workfront Goals授權。
> 
>如需存取Workfront目標的詳細資訊，請參閱[使用Workfront目標的需求](/help/quicksilver/workfront-goals/goal-management/access-needed-for-wf-goals.md)。

Adobe Workfront目標隨附一組事件通知，您可以為您的帳戶啟用這些通知。 每次符合事件定義的條件時，這些事件通知都會觸發電子郵件通訊。

如需可為Workfront目標啟用哪些通知的詳細資訊，請參閱[通知：目標](../../workfront-basics/using-notifications/notifications-goals.md)。

如需有關在Adobe Workfront中管理通知的資訊，請參閱[修改您自己的電子郵件通知](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md)。

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Access requirements</h2>
<p>(NOTE: drafted, no longer available from WF Goals proper. Documented at the links above.) </p>
<p>You must have the following access to perform the actions described in this article:</p>
<table style="table-layout:auto">
<col>
<col>
<tbody>
<tr>
<td role="rowheader">Adobe Workfront plan*</td>
<td> <p>Pro or higher</p> </td>
</tr>
<tr>
<td role="rowheader">Adobe Workfront license*</td>
<td> <p>Request or higher</p> <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p> </td>
</tr>
<tr>
<td role="rowheader">Product</td>
<td> <p>You must purchase an additional license for the Adobe Workfront Goals to access functionality described in this article. </p> <p>For information, see <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requirements to use Workfront Goals</a>. </p> </td>
</tr>
<tr>
<td role="rowheader">Access level*</td>
<td> <p>View or higher access to&nbsp;Goals</p> <note type="note">
<p>If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see:</p>
<ul>
<li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a> </p> </li>
<li> <p><span href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md"><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md" class="MCXref xref">Grant access to Adobe Workfront Goals</a></span> </p> </li>
</ul>
</note> </td>
</tr>
<tr data-mc-conditions="">
<td role="rowheader">Object permissions</td>
<td>
<div>
<p>View or higher permissions on goals</p>
<p>For information about sharing goals, see <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Share a goal in Workfront Goals</a>. </p>
</div> </td>
</tr>
</tbody>
</table>
<p>*To find out what plan, license type, or access you have, contact your Workfront administrator.</p>
<h2>Prerequisites: </h2>
<p>You must have the following before you can start:</p>
<ul>
<li> <p>A Layout Template that includes the Goals area in the Main&nbsp;Menu.</p> </li>
</ul>
<h2>Understand Workfront Goals notifications settings</h2>
<p>Consider the following when configuring and receiving Workfront Goals notifications:</p>
<ul>
<li>They are personal notifications which means that each user can manage their own notifications.</li>
<li>The Workfront administrator does not need to enable event notifications before each user can select which ones they want to receive. </li>
<li>They trigger as soon as the defined events happen on goals, activities, or results and cannot be part of a daily digest. </li>
<li>They trigger regardless of the status of the goal. </li>
<li>They do not trigger when you are the initiator of the event described in the notification setting. </li>
</ul>
<h2>Configure email notifications for Workfront Goals</h2>
<ol>
<li value="1"> <p>Log in to Workfront and ensure that your Workfront administrator gave you access to&nbsp;Workfront Goals.</p> <p>For information about access to&nbsp;Workfront Goals, see <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requirements to use Workfront Goals</a>.</p> </li>
<li value="2"> <p> <p>Click the <strong>Main Menu icon</strong> <img src="assets/main-menu-icon.png"> in the upper-right corner of your screen, then click <strong>Goals</strong>.</p> <p>This opens the Workfront Goals area. </p> </p> </li>
<li value="3"> <p>Click <strong>Goal Settings</strong> in the left panel.</p> <p> <img src="assets/notifications-settings-list-highlighted-350x124.png" style="width: 350;height: 124;"> </p> </li>
<li value="4"> <p>Select any of the check boxes below to enable notifications for the following events:</p>
<table style="table-layout:auto">
<col>
<thead>
<tr>
<th>Notification </th>
</tr>
</thead>
<tbody>
<tr>
<td> <p>Someone created a new personal Goal for you.</p> <p>This is enabled by default.</p> <note type="tip">
A personal goal is a goal where you are designated as the owner.
</note> </td>
</tr>
<tr>
<td> <p>Someone assigned a Result/ an Activity to you.</p> <p>This is enabled by default. </p> </td>
</tr>
<tr>
<td>Someone left a comment on your Goal </td>
</tr>
<tr>
<td>Someone liked updates on your Goal</td>
</tr>
<tr>
<td>Someone liked a comment you left on a Goal</td>
</tr>
<tr>
<td>Someone liked your Aligned Goal</td>
</tr>
</tbody>
</table> </li>
<li value="5"> <p>Click <strong>Save Settings</strong>. </p> </li>
</ol>
</div>
-->

## Workfront目標電子郵件通知範例

當由您啟用的通知所定義的事件發生時，您會收到一封說明該事件的電子郵件。 以下範例是電子郵件通知，您被指派為新目標的「所有者」：

![目標通知電子郵件](assets/wf-align-notification-email-350x164.png)
