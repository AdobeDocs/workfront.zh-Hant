---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: '''查看：任務視圖的同一列中計畫小時數的實際小時數'
description: 在此任務視圖中，每個任務的實際記錄小時數顯示在計畫小時數內。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: c1179283-dc2e-40d3-b8e0-4b1b79f83ad3
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '419'
ht-degree: 0%

---

# 視圖：任務視圖的同一列中計畫小時數的實際小時數

在此任務視圖中，每個任務的實際記錄小時數顯示在計畫小時數內。

![actual_vs_planned_in_task_report_png](assets/actual-vs-planned-in-task-report-350x58.png)

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

## 在任務視圖中查看計畫小時數的實際小時數

要應用此視圖，請執行以下操作：

1. 轉到任務清單。
1. 從 **視圖** 下拉菜單，選擇 **新建視圖**。

1. 在&#x200B;**列預覽** 框中，刪除除一個列之外的所有列。
1. 按一下其餘列的標題，然後按一下 **切換到文本模式**。
1. 將滑鼠移到文本模式區域上，然後按一下 **按一下可編輯文本**。
1. 刪除在中查找的文本 **文本模式** 框，並用以下代碼替換它：
   <pre>column.0.descriptionkey=name<br>column.0.link.linkproperty.0.name=ID<br>column.0.link.linkproperty.0.valuefield=ID<br>column.0.link.linkproperty.0.valueformat=int<br>column.0.link.lookup=link.view<br>column.0.link.valuefield=objCode<br>column.0.link.valueformat=val<br>column.0.linkedname=direct<br>column.0.listsort=string(name)<br>column.0.namekey=name.abbr<br>column.0.querysort=name<br>column.0.shortview=false<br>column.0.stretch=100<br>column.0.valuefield=name<br>column.0.valueformat=HTML<br>column.0.width=150<br>column.1.viewalias=assignments<br>column.1.displayname=<br>column.1.linkedname=direct<br>column.1.namekey=分配<br>column.1.valuefield=assignmentsListString<br>column.1.valueformat=HTML<br>column.1.tile.name=component.assignments清單<br>column.2.displayname=實際/計畫小時數<br>column.2.linkedname=direct<br>column.2.namekey=實際工時要求<br>column.2.querysort=actualWork<br>column.2.textmode=true<br>column.2.valueexpression=CONCAT({actualWorkRequired}/60,' /「，{workRequired}/60)<br>column.2.valuefield=actualWorkRequired<br>column.2.valueformat=複合<br>column.2.viewalias=actualworkred<br>column.3.aggregator.function=SUM<br>column.3.aggregator.valueexpression=SUB({actualWork}, {workRequired})<br>column.3.aggregator.valueformat=compound<br>column.3.displayname=小時數差異<br>column.3.linkedname=direct<br>column.3.textmode=true<br>column.3.valueexpression=SUB({actualWork}, {workRequired})/60<br>column.3.valueformat=customNumberAsString</pre>

1. 按一下 **保存視圖**。
