---
product-area: projects
navigation-topic: manage-projects
title: 重新計算項目時間表
description: 重新計算時間表可讓管理員查看與項目相關的不同因素如何影響項目時間表。 項目時間表是指計畫日期和預計日期。
author: Alina
feature: Work Management
exl-id: ec5d9a07-e45a-4aa2-9f41-9421ca5d5920
source-git-commit: dc3461803e23f61877c31efa2c52fffdc7bd79bf
workflow-type: tm+mt
source-wordcount: '1017'
ht-degree: 0%

---

# 重新計算項目時間表

重新計算時間表可讓管理員查看與項目相關的不同因素如何影響項目時間表。 項目時間表是指計畫日期和預計日期。

對計畫、人員休假和項目範圍之外的其他項目進行更改不會立即影響項目時間表。 重新計算時間軸時，專案時間軸會受到影響。 在重新計算發生之前，外部影響不會對您的專案生效。

本文說明重新計算時間軸的方式。

## 存取需求

<!--drafted for P&P: 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Standard </p> 
   Or
   <p>Legacy license: Plan </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects</p> <p>System administrator to recalculate timeline for all projects in the system</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->
自動時間軸重新計算會針對參與專案工作的任何使用者進行，且無特殊存取權。

但是，您必須具有以下訪問權限才能手動重新計算項目時間軸：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>計劃 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>編輯專案的存取權</p> <p>系統管理員重新計算系統中所有項目的時間表</p> <p><b>附註</b>

如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>管理專案的權限</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 自動重新計算

預設情況下，當項目範圍改變或每晚更改時，每天自動重新計算項目時間軸。 Workfront管理員通過管理「設定」的「項目首選項」區域中的「時間軸」設定，確定是否每晚自動計算時間軸，還是每次更改範圍。 如需詳細資訊，請參閱 [設定專案的時間軸重新計算](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-timeline-recalculations-projects.md).

>[!NOTE]
>
>如果專案的時間軸超過15年，該專案會自動重新計算。 對於超過15年的項目，只能選擇「更新類型手動」。 如果將項目日期更改為少於15年，則必須在自動計算時間軸之前手動重新計算時間軸一次。

