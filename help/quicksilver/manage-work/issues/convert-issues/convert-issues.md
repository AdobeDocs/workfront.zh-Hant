---
product-area: projects
navigation-topic: convert-issues
title: 轉換Adobe Workfront問題概觀
description: 如果提交問題後需要完成更多工作才能完成問題，您可以將問題轉換為專案或任務。
author: Alina
feature: Work Management
exl-id: 97c83b65-208b-4e3f-b4cc-681237d82aa3
source-git-commit: 24cc3ece515fd778a9bc9e8afbcd534f48b24230
workflow-type: tm+mt
source-wordcount: '1264'
ht-degree: 2%

---

# 轉換Adobe Workfront問題概觀

如果提交問題後需要完成更多工作才能完成問題，您可以將問題轉換為專案或任務。

如需將問題轉換為工作的相關資訊，請參閱 [將問題轉換為Adobe Workfront中的任務](../../../manage-work/issues/convert-issues/convert-issue-to-task.md).

如需將問題轉換為專案的相關資訊，請參閱 [將問題轉換為Adobe Workfront中的專案](../../../manage-work/issues/convert-issues/convert-issue-to-project.md).

## 轉換問題時的考量事項

* 您的Workfront管理員或群組管理員已設定問題發生時的偏好設定、問題解決方式，以及將問題轉換為專案或任務時的主要聯絡人存取權，如 [配置全系統任務和問題首選項](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).
* Workfront會移除轉換期間與問題相關聯的任何核准。
* Workfront會在您將問題轉換為任務或專案時覆寫問題的「解決物件」。 新任務或問題在轉換後會變成問題的新「解決對象」。
* 請考量下列事項：

   * 轉換期間，系統可能會詢問您是否要將問題及其解決方法與您建立的專案或任務連結。
   * 如果您保留問題，當專案、任務或問題發生任何變更，或Workfront重新計算時間軸時，專案或任務的狀態和完成百分比會自動更新問題的狀態和完成百分比。

