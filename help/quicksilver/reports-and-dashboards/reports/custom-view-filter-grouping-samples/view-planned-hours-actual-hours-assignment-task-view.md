---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 檢視：計畫時數與任務檢視中每個指派的實際時數
description: 此任務檢視顯示任務的總計畫時數、分配給每個受指派人的計畫時數（當任務受指派給多個使用者時）、任務的總實際時數以及每個受指派人記錄的實際時數。
author: Nolan
feature: Reports and Dashboards
exl-id: f249ff57-50c7-4aa9-a563-cb7f5562b96a
source-git-commit: 6405c01c8b1d842a4175f9caa18a7ed31316a3a1
workflow-type: tm+mt
source-wordcount: '290'
ht-degree: 0%

---

# 檢視：計畫時數與任務檢視中每個指派的實際時數

<!--Audited: 11/2024-->

此任務檢視顯示任務的總計畫時數、分配給每個受指派人的計畫時數（當任務受指派給多個使用者時）、任務的總實際時數以及每個受指派人記錄的實際時數。

![multi_assignment_budget_vs_actual_for_tasks.png](assets/multi-assignment-budget-vs-actual-for-tasks-350x66.png)

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
   <td role="rowheader">Adobe Workfront授權</td> 
   <td> <p> 目前： 
   <ul>
   <li>請求修改檢視</li> 
   <li>計畫修改報表</li>
   </ul>
     </p>
     <p> 新增： 
   <ul>
   <li>修改檢視的貢獻者</li> 
   <li>用於修改報告的標準</li>
   </ul>
     </p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>編輯報告、儀表板、行事曆的存取權以修改報告</p> <p>編輯對篩選器、檢視、群組的存取權以修改檢視</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>管理報表的許可權</p> </td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 在任務檢視中檢視每個指派的計畫時數vs.實際時數

1. 前往工作清單。
1. 從&#x200B;**檢視**&#x200B;下拉式功能表中，選取&#x200B;**新增檢視**。

1. 在&#x200B;**資料行預覽**&#x200B;區域中，排除除一個資料行以外的所有資料行。
1. 按一下剩餘欄的標頭，然後按一下&#x200B;**切換到文字模式** > **編輯文字模式**。
1. 移除您在&#x200B;**編輯文字模式**&#x200B;方塊中找到的文字，並取代為下列程式碼：

   ```
   column.0.descriptionkey=name
   column.0.isInlineEditable=false
   column.0.link.linkproperty.0.name=ID
   column.0.link.linkproperty.0.valuefield=ID
   column.0.link.linkproperty.0.valueformat=int
   column.0.link.lookup=link.view
   column.0.link.valuefield=objCode
   column.0.link.valueformat=val
   column.0.linkedname=direct
   column.0.listsort=string(name)
   column.0.namekey=name.abbr
   column.0.querysort=name
   column.0.section=0
   column.0.shortview=false
   column.0.stretch=0
   column.0.valuefield=name
   column.0.valueformat=HTML
   column.0.width=150
   column.1.descriptionkey=workrequired
   column.1.isInlineEditable=false
   column.1.linkedname=direct
   column.1.listsort=doubleAsDouble(workRequired)
   column.1.namekey=workrequired.abbr
   column.1.querysort=workRequired
   column.1.section=0
   column.1.shortview=false
   column.1.stretch=0
   column.1.valuefield=workFieldLong
   column.1.valueformat=compound
   column.1.viewalias=workrequired
   column.1.width=100
   column.2.listdelimiter=
   column.2.listmethod=nested(assignments).lists
   column.2.name=Wrk Assignment(s)
   column.2.stretch=0
   column.2.type=iterate
   column.2.valueexpression=CONCAT(right(CONCAT('~~~',{assignmentPercent}),3),'% (', {workRequired}/60 ,' Hours) - ',{assignedTo}.{name})
   column.2.valueformat=HTML
   column.2.width=300
   column.3.descriptionkey=actualworkrequired
   column.3.isInlineEditable=false
   column.3.linkedname=direct
   column.3.listsort=intAsInt(actualWorkRequired)
   column.3.namekey=actualworkrequired.abbr
   column.3.querysort=actualWork
   column.3.section=0
   column.3.shortview=false
   column.3.stretch=100
   column.3.valuefield=actualWorkFieldLong
   column.3.valueformat=compound
   column.3.viewalias=actualworkrequired
   column.3.width=100
   column.4.listdelimiter=
   column.4.listmethod=nested(hours).lists
   column.4.name=Actual Hours
   column.4.stretch=0
   column.4.type=iterate
   column.4.valueexpression=CONCAT('(', {hours} ,' Hours) - ',{owner}.{name})
   column.4.valueformat=HTML
   column.4.width=300
   ```

1. 按一下&#x200B;**完成** > **儲存檢視**。
