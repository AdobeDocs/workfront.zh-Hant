---
product-area: reporting
navigation-topic: text-mode-reporting
title: 文本模式概述
description: 文本模式概述
author: Nolan
feature: Reports and Dashboards
exl-id: 8be8cbd0-da1b-4e90-a52e-dc352f646d18
source-git-commit: 888c938e5d649557df69374a55d4e4ecc2da6f55
workflow-type: tm+mt
source-wordcount: '925'
ht-degree: 0%

---

# 文本模式概述

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Linked to the UI (for the areas mentioned in the comments below and the new NWE filters as well))</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: ***Linked to other articles. Do not move, rename or change url.Linked to the product, in the report builder, when using a field that is not recognized in standard mode.)</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: This will be linked to the Ninja feature about adding a filter to the User typeahead field (which originally is open only for text mode filters). Update the Context Sensitive sheet at release time) </p>
-->

在建立構成報表或清單的元素時，可使用標準或文本模式介面在Adobe Workfront建立報表或清單。 標準介面允許您引用在Workfront介面中隨時可用的欄位及其屬性。 使用文本模式，可以引用在標準模式下可能不可用但在Workfront資料庫中可用的欄位和屬性。

## 使用文本模式前的注意事項

>[!TIP]
>
>您還可以使用自定義欄位的文本模式版本來擴展計算的自定義欄位的功能。 用於建立計算的自定義欄位的語法和規則與在報表和清單中使用的語法和規則不同。 有關添加計算的自定義欄位的資訊，請參見 [將計算資料添加到自定義窗體](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)。

* 在您開始在報告中使用文本模式之前，我們強烈建議您學習我們有關高級報告的課程，以便更深入地瞭解我們的文本模式語言。 <!--outdated: For training materials on reporting see [Workfront Reports and Dashboards Learning Paths](https://one.workfront.com/s/learningpath2/workfront-reporting-20Y0z000000blhLEAQ).-->
* 我們建議您使用標準模式，確保在更新Workfront軟體時建立的報告保持不變。 雖然文本模式使您能夠建立更複雜的視圖、篩選器和分組，但維護也更複雜，在更新Workfront軟體時不保證。
* 我們建議您始終嘗試在標準介面中構建所有報告元素，並只對少量調整切換到文本模式生成器。

   >[!TIP]
   >
   >使用標準生成器可為您提供重要的代碼構造塊和模式，然後在文本模式下修改代碼時可以使用這些模組和模式。

* 有一組規則和唯一語法必須使用，才能在文本模式下成功生成報告和清單。 在開始之前，請確保您熟悉文本模式的Workfront語法。

   有關使用文本模式的語法和規則的資訊，請參見 [文本模式語法概述](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md)。

* 在文本模式下自定義報表元素後，可能無法切換回標準模式（在視圖中），或者您建立的元素的代碼可能被刪除（在篩選器和分組中）。 這是因為並非所有在文本模式下支援的欄位都在標準模式下受支援。

## 標準模式介面

「標準模式」介面顯示欄位以映射要在報表或清單中顯示的應用程式元素。 標準模式介面是一組下拉菜單，您可以從中選擇要在報表或清單中顯示的欄位。

有關標準模式介面和瞭解如何建立報表或清單的詳細資訊，請參閱：

* [建立自定義報告](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)。
* [報告元素：篩選器、視圖和分組](../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md)

## 文本模式介面

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: add a section or note with a link to an another article about the syntax of text mode >> link to the Calc custom fields vc calc. columns)</p>
-->

文本模式允許您使用標準模式介面中不可用的欄位，從而建立更複雜的視圖、篩選器、分組和提示。 在Workfront文本模式中，是編碼語句的集合，這些語句指示要在報表或清單中顯示的對象。

有關所有可報告欄位的完整清單，請參閱 [API資源管理器](../../../wf-api/general/api-explorer.md)。

>[!NOTE]
>
>並非所有通過API可用的欄位都通過文本模式介面可用。 如果您在文本模式代碼中使用了正確的欄位，並且未顯示預期的結果，則該欄位可能只能通過API報告。

