---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 「檢視：任務檢視中工期和計畫工時的基準差異比較」
description: 檢視「工期」與「計畫工時」的基線差異。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 2a1eef9c-016c-4a04-acda-6070fcb0e23d
source-git-commit: bcafa607da733b89747f6b448dd295d9b906d060
workflow-type: tm+mt
source-wordcount: '516'
ht-degree: 0%

---

# 檢視：任務檢視中「工期」與「計畫工時」的比較基準差異

此檢視會在工作檢視中顯示下列專案：

* 包含基準線任務資訊的任務資訊。
* 「持續時間」與「預設基準線持續時間」之間的差異。
* 計畫工時與預設比較基準計畫工時之間的差異。

>[!NOTE]
>
> 下列檢視表中顯示的資料會將實際作業值與與「預設基準線」作業相關的值進行比較。

 

![baseline_variance_in_a_task_view.png](assets/baseline-variance-in-a-task-view-350x38.png)

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

## 在任務檢視中檢視工期和計畫工時的比較基準差異

1. 前往工作清單。
1. 在&#x200B;**檢視**&#x200B;下拉式功能表中，選取&#x200B;**新增檢視**。

1. 移除檢視中的所有欄（第一個欄除外）。
1. 選取第一欄後，按一下&#x200B;**切換到文字模式**。
1. 複製下方的文字，並貼到檢視的第一欄：
   <pre>column.0.descriptionkey=name<br>column.0.link.linkproperty.0.name=ID<br>column.0.link.linkproperty.0.valuefield=ID<br>column.0.link.linkproperty.0.valueformat=int<br>column.0.link.lookup=link.view<br>column.0.link.valuefield=objCode<br>column.0.link.valueformat=val<br>column.0.link.dname=direct<br>column.0.listort=string(name){name)<br>column.0.namekey=name.abbr<br>column.0.querysort=name<br>column.0.shortview=false<br>column.0.stretch=100<br>column.0.valuefield=name<br>column.0.valueformat=HTML<br>column.0.width=150<br>column.0.displayname=任務名稱<br>column.1.descriptionkey=duration<br>column.1.linkedname=direct<br>column.1.listsort intAsInt(durationMinutes)<br>column.1.namekey=duration.abbr<br>column.1.querysort=durationMinutes<br>column.1.shortview=false<br>column.1.stretch=0<br>column.1.valuefield=durationFieldLong<br>column.1.valueformat=compound<br>column.1.viewalias=duration<br>column.1000<br>column.1.displayname=TashDuration{2 8}column.2.descriptionkey=view.relatedcolumn<br>column.2.descriptionkeyargkey.0=defaultbaselinetask<br>column.2.descriptionkeyargkey.1=duration<br>column.2.linkedname=defaultBaselinetask<br>column.2.listsort=intAsInt(durationMinutes)<br>column.2.namekey.0=duration{defaultask.0=defaultask{35 {column.2.namekeyargkey.1=duration.abbr<br>column.2.querysort=defaultBaselineTask：durationMinutes<br>column.2.shortview=false<br>column.2.stretch=0<br>column.2.valuefield=defaultBaselineTask：durationFieldLong<br>column.2.valueformat=compound<br>column.2 playname=Dflt基線任務： Dur<br>列。2.durationunitfield=durationUnit.value<br>列。3.description=Duration Variance"列。3.linkedname=direct<br>列。3.listsort=intAsInt(durationMinutes)<br>列。3.name=Duration Variance<br>列。3.querysort=durationMinutes<br>列。3.short=false<br>列。3.stretage=0<br>列。3.valuevaluevalue expression=CONCAT(SUB({duration}，{defaultBaselineTask})<br><br><br><br><br>{duration})/480，" Days")<br>column.3.valueformat=HTML<br>column.3.viewalias=duration<br>column.3.width=100<br>column.3.displayname=Duration Variance<br>column.4.descriptionkey=workrequired<br>column.4.linkedname=direct<br>column.4.listsort=doubleAsDouble(workRequired)<br>column.4.namequirequired.abbr<br>column.4.quired.querysort=work{work1Requirequirequirequirequirequirequired 0}column.4.shortview=false<br>column.4.stretch=0<br>column.4.valuefield=workFieldLong<br>column.4.valueformat=compound<br>column.4.viewalias=workrequired<br>column.4.width=100<br>column.4.displayname=Wrk Req<br>column.5.descriptionkey=view.relatedcolumn<br>column.5.descriptionkeykeyarkey.0=defaultbaselinetask{1 9}column.5.descriptionkeyargkey.1=workrequired<br>column.5.linkedname=defaultBaselineTask<br>column.5.listsort=doubleAsDouble(workRequired)<br>column.5.namekeyargkey.0=defaultbaselinetask.abbr<br>column.5.namekeyargkey.1=workrequirequired.abbr<br>column.querysortBaselineTaskTaskTaskWork：work必需<br>列。5.shortview=false<br>列。5.stretch=0<br>列。5.valuefield=defaultBaselineTask：workFieldLong<br>列。5.valueformat=compound<br>列。5.viewalias=defaultBaselineTask：workrequired<br>列。5.width=100<br>列。5.displayname=Dflt基準任務：工作請求<br>列。6.descriptionkey關鍵字{workreq3} 4}column.6.linkedname=direct<br>column.6.listsort=doubleAsDouble(workRequired)<br>column.6.name=Effort Variance<br>column.6.querysort=workRequired<br>column.6.shortview=false<br>column.6.valueexpression=CONCAT(SUB({workRequired}，{defaultBaselineTask}。<br><br><br><br><br>{workRequired})/60，" Hours")<br>column.6.valueformat=HTML<br>column.6.viewalias=workrequired<br>column.6.width=100<br>column.6.displayname=Effort Variance</pre>

1. 按一下「**儲存視圖**」。