* [自動重新計算項目時間表](#automatic-recalculation-of-project-timelines)
* [觸發自動重新計算項目時間表的操作](#actions-that-trigger-an-automatic-recalculation-of-project-timelines)

### 自動重新計算項目時間表 {#automatic-recalculation-of-project-timelines}

Adobe Workfront僅在滿足下列所有條件的專案中每日重新計算時間表：

* 狀態為「當前」
* 項目的更新類型設定為「自動」或「自動」並且更改時

   有關項目更新類型類型的資訊，請參閱 [專案更新類型概觀](../../../manage-work/projects/planning-a-project/project-update-type-overview.md).

* 在過去三個月內有上次更新日期\
   Workfront管理員可依 [設定專案的時間軸重新計算](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-timeline-recalculations-projects.md).

* 項目時間表的最後計算日期不在當前日曆日內。 這表示專案時間軸的最後計算日期是當天00:00之前。

您可以設定專案時間軸的更新頻率。 更新專案時間軸時，會根據對專案所做的變更重新計算。

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
or changes made to another project that the timeline is dependent on
</MadCap:conditionalText>
-->


<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: above, the last part is drafted because of this: I don't think this is right because we told people that in the case of cross-project predecessors, the timeline must be calculated manually for the successor to see the updates in the predecessor's project. Drafting for now.)</p>
-->

如需詳細資訊，請參閱 [選擇項目更新類型](../../../manage-work/projects/manage-projects/select-project-update-type.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE:&nbsp;content moved to the article linked above)</p>
<p>You can configure how the timeline for your project is updated:</p>
<ol>
<li value="1">Go to the project for which you want to configure how the timeline is updated.</li>
<li value="2"> <p>  Click the <strong>More</strong> icon <img src="assets/more-icon.png"> to the right of the project name, then click&nbsp; <strong>Edit</strong>. </p> <p>The <strong>Edit Project</strong> dialog box is displayed.</p> </li>
<li value="3"> <p>Click<strong>Settings.</strong><br><img src="assets/screen-shot-2013-09-18-at-10.36.16-am-350x347.png" alt="" style="width: 350;height: 347;"></p> </li>
<li value="4">In the <strong>Update Type</strong> drop-down list, select from the following options:<br><strong>- Automatic and On Change:</strong> (Default setting) The project timeline is updated each time a change occurs in the project or in another project that the timeline is dependent on. The project timeline is also updated each night. <br>This is the recommended setting for this field because it ensures that the project timeline is always up to date.<br>When you update a task or the project and trigger a timeline recalculation, all available dates are immediately displayed, allowing you to continue working. On projects with more than 100 tasks, dates that require longer calculations are dimmed.
<div>
<p><img src="assets/dates-dimmed-when-insline-editing-350x146.png" style="width: 350;height: 146;"></p>
</div><br>This indicates that the recalculation is not yet finished, and the dates are subject to change. <br><strong>- Change Only:</strong> The project timeline is updated each time a change occurs in the project or in another project that the timeline is dependent on; scheduled updates do not occur.<br>You might want to select this option if changes rarely occur in the project or in other projects that the timeline is dependent on.<br><strong>- Automatic Only:</strong> The project timeline is updated each night; it is not updated immediately after changes are made.<br>You might want to select this option if many changes occur each day in the project or in other projects that the timeline is dependent on.<br><note type="note">
A project does not automatically recalculate each night if it is in Planning status. It only recalculates on change.
</note><br><strong>- Manual Only:</strong> The project timeline is updated only when you select the option to Recalculate Timelines, as described in <a href="#manual-recalculation" class="MCXref xref">Manual recalculation</a>.<br>You might want to select this option if you are making many changes to the project at one time, and you want the timeline recalculation to occur after all of the changes have been made (rather than after each individual change).<br>For more information about the project Update Type, see <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Select the project Update Type </a><note type="note">
If the timeline of a project is longer than 15 years, the automatic recalculation is disabled. If you change the dates on the project to less than 15 years, you must manually recalculate your timeline one time before it is calculated automatically.
</note></li>
<li value="5">Click <strong>Save Changes.</strong></li>
</ol>
</div>
-->

### 觸發自動重新計算項目時間表的操作 {#actions-that-trigger-an-automatic-recalculation-of-project-timelines}

項目生命週期中的各種範圍更改會自動重新計算項目時間表，包括以下操作：

* 正在更新任務狀態。
* 將任務移動到不同的項目。
* 更新任務的計畫日期或計畫完成日期。
* 更新任務的「持續時間類型」、「任務約束」或受分配人數。
* 更新任務前置關係。
* 將批准添加到任務，該任務還會將時間添加到任務的計畫完成日期。\
   如需核准設定的詳細資訊，請參閱 [配置全局批准設定](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md).

## 手動重新計算 {#manual-recalculation}

作為項目責任人，您可以人工重新計算各個項目的時間表。 Workfront管理員可以手動重新計算Workfront中的所有時間軸。

* [重新計算單個項目或批量項目的時間表](#recalculate-timelines-for-individual-projects-or-in-bulk)
* [在「編輯項目」框中手動重新計算時間軸](#manually-recalculate-timelines-in-bulk-in-the-edit-projects-box)
* [重新計算系統中所有項目的時間表(僅限Workfront管理員)](#recalculate-timelines-for-all-projects-in-the-system-workfront-administrators-only)

### 重新計算單個項目或批量項目的時間表 {#recalculate-timelines-for-individual-projects-or-in-bulk}

您可以從專案頁面或專案清單或報表重新計算Workfront中專案的時間軸。

1. 轉到要重新計算時間軸的項目，然後按一下 **更多** 圖示 ![](assets/qs-more-menu.png) 項目名稱左側

   ![](assets/project-level-more-drop-down-expanded-nwe-350x516.png)

   或

   前往專案清單或報表，選取一或多個專案，然後按一下 **更多** 圖示 ![](assets/qs-more-menu.png) 清單頂端。

   ![](assets/recalculate-expressions-timeline-finances-drop-down-in-project-list-nwe.png)

   >[!TIP]
   >
   >根據您專案的複雜性，我們建議在大量重新計算時間軸時不要選取大量專案，以確保最佳效能。 有些項目可能太複雜，可能是多個相依性或指派，或是大量自訂欄位。

1. 按一下 **重新計算時間表**.

   重新計算時間軸後，您會看到訊息，指出重新計算成功。

   >[!TIP]
   >
   >在時間軸重新計算完成之前，某些計畫日期或預計日期可能會顯示為灰色。 這表示重新計算尚未完成，且日期可能會變更。

### 在「編輯項目」框中手動重新計算時間軸 {#manually-recalculate-timelines-in-bulk-in-the-edit-projects-box}

您可以通過批量編輯多個項目來手動重新計算這些項目的時間軸。

>[!TIP]
>
>根據專案的複雜度，我們建議在大量編輯專案時不要選取大量專案，以確保提供最佳效能。 有些項目可能太複雜，可能是多個相依性或指派，或是大量自訂欄位。

1. 前往專案清單。
1. 在清單中選取數個專案，然後按一下 **編輯**.
1. 按一下 **設定**，然後選取 **重新計算時間表**.

1. 按一下 **儲存變更**.

### 重新計算系統中所有項目的時間表(僅限Workfront管理員) {#recalculate-timelines-for-all-projects-in-the-system-workfront-administrators-only}

Workfront管理員可以運行「重新計算時間軸」診斷程式，以立即重新計算Workfront系統中的所有時間軸。 這可讓所有項目經理立即查看外部更改對計畫日期和預計日期的影響。

如需重新計算整個Workfront網站時間軸的詳細資訊，請參閱 [設定專案的時間軸重新計算](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-timeline-recalculations-projects.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Project Update Types</h2>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: drafted and moved to thisa rticle: /Content/Manage work/Projects/Planning a Project/project-update-type-overview.htm)</p>
<p>For information about how to update the project's Update Type, see <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Select the project Update Type </a>. </p> <note type="important">
If the timeline of a project is longer than 15 years, Workfront does not calculate the timeline automatically or on change. The Update Type of a project longer than 15 years is always Manual.
</note>
<p>You can select how each project calculates its timeline by choosing between the following Update Types:</p> <note type="important">
If the timeline of a project is longer than 15 years, Workfront does not calculate the timeline automatically or on change. The Update Type of a project longer than 15 years is always Manual.
</note>
<ul>
<li> <p><strong>Automatic and On Change:</strong>&nbsp;This is the default setting. The project timeline is updated each time a change occurs&nbsp;in the project or in another project that the timeline is dependent on. The project timeline is also updated each night.&nbsp; <br>This is the recommended setting as it ensures that the project timeline is always up to date.</p> <p>When you update a task or the project and trigger a timeline recalculation, all available dates are immediately displayed, allowing you to continue working. On projects with more than 100 tasks, dates that require longer calculations are dimmed. </p> <p> <img src="assets/dates-dimmed-when-insline-editing-350x146.png" style="width: 350;height: 146;"> </p> <p>This indicates that the recalculation is not yet finished, and the dates are subject to change. </p> </li>
<li><strong>Change Only:</strong>&nbsp;The project timeline is updated each time a change occurs in the project or in another project that the timeline is dependent on; scheduled updates do not occur. <br>You might want to select this option if you are concerned about system performance and if&nbsp;changes rarely occur in the project or in other projects that the timeline is dependent on.</li>
<li> <p><strong>Automatic Only:</strong>&nbsp;The project timeline is updated each night; it is not updated immediately after changes are made.<br>You might want to select this option if you are concerned about system performance and if many changes occur each day in the project or in other projects that the timeline is dependent on.</p> <note type="note">
A project does not automatically recalculate each night if it is in Planning status. It only recalculates on change.
</note> </li>
<li><strong>Manual Only:</strong>&nbsp;The project timeline is updated only&nbsp;when you select the option to <strong>Recalculate Timelines</strong>, as described in the section "Manual Recalculation" in&nbsp;the article <a href="#" class="MCXref xref selected">Recalculate project timelines</a>.<br>You might want to select this option if you are making many changes to the project at one time, and you want the timeline recalculation to occur after all of the changes have been made (rather than after each individual change).</li>
</ul>
</div>
-->
