---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 「檢視：受排程例外影響的任務」
description: 此任務檢視會識別因週末、個人休假或其他排程例外而必須延遲完成的任務。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 7d7c77fa-d9a7-4e91-8dae-ad3aaca6f1da
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '634'
ht-degree: 0%

---

# 檢視：受排程例外影響的任務

此任務檢視會識別因週末、個人休假或其他排程例外而必須延遲完成的任務。

此檢視會顯示下列專案：

* 任務持續時間
* 任務的計劃開始與計畫完成日期
* 根據任務的計劃開始與計畫完成日期之間的天數的任務持續時間（日曆持續時間）
* 任務開始時，專案排程的天數（行事曆開始日期）
* 根據任務的計劃開始與計畫完成日期之間的工作日數任務的工作日持續時間（工作日持續時間）
* 如果「工作日期間」大於工作的期間，這表示工作期間有例外天數，則會將工作標示為「例外」。\
  ![tasks_with_calendar_exceptions.png](assets/tasks-with-calendar-exceptions-350x51.png)

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>請求修改檢視 </p>
   <p>計畫修改報表</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>編輯報告、儀表板、行事曆的存取權以修改報告</p> <p>編輯對篩選器、檢視、群組的存取權以修改檢視</p> <p><b>附註</b>

如果您還是沒有存取權，請詢問您的Workfront管理員，他們是否在您的存取層級中設定其他限制。 如需Workfront管理員如何修改存取層級的詳細資訊，請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>。</p> </td>
</tr>   
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>管理報表的許可權</p> <p>如需請求其他存取權的資訊，請參閱<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求物件</a>的存取權。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的Workfront管理員。

## 檢視受排程例外影響的任務

1. 前往工作清單。
1. 從&#x200B;**檢視**&#x200B;下拉式功能表中，選取&#x200B;**新增檢視**。

1. 在&#x200B;**資料行預覽**&#x200B;區域中，排除除一個資料行以外的所有資料行。
1. 按一下剩餘欄的標題，然後按一下&#x200B;**切換到文字模式**。
1. 將滑鼠移到文字模式區域上，然後按一下&#x200B;**按一下以編輯文字**。
1. 移除您在&#x200B;**文字模式**&#x200B;方塊中找到的文字，並取代為下列程式碼：
   <pre>column.0.descriptionkey=name<br>column.0.link.linkproperty.0.name=ID<br>column.0.link.linkproperty.0.valuefield=ID<br>column.0.link.linkproperty.0.valueformat=int<br>column.0.link.lookup=link.view<br>column.0.link.valuefield=objCode<br>column.0.link.valueformat=val<br>column.0.link.dname=direct<br>column.0.listort=string(name){name)<br>column.0.namekey=name.abbr<br>column.0.querysort=name<br>column.0.shortview=false<br>column.0.stretch=100<br>column.0.valuefield=name<br>column.0.valueformat=HTML<br>column.0.width=150<br>column.1.descriptionkey=duration<br>column.1.listsort=intAsInt(duration)<br>分鐘column.1.namekey=duration.abbr<br>column.1.querysort=durationMinutes<br>column.1.shortview=false<br>column.1.stretch=0<br>column.1.valuefield=durationFieldLong<br>column.1.valueformat=compound<br>column.1.viewalias=duration<br>column.1.widationkey=80<br>column.2.2.descriptionkey=plannedstartdate<br>column.2.linkedname=direct<br> column.2.listsort=atDateAsAtDate(plannedStartDate)<br>column.2.namekey=plannedstartdate.abbr<br>column.2.querysort=plannedStartDate<br>column.2.shortview=false<br>column.2.stretch=0<br>column.2.valuefield=plannedStartDate<br>column.2.widate=at<br>column.2.width=80<br> descriptionkey=plannedcompletiondate<br>column.3.linkedname=direct<br>column.3.listsort=atDateAsAtDate(plannedCompletionDate)<br>column.3.namekey=plannedcompletiondate.abbr<br>column.3.querysort=plannedCompletionDate<br>column.3.short=false<br>column.3.3.valuefield=plannedComplection<br>column 3.valueformat=atDate<br>column.3.width=80<br>column.4.aggregator.displayformat=int<br>column.4.aggregator.function=SUM<br>column.4.aggregator.namekey=id<br>column.4.aggregator.valueexpression=DATEDIFF({plannedCompletionDate}，<br>{plannedStartDate})+1<br>column.4.aggregaggregator.valueformat.valueformat=intAsIntAsInt<br>column.4}column.4.descrin.descript ptionkey=id<br>column.4.linkedname=direct<br>column.4.listsort=intAsInt(ID)<br>column.4.name=Calendar Duration<br>column.4.querysort=ID<br>column.4.shortview=false<br>column.4.stretch=0<br>column.4.valueexpression=DATEDIFF({plannedCompletionDate}，{plannedStartDate})+1<br>column.4.valueformat=int<br>column.column.width=80<br>column.5.aggregator.displayformat=int<br>column.5.aggregator.function=SUM<br>column.5.aggregator.namekey=id<br>column.5.aggregator.valueexpression=DATEDIFF({plannedStartDate}，{project}。<br><br><br>{plannedStartDate})+0<br>column.5.aggregator.valueformat=intAsInt<br>column.5.descriptionkey=id<br>column.5.linkedname=direct<br>column.5.listsort=intAsInt(ID)<br>column.5.name=Calendar開始日期<br>column.5.querysort=ID<br>column.5.short=false<br>column.5.stretage=0<br>column.5.valueexpression=DATEDIFF({plannedStartDate}，{project}。{plannedStartDate})+0<br>column.5.valueformat=int<br>column.5.width=80<br>column.6.aggregator.displayformat=int<br>column.6.aggregator.function=SUM<br>column.6.aggregator.namekey=id<br>column.6.aggregator.valueexpression=WEEKDAYDIFF({plannedStartDate}，<br>{plannedCompletionDate})+0<br>column.6.aggregator.valueformat=HTML<br>column.6.descriptionkey.descriptionkey.descriptionkey.descriptionkey=id=id=id{id{12 {column.6.linkedname=direct<br>column.6.listsort=intAsInt(ID)<br>column.6.name=Week Day Duration<br>column.6.querysort=ID<br>column.6.shortview=false<br>column.6.stretch=0<br>column.6.valueexpression=WEEKDAYDIFF({plannedStartDate}，{plannedCompletionDate})+0<br>column.6.valueformat=int<br>column.6.widain.8.wida 0<br>column.7.aggregator.displayformat=int<br>column.7.aggregator.expression=IF((WEEKDAYDIFF({plannedStartDate}，{plannedCompletionDate}))&gt;({duration}/480)，"Exception"，")<br>column.7.aggregator.function=SUM<br>column.7.aggregator.namekey=id<br>column.7.valueformat=HTML{3.linkedname=direct{direct 2}column.7.listsort=intAsInt(ID)<br>column.7.name=Schedule<br>column.7.querysort=ID<br>column.7.shortview=false<br>column.7.stretch=0<br>column.7.valueexpression=IF((WEEKDAYDIFF({plannedStartDate}，{plannedCompletionDate}))&gt;({duration}/480)，「異常」，「」)<br>column.7.valueformat=HTML 42}column.7.width=80<br><br><br><br></pre>

1. 按一下「**儲存視圖**」。
