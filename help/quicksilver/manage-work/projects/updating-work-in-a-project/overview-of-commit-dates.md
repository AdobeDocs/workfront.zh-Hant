---
content-type: overview
product-area: projects
navigation-topic: update-work-in-a-project
title: 提交日期概述
description: 「提交日期」是分配給任務或問題的用戶提交完成任務或問題的日期。 這與「計畫完成日期」不同，因為它是僅由負責工作的用戶提供的對完成日期更現實的估計。 有關計畫完成日期的資訊，請參閱：任務計畫完成日期概覽
author: Alina
feature: Work Management
exl-id: 47072433-bb8e-4210-947a-8bfa41ec47a9
source-git-commit: 6bb6b834c5af8ad48179fc0d60b184d083b360e4
workflow-type: tm+mt
source-wordcount: '818'
ht-degree: 0%

---

# 提交日期概述

「提交日期」是分配給任務或問題的用戶提交完成任務或問題的日期。 這與「計畫完成日期」不同，因為它是僅由負責工作的用戶提供的對完成日期更現實的估計。 有關計畫完成日期的資訊，請參閱 [任務計畫完成日期概覽](../../../manage-work/tasks/task-information/task-planned-completion-date.md).

## 提交日期概述

使用提交日期時，請考量下列事項：

* 只有任務和問題具有提交日期。
* 提交日期不會由Adobe Workfront自動設定。\
   建立任務或問題時，沒有為任務或問題分配提交日期。
* 如果已分配給任務或問題，則可通過執行以下操作之一來設定提交日期：

   * 通過按一下任務或問題上的「工作」、「開始問題」或「開始任務」，讓Workfront設定「提交日期」以與任務或問題的現有計畫完成日期相匹配。 有關用「開始」按鈕替換「工作在It」按鈕的資訊，請參閱  [將「Work On It（工作完成）」按鈕替換為「Start（開始）」按鈕](../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md).
   * 根據您認為任務或問題可能已完成的時間，自己手動設定提交日期。 這是您作為受託人對項目經理的估計和承諾，您將在特定日期之前完成該任務或問題。

