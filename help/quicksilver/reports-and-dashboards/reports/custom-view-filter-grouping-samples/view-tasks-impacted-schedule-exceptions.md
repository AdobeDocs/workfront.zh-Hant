---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '''查看：受計畫異常影響的任務'
description: 此任務視表徵圖識因週末、個人休息或其他計畫例外而必須延遲完成的任務。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 7d7c77fa-d9a7-4e91-8dae-ad3aaca6f1da
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '722'
ht-degree: 0%

---

# 視圖：受計畫異常影響的任務

此任務視表徵圖識因週末、個人休息或其他計畫例外而必須延遲完成的任務。

此視圖顯示以下內容：

* 任務的持續時間
* 任務的計畫起始日期和計畫完成日期
* 根據任務的「計畫起始日期」和「計畫完成日期」之間的天數（日曆持續時間）的任務持續時間
* 任務開始時項目計畫中的日數（日曆起始日期）
* 根據任務的「計劃開始」和「計畫完成日期」之間的工作日數（週日持續時間）確定任務的週日持續時間
* 如果「週日持續時間」大於任務的持續時間，則任務將標籤為「例外」。\
   ![tasks_with_calendar_exceptions_png](assets/tasks-with-calendar-exceptions-350x51.png)

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

## 查看受計畫異常影響的任務

1. 轉到任務清單。
1. 從 **視圖** 下拉菜單，選擇 **新建視圖**。

1. 在&#x200B;**列預覽** 框中，刪除除一個列之外的所有列。
1. 按一下其餘列的標題，然後按一下 **切換到文本模式**。
1. 將滑鼠移到文本模式區域上，然後按一下 **按一下可編輯文本**。
1. 刪除在中查找的文本 **文本模式** 框，並用以下代碼替換它：
   <pre>column.0.descriptionkey=name<br>column.0.link.linkproperty.0.name=ID<br>column.0.link.linkproperty.0.valuefield=ID<br>column.0.link.linkproperty.0.valueformat=int<br>column.0.link.lookup=link.view<br>column.0.link.valuefield=objCode<br>column.0.link.valueformat=val<br>column.0.linkedname=direct<br>column.0.listsort=string(name)<br>column.0.namekey=name.abbr<br>column.0.querysort=name<br>column.0.shortview=false<br>column.0.stretch=100<br>column.0.valuefield=name<br>column.0.valueformat=HTML<br>column.0.width=150<br>column.1.descriptionkey=duration<br>column.1.linkedname=direct<br>column.1.listsort=intAsInt(durationMinutes)<br>column.1.namekey=duration.abbr<br>column.1.querysort=durationMinutes<br>column.1.shortview=false<br>column.1.stretch=0<br>column.1.valuefield=durationFieldLong<br>column.1.valueformat=複合<br>column.1.viewalias=duration<br>column.1.width=80<br>column.2.descriptionkey=plannedstartdate<br>column.2.linkedname=direct<br>column.2.listsort=atDateAsAtDate(planedStartDate)<br>column.2.namekey=plannedstartdate.abbr<br>column.2.querysort=planedStartDate<br>column.2.shortview=false<br>column.2.strt.0<br>column.2.valuefield=planedStartDate<br>column.2.valueformat=atDate<br>column.2.width=80<br>column.3.descriptionkey=plannedcompletiondate<br>column.3.linkedname=direct<br>column.3.listsort=atDateAsAtDate(planedCompletionDate)<br>column.3.namekey=plannecompletiondate.abbr<br>column.3.querysort=planedCompletionDate<br>column.3.shortview=false<br>column.3.strt.0<br>column.3.valuefield=planedCompletionDate<br>column.3.valueformat=atDate<br>column.3.width=80<br>column.4.aggregator.displayformat=int<br>column.4.aggregator.function=SUM<br>column.4.aggregator.namekey=id<br>column.4.aggregator.valueexpression=DATEDIFF({planedCompletionDate},<br>{planedStartDate})+1<br>column.4.aggregator.valueformat=intAsInt<br>column.4.descriptionkey=id<br>column.4.linkedname=direct<br>column.4.listsort=intAsInt(ID)<br>column.4.name=日曆持續時間<br>column.4.querysort=ID<br>column.4.shortview=false<br>column.4.stretch=0<br>column.4.valueexpression=DATEDIFF({planedCompletionDate},{planedStartDate})+1<br>column.4.valueformat=int<br>column.4.width=80<br>column.5.aggregator.displayformat=int<br>column.5.aggregator.function=SUM<br>column.5.aggregator.namekey=id<br>column.5.aggregator.valueexpression=DATEDIFF({planedStartDate},{project}。<br>{planedStartDate})+0<br>column.5.aggregator.valueformat=intAsInt<br>column.5.descriptionkey=id<br>column.5.linkedname=direct<br>column.5.listsort=intAsInt(ID)<br>column.5.name=日曆開始日期<br>column.5.querysort=ID<br>column.5.shortview=false<br>column.5.strt.0<br>column.5.valueexpression=DATEDIFF({planedStartDate},{project}。{planedStartDate})+0<br>column.5.valueformat=int<br>column.5.width=80<br>column.6.aggregator.displayformat=int<br>column.6.aggregator.function=SUM<br>column.6.aggregator.namekey=id<br>column.6.aggregator.valueexpression=WEEKDAYDIFF({planedStartDate},<br>{planedCompletionDate})+0<br>column.6.aggregator.valueformat=HTML<br>column.6.descriptionkey=id<br>column.6.linkedname=direct<br>column.6.listsort=intAsInt(ID)<br>column.6.name=週日持續時間<br>column.6.querysort=ID<br>column.6.shortview=false<br>column.6.strt.0<br>column.6.valueexpression=WEEDDAYDIFF({planedStartDate},{planedCompletionDate})+0<br>column.6.valueformat=int<br>column.6.width=80<br>column.7.aggregator.displayformat=int<br>column.7.aggregator.expression=IF((WEEDDAYDIFF({planedStartDate},{planedCompletionDate}))&gt;({duration}/480),"異常",")<br>column.7.aggregator.function=SUM<br>column.7.aggregator.namekey=id<br>column.7.aggregator.valueformat=HTML<br>column.7.linkedname=direct<br>column.7.listsort=intAsInt(ID)<br>column.7.name=計畫<br>column.7.querysort=ID<br>column.7.shortview=false<br>column.7.stretch=0<br>column.7.valueexpression=IF((WEEDDAYDIFF({planedStartDate},{planedCompletionDate}))&gt;({duration}/480),"Exception",")<br>column.7.valueformat=HTML<br>column.7.width=80</pre>

1. 按一下 **保存視圖**。
