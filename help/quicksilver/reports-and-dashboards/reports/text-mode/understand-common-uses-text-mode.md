---
product-area: reporting
navigation-topic: text-mode-reporting
title: 文字模式的常見用途概觀
description: 文字模式的常見用途概觀
author: Nolan
feature: Reports and Dashboards
exl-id: 81512837-1ec4-4dbc-ace4-bdf08fe667ce
source-git-commit: 7697327455a7ffdc1a15bfa1676c3a0b091abd04
workflow-type: tm+mt
source-wordcount: '762'
ht-degree: 0%

---

# 文字模式的常見用途概觀

<!-- Audited: 1/2024 -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: ***This is linked to Understanding Text Mode (article), and the TOC article for examples of various reporting elements)</p>
-->

您可以在報表與報表元素中使用文字模式，藉此擴展您的報表功能。 您也可以使用某個版本的文字模式，以建置更複雜的計算自訂欄位。 如需文字模式的詳細資訊，請參閱[文字模式概觀](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md)。

本文僅概述幾個常見範例，說明在Adobe Workfront中極可能需要使用文字模式來擴展報表或計算自訂欄位功能的位置。 如需更詳細的範例清單，請參閱：

* [自訂檢視、篩選和群組範例：發行項索引](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md)
* [報表中計算的自訂資料](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-custom-data-reports.md)

如需使用文字模式建立報表的詳細資訊，包括類別、影片和教學課程，請參閱Adobe Experience League網站上的「瞭解」一節。

<!--this link is outdated: 