* [訪問報告元素並編輯文本模式](#access-reporting-elements-and-edit-text-mode)
* [使用文本模式的常見原因](#common-reasons-to-use-text-mode)

## 訪問報告元素並編輯文本模式 {#access-reporting-elements-and-edit-text-mode}

在從報表或清單訪問視圖、分組和篩選器時，訪問文本模式介面與訪問它們類似。

有關在視圖、篩選器和分組中使用文本模式的資訊，請參閱：

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: see what articles these sections are linked to and edit those articles to link to the individual ones)</p>
-->

* [使用文本模式編輯視圖](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-view.md)
* [使用文本模式編輯篩選器](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md)
* [編輯分組中的文本模式](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-grouping.md)

只能在文本模式下編輯自定義提示。 您只能從報表訪問提示。

有關訪問自定義提示的文本模式介面的資訊，請參見 [向報表添加提示](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)。

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Editing the text mode code inside views, filters, and groupings has some differences outlined below.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: everything below, and the four subsections >>> drafted and created individual articles.)</p>
-->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#edit-text-mode-in-a-view" class="MCXref xref">Edit text mode in a view</a> </li>
  -->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#edit-text-mode-in-a-filter" class="MCXref xref">Edit text mode in a filter</a> </li>
  -->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#edit-text-mode-in-a-grouping" class="MCXref xref">Edit text mode in a grouping</a> </li>
  -->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#edit-a-custom-prompt" class="MCXref xref">Edit a custom prompt</a> </li>
  -->

<!--
<h4 data-mc-conditions="QuicksilverOrClassic.Draft mode" id="edit-text-mode-in-a-view"><strong>Edit text mode in a view</strong> </h4>
-->

<!--
<note type="tip">
We recommend that you build as much of the view as possible in standard mode, then convert it to text mode to edit it.
</note>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">To access the text mode interface for a view:</p>
-->

<!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Find the report you want to modify in text mode.</p>
   -->

<!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must have manage permissions to a report in order to be able to edit it.</p>
   -->

<!--
   <li value="2" data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <strong>Report Actions</strong>. </li>
   -->

<!--
   <li value="3" data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <strong>Edit</strong>.</li>
   -->

<!--
   <li value="4" data-mc-conditions="QuicksilverOrClassic.Draft mode">On the <strong>Columns (View)</strong> tab of the report builder, select a column in the report.</li>
   -->

<!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <strong>Apply</strong> if you want to save your changes and continue editing the report.</p>
   -->

<!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <strong>Save + Close</strong> to save your report.</p>
   -->

<!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <strong>Switch to Text Mode</strong> in the upper-right corner of the report builder.</p>
   -->

<!--
   <note type="note">
   When you edit a column in text mode, Workfront adds the
   <code>textmode=true</code> line of code to the column. This indicates that the column is modified in text mode.
   </note>
   -->

<!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">The following table outlines the key lines in a text mode view or grouping:</p>
   -->

