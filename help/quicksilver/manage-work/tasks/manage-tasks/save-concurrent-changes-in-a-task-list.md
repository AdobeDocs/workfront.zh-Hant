---
product-area: projects
navigation-topic: manage-tasks
title: 在作業清單中儲存並行變更的概要
description: 當您編輯清單中的任務時，可以使用單獨的儲存設定來指示您是否希望在編輯清單中的任務時自動手動儲存變更。
author: Alina
feature: Work Management
exl-id: dff52425-4711-40a8-8f40-205d75c506ef
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '497'
ht-degree: 0%

---

# 在作業清單中儲存並行變更的概要

當您編輯清單中的任務時，可以使用單獨的儲存設定來指示您是否希望在編輯清單中的任務時自動手動儲存變更。

如需有關編輯工作清單中工作的資訊，請參閱文章[編輯清單中的工作](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md)。

有時候，如果兩個使用者對相同的任務進行變更，則可能會出現衝突。

編輯任務清單中的任務時，請考量下列事項：

* 如果專案更新型別是自動、自動或變更時，當您選擇自動儲存您的變更時，Adobe Workfront會立即儲存您對任務所做的變更。 如需有關專案更新型別的資訊，請參閱[選取專案更新型別](../../../manage-work/projects/manage-projects/select-project-update-type.md)。
* Workfront會利用其他使用者在系統中其他地方可能進行的變更，每分鐘更新您正在處理的清單資訊。 這可確保您一律取得有關任務的最新資訊。

有多個使用者編輯相同任務時，會發生下列情況：

* **一位使用者會自動儲存工作清單中的變更，而另一位使用者則是手動儲存**：如果使用者（使用者A）在使用者B編輯相同工作時手動儲存變更，但是他們會自動儲存變更，則使用者B所做的即時變更會每分鐘更新一次使用者A的清單。 如果兩個使用者所做的變更之間發生衝突，手動儲存的使用者（使用者A）在儲存變更之前會看到警告訊息。 警告訊息會顯示具有衝突變更的專案。 此時，使用者A可以選擇是保留變更（覆寫使用者B所做的變更）還是捨棄變更（保留使用者B所做的變更）。

>[!NOTE]
>
>當您選取捨棄您所做的變更時，這會套用至所有變更，而不只是套用至與其他使用者所做的編輯有衝突的變更。

* **多位使用者正在手動儲存工作清單中的變更**：如果多位使用者正在手動同時儲存清單中的工作變更，則Workfront會儲存最先儲存的使用者所做的變更。 儲存這些變更不會發生任何衝突。 接著，Workfront會比較所有其他使用者所做的變更與其已儲存的資訊，並在其他使用者儲存其資訊之前，顯示關於衝突變更的警告。

>[!IMPORTANT]
>
>當您選擇保留您對所有其他變更所做的變更時，除非您對所做變更的任務已被其他使用者刪除，否則會儲存您的所有變更。 在這種情況下，警告訊息會通知您對已刪除的任務所做的變更遺失。

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
<p class="preview" data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: drafted - when replaced with the above live section; does it need an edit??) </p>
<div>
<p>When editing tasks in a list, you can select whether you want each change to be saved automatically or if you want to manually save multiple changes at one time by clicking the Save button. This depends on whether you enable the Autosave setting in the task list or not. </p>
<p>For information about editing tasks in a task list, see the article <a href="../../../manage-work/tasks/manage-tasks/edit-tasks.md" class="MCXref xref" xrefformat="{para}">Edit tasks</a>. </p>
<p>Sometimes, conflicts might appear if two users are making changes on the same tasks. </p>
<p>Consider the following when editing tasks in a task list: </p>
<ul>
<li>Workfront saves the changes you make to tasks immediately when you have enabled the Autosave setting. </li>
<li>Workfront updates the information on the list you are working on every minute with changes that other users might make anywhere else in the system. This ensures that you always get the latest information on the tasks. </li>
</ul>
<p>The following scenarios exist when multiple users are editing the same tasks:</p>
<ul>
<li>One user has Autosave disabled and another has it enabled: If a user (User A) has disabled the Autosave setting and is editing the task list while User B is editing the same tasks but they have enabled the Autosave setting, the live changes made by User B are updated on the list for User A every minute. If there are conflicts between the changes made by the two users, the user with the Autosave setting disabled (User A) sees a warning message before they can save their changes, that shows the items that have those conflicting changes. At this time, User A can choose whether they should keep their changes (which overwrites the changes made by User B), or discard them (which keeps the changes made by User B.) </li>
</ul> <note type="note">
When you select to discard the changes you made, this applies to all the changes and not just to those that have conflicts with the edits made by another user.
</note>
<ul>
<li>Several users have disabled the Autosave setting: If several users that have disabled the Autosave setting are making changes at the same time, Workfront saves the changes made by the user who saves first. Saving these changes should not encounter any conflicts. Workfrontthen compares the changes made by all the other users with the information that it already saved and displays a warning about the conflicting changes to the other users before they can save their information. </li>
</ul> <note type="important">
When you select to keep your changes over all other changes, your changes are saved, unless the tasks you made changes to were deleted by another user. In this case, the warning message informs you that the changes you made to the deleted tasks are lost.
</note>
</div>
</div>
-->
