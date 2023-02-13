---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '''檢視：具有父任務資訊的小時數'
description: 此小時視圖顯示記錄小時的任務名稱以及父任務的名稱。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: c24555fc-3bae-451b-8a44-28a8158199d1
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '435'
ht-degree: 0%

---

# 查看：父任務資訊的小時數

此小時視圖顯示記錄小時的任務名稱以及父任務的名稱。

![custom_hour_view_with_task_and_parent_task_info.png](assets/custom-hour-view-with-task-and-parent-task-info-350x55.png)

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

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
   <td> <p>計劃 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>編輯對報表、控制面板、日曆的存取</p> <p>編輯對篩選器、檢視、群組的存取</p> <p>注意：如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>管理報表權限</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 查看具有父任務資訊的小時數

1. 去查一下小時清單。
1. 從 **檢視** 下拉式功能表，選取 **新建視圖**.

1. 在&#x200B;**欄預覽** 區域中，除一列外，刪除所有列。
1. 按一下剩餘欄的標題，然後按一下 **切換到文本模式**.
1. 將滑鼠移到文字模式區域上，然後按一下 **按一下「 」以編輯文字**.
1. 移除您在 **文字模式** 框中，並將其替換為以下代碼：
   <pre>column.0.aggregator.displayformat=doubleAsString<br>column.0.aggrator.function=SUM<br>column.0.aggregator.namekey=hours<br>column.0.aggregator.valuefield=hours<br>column.0.aggregator.valueformat=doubleAsDouble<br>column.0.descriptionkey=hours<br>column.0.link.linkproperty.0.name=ID<br>column.0.link.linkproperty.0.valuefield=ID<br>column.0.link.linkproperty.0.valueformat=int<br>column.0.link.lookup=link.view<br>column.0.link.valuefield=objCode<br>column.0.link.valueformat=val<br>column.0.linkedname=direct<br>column.0.listsort=doubleAsDouble(hours)<br>column.0.namekey=hours.abbr<br>column.0.querysort=hours<br>column.0.shortview=false<br>column.0.stretch=100<br>column.0.valuefield=hours<br>column.0.valueformat=doubleAsString<br>column.0.width=150<br>column.1.descriptionkey=task<br>column.1.link.linkproperty.0.name=ID<br>column.1.link.linkproperty.0.valuefield=task:ID<br>column.1.link.linkproperty.0.valueformat=int<br>column.1.link.lookup=link.view<br>column.1.link.valuefield=task:objCode<br>column.1.link.valueformat=val<br>column.1.linkedname=task<br>column.1.listsort=nested(task)。string(name)<br>column.1.namekey=task<br>column.1.querysort=task:name<br>column.1.shortview=false<br>column.1.stretch=0<br>column.1.valuefield=task:name<br>column.1.valueformat=HTML<br>column.1.width=150<br>column.2.description=父任務名稱<br>column.2.link.linkproperty.0.name=ID<br>column.2.link.linkproperty.0.valuefield=task:parent:ID<br>column.2.link.linkproperty.0.valueformat=int<br>column.2.link.lookup=link.view<br>column.2.link.valuefield=task:objCode<br>column.2.link.valueformat=val<br>column.2.linkedname=task<br>column.2.listsort=nested(task:parent)。string(name)<br>column.2.name=父任務名稱<br>column.2.querysort=task:parent:名稱<br>column.2.shortview=false<br>column.2.stretch=0<br>column.2.valuefield=task:parent:名稱<br>column.2.valueformat=HTML<br>column.2.width=150</pre>

1. 按一下 **保存視圖**.