For additional real-life text mode examples that other Workfront customers might have identified, visit the [Text Mode Reporting Discussions](https://one.workfront.com/s/topic/0TO0z000000cdHmGAI/text-mode-reporting?tabset-21363=3) tab in&nbsp; Adobe Workfront One or join the [Workfront Community](https://one.workfront.com/s/community) (requires logging in). &nbsp;

-->

## 您可能在清單和報告中使用文字模式的例項

建議您使用Report和List Builder來建置檢視、篩選器和群組。 不過，在某些情況下，您可以使用文字模式來增強報表和清單。

當您想要在Workfront中達成下列目標時，可以使用文字模式：

* 在自訂表單中建立自訂計算自訂欄位。\
  如需有關計算自訂欄位的詳細資訊，請參閱本文中的[在計算自訂欄位中使用文字模式](#use-text-mode-in-calculated-custom-fields)區段。
* 增強超出Report Builder可能的篩選器、檢視和群組。 如需有關使用文字模式進行篩選、檢視和分組的資訊，請參閱本文中的下列章節：

   * [在檢視中使用文字模式](#use-text-mode-in-views)
   * [在篩選中使用文字模式](#use-text-mode-in-filters)
   * [在分組中使用文字模式](#use-text-mode-in-groupings)

* 建立自訂提示。 您只能使用文字模式建立自訂提示。

  如需建立自訂提示的相關資訊，請參閱[新增提示至報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)。

## 在計算自訂欄位中使用文字模式 {#use-text-mode-in-calculated-custom-fields}

您可以使用文字模式將計算的自訂欄位新增到自訂表單。

如需將計算自訂欄位新增至自訂表單的詳細資訊，請參閱[建立自訂表單](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)。

如需以文字模式建立計算自訂欄位的詳細資訊，請參閱[將計算欄位新增至表單](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md)。

例如，您可以新增計算自訂欄位，顯示專案標示為進行中時的時間和日期戳記。 您可以將此計算用於其他狀態。

如需詳細資訊，請參閱[計算自訂欄位範例：在自訂表單中顯示[狀態]時間戳記](../../../reports-and-dashboards/reports/calc-cstm-data-reports/example-status-timestamp-in-calculated-field.md)。

<!--
<ul data-mc-conditions="QuicksilverOrClassic.Draft mode">
<li><a href="#display-a-status-timestamp-in-a-custom-form" class="MCXref xref">Display a Status timestamp in a Custom Form</a> </li>
</ul>
-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p><strong>Display a Status timestamp in a Custom Form</strong></p> 
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: This section used to be undrafted but replaced it with a standlone article. See new article: /Content/Reports and Dashboards/Reports/Calc Cstm Data-Reports/example-status-timestamp-in-calculated-field.htm)</p>
<p>The following calculated field displays the date when the specified object status was modified. </p>
<ol>
<li value="1">Navigate to a Custom form where you want to add the field.</li>
<li value="2">Click <strong>Calculated</strong> to add a calculated custom field to the form.<br></li>
<li value="3">Specify a <strong>Label</strong> for the Custom Field, for example: <i>Status Timestamp Custom Field</i>.</li>
<li value="4">(Optional) Click the <strong>Name</strong> field to update it. The Name of the field matches the Label you just entered by default. </li>
<li value="5">Click&nbsp;<strong>Done</strong>. </li>
<li value="6">Click <strong>Save+Close</strong>.</li>
<li value="7">Re-open the Custom Form, and click the new Status Timestamp Custom Field on the form.</li>
<li value="8"> In the <strong>Calculation</strong> field, specify the following calculation for your Custom Field:<br><pre>IF(Status='INP',IF(ISBLANK({DE:Status Timestamp Custom Field}),$$NOW,{DE:Status Timestamp Custom Field}),{DE:Status Timestamp Custom Field}) </pre>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:Alina: text should wrap here.)</p>
<note type="note">  You must always use the three letter key for the Status in this calculation.
<br>For more information about the keys for Statuses, see
<a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md" class="MCXref xref">Create or edit a status</a>.
</note></li>
<li value="9"> Click <strong>Save+Close</strong>.<br>You can then report on the Status Timestamp Custom Field, or use it in other calculations in reports or Custom Fields.<br> <note type="note">  If your status changes to INP, then another status, then back to INP, Workfront captures only the timestamp of the first change to INP.
</note><br></li>
</ol>
</div>
-->

## 在檢視中使用文字模式 {#use-text-mode-in-views}

您可以在檢視中使用文字模式，展開您可以在檢視中顯示的欄位和物件。

如需在檢視中使用文字模式的最常見原因範例，請參閱下列文章：

* [檢視：顯示未包含在標準介面中的物件](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-display-objects-not-in-standard-interface.md)
* [檢視：顯示資料行](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-calculation-between-two-fields.md)中兩個欄位之間的計算結果
* [檢視：永久編輯資料行的寬度](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-edit-column-width-permanently.md)
* [檢視：合併一個共用資料行中多個資料行的資訊](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-merge-columns.md)
* [檢視：移除資料行](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-remove-link-to-object.md)中物件的連結
* [報表中的參考集合](../../../reports-and-dashboards/reports/text-mode/reference-collections-report.md)
* [檢視：隱藏資料行的內容](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-hide-column-content.md)
* [檢視：在欄中顯示影像，而非字串](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-display-image-in-view.md)
* [檢視：在任務清單中顯示任務縮排](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-display-task-identations.md)
* [檢視：計算時間和日期差異](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-calculate-time-and-date-differences.md)

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>The most common reason for using text mode in a view are: </p>
<ul>
<li><a href="#display-objects-that-are-not-included-in-the-standard-interface" class="MCXref xref">Display objects that are not included in the standard interface</a> </li>
<li><a href="#make-a-calculation-between-two-fields-in-a-column" class="MCXref xref">Make a calculation between two fields in a column</a> </li>
<li><a href="#edit-the-width-of-a-column-permanently" class="MCXref xref">Edit the width of a column permanently</a> </li>
<li>
<div>
<h2>Access requirements</h2>
<p>You must have the following access to perform the steps in this article:</p>
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
<td> <p>Plan </p> </td>
</tr>
<tr>
<td role="rowheader">Access level configurations*</td>
<td> <p>Edit access to Filters, Views, Groupings</p> <p>Edit access to&nbsp;Reports,&nbsp;Dashboards,&nbsp;Calendars to create a view in a report</p> <note type="note">
If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see
<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.
</note> </td>
</tr>
<tr>
<td role="rowheader">Object permissions</td>
<td> <p>Manage permissions to a report to create or edit a view in a report</p> <p>Manage permissions to a view to edit it</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td>
</tr>
</tbody>
</table>
<p>*To find out what plan, license type, or access you have, contact your Workfront administrator.</p>
</div> </li>
<li><a href="#edit-the-width-of-a-column-permanently" class="MCXref xref">Edit the width of a column permanently</a> </li>
<li><a href="#merge-multiple-columns-into-a-single-column" class="MCXref xref">Merge multiple columns into a single column</a> </li>
<li><a href="#remove-a-link-to-an-object-from-the-view" class="MCXref xref">Remove a link to an object from the view</a> </li>
<li><a href="#display-a-collection-in-a-view" class="MCXref xref">Display a collection in a view</a> </li>
<li><a href="#hide-the-content-of-a-column-in-a-view" class="MCXref xref">Hide the content of a column in a view</a> </li>
<li><a href="#display-an-image-in-a-view" class="MCXref xref">Display an image in a view</a> </li>
<li><a href="#display-task-indentations-in-a-view" class="MCXref xref">Display task indentations in a view</a> </li>
<li><a href="#calculate-time-and-date-differences" class="MCXref xref">Calculate time and date differences</a> </li>
</ul>
</div>
-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p><strong>Display objects that are not included in the standard interface</strong></p>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: see new article: /Content/Reports and Dashboards/Reports/Custom View Filter Grouping Samples/view-display-objects-not-in-standard-interface.htm)</p>
<p>You can display objects in a view that are not included in the standard mode interface. Some objects can be included in a view only by referencing them via text mode.<br>You can know which fields can be included in a view in either of the following ways:</p>
<ul>
<li>Use the <a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">API Explorer</a> to discover other objects that can be referenced via text mode.<br>Not all the fields documented in the API Explorer are valid fields for text mode. Some fields are only reportable through the API.</li>
<li>A column or field name is not available in the standard mode interface, but the column or field ID is. Most objects that have a column or field ID also have a corresponding column or field name. However, in some cases, only the ID is displayed in the standard mode Interface. You can use text mode to include the column or field name in a view by replacing the <strong>fieldnameID</strong> with the <strong>fieldname:name</strong>.<br>For example, in the standard mode interface, the <strong>Sponsor ID</strong> field is available for a project, but the <strong>Sponsor Name</strong> field is not. You can use text mode to display the <strong>Sponsor Name</strong>, if you switch the <strong>Sponsor ID</strong> column to text mode and replace the text in the column with:<br><pre>valuefield=project:sponsor:name<br>querysort=project:sponsor:name<br>valueformat=HTML<br>displayname=Project Sponsor Name<br>linkedname=project<br>namekey=view.relatedcolumn<br>namekeyargkey.0=project<br>namekeyargkey.1=sponsorID</pre></li>
</ul>
<p><strong>Make a calculation between two fields in a column</strong></p> 
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: see new article: /Content/Reports and Dashboards/Reports/Custom View Filter Grouping Samples/column-calculation-between-two-fields.htm)</p>
<p>For example, if you want to find out the number of week days that elapsed between two dates, you can use text mode syntax and data expressions to calculate this difference.<br>For example, we want to calculate the week day difference between the Planned Completion Date and the Actual Completion Date of a task.<br>To do this, you can add a new column to a task view, and <strong>Switch to Text Mode</strong>. In the <strong>Click to edit text</strong> dialog box, paste the following text: </p>
<pre>displayname=Week Day Difference<br>textmode=true<br>valueexpression=WEEKDAYDIFF({plannedCompletionDate},{actualCompletionDate})<br>valueformat=HTML</pre>
<p>You can use any other two dates in this calculation (Actual Start, Actual Completion, Projected Start, Projected Completion, etc).<br>For more information about calculated data expressions, see <a href="../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md" class="MCXref xref">Overview of calculated data expressions</a>.</p>
<p><strong>Edit the width of a column permanently</strong></p> 
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: see new article: /Content/Reports and Dashboards/Reports/Custom View Filter Grouping Samples/column-edit-column-width-permanently.htm) </p>
<p>You can permanently change the width of a column by using these lines in the text mode of the column:</p>
<pre>width=200<br>usewidths=true</pre>
<p>For the <strong>width</strong> line, specify any number (in pixels), according to how wide you want the column to display in the report.</p>
<p><strong>Merge multiple columns into a single column</strong></p> 
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: see new article: /Content/Reports and Dashboards/Reports/Custom View Filter Grouping Samples/view--merge-columns.htm)</p>
<ul>
<li> <p><a href="#merge-data-from-two-columns-with-a-line-break" class="MCXref xref">Merge data from two columns with a line break </a> </p> </li>
<li> <p><a href="#merge-data-from-two-columns-with-no-line-break" class="MCXref xref">Merge data from two columns with no line break </a> </p> </li>
</ul>
<h4 id="merge-data-from-two-columns-with-a-line-break">Merge data from two columns with a line break </h4>
<p>Do the following to share the data from multiple columns to display it in one common column with a line break between the values from each column:</p>
<ol>
<li value="1"> <p>Add a third column between the two columns you want to merge. </p> </li>
<li value="2"> <p>Add the following code in the middle column: </p> <p><pre>value=<br></pre><pre>valueformat=HTML</pre><pre>width=1</pre><pre>sharecol=true</pre> </p> </li>
<li value="3"> <p>Add the following text to the first column:</p> <p><code>sharecol=true</code> </p> </li>
</ol>
</div>
-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h4 id="merge-data-from-two-columns-with-no-line-break">Merge data from two columns with no line break </h4>
<p>You can share the data from multiple separate columns to display it in one column with no breaks or spaces between the values from each column. </p>
<p>To do this:</p>
<ol>
<li value="1"> <p>Add the following text to the first column:</p> <p><code>sharecol=true</code> </p> </li>
</ol> <note type="note">  Consider the following when using shared columns:
<ul>
<li>The <code>valueformat=HTML</code> line is mandatory in a shared column. Otherwise, the columns contain no information (they will be blank) when the report is exported from Workfront.</li>
<li>Conditional formatting may not be supported in merged columns.</li>
<li>Columns with the <strong>viewalias</strong> attribute can limit the amount of columns that you can merge. To avoid these limits, avoid using the <strong>viewalias</strong> attribute. If you must include the <strong>viewalias</strong> attribute in a column, make sure that they are the last item listed in the column.</li>
</ul>
</note>
<p><strong>Remove a link to an object from the view</strong></p> 
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: see this new article: /Content/Reports and Dashboards/Reports/Custom View Filter Grouping Samples/column-remove-link-to-object.htm)</p>
<p>Some objects that you display in a view are links to the Details page of the object, by default. For example, the column that displays the Name of a project is a link to the project; the column that displays the Name of a user is a link to the user profile page.</p>
<p>You can remove this link using text mode.<br>For example, to remove the link to a task in a project report, you may use the following text mode in a column:</p>
<pre>displayname=Task Name<br>linkedname=direct<br>namekey=name<br>querysort=name<br>textmode=true<br>valueexpression={name}<br>valueformat=Compound</pre> <note type="note">  You can use similar code for other objects, and just replace the
<strong>valuefield</strong> line of the code with
<strong>valueexpression</strong>. This removes the link from the view.
</note>
<p><strong>Display a collection in a view</strong></p> 
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this already has its own article, maybe just list the other article in the TOC of the example) </p>
<p>Display a collection in a report view. A collection is a list of objects that are linked to one other object.<br>For information about displaying a collection in a report view, see the "Reference collections in a View of a report" section in the article <a href="../../../reports-and-dashboards/reports/text-mode/reference-collections-report.md" class="MCXref xref">Reference collections in a report</a>.</p>
<p><strong>Hide the content of a column in a view</strong></p> 
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: see new article: /Content/Reports and Dashboards/Reports/Custom View Filter Grouping Samples/column-hide-column-content.htm) </p>
<p>You can build a column in a view for purposes of sorting the view by a certain field, but you can use text mode to hide the information inside the column from displaying in the view. In this case, the object in the column helps sort the view, but the information of that object does not display in the view.</p>
<p>For example, to hide the Task Number column in a task report, replace the text in the Task Number column with the following:</p>
<pre><strong>displayname=</strong>linkedname=direct<br>querysort=taskNumber<br>sortOrder=1<br>sortType=asc<br>textmode=true<br><strong>value=</strong>valueformat=int<br><strong>width=0</strong></pre>
<p>The important changes in this code which make the column hidden are:</p>
<ul>
<li><code>displayname</code>: This line must be blank.</li>
<li><code>valuefield</code>: This has been replaced by <em>value</em>, and must be blank.</li>
<li><code>width</code>: Depending on the field, this must have a value of <i>0</i> or <i>1</i>.</li>
</ul> <note type="note">  
<ul>
<li>You can use hidden columns to sort by a certain object that you do not want to display in the view.<br>For example, you can sort by Task Number in a task view in the example provided above, and hide the Task Number information from the view.</li>
<li>When you hide a column, note that the information in the column is hidden, but the column still exists in the view.</li>
</ul>
</note>
</div>
-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p><strong>Display an image in a view</strong></p>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: see new article: /Content/Reports and Dashboards/Reports/Custom View Filter Grouping Samples/column-display-image-in-view.htm) </p>
<p>You can replace the name of an object in a view with an image.</p> <note type="note">  Images appear in their actual resolution so try to use small images. This example is for projects, but it applies to any object with a
<strong>URL</strong> field. You can add it to any column to replace the value of the column with an image.
</note>
<p>To replace the name of a project in a project view with an image:</p>
<ol>
<li value="1"> <p>Ensure that you have an image that is stored on a server accessible from Workfront.</p> <note type="tip">
Avoid using images that are uploaded to Workfront. Because images stored in Workfront are not publicly available and have an access key that expires after a period of time, these images stop displaying in the view over time.
</note> </li>
<li value="2">  Go to a project, click the <strong>More</strong> menu <img src="assets/more-icon-45x33.png" style="width: 45;height: 33;"> next to the name of the project, then click <strong>Edit</strong>.  </li>
<li value="3">In the <strong>URL</strong> field, add the link to the image.</li>
<li value="4">Navigate to a project view in a list or report and customize the view.</li>
<li value="5">Click the header of the column for the <strong>Project Name</strong>, then click <strong>Switch to Text Mode</strong>.</li>
<li value="6">Add the following code to the column to the existing code:<br><pre>displayname=Link Project<br>image.name=Link Project<br>image.valuefield=URL<br>link.linkproperty.0.name=projectID<br>link.linkproperty.0.value=ID<br>link.lookup=link.edit<br>link.page=/view<br>link.valuefield=objCode<br>link.valueformat=val<br>textmode=true<br>type=image<br>valueformat=</pre> The image you selected replaces the Project Name in the project view.</li>
<li value="7">Click <strong>Save View</strong>.</li>
</ol>
</div>
-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p><strong>Display task indentations in a view</strong></p>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:new article to replace this: /Content/Reports and Dashboards/Reports/Custom View Filter Grouping Samples/view-display-task-identations.htm) </p>
<p>Add this code to the Task Name column in a task view, to display the tasks indented according to the Work Breakdown Structure of the project:</p>
<pre>valueexpression=IF({indent}<1,{name},IF({indent}<2,CONCAT(' - ',{name}),IF({indent}<3,CONCAT(' - - ',{name}),IF({indent}<4,CONCAT(' - - - ',{name}),CONCAT(' - - - - ',{name}))))) </pre>
<p>This adds up to four dashes before the task name to indicate the position of the child task. </p>
<p><strong>Calculate time and date differences</strong></p>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: replace with this article: /Content/Reports and Dashboards/Reports/Custom View Filter Grouping Samples/view-calculate-time-and-date-differences.htm ----- add to the toc article--- hide this content in this article) </p>
<note type="important">  You cannot calculate the time and date difference in Workfront between two different objects of the same kind. For example, you cannot calculate the time and date difference between two dates on two different projects, tasks, or issues.
</note>
<p>You can only calculate the difference between the following:</p>
<ul>
<li><a href="#calculate-the-time-and-date-difference-between-two-date-fields-on-the-same-object" class="MCXref xref">Calculate the time and date difference between two date fields on the same object</a> </li>
<li><a href="#calculate-the-time-and-date-difference-between-the-field-on-an-object-and-another-field-on-the-parent-object" class="MCXref xref">Calculate the time and date difference between the field on an object and another field on the parent object</a> </li>
</ul>
<h4 id="calculate-the-time-and-date-difference-between-two-date-fields-on-the-same-object"><strong>Calculate the time and date difference between two date fields on the same object</strong> </h4>
<p>For example, to calculate the difference between the Planned Completion Date and the Actual Completion Date of a task add the following column to a task report:</p>
<pre>displayname=Planned-Actual Completion Date<br>linkedname=direct<br>querysort=plannedCompletionDate<br>textmode=true<br>valueexpression=ROUND(DATEDIFF({plannedCompletionDate},{actualCompletionDate}),2)<br>valueformat=HTML</pre>
<p>The result displays in days. The timestamp on the date field is also taken into account, and the number of days might be followed by decimals if the timestamps don't match.</p>
<h4 id="calculate-the-time-and-date-difference-between-the-field-on-an-object-and-another-field-on-the-parent-object"><strong>Calculate the time and date difference between the field on an object and another field on the parent object</strong> </h4>
<p>For a list of objects and their parents, see the "Understanding the Interdependency and Hierarchy of Objects" section in <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">Understand objects in Adobe Workfront</a>.<br>For example, you can calculate the difference between the Planned Completion Date of a task and the Planned Completion Date of its parent task, or of the project that the task is on.</p>
<ul>
<li>Add the following column to a task view or report to calculate the difference between the Planned Completion Date of the task and that of the parent task:<br><pre>valueexpression=ROUND(DATEDIFF({plannedCompletionDate},{parent}.{plannedCompletionDate}),2)<br>textmode=true<br>valueformat=HTML<br>displayname=Parent Planned Completion - Planned Completion</pre></li>
<li>Add the following column to a task view or report to calculate the difference between the Planned Completion Date of the task and that of the project:<br><pre>displayname=Project Planned Completion - Planned Completion<br>textmode=true<br>valueexpression=ROUND(DATEDIFF({plannedCompletionDate},{project}.{plannedCompletionDate}),2)<br>valueformat=HTML</pre></li>
</ul>
</div>
-->

