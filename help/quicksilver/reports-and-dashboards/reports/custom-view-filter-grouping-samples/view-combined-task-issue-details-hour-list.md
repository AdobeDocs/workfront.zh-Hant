---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 「檢視：在時數清單中合併任務和問題的詳細資訊」
description: 此時數檢視結合了「任務」和「問題名稱」欄，以及使用sharecol標籤的「任務」和「問題計畫時數」。 由於小時條目只能屬於任務或問題，因此兩個物件不能同時出現在同一欄中。 檢視的每一行都會填入任務或問題的資訊。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: cf1137fd-c26a-4907-afe9-2373d3434631
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '584'
ht-degree: 0%

---

# 檢視：在時數清單中合併任務和問題的詳細資訊

此時數檢視結合了「任務」和「問題名稱」欄，以及使用

```
sharecol
```

標籤之間。 由於小時條目只能屬於任務或問題，因此兩個物件不能同時出現在同一欄中。 檢視的每一行都會填入任務或問題的資訊。

若要進一步瞭解

```
sharecol
```

標籤中，請參閱[檢視：合併一個共用資料行](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-merge-columns.md)中多個資料行的資訊。\
![custom_view_hours_with_task_and_issue_information.png](assets/custom-view-hours-with-350x48.png)

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

## 在時數清單中檢視合併的任務和問題詳細資訊

若要套用此檢視：

1. 前往時數清單。
1. 從&#x200B;**檢視**&#x200B;下拉式功能表中，選取&#x200B;**新增檢視**。

1. 在&#x200B;**資料行預覽**&#x200B;區域中，排除除一個資料行以外的所有資料行。
1. 按一下剩餘欄的標題，然後按一下&#x200B;**切換到文字模式**。
1. 將滑鼠移到文字模式區域上，然後按一下&#x200B;**按一下以編輯文字**。
1. 移除您在&#x200B;**文字模式**&#x200B;方塊中找到的文字，並取代為下列程式碼：
   <pre>column.1.querysort=project：name<br>column.1.shortview=false<br>column.1.stretch=0<br>column.1.valuefield=project：name<br>column.1.valueformat=HTML<br>column.1.width=100<br>column.2.description=Task或Issue<br>column.2.link.linkproperty.0.name=ID<br>column.0.valuefield：ID<br>column.link.link.0.valueformat=int{int}int{int column.2.link.lookup=link.view<br>column.2.link.valuefield=task：objCode<br>column.2.linkedname=task<br>column.2.listsort=nested(task)。string(name)<br>column.2.name=Task或Issue<br>column.2.querysort=task：name<br>column.2.sharecol=true<br>column.2.short=false<br>column.stretation =0<br>列。2.valuefield=任務：名稱<br>列。2.valueformat=HTML<br>列。2.width=100<br>列。3.descriptionkey=optask<br>列。3.link.linkproperty.0.name=ID<br>列。3.link.linkproperty.0.valuefield=opTask：ID<br>列。3.link.link.0.valueformat=int<br>列。3.link.lookup.link view<br>column.3.link.valuefield=opTask：objCode<br>column.3.link.valueformat=val<br>column.3.linkedname=optask<br>column.3.listsort=nested(opTask)。string(name)<br>column.3.namekey=opTask<br>column.3.querysort=opTask：name<br>column.3.stretation=false.3.3.stretasn.3.valuefield =opTask：name<br>column.3.valueformat=HTML<br>column.3.width=1<br>column.4.valuefield=task：work<br>column.4.sharecol=true<br>column.4.linkedname=task<br>column.4.valueformat=doubleAsInt<br>column.4.namekey=view.relatedcolumn<br>column.4.querysort=task：work<br>column.true<br>column.true.namekeyargkey.0=task<br>column.4.namekeyargkey.1=work<br>column.4.displayname=計畫投入<br>column.5.displayname=計畫投入<br>column.5.viewalias=opTask：workrequired<br>column.5.valuefield=opTask：workRequired<br>column.5.valueformat=compound<br>column.5.querysort=opTask：op必需<br>column.5.namekeyargkey.0=opTask<br>column.5.namekeyargkey.1=workrequired<br>column.5.namekey=view.relatedcolumn<br>column.5.textmode=true<br>column.6.descriptionkey=hours<br>column.6.linkedname=direct<br>column.6.listsort=doubleAsDouble(hours)<br>column.61}column.6.namekey=hours.abbr<br>column.namequerysort=hours =hours<br>column.6.shortview=false<br>column.6.stretch=0<br>column.6.valuefield=hours<br>column.6.valueformat=doubleAsString<br>column.6.width=75<br>column.7.descriptionkey=entrydate<br>column.7.linkedname=direct<br>column.7.listsort=atAsAsAtAtDate(entDate)<br>column.7.name=entrydate.abbr<br>column.7.querysort=entryDate<br>column.7.shortview=false<br>column.7.stretch=0<br>column.7.valuefield=entryDate<br>column.7.valueformat=atDate<br>column.7.width=75<br>column.8.descriptionkey=description<br>column.8.linkedname=direct<br>column.listort=string(description)<br>column.8.name.name.name.abmekey=string br<br>column.8.querysort=description<br>column.8.shortview=false<br>column.8.stretch=0<br>column.8.valuefield=description<br>column.8.valueformat=HTML<br>column.8.width=150<br><br><br><br><br></pre>

1. 按一下「**儲存視圖**」。
