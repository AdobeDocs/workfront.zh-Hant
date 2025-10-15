---
product-area: reporting
navigation-topic: text-mode-reporting
title: 使用文字模式編輯檢視
description: 您可以使用文字模式來編輯清單或報表中的檢視，以存取標準介面中無法使用的欄位，並建立更複雜的檢視。
author: Nolan
feature: Reports and Dashboards
exl-id: b99a2d14-a226-4075-9b1b-ac9426fd41b8
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '461'
ht-degree: 3%

---

# 使用文字模式編輯檢視

<!-- Audited: 1/2025 -->

您可以使用文字模式來編輯清單或報表中的檢視，以存取標準介面中無法使用的欄位，並建立更複雜的檢視。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront套件</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td> 
     <p>標準</p>
     <p>規劃</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>編輯對篩選器、檢視、群組的存取權</p> <p>編輯報告、儀表板、行事曆的存取權，以編輯報告中的報告元素</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>管理報表的許可權，以編輯報表中的檢視</p> <p>管理檢視的許可權以進行編輯</p> </td> 
  </tr>
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 先決條件

在報表或清單中開始使用文字模式之前，請務必熟悉Workfront文字模式語法。

如需詳細資訊，請參閱：

* [文字模式概觀](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md)
* [文字模式語法概觀](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md)
* [自訂檢視、篩選和分組範例：文章索引](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md)

## 在檢視中編輯文字模式

對於報告和清單，使用文字模式編輯檢視是相同的。 從報表或清單存取檢視表的方式會有所不同。

>[!TIP]
>
>建議您在標準模式中建立儘可能多的檢視，然後將其轉換為文字模式以進行編輯。

如需有關建立檢視的資訊，請參閱[Adobe Workfront中的檢視總覽](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)。

如需建立報告的詳細資訊，請參閱[建立自訂報告](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)。

1. 執行下列其中一項：

   1. 若要從報告存取檢視，請移至報告，然後按一下&#x200B;**報告動作** > **編輯** > **欄（檢視）**&#x200B;標籤。
   1. 若要從清單存取檢視，請移至清單，然後從&#x200B;**檢視**&#x200B;下拉式功能表，將游標移至您要修改的檢視上，然後按一下&#x200B;**編輯**&#x200B;圖示![編輯圖示](assets/edit-icon.png)。

      檢視產生器隨即開啟。

1. 在檢視中選取欄。

   或

   選取Report Builder的&#x200B;**欄（檢視）**&#x200B;標籤，然後選取欄。

   >[!TIP]
   >
   >若要使用文字模式編輯檢視，您必須一次編輯一欄。