## 在篩選中使用文字模式 {#use-text-mode-in-filters}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: replace all these links with the link to the actual articles; --- hide all the sections below)</p>
-->

當您建立篩選時，可以使用文字模式來展開可依其篩選的欄位和物件。

如需在篩選中使用文字模式的最常見原因範例，請參閱下列文章：

* [篩選器：建立參考相同欄位（「AND」陳述式）的多個篩選器規則](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/filter-refrence-the-same-field-multiple-times.md)
* [篩選器：僅顯示核准狀態的專案](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/filter-for-items-in-approval-status.md)
* [篩選器：當狀態與不同群組相關聯時，依相同名稱狀態顯示專案](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/filter-same-name-statuses-from-different-groups.md)
* [篩選器：比較兩個欄位來排除清單中的專案](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/filter-items-by-comparing-two-fields.md)
* 在發行項[使用EXISTS陳述式建立複雜文字模式篩選器](../../../reports-and-dashboards/reports/text-mode/create-complex-text-mode-filters-using-exists-statements.md)中，橫跨物件階層](../../../reports-and-dashboards/reports/text-mode/create-complex-text-mode-filters-using-exists-statements.md#examples)多個層級的文字模式篩選器範例[
* 區段[為發行項[使用EXISTS陳述式建立複雜文字模式篩選器](../../../reports-and-dashboards/reports/text-mode/create-complex-text-mode-filters-using-exists-statements.md)中的遺失物件建立複雜文字模式篩選器](../../../reports-and-dashboards/reports/text-mode/create-complex-text-mode-filters-using-exists-statements.md#missing-object-filters)

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>The most common reasons for using text mode in a filter are:</p>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: previous content that was drafted when it was replaced by standalone articles linked above) </p>
<ul>
<li> <p><a href="#create-multiple-filter-rules-that-reference-the-same-field" class="MCXref xref">Create multiple Filter Rules that reference the same field</a> </p> </li>
<li> <p><a href="#filter-for-items-in-an-approval-status" class="MCXref xref">Filter for items in an approval status</a> </p> </li>
<li> <p><a href="#filter-for-items-by-same-name-statuses-when-the-statuses-are-associated-with-different-groups" class="MCXref xref">Filter for items by same-name statuses when the statuses are associated with different groups</a> </p> </li>
<li> <p><a href="#filter-items-by-comparing-two-fields" class="MCXref xref">Filter items by comparing two fields</a> </p> </li>
<li> <p><a href="#create-complex-text-mode-filters-that-span-multiple-levels-in-the-object-hierarchy">Creating Complex Text-Mode Filters that Span Multiple Levels in the Object Hierarchy</a> </p> </li>
<li> <p><a href="#create-complex-text-mode-filters-for-missing-objects">Creating Complex Text-Mode Filters for Missing Objects</a> </p> </li>
</ul>
<p><strong>Create multiple Filter Rules that reference the same field</strong></p>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: replace content with a link to here: /Content/Reports and Dashboards/Reports/Custom View Filter Grouping Samples/filter-refrence-the-same-field-multiple-times.htm) </p>
<p>In the standard mode interface, when attempting to create multiple filters that reference the same field (using the AND qualifier), one of the filters is deleted when you save the report and exit the report builder.<br>For example, Workfront does not allow you to save the following filter rules using the standard mode interface:<br>Task Name > Contains > Green<br>Task Name > Does Not Contain > Red<br>However, you can create these filters using text mode:</p>
<pre>name=green<br>name_Mod=cicontains<br>AND:1:name=red<br>AND:1:name_Mod=cinotcontains</pre>
<p><strong>Filter for items in an approval status</strong></p>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: replace this with a link to this: /Content/Reports and Dashboards/Reports/Custom View Filter Grouping Samples/filter-for-items-in-approval-status.htm--- hide the content from here) </p>
<p>To display only items in a certain status which is currently in Pending Approval:</p>
<ol>
<li value="1">Go to the filter you want to customize for a list of projects, for example.<br>This works the same for any other object with an approval status.</li>
<li value="2">Add a<strong>Filter Rule</strong> for the <strong>Status</strong> field of the object of your list.<br>For example, in a project report, add <strong>Status Equal Planning</strong>, if you want to display only projects which are in a status of <strong>Planning - Pending Approval</strong>.</li>
<li value="3">Click <strong>Switch to Text Mode</strong>.</li>
<li value="4">Modify the <em>status</em> line by adding a <strong>:A</strong> to the three letter key of the status:<br><pre>status=PLN:A<br>status_Mod=in</pre></li>
<li value="5">Click <strong>Save Filter</strong>.<br>You can use the same steps to filter for all statuses of all objects that could be associated with an approval process.</li>
</ol>
<p><strong>Filter for items by same-name statuses when the statuses are associated with different groups</strong></p> 
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: link to this article: /Content/Reports and Dashboards/Reports/Custom View Filter Grouping Samples/filter-same-name-statuses-from-different-groups.htm) </p>
<p>You can have a task status assigned to Group A named <em>New Status</em> with the three-letter key <em>NST</em>. You may have another task status assigned to Group B also named <em>New Status</em> with the three-letter key <em>NES.</em> Although the names for the two statuses can be identical, the three letter code is always unique.<br>For more information about group statuses, see <a href="../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md" class="MCXref xref">Create or edit a group status</a>.<br>To distinguish between the two statuses in our example you can modify the text mode of the filter applied to a task list to ensure items in both statuses are identified:</p>
<ol>
<li value="1">Go to the filter you want to customize for a list of tasks, for example.<br>This works the same for projects and issues, as well.</li>
<li value="2">Add a<strong>Filter Rule</strong> for the <strong>Status</strong> field of the object of your list.<br>For example, in a task report, add <strong>Status Equal New Status</strong>, if you want to display only tasks which are in a status of <strong>New Status</strong>.<br>Notice that you have only one option for a status named New Status.</li>
<li value="3">Click <strong>Switch to Text Mode</strong>.<br>The following code should display:<br><pre xml:space="preserve">status=NST<br>status_Mod=in </pre><note type="note">
Only one status displays here. The status line displays one of the three-letter keys for one of the statuses.
</note></li>
<li value="4">Add the following two lines of code to add the status that is missing from the filter:<br><pre>status=NST<br>status_Mod=in<br>OR:1:status=NES<br>OR:1:status_Mod=in</pre></li>
<li value="5">Click <strong>Save Filter</strong>.</li>
</ol>
<p><strong>Filter items by comparing two fields</strong></p>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: replace this and hide, the new article is: /Content/Reports and Dashboards/Reports/Custom View Filter Grouping Samples/filter-items-by-comparing-two-fields.htm)</p>
<p>For example, you can display only tasks where the Actual Completion Date of the task is greater than the Planned Completion Date:</p>
<ol>
<li value="1">Go to the filter you want to customize on a task list, for example.</li>
<li value="2">Click <strong>Add Filter Rule</strong> for the <strong>Actual Completion Date</strong> field.</li>
<li value="3">Click <strong>Switch to Text Mode</strong>.</li>
<li value="4">Replace the text with the following code:<br><pre>actualCompletionDate=FIELD:plannedCompletionDate<br>actualCompletionDate_Mod=gt</pre></li>
<li value="5">Click <strong>Save Filter</strong>.</li>
</ol>
<p><strong>Create complex Text Mode filters that span multiple levels in the object hierarchy</strong></p>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina - links in this section and the following one are correct.)&nbsp;</p>
<p>Using EXISTS statements in the text mode interface, you can filter for objects that are removed from the filter object by more than two levels of hierarchy.</p>
<p>For information about filtering across multiple levels of object hierarchy, see the section <a href="../../../reports-and-dashboards/reports/text-mode/create-complex-text-mode-filters-using-exists-statements.md#examples" class="MCXref xref">Examples of text mode filters that span multiple levels in the object hierarchy</a> in the article <a href="../../../reports-and-dashboards/reports/text-mode/create-complex-text-mode-filters-using-exists-statements.md" class="MCXref xref">Create complex Text Mode filters using EXISTS statements</a>.</p>
<p><strong>Create complex Text Mode filters for missing objects</strong></p>
<p>Using EXISTS statements in the text mode interface, you can filter for objects that are missing. For example, you can display a list of users who did not log time in Workfront within a certain period of time or a list of custom fields that are not associated with any custom forms.</p>
<p>For information about filtering for missing objects, see the section <a href="../../../reports-and-dashboards/reports/text-mode/create-complex-text-mode-filters-using-exists-statements.md#missing-object-filters" class="MCXref xref">Create complex text mode filters for missing objects</a> in the article <a href="../../../reports-and-dashboards/reports/text-mode/create-complex-text-mode-filters-using-exists-statements.md" class="MCXref xref">Create complex Text Mode filters using EXISTS statements</a>.</p>
</div>
-->

