---
title: Filter a table in Reporting Canvas
description: Filter a table in Reporting Canvas
hidefromtoc: yes
hide: yes
exl-id: 1838b142-d845-4795-b27f-80bfba18e9d4
---
# Filter a table in Reporting Canvas

After you add a table block to a report, you can set up filters to limit the information that displays in the table.

There are 3 components in a filter rule:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Field</td> 
   <td> <p>The field that contains the information by which you would like to filter your table .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Operator</td> 
   <td> <p>The way that the filter determines which field values are included in or excluded from your table. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Value</td> 
   <td> <p>The values within your selected field that are evaluated according to the operator.</p> </td> 
  </tr> 
 </tbody> 
</table>

**Example:** If you wanted to limit results in your report to only display projects that are owned by Jane Doe, you could create a filter rule with the field "Project Owner," the operator "Equal To," and the value "Jane Doe."

Or you could display only projects that have an assigned project owner, which would have the field "Project Owner" and the operator "Is Not Blank."

## Prerequisites

Before you begin, you must enroll in the Reporting Canvas beta. For more information, see [Reporting Canvas beta: overview](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/reporting-canvas-beta-overview.md).

## Configure filter rules for a table

1. Click the **Main Menu** icon ![Main Menu icon](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click**Reporting**.

1. Click **New report**.

   Or

   Go to an existing report, click the **More Menu** icon ![More icon](assets/more-icon.png) in the report header, then select **Edit**.

1. To group rows on a new table, drag or double-click a table block onto the canvas.

   Or

   To group rows on an existing table, click the **Edit** icon ![Edit icon](assets/edit-icon.png) in the table header.

1. In the right panel, locate the field by which you want to filter your table, then drag it to the Filter section.

   A filter rule set displays with the name of the field you selected.

1. Select the operator that you want from the drop-down menu:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Equal To</strong> </td> 
      <td> <p>This only returns an exact match of the searched value.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Not Equal To</strong> </td> 
      <td> <p>This only returns results that are not exact matches of the searched value.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Is Blank</strong> </td> 
      <td> <p>The field exists for the object but the field has not yet been given a value.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Is Not Blank</strong> </td> 
      <td> <p>The field you are filtering for exists and has been given a value.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Is Less Than</strong> </td> 
      <td> <p>This searches for all results with a value less than what is entered, without including the entered value.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Is Less Than Or Equal To</strong> </td> 
      <td> <p>This searches for all results with a value less than or equal to the entered value.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Is Greater Than</strong> </td> 
      <td> <p>This searches for all results with a value greater than the value entered, without including the entered value.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Is Greater Than Or Equal To</strong> </td> 
      <td> <p>This searches for all results with values greater than or equal to the entered value.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Between</strong> </td> 
      <td> <p>Provides 2 required field values and searches for all results within range of both fields including the entered values.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Contains</strong> </td> 
      <td> <p>This searches for the specified text throughout an entire text string.</p> <p>For example, using "Contains Inf" captures anything with "Inf" or "inf" in it, such as the word "Infinity".</p> <p>Note: Adobe Workfront searches for the entire word or phrase that you enter for each filter rule. For example, if you are searching for fields with the phrase "new project" in their name, Workfront does not display projects that have only "new" or "project" in their names, or phrases that contain extra words in between such as "new main project". The filter finds only projects with the exact phrase "new project" in the name.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Does Not Contain</strong> </td> 
      <td> <p>This filters out items that are missing specified text.</p> <p>For example, "does not contain inf" returns any fields without "Inf" or "inf" in their names.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Enter the last value to complete the filter rule, based on the operator you selected.

   >[!NOTE]
   >
   >Values entered here are **not** case sensitive.

1. (Optional) To add another filter rule to your rule set, do the following:

   1. Drag another field to the **Drop to add another rule** area in the Filters section below your other rule.
   1. Repeat Steps 4-6.
   1. In the operator drop-down left of the new rule, select **AND** or **OR**.

      <table style="table-layout:auto"> 
       <col> 
       </col> 
       <col> 
       </col> 
       <tbody> 
        <tr> 
         <td role="rowheader"> <p>AND</p> </td> 
         <td> <p>When you join filter rules or rule sets with the AND operator, you indicate that you want all rules at the same level to be met.</p> <p>By default, the statements in a filter are joined by the AND operator.</p> </td> 
        </tr> 
        <tr> 
         <td role="rowheader"> <p>OR</p> </td> 
         <td> <p>When you join filter rules or rule set with the OR operator you indicate that you want <strong>at least</strong> one rule—or rule set—at that level to be met.</p> </td> 
        </tr> 
       </tbody> 
      </table>

      >[!IMPORTANT]
      >
      >AND and OR operators at the same level—connecting either multiple rules within a rule set or entire rule sets together—will always match. For example, If you change the operator between two rules within a rule set, all other operators in that rule set will automatically change to match it.

1. (Conditional) To add an additional filter rule set, do the following:

   1. Drag the field that you want to add to the **Add a rule set** area below your other filter rule sets.
   1. Repeat Steps 4-7.
   1. In the operator drop-down left of the new rule set, select **AND** or **OR**. These operators function the same as those listed in Step 7, but apply to entire rule sets as opposed to individual rules within a set.****
