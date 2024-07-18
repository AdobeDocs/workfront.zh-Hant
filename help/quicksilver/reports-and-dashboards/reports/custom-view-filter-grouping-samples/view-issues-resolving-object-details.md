---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 「檢視：解析物件詳細資料的問題」
description: 此問題檢視顯示問題的解決物件的名稱和完成百分比，即使沒有解決任務或專案的存取權，問題建立者也可以洞察問題的進度。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 7f4c923a-01e4-4896-9f54-1f0c66d64bb5
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '549'
ht-degree: 0%

---

# 檢視：解析物件詳細資料的問題

此問題檢視顯示問題的解決物件的名稱和完成百分比，即使沒有解決任務或專案的存取權，問題建立者也可以洞察問題的進度。

此檢視使用

```
sharecol=true
```

標籤來組合相同欄標題下的多個欄位。 如需詳細資訊，請參閱

```
sharecol
```

標籤中，請參閱[檢視：合併一個共用資料行](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-merge-columns.md)中多個資料行的資訊。

![issue_custom_view_with_resolving_object_name_and_percent_complete.png](assets/issue-custom-view-350x77.png)

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

## 檢視有關解析物件詳細資料的問題

1. 前往問題清單。
1. 從&#x200B;**檢視**&#x200B;下拉式功能表中，選取&#x200B;**新增檢視**。

1. 在&#x200B;**資料行預覽**&#x200B;區域中，排除除一個資料行以外的所有資料行。
1. 按一下剩餘欄的標題，然後按一下&#x200B;**切換到文字模式**。
1. 將滑鼠移到文字模式區域上，然後按一下&#x200B;**按一下以編輯文字**。
1. 移除您在&#x200B;**文字模式**&#x200B;方塊中找到的文字，並取代為下列程式碼：<pre>column.0.querysort=name</pre><pre>column.0.stretch=0<br>column.0.valuefield=name<br>column.0.valueformat=HTML<br>column.0.width=150<br>column.1.descriptionkey=sourceobject<br>column.1.linkedname=direct<br>column.1.listsort=nested(referenceObject)。HTML(name)<br>column.1.namekey=sourceobject.abbr<br>column.1.1.short=false<br>column.1.stretch=0<br>column.column.column.1.column=0<br>column.column.column.1.1.column.reference物件。1.column.reference物件物件物件<br>column.1.valueformat=HTML<br>column.1.viewalias=source<br>column.1.width=100<br>column.2.descriptionkey=assignedto<br>column.2.link.linkproperty.0.name=ID<br>column.2.linkproperty.0.valuefield=assignedTo：ID<br>column.2.link.0.valueformat.valueformat=int{int{link.lookup.link.view 18}column.2.link.valuefield=assignedTo：objCode<br>column.2.link.valueformat=val<br>column.2.linkedname=assignedTo<br>column.2.listsort=nested(assignedTo)。string(name)<br>column.2.querysort=assignedTo：name<br>column.2.short=false<br>column.2.stretch=25<br>column.2 uefield=assignedTo：name<br>column.2.valueformat=HTML<br>column.2.width=150<br>column.3.descriptionkey=entrydate<br>column.3.linkedname=direct<br>column.3.listsort=atDateAsAtDate(entryDate)<br>column.3.namekey=entrydate.abbr<br>column.3.querysort=entryDateDateDateFalse=entrateDate{false{false 35}column.3.stretch=0<br>column.3.valuefield=entryDate<br>column.3.valueformat=atDate<br>column.3.width=150<br>column.4.descriptionkey=description<br>column.4.linkedname=direct<br>column.4.listsort=string(description)<br>column.4.query.querysort=description<br>column.4.querysort=description{faly{445 {column.4.stretch=75<br>column.4.valuefield=description<br>column.4.valueformat=HTML<br>column.4.width=150<br>column.5.descriptionkey=status<br>column.5.enumclass=com.attask.common.constants.OpTaskStatusEnum<br>column.5.linkedname=direct<br>column.5.listort=string(status)<br>column(status){status){status.status.status.status.status.status{status.status {column.5.querysort=status<br>column.5.shortview=false<br>column.5.stretch=0<br>column.5.type=enum<br>column.5.valuefield=status<br>column.5.valueformat=val<br>column.5.width=150<br>column.6.displayname=Resolving Object Name<br>column.6.link=resolve6Tassalle<br>column.6.namekey.view.relatedcolumn.view.relatedcolumn.namekeyargkey.0=resolveTask<br>column.6.namekeyargkey.1=name<br>column.6.querysort=resolveTask：name<br>column.6.sharecol=true<br>column.6.textmode=true<br>column.6.valuefield=resolveTask：name<br>column.6.valueformat=HTML<br>column.7.displayname=<br>column.7.linkedname=resolveOpOpTaskTaskTaskTask{7Task7TaskTask<br>column.7 mekey=view.relatedcolumn<br>column.7.namekeyargkey.0=resolveOpTask<br>column.7.namekeyargkey.1=name<br>column.7.querysort=resolveOpTask：name<br>column.7.sharecol=true<br>column.7.valuefield=resolveOpTask：name<br>column.7.valueformat=HTML<br>column.82 column.8.linkedname=resolveProject<br>column.8.namekey=view.relatedcolumn<br>column.8.namekeyargkey.0=resolveProject<br>column.8.namekeyargkey.1=name<br>column.8.querysort=resolveProject：name<br>column.8.textmode=true<br>column.8.valuefield=resolveProject<br>column.9HTML9.displayname=解析對象完成百分比<br>列。9.textmode=true<br>列。9.valueexpression=IF(ISBLANK({resolveTask})。<br><br><br><br><br><br><br><br><br><br><br>{ID})，{resolveProject}。{percentComplete}，IF(ISBLANK({resolveProject}。{ID})，{resolveTask}。{percentComplete}，&quot;)<br>column.9.valueformat=doubleAsPercentRounded</pre>

1. 按一下「**儲存視圖**」。