## 在分組中使用文字模式 {#use-text-mode-in-groupings}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: replace all these links with the link to the actual articles; --- hide all the sections below)</p>
-->

建立群組時，您可以使用文字模式來展開您可在清單和報告中作為群組依據的欄位和物件。

如需在群組中使用文字模式最常見原因的範例，請參閱下列文章：

* [群組：依照群組中所有物件通用的計算值來組織清單結果](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/grouping-by-calculated-common-values.md)
* [群組：新增第四個群組至清單](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/grouping-add-fourth-grouping.md)
* [群組：編輯群組中的顯示名稱](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/grouping-rename-grouping.md)
* [群組：指出群組結果應使用文字模式收合或展開](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/grouping-collapsed-or-expanded-results.md)

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>The most common reasons for using text mode in a grouping are:</p> 
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: drafted this content when the standalone articles that replaced these sections were turned live) </p>
<ul>
<li><a href="#group-results-by-a-calculated-value-common-to-all-objects-in-the-grouping" class="MCXref xref">Group results by a calculated value common to all objects in the grouping</a> </li>
<li><a href="#add-a-fourth-grouping-in-a-standard-report" class="MCXref xref">Add a fourth grouping in a standard report</a> </li>
<li><a href="#rename-a-grouping" class="MCXref xref">Rename a Grouping</a> </li>
<li data-mc-conditions="QuicksilverOrClassic.Quicksilver"><a href="#indicate-whether-the-results-in-a-grouping-should-be-collapsed-or-expanded" class="MCXref xref">Indicate whether the results in a Grouping should be collapsed or expanded</a> </li>
</ul>
<p><strong>Group results by a calculated value common to all objects in the grouping</strong></p> 
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: hide this and see this article instead: /Content/Reports and Dashboards/Reports/Custom View Filter Grouping Samples/grouping-by-calculated-common-values.htm) </p>
<p>For example, you might want to view your tasks grouped by Percent Complete in ranges of 0-25, 26-50, 51-75, 75-99, and 100. Doing so would require using text mode for your grouping.<br>The grouping that you want to use for this example is:</p> 
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;Alina: this should wrap within the page margins)</p>
<pre>textmode=true<br>group.0.valueexpression=IF({percentComplete}>=0&&{percentComplete}<=25,'0-25%',IF({percentComplete}>25&&{percentComplete}<=50,'26-50%',IF({percentComplete}>50&&{percentComplete}<=75,'51-75%',IF({percentComplete}>75&&{percentComplete}<=100,'76-100%',''))))<br>group.0.linkedname=direct<br>group.0.valueformat=doubleAsString<br>group.0.namekey=percentComplete</pre>
<p><strong>Add a fourth grouping in a standard report</strong></p>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: hide and replace this with: /Content/Reports and Dashboards/Reports/Custom View Filter Grouping Samples/grouping-add-fourth-grouping.htm)&nbsp;</p>
<p>You can have four groupings in a matrix report. For more information about matrix reports, see <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md" class="MCXref xref">Create a matrix report</a>.<br>You can only have three groupings in a standard report through the standard interface. To add a fourth grouping in a standard report, you must use text mode.<br><img src="assets/four-groupings-in-a-standard-report-350x59.png" alt="Four_groupings_in_a_standard_report.png" style="width: 350;height: 59;"><br>For example, you have a task report which is grouped by Project Name, Progress Status and Planned Completion Date. You want to add a fourth grouping, for Assigned To Name. You can do that, with the following code inside your grouping builder:</p>
<pre>group.0.linkedname=project<br>group.0.namekey=view.relatedcolumn<br>group.0.namekeyargkey.0=project<br>group.0.namekeyargkey.1=name<br>group.0.valuefield=project:name<br>group.0.valueformat=string<br>group.1.enumclass=com.attask.common.constants.ProgressStatusEnum<br>group.1.enumtype=TASK<br>group.1.linkedname=direct<br>group.1.namekey=progressStatus<br>group.1.type=enum<br>group.1.valuefield=progressStatus<br>group.1.valueformat=val<br>group.2.groupdatesby=WY<br>group.2.linkedname=direct<br>group.2.namekey=plannedCompletionDate<br>group.2.notime=false<br>group.2.valuefield=plannedCompletionDate<br>group.2.valueformat=atDateAsWeekString<br>group.3.valuefield=assignedTo:name<br>group.3.valueformat=HTML<br>textmode=true</pre>
<p><strong>Rename a Grouping</strong></p>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: hide here and this is the new article: /Content/Reports and Dashboards/Reports/Custom View Filter Grouping Samples/grouping-rename-grouping.htm) </p>
<p>You can rename groupings to something more familiar to your users. To do that, you can do one of the following in a grouping:</p>
<ol>
<li value="1">When customizing a grouping, click <strong>Switch to Text Mode</strong>.</li>
<li value="2">Remove all the lines in the text mode interface of the grouping that have the word "name" in them, then add the line: <pre>group.0.name=Your Value</pre> You can also leave the <code>group.0.name</code> line blank, in which case the grouping shows the name of the value you are grouping by.<br>Or</li>
<li value="3">Add the following line to the existing text mode code in a Grouping:<br><pre>group.0.displayname=Your Value</pre>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: maybe add a screen shot here?) </p>
</li>
</ol>
<div data-mc-conditions="QuicksilverOrClassic.Quicksilver">
<p><strong>Indicate whether the results in a Grouping should be collapsed or expanded</strong></p>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: hide this and its own article: /Content/Reports and Dashboards/Reports/Custom View Filter Grouping Samples/grouping-collapsed-or-expanded-results.htm) </p>
<p>You can indicate whether the results in a grouping should display collapsed or expanded in a list or report. The results in a grouping display expanded, by default. For information about creating a grouping, see <a href="../../../reports-and-dashboards/reports/reporting-elements/create-groupings.md" class="MCXref xref">Create groupings in Adobe Workfront</a>.</p>
<ol>
<li value="1">When customizing a grouping, click <strong>Switch to Text Mode</strong>.</li>
<li value="2"> <p>Add the code for your custom grouping, then add the following line for a first-level grouping:</p> <p><code>group.0.iscollapsed=true</code> to display the grouping collapsed</p> <p>Or</p> <p><code>group.0.iscollapsed=false</code> to display the grouping expanded.</p> </li>
<li value="3"> <p>Click <strong>Done</strong>, then <strong>Save Grouping</strong> when you modify the grouping in a list.</p> <p>Or </p> <p>Click <strong>Done</strong>, then <strong>Save + Close</strong> when you modify the grouping in a report.</p> </li>
</ol> <note type="tip">  
<ul>
<li>When you manually adjust groupings when viewing a list, Workfront remembers your manual preference until you log out. When you log back in, the list displays according to this setting.</li>
<li>The results of a grouping always display expanded after accessing them from a chart element.
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
(NOTE: the tips repeat in the Create groupings to organize results article, Understanding text mode, Edit groupings to organize reports, Create a Custom Report)
</MadCap:conditionalText>
</li>
</ul>
</note>
</div>
</div>
-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Examples of views, filters, and groupings built in text mode</h2>
<p>You can use the text mode of complex views, filters and groupings which have been built by Workfront.</p>
<p>For more examples of already built text mode views, groupings and filters, see <a href="../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md" class="MCXref xref">Custom View, Filter, and Grouping samples</a>.</p>
</div>
-->