1. 按一下產生器右上角的&#x200B;**切換至文字模式**，然後按一下&#x200B;**編輯文字模式**。

   >[!NOTE]
   >
   >當您以文字模式編輯欄時，Workfront會將`textmode=true`行程式碼新增至欄。 這表示在文字模式中修改了欄。

   下表概述文字模式檢視中的關鍵行：

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: make this a snippet and add it to the grouping article too)</p>
   -->

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>範例行</th> 
      <th>說明</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td> <p><ol><tr><tr><ol><tr><tr><tr><tr><tr><tr><tr><tr><tr><tr><div class="example" data-mc-autonum="<b>Example: </b>"><code><strong>valuefield</strong>=</cod></p> </td> 
      <td> <p>This is the name of the object or of the field as it appears in the database. For more information about how objects and fields appear in the database, see <a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">API Explorer</a>.</p> <p>The following scenarios exist:</p> 
        
        <li value="1"> <p> If the name of the field you display is a phrase instead of a single noun, you must use camel case syntax for the <code>valuefield</code>. For example, for the Planned Start Date of a task the code is: </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Example: </b></span></span><code>valuefield=plannedStartDate</code> </p> </li> 
        <li value="2"> <p>If you want to display a custom field, the <code>valuefield</code> value is the actual name of the field, as you see it in the interface. For example, for a custom field named "More information", the code is:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Example: </b></span></span><code>valuefield=More information</code> </p> </li> 
        <li value="3"> <p>If you want to display objects that are related to other objects in a view using the <code>valuefield</code> line of code the object names and attributes are separated by colons. </p> <p>For example, a column in a task view that would display the name of the Portfolio Owner has the following value for the valuefield line:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Example: </b></span></span><code>valuefield=project:portfolio:owner:name</code> </p> <p>This indicates that from the object of the report (task), you can access the next related object (project), from there, you can access the following related object from project (portfolio), then the portfolio owner (owner) and then their name (name). </p> </li> 
       </ol> <p>For information about how objects connect to one another, see the section <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-interdependency-and-hierarchy-of-objects" class="MCXref xref">Interdependency and hierarchy of objects</a> in <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">Understand objects in Adobe Workfront</a>.</p> <p>Note: If you choose a field in text mode that is not valid in the standard interface, you are not able to switch back to the standard interface within the column.</p> </td> 
     </tr> 
      
      <td><code><strong>valueformat=</strong></code> </td> 
      <td> <p>This line represents the format used to display the <code>valuefield</code>. The <code>valueformat</code> identifies whether an object or field displays as text, number, percentage, or date.</p> <p>We recommend using <code>HTML</code> for your <code>valueformat</code>, especially when using <code>valueexpression</code>, to ensure the most accurate display of your information. </p> <p>For information about additional values for this line, see <a href="../../../reports-and-dashboards/reports/text-mode/use-conditional-formatting-text-mode.md" class="MCXref xref">Use conditional formatting in Text Mode</a>.</p> </td> 
     </tr> 
      
      <td> <p><code><strong>valueexpression=</strong></code> </p> </td> 
      <td> <p>You can add this line to replace <code>valuefield</code>, if you want to display a calculated field in the column.</p> <p>You must enclose the <code>valuefield</code> of the objects in curly brackets every time you use it in a <code>valueexpression</code>.</p> <p>The following scenarios exist: </p> 
        
        <li value="1"> <p>If you want to display a field in a column in upper case, you would use:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Example: </b></span></span><code>valueexpression=UPPER({valuefield})</code> </p> <p>The <code>valuefield</code> of the object is spelled as it appears in the API Explorer. </p> </li> 
        <li value="2">If you want to add multiple <code>valuefields</code> by stringing them together, you must separate them by a period.</li> 
        <li value="3"> <p>For example, if you want to display the name of the Primary Assignee of a task using <code>valueexpression</code>, you would use:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Example: </b></span></span><code>valueexpreesion={assignedTo}.{name}</code> </p> </li> 
        <li value="4"> <p>If you want to use a custom field in a <code>valueexpression</code> line you must precede the name of the field by <code>DE:</code> to indicate that it is a custom field. The name of the field is spelled as it appears in the interface. </p> <p>Important: When you use a custom field that is placed in a custom form section that has restricted permissions for some users, the calculation of the valueexpression is blank when those users view this calculation in a report. For information about adjusting permissions on custom form sections, see <span help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md"><a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md">Create a custom form</a></span>.</p> <p>For example, if you have a custom field labeled "Developer Name" and you want to display this field in upper case in a column, you can use the following <code>valueexpression</code> to indicate this:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Example: </b></span></span><code>valueexpression=UPPER({DE:Developer Name}</code>) </p> <p>When referencing a Typeahead type custom field, use the following expression to reference the name of the object selected in a field labeled "Developer Name":</p> <p><code>valueexpression=UPPER({DE:Developer Name:name})</code> </p> </li> 
       </ol> </td> 
     </tr> 
      
      <td> <p><code><strong>descriptionkey=</strong></code> / <code><strong>description=</strong></code> </p> </td> 
      <td> <p>This line defines the text of a tool tip as you mouse over the name of the column. In this case it is using a key to translate the name value in the description text. If you want to modify the description, change this line to read: </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Example: </b></span></span><code>description=Your Value</code>.</p> </td> 
     </tr> 
      
      <td><code><strong>namekey=</code> / <code><strong>name=</strong></code> </td> 
      <td> <p>This line defines the column label. In this case it is using the abbreviated value based on the key.</p> <p>If you want to modify the column name you can change this value to: </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Example: </b></span></span><code>name=Your Value</code> </p> <p><code>Name</code> allows you to enter any text for the column name, while<code>namekey</code> requires you enter a key that is used to translate the name of a column.</p> <p>To change the column name you can also add the <code>displayname </code>line, if one is not present.</p> </td> 
     </tr> 
      
      <td><code><strong>displayname =</strong></code> </td> 
      <td> <p>You can add the following line to change the name of a column, which suspends the <code>namekey/name</code> value:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Example: </b></span></span><code>displayname=Your Value</code> </p> </td> 
     </tr> 
      
      <td><code><strong>querysort=</strong> </code></td> 
      <td>This line defines how the results are sorted when the column header is clicked. If it is not present then the column cannot be sorted after the report is run.</td> 
     </tr> 
      
      <td><code><strong>width=</strong></code> </td> 
      <td> <p>This line represents the number of pixels that are used for the column. If the line is omitted or set to 0 (zero) then the column does not appear in the view.</p> <p>When you modify this field manually in text mode, you must also add the <code>usewidths=true</code> value to your column.</p> </td> 
     </tr> 
      
      <td><code><strong>usewidths=true</strong></code> </td> 
      <td> <p>You must use this line in addition to the <code>width=</code> line when customizing the width of a column. </p> </td> 
     </tr> 
      
      <td><code><strong>makeFieldEditable=</strong></code> </td> 
      <td> <p>This line defines whether the value displayed in a column is inline editable or not. If this line equals <strong>true</strong>, the value in the column is inline editable. If this line equals <code>false</code>, the value in the column is not inline editable.</p> </td> 
     </tr> 
      
      <td><code><strong>link.valuefield=</strong> </code></td> 
      <td> <p>Insert this line only when you want the value displayed in a column to link to the object associated with it. The link opens the details page of the object. This value should match the <code>valuefield=</code> line. When you insert this, you must also add the <code>link.valueformat=</code> line. </p> <p> For example, you can insert <code>link.valuefield=priority</code> in an issue view, and the Priority of the issue displays as a link. Clicking this link opens the Issue page.</p> </td> 
     </tr> 
      
      <td><code><strong>link.valueformat=</strong> </code></td> 
      <td> <p>Insert this line only when you have inserted the <code>link.valuefield</code> line to add a link to the value in a column. The link opens the details page of the object. This value should match the <code>valueformat=</code> line and indicates the format used to display the <code>valuefield</code>. </p> <p>Important: When viewing the text mode in a built-in column that also includes a link, you notice a number of lines referring to the link. Some of those lines might no longer be supported or are unnecessary when you create your own custom column in text mode and add the link statements to it. The lines that are mandatory when adding a linked value are<code> link.valuefield</code> and <code>link.valueformat</code>. </p> </td> 
     </tr> 
      
      <td><code><strong>aggregator.function=</strong></code> </td> 
      <td> <p>This refers to how the values of each column are summarized. There are multiple lines that start with <code>aggregator.</code> and they all refer to the aggregator that summarizes the results of the column. </p> <p>As a general rule, the <code>aggregator.</code> lines match those of the column object. </p> 
       
        <span class="autonumber"><span><b>Example: </b></span></span> 
        <p>The Planned&nbsp;Hours column in a task report summarized by Sum may look like the following: </p>

   <div>
         <code>textmode=true</code>
         <code>valuefield=workRequired</code>
         <code>valueformat=compound</code>
         <code>aggregator.function=SUM</code>
         <code>aggregator.valuefield=workRequired</code>
         <code>aggregator.displayformat=minutesAsHoursString</code>
         <code>aggregator.valueformat=compound</code>
         <code>namekey=workRequired</code>
         <code>shortview=false</code> 
        </div> 
       </div>

   <div>
      <code>aggregator. </code>行可能包含<code>valuefield </code>或<code>valueexpression</code>。
       </div> </td> 
     </tr> 
    </tbody> 
   </table>

1. 如果要儲存變更並繼續編輯檢視，請按一下[套用]。****
1. 按一下&#x200B;**儲存+關閉**&#x200B;以儲存您的報告。

   或

   按一下&#x200B;**儲存檢視**，將檢視儲存在清單中。