* 使用範本將問題轉換為專案時，範本中的大部分資訊都會傳送到新專案。 不過，問題中的一些資訊也可轉移到新項目。 如需詳細資訊，請參閱 [使用範本將問題轉換為專案時的專案欄位概觀](#overview-of-project-fields-when-converting-an-issue-to-a-project-using-a-template) 一節。
* 轉換問題時，並非所有文檔或其資訊都移動到問題轉換為的新對象。 轉換附加了文檔或文檔連結的問題時，將包括以下項目：

   * 文件
   * 第三方服務(例如Google Drive或SharePoint)的檔案連結。
   * 版本
   * 只有在選項時才包含校樣 **保留原始問題，並將其解決辦法與此任務聯繫起來** 未選取。
   * 轉換附加了文檔和文檔連結的問題時，不包括文檔批准。

* 如果您決定將問題保留在轉換中，且問題已附加文檔，則文檔及其版本將複製到項目或任務。 校樣和文檔批准不會複製到項目或任務。
* 如果您決定不將問題保留在轉換中，且問題中已附上檔案、檔案、其版本，以及校樣會轉移至專案或工作。 文檔批准不會轉移到項目或任務。
* 如果您的檔案和資料夾連結至來自協力廠商服務(例如Google Drive)的原始問題，無論您是否在轉換期間保留問題，這些連結都會複製到新物件。
* 也會將問題注釋複製到從問題轉換的任務或項目中，但標籤的用戶將不會轉移。
* 如果要將自定義表單資訊從問題傳輸到要轉換為項目或任務的項目或任務，請確保您有項目或任務自定義表單，其中包含要從問題傳輸的相同欄位。 如需詳細資訊，請參閱 [轉換物件時傳輸自訂表單資料](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/transfer-custom-form-data-larger-item.md).

## 使用範本將問題轉換為專案時的專案欄位概觀 {#overview-of-project-fields-when-converting-an-issue-to-a-project-using-a-template}

將問題轉換為專案時，您可以將問題轉換為空白專案或使用範本。

如需詳細資訊，請參閱 [將問題轉換為Adobe Workfront中的專案](../../../manage-work/issues/convert-issues/convert-issue-to-project.md).

使用範本時，某些填入在範本上的欄位會轉移至從轉換的問題建立的專案。 其他欄位會從轉換的問題轉移至專案。

下表列出項目資訊，以及項目資訊是從模板還是從問題中傳輸的：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>說明</td> 
   <td> <p>問題說明會轉移至新專案。 </p> <p> 如果問題沒有說明，範本中的說明會轉移至專案。 </p> <p>如果問題和範本的「說明」欄位都空白，專案上的欄位會是空的。 </p> </td> 
  </tr> 
  <tr> 
   <td>狀態</td> 
   <td>為模板上的組選擇預設狀態。 如果模板未與組關聯，則項目狀態將設定為Workfront管理員在「設定」的「項目首選項」區域中設定的預設狀態。 如需詳細資訊，請參閱 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">配置系統範圍的項目首選項</a>.</td> 
  </tr> 
  <tr> 
   <td>優先順序</td> 
   <td>從範本傳輸。 </td> 
  </tr> 
  <tr> 
   <td>URL</td> 
   <td> <p>問題的URL會傳輸至新專案。 </p> <p> 如果問題上未指定URL，則範本的URL會傳輸至專案。 </p> <p>如果問題和範本的URL欄位都空白，專案上的欄位會是空的。 </p> </td> 
  </tr> 
  <tr> 
   <td>專案條件類型</td> 
   <td>從範本傳輸。</td> 
  </tr> 
  <tr> 
   <td>專案條件</td> 
   <td>與Workfront管理員在「設定」區域中確定的系統級預設首選項匹配。 如需詳細資訊，請參閱 <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-projects.md" class="MCXref xref">將自訂條件設為專案的預設值</a></td> 
  </tr> 
  <tr> 
   <td>排程開始時間</td> 
   <td>從範本傳輸。</td> 
  </tr> 
  <tr> 
   <td>專案日期</td> 
   <td> 
    <ul> 
     <li> <p><b>計劃開始日期</b>:根據範本排程的時區，應預先選取以範本排程的工作時間為基礎的最接近工作時間。 如果「排程自」欄位設定為「自完成」，則此欄位將被禁用。 </p> </li> 
     <li> <p><b>計畫完成日期</b>:根據範本排程的時區，應預先選取以範本排程的工作時間為基礎的最接近工作時間。 如果「排程從」欄位設定為「從開始」，則此欄位將被禁用。 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>專案組合</td> 
   <td>從範本傳輸。 否則，此欄位為空。</td> 
  </tr> 
  <tr> 
   <td>方案</td> 
   <td>從範本傳輸。 否則，此欄位為空。</td> 
  </tr> 
  <tr> 
   <td>群組</td> 
   <td>從範本傳輸。 如果模板上沒有組，則該組將設定為問題所屬的項目組。</td> 
  </tr> 
  <tr> 
   <td>公司</td> 
   <td>從範本傳輸。 否則，此欄位為空。</td> 
  </tr> 
  <tr> 
   <td>專案所有者</td> 
   <td>從範本上的範本擁有者欄位傳輸。 否則，則會設為執行轉換的登入使用者。 </td> 
  </tr> 
  <tr> 
   <td>專案贊助者</td> 
   <td>從模板上的「模板發起人」欄位進行傳輸。 否則，此欄位為空。</td> 
  </tr> 
  <tr> 
   <td>資源管理器</td> 
   <td>從範本傳輸。 否則，此欄位為空。</td> 
  </tr> 
  <tr> 
   <td>任務設定</td> 
   <td>從範本傳輸。</td> 
  </tr> 
  <tr> 
   <td>問題設定</td> 
   <td>從範本傳輸。 </td> 
  </tr> 
  <tr> 
   <td>存取</td> 
   <td> <p>從範本上的存取區段傳輸。 </p> </td> 
  </tr> 
  <tr> 
   <td>核准</td> 
   <td>從範本傳輸。 轉換期間會移除與問題相關的核准。 </td> 
  </tr> 
 </tbody> 
</table>

<!--WRITER
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Convert an issue to a project</h2> 
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;moved to its own article)</p>
-->
<!--
<ol>
<li value="1"> Click the <strong>Issues</strong> icon on a project. <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <img src="assets/qs-issues-icon-highlighted-on-project.png"> </p> </li>
<li value="2"> <p>Click the issue to be converted to access the issue.</p> </li>
<li value="3"> <p> Click the <strong>More</strong> menu, then click <strong>Convert to Project</strong>. </p> <p> <img src="assets/qs-issue-more-menu-highlighted-350x469.png" style="width: 350;height: 469;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> </p> </li>
<li value="4"> <p>In the submenu that displays, do one of the following:</p>
<ul>
<li>Click <strong>New Project</strong></li>
<li>Under <strong>New from Template</strong>, click the name of a project template you want to use</li>
</ul> </li>
<li value="5"> <p>Specify a name for the project.</p> <p>The default name is the name of the issue you are converting.</p> </li>
<li value="6">(Optional and conditional) If you are creating this project from a template, update the available fields in the Convert to Project box.<br>For more information about editing fields on projects, see <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">Edit projects</a>.</li>
<li value="7"> <p>(Optional and conditional) Under <strong>Options</strong>, select any of the available options:</p>
<ul>
<li> <p><strong>Keep the original issue and tie its resolution to the this project</strong>When deselected, the original issue is deleted.</p> <note type="note">
<p>Users without access or permissions to delete issues will not be able to delete the issue as they are converting it, regardless of the status of this setting. For information about access and permissions to issues, see:</p>
<ul>
<li> <p><a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">Grant access to issues</a> </p> </li>
<li> <p><a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Share an issue </a> </p> </li>
</ul>
</note> </li>
<li><strong>Allow <User Name> to have access to this project</strong>If unselected, the user who entered the issue has no access to the new task.</li>
</ul> <note type="note">
<div>
<p>The options that are available here depend on how the Workfront administrator has configured them for everyone in the system or for your group. For more information, see <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md" class="MCXref xref">Configure system-wide task and issue preferences</a>.</p>
<p>Or, if the top-level groups in your organization configured them separately, the options available here depend on which group you selected for the new project in step 6. For more information, see <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md" class="MCXref xref">Configure task and issue preferences for a group</a><span class="preview">.</span></p>
</div>
</note> </li>
<li value="8">(Optional) In the <strong>Custom Forms</strong> section, attach any custom forms.<br>For more information about transferring information from the custom form of the issue to that of the new project, see <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/transfer-custom-form-data-larger-item.md" class="MCXref xref">Transfer custom form data when converting an object</a>.</li>
<li value="9"> <p>Click <strong>Save Changes.</strong></p> <p> <img src="assets/qs-issue-convert-to-project-before-saving-ui-350x366.png" style="width: 350;height: 366;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> </p> <p>The issue is now a project, if you decided to delete the original issue.<br>Or<br>The issue is now linked to the new project and it will complete when the project completes, if you decided to keep the original issue. </p> <p>Some issue fields transfer to the project. For information, see the <a href="#view-original-issue-information-on-projects-and-tasks" class="MCXref xref">View original issue information on projects and tasks</a> section in this article. </p> </li>
<li value="10"> <p>(Optional) Set any further project details ​(project owner, project dates) and tasks as necessary.</p> </li>
</ol>
</div>
-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Convert an issue to a task</h2> <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: moved to its own article)</p>
-->
<!--
<ol>
<li value="1"> Click the Issues icon on a project.  </li>
<li value="2"> <p>Click the issue you want to convert to go to the issue's landing page. </p> </li>
<li value="3"> <p> Click the <strong>More</strong> menu on the issue, then <strong>Convert to Task</strong>.  </p> <p> <img src="assets/qs-issue-more-menu-highlighted-350x469.png" style="width: 350;height: 469;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> </p> </li>
<li value="4"> <p>Name the task.</p> </li>
<li value="5"> <p>Identify the project where the task will reside. </p> <p>You can select a different project from the project that the issue is on.</p> </li>
<li value="6"> <p>In the <strong>Project</strong> box, start typing the name of the project where you want to put the new task, then press <strong>Enter</strong> when it appears.</p> <p>By default, this box the name of the project containing the issue that you are converting.</p> </li>
<li value="7"> <p>(Optional and conditional) Under <strong>Options</strong>, select any of the following options. </p> <p>The Workfront administrator or group administrator must enable these preferences before they are visible during the conversion of issues: </p>
<ul>
<li> <p><strong>Keep the original issue and tie its resolution to the this task</strong> </p> <p>If unselected, the original issue is deleted.</p> <note type="note">
<p>Users without access or permissions to delete issues will not be able to delete the issue as they are converting it, regardless of the status of this setting. For information about access and permissions to issues, see:</p>
<ul>
<li> <p><a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">Grant access to issues</a> </p> </li>
<li> <p><a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Share an issue </a> </p> </li>
</ul>
</note> </li>
<li> <p><strong>Allow <User Name> to have access to this task</strong> </p> <p>If unselected, the user who entered the issue has no access to the new task.</p> </li>
<li> <p><strong>Keep the planned completion date of the issue</strong> </p> <p>If unselected, the Planned Completion Date of the new task is calculated from the Planned Start Date of the task. The Planned Start Date of the new task is set according to the system preferences for new tasks.</p> </li>
</ul> <note type="note">
<div>
<p>The options that display here depend on how the Workfront administrator configured them for everyone in the system. For more information, see <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md" class="MCXref xref">Configure system-wide task and issue preferences</a>.</p>
<p>Or, if the top-level groups in your organization configured them separately, the options that display here depend on which group is associated with the project you selected in step 6. For more information, see <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md" class="MCXref xref">Configure task and issue preferences for a group</a>.</p>
</div>
</note> </li>
<li value="8">(Optional) Attach custom forms.<br>For more information about transferring information from the custom form of the issue to that of the new task, see <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/transfer-custom-form-data-larger-item.md" class="MCXref xref">Transfer custom form data when converting an object</a>.<br><p><img src="assets/qs-issue-convert-to-task-before-saving-ui-350x367.png" style="width: 350;height: 367;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"></p></li>
<li value="9"> <p>Click <strong>Save Changes</strong> when all task settings are set.</p> <p>The issue is now a task on the designated project, if you decided to delete the original issue.</p> <p>Or</p> <p>The issue is now linked to the new task on the project you chose, and it will complete once the task completes, if you decided to keep the original issue.</p> <p>Some issue fields transfer to the task. For information, see the <a href="#view-original-issue-information-on-projects-and-tasks" class="MCXref xref">View original issue information on projects and tasks</a> section in this article. <br></p> </li>
<li value="10"> <p>(Optional) Continue editing the task (assignments, dates) as necessary. </p> </li>
</ol>
</div>
-->

## 查看有關項目和任務的原始問題資訊 {#view-original-issue-information-on-projects-and-tasks}

您可以在項目和任務清單和報表中或在「項目詳細資訊」區域中查看原始問題資訊。 如需建立報表的相關資訊，請參閱 [建立自訂報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

下表說明了從轉換的項目和任務中可看到的問題欄位。

| 問題欄位 | 項目或任務欄位 | 專案清單或報表 | 項目詳細資訊區域 | 任務清單或報告 | 任務詳細資訊區域 |
|---|---|---|---|---|---|
| 問題名稱 | 轉換的問題名稱 | ✔ | ✔ | ✔ | ✔ |
| 主要連絡人 | 轉換的問題創作者名稱 | ✔ | `✔` | ✔ |   |
| 輸入日期 | 轉換的發行錄入日期 | ✔ |   | ✔ |   |


>[!CAUTION]
>
>如果問題的主要聯繫人更改，或者問題在轉換後從項目或任務中取消連結，則「轉換的問題發起人名稱」不會更新，它將在轉換問題時顯示問題的原始主要聯繫人。
