---
content-type: overview
product-area: projects
navigation-topic: task-information
title: 任務追蹤模式概觀
description: 在建立或編輯任務時，您可以調整任務的「跟蹤模式」設定，以控制任務的「進度狀態」指示符的顯示方式和顯示時間。 Adobe Workfront會在您配置特定設定以追蹤工作進度時顯示進度狀態旗標。
author: Alina
feature: Work Management
exl-id: 397b5593-ac01-40cf-b683-fcf671a53d26
source-git-commit: 6bb6b834c5af8ad48179fc0d60b184d083b360e4
workflow-type: tm+mt
source-wordcount: '626'
ht-degree: 3%

---

# 任務追蹤模式概觀

在建立或編輯任務時，您可以調整任務的「跟蹤模式」設定，以控制任務的「進度狀態」指示符的顯示方式和顯示時間。 Adobe Workfront會在您配置特定設定以追蹤工作進度時顯示進度狀態旗標。

有關任務的進度狀態的詳細資訊，請參見 [任務進度狀態概述](../../../manage-work/tasks/task-information/task-progress-status.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Set Tracking Mode for tasks</h2>
<p>(NOTE: drafted, because we created a new article and linked it below. Left this article as a "Overview" article only.) </p>
<p>To set the tracking mode:</p>
<ol>
<li value="1">Go to the task you want to set the tracking mode for.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png">next to the name of the task, then click&nbsp;<strong>Edit</strong>.</p> <p>The Edit Task dialog box opens. </p> </li>
<li value="3"> <p>In the&nbsp;<strong>Settings</strong> section, use the&nbsp;<strong>Tracking Mode</strong> drop-down menu to select the Tracking Mode for the task.</p> <p>For more information about the tracking mode options, see the <a href="#tracking-mode-options" class="MCXref xref" xrefformat="{para}">Tracking Mode options</a> section in this article. </p> </li>
<li value="4">Click&nbsp;<strong>Save Changes.</strong></li>
</ol>
</div>
-->

## 追蹤模式選項 {#tracking-mode-options}

作為任務所有者或項目經理，您可以選擇Workfront如何指示每個任務的進度狀態。 如需如何在工作上設定追蹤模式的詳細資訊，請參閱 [設定任務的追蹤模式](../../../manage-work/tasks/task-information/set-tracking-mode-for-tasks.md).

您可以選取下列選項：

* [使用者必須更新](#user-must-update)
* [假設準時](#assume-on-time)
* [忽略遲到警告](#ignore-late-warnings)
* [自動完成](#auto-complete)
* [前置任務](#predecessor)

### 使用者必須更新 {#user-must-update}

選取此選項時，Workfront會使用任務的「完成百分比」和「實際記錄小時數」來確定任務的「進度狀態」。 這是預設選項。

### 假設準時 {#assume-on-time}

Workfront假設無論目前的完成狀態為何，任務都會準時完成。 若未包含，Workfront會自動假設下一個工作日的計畫完成日期。 您仍必須指出任務何時完成。 當使用者不會定期更新其工作時，請使用此選項。

### 忽略遲到警告 {#ignore-late-warnings}

任務的進度狀態將為「準時」，直到延遲。 例如，如果您將任務安排為10天，並在任務完成的當天，任務顯示60%的完成百分比，則Workfront會添加4天來更新預計完成日期，任務的進度狀態變為延遲。

### 自動完成 {#auto-complete}

Workfront假設工作會依排程完成，並在到期或計畫完成日期將其標示為已完成。 在此之前，Workfront會使用完成百分比和實際記錄小時數來判斷進度狀態。 不過，無論排程完成日期前的進度狀態為何，Workfront仍會標籤任務完成。

存在下列例外：

* 如果任務的前置任務不完整，則在所有前置任務完成之前，不會自動完成該任務。
* 如果任務的約束為「固定日期」，則無論其前置任務是否已完成，任務始終在「計畫完成日期」完成。

>[!IMPORTANT]
>
>如果選擇讓任務自動完成，則在重新計算項目時間時，任務將標籤為「完成」。 如果項目的「更新類型」設定為「自動」或「自動」並且「更改時」，則每天計算項目時間軸。 如需重新計算專案時間軸的相關資訊，請參閱 [重新計算項目時間表](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).
>
>實際完成日期的時間是自動計算時間軸的午夜。 用於產生此時間戳記的時間是您系統的時區，如「設定」中「客戶資訊」區段中的Workfront管理員所定義。 有關設定系統時區的資訊，請參閱 [配置系統的基本資訊](../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).

### 前置任務 {#predecessor}

Workfront根據其前身關係估計任務的預計完成日期。 根據此估計確定任務的進度狀態。 例如，任務B的持續時間為1天，計畫在其前一個任務A之後完成兩天，該時間應為5天。 然後，用戶將任務B更新為50%完成，但前身任務A尚未啟動。 Workfront將相依任務B排程在前一任務開始日期後6天完成，使任務A有5天，任務B有1天。