>[!NOTE]
>
>您必須是任務的任務所有者才能更改提交日期。 以下用戶無法更改任務的提交日期：
>
>* 專案所有者
>* 專案贊助者
>* 資源管理員
>* 系統管理員
>* 任何任務上的其他受託人
>* 具有任務權限的任何其他用戶。
>
>有關「任務所有者」的詳細資訊，請參閱 [編輯任務](../../../manage-work/tasks/manage-tasks/edit-tasks.md#assignments) 在文章中 [編輯任務](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

## 通過更改提交日期觸發的通知和更新 {#notifications-and-updates-triggered-by-changing-the-commit-date}

當任務或問題受託人選擇的提交日期與項目責任人設定的計畫完成日期不同時，有許多通知和更新會提醒項目責任人和其他用戶注意此更改。

>[!NOTE]
>
>對提交日期所做的更改不會自動更改計畫日期，對計畫日期所做的更改不會自動更改提交日期。 

為任務或問題設定提交日期會觸發以下更改：

* 提交日期將填充到任務或問題的更新流中。

   ![](assets/update-stream-confirmation-that-commit-date-changed-nwe-350x73.png)

   當Workfront管理員在「設定」的「更新摘要」區域中啟用此更新時，「提交日期」的更改將顯示在任務或問題的「更新」區域中。 如需詳細資訊，請參閱 [系統追蹤更新](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/system-tracked-update-feeds.md).

* 任務或問題的「預計完成日期」設定為同一日期，因為任務現在可以更準確地指明何時可能完成。

   有關預計完成日期的詳細資訊，請參閱 [項目、任務和問題的預計完成日期概覽](../../../manage-work/projects/planning-a-project/project-projected-completion-date.md).

   ![](assets/task-projected-completion-date-in-details-highlighted-nwe-350x230.png)

* 在任務的通知區和更新頁簽中，將通知項目所有者此更改是否會影響項目時間軸。

   ![](assets/in-product-notification-commit-date-changed-nwe-350x149.png)

   <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: the tip below is actually wrong and the updates feeds should not control this setting, but at this time it does, according to this issue in Hub: https://hub.workfront.com/issue/61e1aa5e0002a186fdd0a73a10db0fc3/updates?email-source=comm</p>
  -->

   >[!TIP]
   只有當Workfront管理員啟用在「設定」的「更新摘要」區域中顯示「提交日期」時，「提交日期」已變更的通知才會傳送給專案擁有者。 如需詳細資訊，請參閱 [系統追蹤更新](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/system-tracked-update-feeds.md).

   如果項目所有者不想接受更改，我們建議他們向提出新日期的用戶進行評論，以要求他們將提交日期更改回原始計畫日期，或選擇新日期。 如果項目責任人接受更改，則他們可以手動調整計畫完成日期，以匹配分配給物料的用戶提供的提交日期。

   項目所有者可以使用提交日期重置計畫完成日期。 要執行此操作，請在任務的「更新」頁簽中選擇「將計畫日期設定為」選項。 您必須擁有管理任務和項目的權限才能接受此更改。

   >[!NOTE]
   如果要了解接受更改任務的計畫完成日期對項目時間軸的影響，請按一下 **專案時間表**. 這會開啟甘特圖，供您評估日期變更。
   ![](assets/project-owner-notification-update-stream-that-commit-date-affects-project-timeline-highlighted-nwe-350x139.png)  >

有關更新工作項時可用的其他功能的資訊，請參閱  [更新工作](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md). 

有關更新任務和問題的提交日期的資訊，請參閱 [更新任務和問題的提交日期](../../../manage-work/projects/updating-work-in-a-project/update-commit-date-on-tasks-and-issues.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Update Commit Dates on tasks and issues</h2>
<p>(NOTE:&nbsp;moved to its own article) </p>
<p>Updating the Commit Date is identical for tasks and issues.</p>
<ol>
<li value="1"> <p>Go to a task or issue that you are assigned to as the <strong>Task Owner</strong>.</p> <p>For more information about finding out who the Task Owner for an issue or task is, see the section <a href="../../../manage-work/tasks/manage-tasks/edit-tasks.md#assignments" class="MCXref xref">Edit tasks</a> in the article <a href="../../../manage-work/tasks/manage-tasks/edit-tasks.md" class="MCXref xref">Edit tasks</a>.</p> </li>
<li value="2"> <p>Click Work on it in the task or issue header</p> <p>Or</p> <p>Click <strong>Start Task</strong> or <strong>Start Issue</strong> if the Work on it button has been customized in your environment to indicate that you are now working on the work item. </p> <p>At this time, the Commit Date and the Planned Completion Date of the task or issue are the same.</p> </li>
<li value="3"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">(Optional) If you clicked Start Task or Start Issue, click <strong>Undo</strong> in the lower-left corner of the screen. The Commit Date is removed. </p> <p>For information about replacing the Work On&nbsp;It button with a Start button, see <span href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md"><a href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">Replace the Work On It button with a Start button</a></span>.</p> <note type="tip">
The option to undo your selection to start your work is not available when you click
<span style="font-weight: bold;" data-mc-conditions="QuicksilverOrClassic.Quicksilver">Work on it</span>.
</note> </li>
<li value="4"> <p> Expand the <strong>This will be done by</strong> date picker, and select a new Commit Date.</p>
<div>
<div data-mc-conditions="QuicksilverOrClassic.Quicksilver">
<p>Click <strong>Updates</strong> in the left panel, then click the <strong>Start a new update</strong>><strong>Commit Date</strong></p>
<p>Or</p>
<p>Click <strong>Task Details</strong> or <strong>Issue Details</strong> in the left panel, then double click&nbsp;<strong>Commit Date</strong> and select a new date from calendar. </p>
</div>
<p>The Commit Date and the Planned Completion date are no longer the same.</p>
<p>Instead, the Commit Date and the Projected Completion Date of the task or issue become the same.</p>
<p>The changes are saved automatically.</p>
<p>The Project Owner is notified that you have suggested a new Commit Date for the task or issue and can, at this time, update the Planned Completion Date of the task or issue to match the Commit Date you suggested. For information about the notifications and updates that are triggered by this change, see the section <a href="#notifications-and-updates-triggered-by-changing-the-commit-date" class="MCXref xref">Notifications and updates triggered by changing the Commit Date</a> in this article.</p>
</div> </li>
</ol>
</div>
-->
