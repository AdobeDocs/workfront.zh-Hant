---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 按多選自定義欄位對報表進行分組
description: 您可以按Adobe Workfront報告中多選自定義欄位中的值進行分組。 多選自定義欄位的示例有 — EDIT ME。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 530dff59-0d4c-490e-b464-1d3bb1d0f36f
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '485'
ht-degree: 0%

---

# 按多選自定義欄位對報表進行分組

您可以按Adobe Workfront報告中多選自定義欄位中的值進行分組。 多選自定義欄位的示例有：

* 核取方塊
* 多選下拉菜單

只能使用文本模式按此類型的欄位進行分組。 有關使用文本模式的資訊，請參閱文章 [文本模式概述](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md)。

>[!NOTE]
>
>不能通過多選自定義欄位繪製報表圖表。 您需要建立引用多選自定義欄位的附加計算欄位，以便還按多選自定義欄位的值繪製報表圖表。 有關詳細資訊，請參見 [按多選自定義欄位繪製報表圖表](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/chart-report-by-multi-select-custom-field.md)。

## 訪問要求

您必須具有以下訪問權限才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront許可證*</td> 
   <td> <p>請求修改分組 </p>
   <p>計畫修改報表</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>編輯對報表、儀表板、日曆的訪問以修改報表</p> <p>編輯對篩選器、視圖、分組的訪問以修改分組</p> <p><b>附註</b>

如果您仍然沒有訪問權限，請詢問您的Workfront管理員是否在您的訪問級別設定了其他限制。 有關Workfront管理員如何修改您的訪問級別的資訊，請參見 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自定義訪問級別</a>。</p> </td>
</tr>  
  <tr> 
   <td role="rowheader">對象權限</td> 
   <td> <p>管理對報表的權限</p> <p>有關請求附加訪問的資訊，請參見 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求訪問對象 </a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要瞭解您擁有的計畫、許可證類型或訪問權限，請與您的Workfront管理員聯繫。

## 按多選自定義欄位對報表進行分組

若要能夠按多選自定義欄位進行分組，必須具備以下先決條件：

* 以自定義表單構建多選自定義欄位。\
   有關構建自定義表單和向其添加自定義欄位的資訊，請參閱文章 [建立或編輯自定義表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md)。

* 將自定義窗體附加到對象。
* 使用每個對象上的值填充多選自定義欄位。 

要按報表中的多選自定義欄位分組：

1. 建立報告或編輯要為多選自定義欄位添加分組的現有報告。\
   有關建立報告的資訊，請參閱文章 [建立自定義報告](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)。

1. 選擇 **分組** 頁籤。
1. 按一下 **切換到文本模式**。

1. 選擇 **將報告分組** 框，並用以下代碼替換它：

   <pre>group.0.displayname=多選自定義欄位名<br>group.0.valueexpression={DE：多選自定義欄位名稱}<br>group.0.valueformat=HTML<br>textmode=true</pre>

1. 將「多選自定義欄位名稱」替換為多選自定義欄位的實際名稱，如在Workfront中顯示的那樣。  
1. 按一下 **保存並關閉**。\
   報告中的對象按多選自定義欄位的值分組。\
   報告分組的名稱是多選自定義欄位的名稱，後跟欄位中選定的值。 

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Chart a report by multi-select Custom Fields</h2>
<p>(NOTE: this moved to its own article, linked in the Note above!)</p>
<p>You cannot build a chart in a report by referencing a multi-select custom field. Instead, you can create a calculated field that records the values of the multi-select custom field on a given object and group by the calculated field.&nbsp;</p>
<ul>
<li><a href="#build-a-calculated-custom-field-that-references-a-multi-select-custom-field" class="MCXref xref">Build a calculated custom field that references a multi-select custom field</a> </li>
<li><a href="#build-a-chart-that-references-a-calculated-custom-field" class="MCXref xref">Build a chart that references a calculated custom field</a> </li>
</ul>
<p><strong>Build a calculated custom field that references a multi-select custom field</strong></p>
<p>To be able to build a calculated field that references a multi-select custom field, you must have the following prerequisites:</p>
<ul>
<li>Build the multi-select custom field in a custom form.<br>For information about building custom forms and adding custom fields to them, see the article <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">Create or edit a custom form</a>.</li>
<li>Attach the custom form to objects.</li>
<li>Populate the multi-select custom field with a value on each object.</li>
</ul>
<p>To build the calculated custom field that references the multi-select custom field:</p>
<ol>
<li value="1">Create a custom form, or edit an existing one.<br>For information about creating custom forms, see the article <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">Create or edit a custom form</a>.</li>
<li value="2">Click<strong>Add a Field</strong>, then <strong>Calculated</strong> to add the multi-select custom field to the form.</li>
<li value="3">In the <strong>Label</strong> box, name the new calculated field to indicate that it references the multi-select custom field.<br>For example: "Calculated Multi-select Field."</li>
<li value="4"> <p>In the <strong>Calculation</strong> box, enter the following code:</p><pre>{DE:Multi-select Custom Field}</pre> <p> <img src="assets/calculated-multi-select-custom-field-350x201.png" style="width: 350;height: 201;"> <br> </p> </li>
<li value="5">Replace "Multi-select Custom Field" with the actual name of your multi-select custom field, as it appears in Workfront.</li>
<li value="6"> <p>(Optional) If the multi-select custom field is already on this form and if this form is already attached to objects, enable the <strong>Update previous calculations</strong>&nbsp;option.</p> <p>This ensures that the new field is automatically populated with the value from the multi-select custom field as it is added to the forms attached to the objects already.</p> </li>
<li value="7">Click <strong>Done</strong>.</li>
<li value="8">Click <strong>Save +Close</strong>.</li>
</ol>
<p><strong>Build a chart that references a calculated custom field</strong></p>
<ol>
<li value="1"> Go to the report where you want to add the chart for the calculated field that references the multi-select custom field. </li>
<li value="2"> (Optional) To ensure that all the calculated fields that you want to chart by are populated with values, select all the objects in your report, then click <strong>Edit</strong>. </li>
<li value="3"> <p> (Optional and conditional) Enable the <strong>Recalculate Custom Expressions</strong> field, then click <strong>Save Changes</strong>.</p> <p> <img src="assets/recalculate-custom-expressions-350x259.png" style="width: 350;height: 259;"> <br> </p> </li>
<li value="4"> Click <strong>Report Actions</strong>, then <strong>Edit</strong>. </li>
<li value="5">Select the <strong>Groupings</strong> tab, then click <strong>Add Grouping</strong>. </li>
<li value="6">Add the<strong>Calculated Multi-select Field</strong> you created as your grouping. </li>
<li value="7"> <p>Select the <strong>Chart</strong> tab, and add a chart to your report.</p> <p>For information about adding a chart to a report, see the section <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md#add-a-chart" class="MCXref xref">Add a chart to a report</a> in the article <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Create a custom report</a>. </p> </li>
<li value="8">Select the <strong>Calculated Multi-select Field</strong> as one of the fields to display in the chart. </li>
<li value="9"> <p>Click <strong>Save + Close</strong>.</p> <p>The report displays the results grouped by the Calculated Multi-select Field in a chart. </p> </li>
</ol>
</div>
-->
