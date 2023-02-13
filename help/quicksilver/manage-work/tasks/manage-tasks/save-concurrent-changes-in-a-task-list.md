---
product-area: projects
navigation-topic: manage-tasks
title: 在任務清單中保存併發更改的概述
description: 當您編輯清單中的任務時，可以使用單獨的保存設定來指示在編輯清單中的任務時是否要手動保存更改。
author: Alina
feature: Work Management
exl-id: dff52425-4711-40a8-8f40-205d75c506ef
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '497'
ht-degree: 0%

---

# 在任務清單中保存併發更改的概述

當您編輯清單中的任務時，可以使用單獨的保存設定來指示在編輯清單中的任務時是否要手動保存更改。

有關編輯任務清單中任務的資訊，請參閱文章 [編輯清單中的任務](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md).

有時，如果兩個使用者對相同的工作進行變更，則可能會出現衝突。

在編輯任務清單中的任務時，請考慮以下事項：

* 如果項目「更新類型」為「自動」、「自動」或「更改時」，當您選擇自動保存更改時，Adobe Workfront會立即保存您對任務所做的更改。 有關項目更新類型的資訊，請參閱 [選擇項目更新類型](../../../manage-work/projects/manage-projects/select-project-update-type.md).
* Workfront會每分鐘更新您正在處理的清單上的資訊，並有其他使用者可能在系統的其他位置進行的變更。 這可確保您隨時獲得有關任務的最新資訊。

當多個使用者編輯相同的工作時，會出現下列情況：

* **一個用戶將更改自動保存到任務清單中，另一個用戶將手動保存更改**:如果用戶（用戶A）在用戶B編輯相同任務時手動保存更改，但他們自動保存更改，則用戶B所做的即時更改將每分鐘更新在用戶A的清單上。 如果兩個使用者所做的變更之間有衝突，手動儲存的使用者（使用者A）會在可以儲存其變更前看到警告訊息。 警告訊息會顯示有衝突變更的項目。 此時，使用者A可以選擇是保留變更（會覆寫使用者B所做的變更），還是捨棄變更（會保留使用者B所做的變更）。

>[!NOTE]
>
>當您選擇放棄所做的更改時，這將應用於所有更改，而不僅適用於那些與其他用戶所做的編輯衝突的更改。

* **有幾個用戶正在手動將更改保存到任務清單中**:如果對清單中的任務進行變更的數個使用者同時手動儲存，Workfront會儲存先儲存的使用者所進行的變更。 保存這些更改時不應遇到任何衝突。 Workfrontthen會比較所有其他用戶所做的更改與它已保存的資訊，並在其他用戶保存資訊之前顯示有關這些衝突更改的警告。

>[!IMPORTANT]
>
>當您選擇保留對所有其他更改所做的更改時，將保存所有更改，除非您對所做更改的任務已被其他用戶刪除。 在這種情況下，警告消息會通知您，您對已刪除任務所做的更改將丟失。

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