<!--
   <table style="table-layout:auto">
   <col>
   <col>
   <thead>
   <tr>
   <th data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Sample Line</strong> </th>
   <th data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Description</strong> </th>
   </tr>
   </thead>
   <tbody>
   <tr>
   <td>
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>valuefield</strong>=</p>
   </td>
   <td>
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">This is the name of the object or of the field as it appears in the database. For more information about how objects and fields appear in the database, see <a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">API Explorer</a>.</p>
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">The following scenarios exist:</p>
   <ol>
   <li value="1" data-mc-conditions="QuicksilverOrClassic.Draft mode"> If the name of the field you display is a phrase instead of a single noun, you must use camel case syntax for the <code>valuefield</code>. For example, for the Planned Start Date of a task the code is: <code>valuefield=plannedStartDate</code></li>
   <li value="2">
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">If you want to display a custom field, the <code>valuefield</code> value is the actual name of the field, as you see it in the interface. For example, for a custom field named "More information", the code is:</p>
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode"><code>valuefield=More information</code> </p>
   </li>
   <li value="3">
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">If you want to display objects that are related to other objects in a view using the <code>valuefield</code> line of code the object names and attributes are separated by colons. </p>
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For example, a column in a task view that would display the name of the Portfolio Owner has the following value for the valuefield line:</p>
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode"><code>valuefield=project:portfolio:owner:name</code> </p>
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">This indicates that from the object of the report (task), you can access the next related object (project), from there, you can access the following related object from project (portfolio), then the portfolio owner (owner) and then their name (name). </p>
   </li>
   </ol>
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For information about how objects connect to one another, see the section <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-interdependency-and-hierarchy-of-objects" class="MCXref xref">Interdependency and hierarchy of objects</a> in <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">Understand objects in Adobe Workfront</a>.</p>
   <note type="note">
   If you choose a field in text mode that is not valid in the standard interface, you are not able to switch back to the standard interface within the column.
   </note>
   </td>
   </tr>
   <tr>
   <td data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>valueformat=</strong> </td>
   <td>
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">This line represents the format used to display the <code>valuefield</code>. The <code>valueformat</code> identifies whether an object or field displays as text, number, percentage, or date.</p>
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">We recommend using <code>HTML</code> for your <code>valueformat</code>, especially when using <code>valueexpression</code>, to ensure the most accurate display of your information. </p>
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For information about additional values for this line, see <a href="../../../reports-and-dashboards/reports/text-mode/use-conditional-formatting-text-mode.md" class="MCXref xref">Use conditional formatting in Text Mode</a>.</p>
   </td>
   </tr>
   <tr>
   <td>
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>valueexpression=</strong> </p>
   </td>
   <td>
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can add this line to replace <code>valuefield</code>, if you want to display a calculated field in the column.</p>
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must enclose the <code>valuefield</code> of the objects in curly brackets every time you use it in a <code>valueexpression</code>.</p>
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">The following scenarios exist: </p>
   <ol>
   <li value="1">
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">If you want to display a field in a column in upper case, you would use:</p>
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode"><code>valueexpression=UPPER({valuefield})</code> </p>
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">The <code>valuefield</code> of the object is spelled as it appears in the API Explorer. </p>
   </li>
   <li value="2" data-mc-conditions="QuicksilverOrClassic.Draft mode">If you want to add multiple <code>valuefields</code> by stringing them together, you must separate them by a period.</li>
   <li value="3">
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For example, if you want to display the name of the Primary Assignee of a task using <code>valueexpression</code>, you would use:</p>
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode"><code>valueexpreesion={assignedTo}.{name}</code> </p>
   </li>
   <li value="4">
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">If you want to use a custom field in a <code>valueexpression</code> line you must precede the name of the field by <code>DE:</code> to indicate that it is a custom field. The name of the field is spelled as it appears in the interface. </p>
   <note type="important">
   <span>When you use a custom field that is placed in a custom form section that has restricted permissions for some users, the calculation of the valueexpression is blank when those users view this calculation in a report. For information about adjusting permissions on custom form sections, see</span>
   <span href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md"><a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">Create or edit a custom form</a></span>.
   </note>
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For example, if you have a custom field labeled "Developer Name" and you want to display this field in upper case in a column, you can use the following <code>valueexpression</code> to indicate this:</p>
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode"><code>valueexpression=UPPER({DE:Developer Name}</code>) </p>
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">When referencing a Typeahead type custom field, use the following expression to reference the name of the object selected in a field labeled "Developer Name":</p>
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode"><code>valueexpression=UPPER({DE:Developer Name:name})</code> </p>
   </li>
   </ol> </td>
   </tr>
   <tr>
   <td>
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>descriptionkey= / description=</strong> </p>
   </td>
   <td data-mc-conditions="QuicksilverOrClassic.Draft mode">This line defines the text of a tool tip as you mouse over the name of the column. In this case it is using a key to translate the name value in the description text. If you want to modify the description, change this line to read: <code>description=Your Value</code>.</td>
   </tr>
   <tr>
   <td data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>namekey= / name=</strong> </td>
   <td>
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">This line defines the column label. In this case it is using the abbreviated value based on the key.</p>
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">If you want to modify the column name you can change this value to: <code>name=Your Value</code></p>
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode"><code>Name</code> allows you to enter any text for the column name, while<code>namekey</code> requires you enter a key that is used to translate the name of a column.</p>
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">To change the column name you can also add the <code>displayname </code>line, if one is not present.</p>
   </td>
   </tr>
   <tr>
   <td data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>displayname =</strong> </td>
   <td>
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can add the following line to change the name of a column, which suspends the <code>namekey/name</code> value:</p>
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode"><code>displayname=Your Value</code> </p>
   </td>
   </tr>
   <tr>
   <td data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>querysort=</strong> </td>
   <td data-mc-conditions="QuicksilverOrClassic.Draft mode">This line defines how the results are sorted when the column header is clicked. If it is not present then the column cannot be sorted after the report is run.</td>
   </tr>
   <tr>
   <td data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>width=</strong> </td>
   <td>
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">This line represents the number of pixels that are used for the column. If the line is omitted or set to 0 (zero) then the column does not appear in the view.</p>
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">When you modify this field manually in text mode, you must also add the <code>usewidths=true</code> value to your column.</p>
   </td>
   </tr>
   <tr>
   <td data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>usewidths=true</strong> </td>
   <td>
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must use this line in addition to the <code>width=</code> line when customizing the width of a column. </p>
   </td>
   </tr>
   <tr>
   <td data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>makeFieldEditable=</strong> </td>
   <td>
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">This line defines whether the value displayed in a column is inline editable or not. If this line equals <strong>true,</strong> the value in the column is inline editable. If this line equals <code>false</code>, the value in the column is not inline editable.</p>
   </td>
   </tr>
   <tr>
   <td data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>link.valuefield=</strong> </td>
   <td>
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Insert this line only when you want the value displayed in a column to link to the object associated with it. The link opens the details page of the object. This value should match the <code>valuefield=</code> line. When you insert this, you must also add the <code>link.valueformat=</code> line. </p>
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode"> For example, you can insert link.valuefield=priority in an issue view, and the Priority of the issue displays as a link. Clicking this link opens the Issue page.</p>
   --> </td>
