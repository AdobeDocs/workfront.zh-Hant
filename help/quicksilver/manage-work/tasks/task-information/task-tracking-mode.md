---
content-type: overview
product-area: projects
navigation-topic: task-information
title: 任務追蹤模式概觀
description: 建立或編輯任務時，您可以調整任務的「追蹤模式」設定，以控制任務的「進度狀態」指示器的顯示方式和時間。 當您設定某些設定來追蹤任務的進度時，Adobe Workfront會顯示進度狀態旗標。
author: Alina
feature: Work Management
exl-id: 397b5593-ac01-40cf-b683-fcf671a53d26
source-git-commit: 40b6ba5c4deb312fb40aecad4978b5a385e0f1e9
workflow-type: tm+mt
source-wordcount: '630'
ht-degree: 3%

---

# 任務追蹤模式概觀

建立或編輯任務時，您可以調整任務的「追蹤模式」設定，以控制任務的「進度狀態」指示器的顯示方式和時間。 當您設定某些設定來追蹤任務的進度時，Adobe Workfront會顯示進度狀態旗標。

如需有關任務進度狀態的詳細資訊，請參閱 [任務進度狀態總覽](../../../manage-work/tasks/task-information/task-progress-status.md).

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

身為任務擁有者或專案經理，您可以選取Workfront指示每個任務之進度狀態的方式。 如需如何在工作上設定追蹤模式的詳細資訊，請參閱 [設定任務的追蹤模式](../../../manage-work/tasks/task-information/set-tracking-mode-for-tasks.md).

您可以從下列選項中選取：

* [使用者必須更新](#user-must-update)
* [假設準時](#assume-on-time)
* [忽略遲到警告](#ignore-late-warnings)
* [自動完成](#auto-complete)
* [前置任務](#predecessor)

### 使用者必須更新 {#user-must-update}

選取此選項時，Workfront會使用任務的完成百分比和記錄的實際時數來判斷任務的進度狀態。 這是預設選項。

### 假設準時 {#assume-on-time}

Workfront假設任務將準時完成，無論目前完成狀態為何。 如果不適用，Workfront會自動假定下一個工作日的規劃完成日期。 您仍然必須指出任務何時完成。 當使用者不會定期更新其任務時，請使用此選項。

### 忽略遲到警告 {#ignore-late-warnings}

任務的進度狀態將為「準時」，直到變為「延遲」。 例如，如果您排程一項任務要花10天，而要在完成當天，該任務會顯示完成百分比為60%，則Workfront會新增四天來更新「預計完成日期」，且任務的「進度狀態」會變成「延遲」。

### 自動完成 {#auto-complete}

Workfront假設任務將依排程完成，並在其到期日或計畫完成日期將任務標示為完成。 在此之前，Workfront會使用完成百分比和記錄的實際時數來判斷進度狀態。 不過，無論排程完成日期前的進度狀態為何，Workfront仍會標籤任務已完成。

存在下列例外：

* 如果任務具有未完成的前置任務，則在完成所有前置任務之前不會自動完成該任務。 前置任務必須強制執行。
* 如果任務具有固定日期的限制，則無論前置任務是否已完成，任務一律在計畫完成日期完成。

>[!IMPORTANT]
>
>選取讓任務自動完成會在重新計算專案時間時將任務標籤為「完成」。 如果專案的「更新型別」設定為「自動」或「自動」及「變更時」，則會每天計算專案時間表。 如需關於專案時間表重新計算的資訊，請參閱 [重新計算專案時間表](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).
>
>實際完成日期的時間是自動計算時間表當天的午夜。 用來產生這個時間戳記的時間是您的系統時區，由您的Workfront管理員在設定的客戶資訊區段中定義。 如需有關設定系統時區的資訊，請參閱 [為您的系統設定基本資訊](../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).

### 前置任務 {#predecessor}

Workfront會根據前置任務關係來估計任務的預計完成日期。 任務的進度狀態是根據此估計來決定。 例如，任務B的工期為1天，並且排程在其前置任務任務A的兩天後完成，這應該需要5天。 然後，使用者將任務B更新為50%完成，但前置任務A尚未開始。 Workfront會在前置任務開始日期後六天，將相依任務B排程完成，任務A允許5天，任務B允許1天。
