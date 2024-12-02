---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 檢視：以時數清單合併任務和問題詳細資訊
description: 此時數檢視結合了「任務」和「問題名稱」欄，以及使用sharecol標籤的「任務」和「問題計畫時數」。 由於小時條目只能屬於任務或問題，因此兩個物件不能同時出現在同一欄中。 檢視的每一行都會填入任務或問題的資訊。
author: Nolan
feature: Reports and Dashboards
exl-id: cf1137fd-c26a-4907-afe9-2373d3434631
source-git-commit: ecce7484423419823effa2cb41da892ba3fb207c
workflow-type: tm+mt
source-wordcount: '340'
ht-degree: 0%

---

# 檢視：在時數清單中合併任務和問題的詳細資訊

<!--Audited:11/2024-->

此時數檢視結合了「任務」和「問題名稱」欄，以及使用`sharecol`標籤的「任務」和「問題計畫時數」。 由於小時條目只能屬於任務或問題，因此兩個物件不能同時出現在同一欄中。 檢視的每一行都會填入任務或問題的資訊。

若要深入瞭解`sharecol`標籤，請參閱[檢視：合併一個共用資料行中多個資料行的資訊](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-merge-columns.md)。

![custom_view_hours_with_task_and_issue_information.png](assets/custom-view-hours-with-350x48.png)

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> 
    <p>新增：</p>
   <ul><li><p>修改篩選器的貢獻者 </p></li>
   <li><p>用於修改報告的標準</p></li> </ul>

<p>目前：</p>
   <ul><li><p>請求修改篩選器 </p></li>
   <li><p>計畫修改報表</p></li> </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>編輯報告、儀表板、行事曆的存取權以修改報告</p> <p>編輯篩選器、檢視和群組的存取權以修改篩選器</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>管理報表的許可權</p>  </td> 
  </tr> 
 </tbody> 
</table>

*如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 在時數清單中檢視合併的任務和問題詳細資訊

1. 前往時數清單。
1. 從&#x200B;**檢視**&#x200B;下拉式功能表，按一下&#x200B;**新增檢視**。
1. 在&#x200B;**資料行預覽**&#x200B;區域中，排除除一個資料行以外的所有資料行。
1. 按一下剩餘欄的標題，然後按一下&#x200B;**切換到文字模式** > **編輯文字模式**。
1. 移除您在&#x200B;**編輯文字模式**&#x200B;方塊中找到的文字，並取代為下列程式碼：

   ```
   column.1.querysort=project:name
   column.1.shortview=false
   column.1.stretch=0
   column.1.valuefield=project:name
   column.1.valueformat=HTML
   column.1.width=100
   column.2.description=Task or Issue
   column.2.link.linkproperty.0.name=ID
   column.2.link.linkproperty.0.valuefield=task:ID
   column.2.link.linkproperty.0.valueformat=int
   column.2.link.lookup=link.view
   column.2.link.valuefield=task:objCode
   column.2.link.valueformat=val
   column.2.linkedname=task
   column.2.listsort=nested(task).string(name)
   column.2.name=Task or Issue
   column.2.querysort=task:name
   column.2.sharecol=true
   column.2.shortview=false
   column.2.stretch=0
   column.2.valuefield=task:name
   column.2.valueformat=HTML
   column.2.width=100
   column.3.descriptionkey=optask
   column.3.link.linkproperty.0.name=ID
   column.3.link.linkproperty.0.valuefield=opTask:ID
   column.3.link.linkproperty.0.valueformat=int
   column.3.link.lookup=link.view
   column.3.link.valuefield=opTask:objCode
   column.3.link.valueformat=val
   column.3.linkedname=optask
   column.3.listsort=nested(opTask).string(name)
   column.3.namekey=opTask
   column.3.querysort=opTask:name
   column.3.shortview=false
   column.3.stretch=0
   column.3.valuefield=opTask:name
   column.3.valueformat=HTML
   column.3.width=1
   column.4.valuefield=task:work
   column.4.sharecol=true
   column.4.linkedname=task
   column.4.valueformat=doubleAsInt
   column.4.namekey=view.relatedcolumn
   column.4.querysort=task:work
   column.4.textmode=true
   column.4.namekeyargkey.0=task
   column.4.namekeyargkey.1=work
   column.4.displayname=Planned Effort
   column.5.displayname=Planned Effort
   column.5.viewalias=opTask:workrequired
   column.5.linkedname=opTask
   column.5.valuefield=opTask:workRequired
   column.5.valueformat=compound
   column.5.querysort=opTask:workRequired
   column.5.namekeyargkey.0=opTask
   column.5.namekeyargkey.1=workrequired
   column.5.namekey=view.relatedcolumn
   column.5.textmode=true
   column.6.descriptionkey=hours
   column.6.linkedname=direct
   column.6.listsort=doubleAsDouble(hours)
   column.6.namekey=hours.abbr
   column.6.querysort=hours
   column.6.shortview=false
   column.6.stretch=0
   column.6.valuefield=hours
   column.6.valueformat=doubleAsString
   column.6.width=75
   column.7.descriptionkey=entrydate
   column.7.linkedname=direct
   column.7.listsort=atDateAsAtDate(entryDate)
   column.7.namekey=entrydate.abbr
   column.7.querysort=entryDate
   column.7.shortview=false
   column.7.stretch=0
   column.7.valuefield=entryDate
   column.7.valueformat=atDate
   column.7.width=75
   column.8.descriptionkey=description
   column.8.linkedname=direct
   column.8.listsort=string(description)
   column.8.namekey=description.abbr
   column.8.querysort=description
   column.8.shortview=false
   column.8.stretch=0
   column.8.valuefield=description
   column.8.valueformat=HTML
   column.8.width=150
   ```

1. 按一下&#x200B;**完成** > **儲存檢視**。
1. （選擇性）更新檢視名稱，然後按一下&#x200B;**儲存檢視**。