</tr>
   <tr> <!--
   <td data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>link.valueformat=</strong> </td>
<td>
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Insert this line only when you have inserted the <code>link.valuefield</code> line to add a link to the value in a column. The link opens the details page of the object. This value should match the <code>valueformat=</code> line and indicates the format used to display the <code>valuefield</code>. </p>
   <note type="important">
   When viewing the text mode in a built-in column that also includes a link, you notice a number of lines referring to the link. Some of those lines might no longer be supported or are unnecessary when you create your own custom column in text mode and add the link statements to it. The lines that are mandatory when adding a linked value are
   <code> link.valuefield</code> and
   <code>link.valueformat</code>.
   </note>
   </td>
   </tr>
   </tbody>
   </table>
   -->

<!--
   <li value="8" data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <strong>Apply</strong> if you want to save your changes and continue editing the report.</li>
   -->

<!--
   <li value="9" data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <strong>Save + Close</strong> to save your report.</li>
   -->

<!--
<h4 data-mc-conditions="QuicksilverOrClassic.Draft mode" id="edit-text-mode-in-a-filter"><strong>Edit text mode in a filter</strong> </h4>
-->

<!--
<note type="tip">
We recommend that you build as much of the filter of the report as possible in standard mode, then convert the filter to text mode to edit it.
</note>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">For more information about building filters, see <a href="../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md" class="MCXref xref">Filters overview in Adobe Workfront</a>.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">To access the text mode interface for a filter:</p>
-->

<!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Find the report you want to modify in text mode.</p>
   -->

<!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must have manage permissions to a report in order to be able to edit it.</p>
   -->

<!--
   <li value="2" data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <strong>Report Actions</strong>.</li>
   -->

<!--
   <li value="3" data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <strong>Edit</strong>.</li>
   -->

<!--
   <li value="4" data-mc-conditions="QuicksilverOrClassic.Draft mode">On the <strong>Filters</strong> tab of the report, choose either <strong>Apply Existing Filter</strong>, or <strong>Add a Filter Rule.</strong></li>
   -->

<!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Define the conditions of your filter.</p>
   -->

<!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Use the filter modifiers to define the condition of your filter. For more information about filter modifiers, see <a href="../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md" class="MCXref xref">Filter and condition modifiers</a>.</p>
   -->

