---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: 檢視：使用者個人休假
description: 檢視：使用者個人休假
author: Nolan
feature: Reports and Dashboards
exl-id: 9b55b302-5cdc-4437-9ce4-a15b5b43dccb
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '239'
ht-degree: 5%

---

# 檢視：使用者個人休假

<!--Audited: 11/2024-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: consider hiding this article because this is not a custom view anymore.)</p>
-->

您可以建立休假報告來擷取使用者的休假資訊。

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
   <p>投稿人或請求修改檢視 </p>
   <p>要修改報告的標準或計畫</p>
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>編輯報告、儀表板、行事曆的存取權以修改報告</p> <p>編輯對篩選器、檢視、群組的存取權以修改檢視</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>管理報表的許可權</p>  </td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 檢視使用者個人休假

1. 按一下右上角的&#x200B;**主功能表**&#x200B;圖示![主功能表圖示](assets/main-menu-icon.png)，然後按一下&#x200B;**報表>新增報表**。
1. 從下拉式功能表中選取&#x200B;**休假**。
1. 按一下「**儲存並關閉**」。

   依預設，報表在檢視中顯示下列欄位：

   | 使用者 | 在其設定檔中指出休假的使用者名稱。 |
   |---|---|
   | 開始日期 | 使用者指定的休假期間的開始日期。 |
   | 結束日期 | 使用者指定的休假期間的結束日期。 |

   {style="table-layout:auto"}

1. （可選）編輯下列任一標籤以完成報表的建立：

   * 欄（檢視）
   * 群組
   * 篩選器
   * 圖表

   如需有關建立報告的資訊，請參閱文章[建立自訂報告](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)。

   >[!TIP]
   >
   >我們建議為使用者物件新增分組，讓報告更易於閱讀。

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode">Add Time Off information to a user report</h2>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: old way of doing this, not working anymore)</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">To add a column to a user view or report to display a list of future days which have been marked for time off by users:</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/time-off-report-350x61.png" alt="time_off_report.png" style="width: 350;height: 61;"> </p>
-->

<!--
   <li value="1" data-mc-conditions="QuicksilverOrClassic.Draft mode">  Click the <strong>Main Menu</strong> icon <img src="assets/main-menu-icon.png"> in the upper-right corner, then click&nbsp;<strong>Reports > New Report.</strong> </li>
   -->

<!--
   <li value="2" data-mc-conditions="QuicksilverOrClassic.Draft mode">From the&nbsp;<strong>New Report</strong> drop-down menu, select&nbsp;<strong>User Report</strong>.</li>
   -->

<!--
   <li value="3" data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <strong>Add Column</strong>.</li>
   -->

<!--
   <li value="4" data-mc-conditions="QuicksilverOrClassic.Draft mode">From the <strong>View</strong> drop-down menu, select <strong>New View</strong>.</li>
   -->

<!--
   <li value="5" data-mc-conditions="QuicksilverOrClassic.Draft mode">Click the header of the new column, then click<strong>Switch to Text Mode</strong>.</li>
   -->

<!--
   <li value="6" data-mc-conditions="QuicksilverOrClassic.Draft mode">Mouse over the text mode area, and click <strong>Click to edit text</strong>.</li>
   -->

<!--
   <li value="7" data-mc-conditions="QuicksilverOrClassic.Draft mode">Remove the text you find in the <strong>Text Mode</strong> box, and replace it with the following code:<br><!--
   <pre data-mc-conditions="QuicksilverOrClassic.Draft mode">displayname=Personal Time Off<br>listdelimiter=<span><br>listmethod=nested(reservedTimes).lists<br>name=Upcoming Time Off<br>stretch=0<br>textmode=true<br>type=iterate<br>valueexpression=IF({startDate}>$$TODAY,CONCAT({startDate}," - ",{endDate}),'')<br>valueformat=HTML<br>width=150</pre>
   </li>
   -->

<!--
   <li value="8" data-mc-conditions="QuicksilverOrClassic.Draft mode"> Click <strong>Save</strong>+<strong>Close</strong>.</li>
   -->
