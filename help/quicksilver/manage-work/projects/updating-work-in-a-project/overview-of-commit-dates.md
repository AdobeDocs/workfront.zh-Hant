---
content-type: overview
product-area: projects
navigation-topic: update-work-in-a-project
title: 認可日期總覽
description: 認可日期是指使用者指派給任務或問題認可完成任務或問題的日期。 這與計畫完成日期不同，因為這是由直接負責工作的使用者提供的完成日期更實際的估計值。
author: Alina
feature: Work Management
exl-id: 47072433-bb8e-4210-947a-8bfa41ec47a9
source-git-commit: 0792651822fd85cb3bfbb754aaf949c4fc4038a1
workflow-type: tm+mt
source-wordcount: '869'
ht-degree: 0%

---

# 認可日期總覽

<!--Audited: 05/2025-->

<!-- <span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers, or in the Production environment for customers who enabled fast releases.</span>

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview">For information about the current release, see [Third Quarter 2024 release overview](/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-release-overview.md).</span>-->

認可日期是指使用者指派給任務或問題認可完成任務或問題的日期。 這與任務或問題的規劃完成日期不同，因為這是僅由負責工作的使用者提供的完成日期更實際的估計值。

如需計畫完成日期的詳細資訊，請參閱[任務計畫完成日期的總覽](../../../manage-work/tasks/task-information/task-planned-completion-date.md)。

## 認可日期總覽

處理認可日期時，請考量下列事項：

* 只有任務和問題具有認可日期。
* Adobe Workfront不會自動設定認可日期。 當您建立任務或問題時，沒有為其指派認可日期。
* 如果您被指派到任務或問題，則可以執行下列操作之一來設定「認可日期」：

   * 透過按一下任務或問題上的「處理任務」、「開始問題」或「開始任務」，讓Workfront設定認可日期以符合任務或問題的現有規劃完成日期。 如需詳細資訊，請參閱[以開始按鈕取代處理它按鈕](../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md)。
   * 根據您認為任務或問題將完成的時間，手動設定認可日期。 這是您作為受託人，對「專案經理」的估計與承諾，表示您將在特定日期前完成任務或問題。 如需詳細資訊，請參閱[更新任務和問題的認可日期](/help/quicksilver/manage-work/projects/updating-work-in-a-project/update-commit-date-on-tasks-and-issues.md)。

>[!NOTE]
>
>您必須是任務的任務擁有者才能變更認可日期。 下列使用者無法變更任務的認可日期：
>
>* 專案所有者
>* 專案贊助者
>* 資源管理員
>* 系統管理員
>* 任務上的任何其他受指派人
>* 擁有任務許可權的任何其他使用者
>
>如需有關工作擁有者的詳細資訊，請參閱[編輯工作](../../../manage-work/tasks/manage-tasks/edit-tasks.md)。

## 找出任務和問題的認可日期

您可以在Workfront的下列區域中找到任務和問題的認可日期：

* 詳細資訊頁面
* Workfront或群組管理員新增至您的版面配置範本後的「摘要」面板。 如需詳細資訊，請參閱[使用配置範本自訂摘要面板](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md)。
* Workfront或群組管理員將任務或問題的標題新增到您的版面配置範本後。 如需詳細資訊，請參閱[使用配置範本自訂物件標頭](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md)。

## 變更認可日期所觸發的通知和更新 {#notifications-and-updates-triggered-by-changing-the-commit-date}

當任務或問題受指派人手動將「認可日期」變更為與「專案所有者」設定的「計畫完成日期」不同的日期時，會有許多通知和更新會提醒專案所有者和其他使用者此變更。

>[!NOTE]
>
>對認可日期所做的變更不會自動變更計畫日期，對計畫日期所做的變更不會自動變更認可日期。

手動設定任務或問題的認可日期會觸發下列變更：

* 認可日期變更會填入任務或問題的「系統活動」和「更新」區段的「所有」標籤中。

  ![認可日期變更通知](assets/project-owner-notification-update-stream-that-commit-date-affects-project-timeline.png)

  當Workfront管理員在設定的更新摘要區域中啟用此更新時，認可日期變更會顯示在任務或問題的更新區域中。 如需詳細資訊，請參閱[系統追蹤的更新](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/system-tracked-update-feeds.md)。

  如果專案所有者不想接受變更，我們建議他們使用「更新」區段中的「註解」索引標籤，將註解回覆給提出新日期的使用者，讓他們將「認可日期」變更回原始計畫日期，或選取新日期。

  如果專案所有者接受變更，他們可以通過編輯任務或問題手動調整計畫完成日期，以符合指派給專案的使用者所提供的認可日期。

  您必須有管理任務或問題的存取權才能編輯它們。

  >[!TIP]
  >
  >您可以要求系統或群組管理員將「認可日期」欄位新增到「摘要」面板或標題，以便於更新。
  >
  >如需詳細資訊，請參閱下列文章：
  >
  >* [摘要概述](/help/quicksilver/workfront-basics/the-new-workfront-experience/summary-overview.md)
  >* [使用配置範本自訂摘要面板](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md)
  >* [使用配置範本自訂物件標頭](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md)