<!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <strong>Switch to Text Mode</strong> in the upper-right corner of the report builder.</p>
   -->

<!--
   <li value="7" data-mc-conditions="QuicksilverOrClassic.Draft mode">When using filter modifiers that are available only in text mode, remember that for each filter condition you have two lines of code: one defines the condition and the second one defines the modifier of the filter.</li>
   -->

<!--
   <li value="8" data-mc-conditions="QuicksilverOrClassic.Draft mode">For example, if you want to filter for users who are in the same Home Group but not in the same Home Team as the logged in user, your filter should look like the following, in text mode:</li>
   -->

<!--
   <pre data-mc-conditions="QuicksilverOrClassic.Draft mode">homeGroupID=$$USER.homeGroupID</pre>
   -->

<!--
   <pre data-mc-conditions="QuicksilverOrClassic.Draft mode">homeGroupID_Mod=in</pre>
   -->

<!--
   <pre data-mc-conditions="QuicksilverOrClassic.Draft mode">homeTeamID=$$USER.homeTeamID</pre>
   -->

<!--
   <pre data-mc-conditions="QuicksilverOrClassic.Draft mode">homeTeamID_Mod=notin</pre>
   -->

<!--
   <li value="13" data-mc-conditions="QuicksilverOrClassic.Draft mode">For a complete list of filter modifiers in text mode, see the article <a href="../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md" class="MCXref xref">Filter and condition modifiers</a>.</li>
   -->

<!--
   <li value="14" data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <strong>Apply</strong> if you want to save your changes and continue editing the report.</li>
   -->

<!--
   <li value="15" data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <strong>Save + Close</strong> to save your report.</li>
   -->

<!--
<h4 data-mc-conditions="QuicksilverOrClassic.Draft mode" id="edit-text-mode-in-a-grouping"><strong>Edit text mode in a grouping</strong> </h4>
-->

<!--
<note type="tip">
We recommend that you build as much of the grouping as possible in standard mode, then convert it to text mode to edit it.
</note>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">To access the text mode interface for a grouping:</p>
-->

<!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Find the report you want to modify in text mode.</p>
   -->

<!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must have manage permissions to a report in order to be able to edit it.</p>
   -->

<!--
   <li value="2" data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <strong>Report Actions</strong>.</li>
   -->

<!--
   <li value="3" data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <strong>Edit</strong>.</li>
   -->

<!--
   <li value="4" data-mc-conditions="QuicksilverOrClassic.Draft mode">On the <strong>Groupings</strong> tab of the report builder, choose either <strong>Apply Existing Grouping</strong>, or <strong>Add Grouping.</strong></li>
   -->

<!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Start typing the name of a field that you want to group by.</p>
   -->

<!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Select the name of the field when you see it in the list.</p>
   -->

<!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode"> Click <strong>Switch to Text Mode</strong> in the upper-right corner of the report builder.</p>
   -->

<!--
   <note type="note">
   When you edit a grouping in text mode, Workfront adds the
   <code>textmode=true</code> line of code to the grouping. This indicates that the grouping is modified in text mode.
   </note>
   -->

<!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/grouping-switch-to-text-mode-350x173.png" alt="grouping_switch_to_text_mode.png" style="width: 350;height: 173;"> </p>
   -->

<!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">The grouping is then displayed in text mode. </p>
   -->

<!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For example, if you want to group a list of tasks by the Project Name and then by the name of the Primary Assignee, your grouping should look like the following, in text mode: </p>
   -->

<!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode"><code>textmode=true</code> </p>
   -->

<!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode"><code>group.0.linkedname=project</code> </p>
   -->

<!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode"><code>group.0.namekey=view.relatedcolumn</code> </p>
   -->

<!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode"><code>group.0.valuefield=project:name</code> </p>
   -->

<!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode"><code>group.0.namekeyargkey.0=project</code> </p>
   -->

<!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode"><code>group.0.namekeyargkey.1=name</code> </p>
   -->

<!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode"><code>group.0.valueformat=string</code> </p>
   -->

<!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode"><code>group.1.linkedname=assignedTo</code> </p>
   -->

