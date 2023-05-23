---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: '''查看：用戶個人休息'
description: '''查看：用戶個人休息'
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 9b55b302-5cdc-4437-9ce4-a15b5b43dccb
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '284'
ht-degree: 4%

---

# 視圖：用戶個人時間關閉

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: consider hiding this article because this is not a custom view anymore.)</p>
-->

您可以生成「關機時間」報告以捕獲用戶的關機時間資訊。

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
   <td> <p>請求修改視圖 </p>
   <p>計畫修改報表</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>編輯對報表、儀表板、日曆的訪問以修改報表</p> <p>編輯對篩選器、視圖、分組的訪問以修改視圖</p> <p><b>附註</b>

如果您仍然沒有訪問權限，請詢問您的Workfront管理員是否在您的訪問級別設定了其他限制。 有關Workfront管理員如何修改您的訪問級別的資訊，請參見 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自定義訪問級別</a>。</p> </td>
</tr>  
  <tr> 
   <td role="rowheader">對象權限</td> 
   <td> <p>管理對報表的權限</p> <p>有關請求附加訪問的資訊，請參見 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求訪問對象 </a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要瞭解您擁有的計畫、許可證類型或訪問權限，請與您的Workfront管理員聯繫。

## 查看用戶個人休息時間

1. 按一下 **主菜單** 表徵圖 ![](assets/main-menu-icon.png) 在右上角，按一下 **報表>新建報表**。

1. 從下拉菜單中，選擇 **關閉時間**。
1. 按一下 **保存+關閉**。

   預設情況下，該報表在視圖中顯示以下欄位：

   | 使用者 | 在其配置檔案中指示休息時間的用戶的名稱。 |
   |---|---|
   | 從開始日期安排 | 用戶指示的時間段的開始日期。 |
   | 結束日期 | 用戶指示的時間段的結束日期。 |

   {style="table-layout:auto"}

1. （可選）通過編輯以下任意頁籤完成報表的建立：

   * 欄（檢視）
   * 群組
   * 篩選器
   * 圖表

   有關建立報告的資訊，請參閱文章 [建立自定義報告](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)。

   >[!TIP]
   >
   >我們建議為User對象添加分組，以便更易於讀取報告。

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