<!--this is no longer possible: 
>[!NOTE]
>
>If you want to see how the timeline of the project is affected by accepting to change the Planned Completion Date of the task, click **Project Timeline**. This opens the task list where you can evaluate the date changes and the project timeline.
>
>
>![](assets/project-owner-notification-update-stream-that-commit-date-affects-project-timeline-highlighted-nwe-350x139.png)  >
>
-->


* 任務或問題的預計完成日期設定為相同日期，因為任務現在有更準確的指示可能完成的時間。

  如需詳細資訊，請參閱[專案、任務和問題的預計完成日期總覽](../../../manage-work/projects/planning-a-project/project-projected-completion-date.md)。

  ![](assets/task-projected-completion-date-in-details-highlighted-nwe-350x230.png)

* 在「通知」區域中通知專案所有者，任務或問題的認可日期已變更。

  ![認可日期變更通知](assets/in-product-notification-commit-date-changed-nwe-350x149.png)

  <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: the tip below is actually wrong and the updates feeds should not control this setting, but at this time it does, according to this issue in Hub: https://hub.workfront.com/issue/61e1aa5e0002a186fdd0a73a10db0fc3/updates?email-source=comm</p>
  -->

  >[!TIP]
  >
  >只有在Workfront管理員啟用在「設定」的更新摘要區域顯示認可日期時，才會將認可日期已變更的通知傳送給專案所有者。 如需詳細資訊，請參閱[系統追蹤的更新](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/system-tracked-update-feeds.md)。

如需有關更新工作專案時可用的其他功能的資訊，請參閱[更新工作](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md)。

如需更新任務和問題的認可日期的詳細資訊，請參閱[更新任務和問題的認可日期](../../../manage-work/projects/updating-work-in-a-project/update-commit-date-on-tasks-and-issues.md)。

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Update Commit Dates on tasks and issues</h2>
<p>(NOTE: moved to its own article) </p>
<p>Updating the Commit Date is identical for tasks and issues.</p>
<ol>
<li value="1"> <p>Go to a task or issue that you are assigned to as the <strong>Task Owner</strong>.</p> <p>For more information about finding out who the Task Owner for an issue or task is, see the section <a href="../../../manage-work/tasks/manage-tasks/edit-tasks.md#assignments" class="MCXref xref">Edit tasks</a> in the article <a href="../../../manage-work/tasks/manage-tasks/edit-tasks.md" class="MCXref xref">Edit tasks</a>.</p> </li>
<li value="2"> <p>Click Work on it in the task or issue header</p> <p>Or</p> <p>Click <strong>Start Task</strong> or <strong>Start Issue</strong> if the Work on it button has been customized in your environment to indicate that you are now working on the work item. </p> <p>At this time, the Commit Date and the Planned Completion Date of the task or issue are the same.</p> </li>
<li value="3"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">(Optional) If you clicked Start Task or Start Issue, click <strong>Undo</strong> in the lower-left corner of the screen. The Commit Date is removed. </p> <p>For information about replacing the Work On It button with a Start button, see <span href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md"><a href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">Replace the Work On It button with a Start button</a></span>.</p> <note type="tip">
The option to undo your selection to start your work is not available when you click
<span style="font-weight: bold;" data-mc-conditions="QuicksilverOrClassic.Quicksilver">Work on it</span>.
</note> </li>
<li value="4"> <p> Expand the <strong>This will be done by</strong> date picker, and select a new Commit Date.</p>
<div>
<div data-mc-conditions="QuicksilverOrClassic.Quicksilver">
<p>Click <strong>Updates</strong> in the left panel, then click the <strong>Start a new update</strong>><strong>Commit Date</strong></p>
<p>Or</p>
<p>Click <strong>Task Details</strong> or <strong>Issue Details</strong> in the left panel, then double click <strong>Commit Date</strong> and select a new date from calendar. </p>
</div>
<p>The Commit Date and the Planned Completion date are no longer the same.</p>
<p>Instead, the Commit Date and the Projected Completion Date of the task or issue become the same.</p>
<p>The changes are saved automatically.</p>
<p>The Project Owner is notified that you have suggested a new Commit Date for the task or issue and can, at this time, update the Planned Completion Date of the task or issue to match the Commit Date you suggested. For information about the notifications and updates that are triggered by this change, see the section <a href="#notifications-and-updates-triggered-by-changing-the-commit-date" class="MCXref xref">Notifications and updates triggered by changing the Commit Date</a> in this article.</p>
</div> </li>
</ol>
</div>
-->