<!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode"><code>group.1.namekey=view.relatedcolumn</code> </p>
   -->

<!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode"><code>group.1.valuefield=assignedTo:name</code> </p>
   -->

<!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode"><code>group.1.namekeyargkey.0=assignedTo</code> </p>
   -->

<!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode"><code>group.1.namekeyargkey.1=nam</code>e</p>
   -->

<!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode"><code>group.1.valueformat=string</code> </p>
   -->

<!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Each field in the grouping has several lines of code that refer to that field. </p>
   -->

<!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">The lines of code that refer to the same field selected in the grouping are numbered with the same number, as follows:</p>
   -->

    &lt;!—
    &lt;li data-mc-conditions=&quot;QuicksilverOrClassic.Draft mode&quot;>報告的第一個分組的組編號為0。 引用第一個分組的所有行以group.0開頭。&lt;/code>&lt;/li>
    —>
    
    &lt;!>—
    &lt;li data-mc-conditions=&quot;QuicksilverOrClassic.Draft mode&quot;>報告的第二組具有組編號1。 引用第二個分組的所有行以&lt;code>group.1開頭&lt;/code>。&lt;/em>&lt;/li>
    —>
    
    &lt;!>—
    &lt;li data-mc-conditions=&quot;QuicksilverOrClassic.Draft mode&quot;>報告的第三組具有組編號2。 引用第三個分組的所有行以&lt;code>group.2開頭&lt;/code>。&lt;/em>&lt;/li>
    —>
    
    &lt;!>—
    &lt;li data-mc-conditions=&quot;QuicksilverOrClassic.Draft mode&quot;>只有在文本模式下，您才能為第四個分組添加組編號3。 引用第四個分組的所有行以&lt;code>group.3開頭&lt;/code>。&lt;/em>&lt;/li>
    —>

<!--
   <note type="note">
   Four groupings are not supported in the report builder. They are only supported when using text mode. Workfront does not support more than four levels of groupings.
   </note>
   -->

<!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">The key lines in a text mode grouping are similar to the fields available in views. The only lines that are not found in a grouping but are found in a view are <code>width</code> and <code>makeFieldEditable</code>. </p>
   -->

<!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For more information about the key lines in text mode in a view or grouping, see the section <a href="#edit-text-mode-in-a-view" class="MCXref xref">Edit text mode in a view</a> in this article. </p>
   -->

<!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(Optional) Add one of the following lines of code to any grouping to indicate whether the results in the grouping should display in an expanded or collapsed list. By default, groupings display expanded:</p>
   -->

<!--   
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><code>group.0.iscollapsed=true </code>if you want the grouping to display with the results collapsed</li>   
   -->

<!--   
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode"><code>group.0.iscollapsed=false</code> if you want the grouping to display with the results expanded</p>   
   -->

<!--   
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: the tips repeat in the Create groupings to organize results article, Common uses of text mode, Edit groupings to organize reports, Create a Custom Report)</p>   
   -->

>[!TIP]
>
>當您在查看清單時手動調整分組時，Workfront會記住您的手動首選項，直到您註銷。 當您重新登錄時，會根據此設定顯示清單。
>
>從圖表元素訪問分組結果後，始終顯示已展開的分組結果。

<!--
   <li value="8" data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <strong>Apply</strong> if you want to save your changes and continue editing the report.</li>
   -->

<!--
   <li value="9" data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <strong>Save + Close</strong> to save your report.</li>
   -->

<!--
<h4 data-mc-conditions="QuicksilverOrClassic.Draft mode" id="edit-a-custom-prompt">Edit a custom prompt</h4>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Custom prompts can only be edited in text mode. </p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">For more information about creating a custom prompt, see <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md" class="MCXref xref">Add a prompt to a report</a>.</p>
-->

## 使用文本模式的常見原因 {#common-reasons-to-use-text-mode}

除了建立只能使用文本模式配置的自定義提示外，我們建議您使用報表生成器來構建視圖、篩選器和分組。 但是，有些實例可以使用文本模式來增強報告和清單。

有關文本模式的常用用途的詳細資訊，請參見 [文本模式常用概述](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md)。
