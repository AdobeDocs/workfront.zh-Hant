---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: 「查看：已分配用戶的公司和家庭組」
description: 此任務視圖顯示任務的主要所有者的公司和主組。 這些值在標準介面中不可用，但可透過文字模式存取。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 818c1f3a-4e82-4dc3-af86-4f9dcf5c11a4
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '461'
ht-degree: 0%

---

# 查看：已分配用戶的公司和主組

此任務視圖顯示任務的主要所有者的公司和主組。 這些值在標準介面中不可用，但可透過文字模式存取。

![](assets/view--assigned-user-s-company-and-home-group-350x80.png)

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

## 查看已分配用戶的公司和家庭組

1. 轉到任務清單。
1. 從 **檢視** 下拉式功能表，選取 **新建視圖**.

1. 在&#x200B;**欄預覽** 區域中，除一列外，刪除所有列。
1. 按一下剩餘欄的標題，然後按一下 **切換到文本模式**.
1. 將滑鼠移到文字模式區域上，然後按一下 **按一下「 」以編輯文字**.
1. 移除您在 **文字模式** 框中，並將其替換為以下代碼：
   <pre>column.0.descriptionkey=name<br> column.0.link.linkproperty.0.name=ID<br> column.0.link.linkproperty.0.valuefield=ID<br> column.0.link.linkproperty.0.valueformat=int<br> column.0.link.lookup=link.view<br> column.0.link.valuefield=objCode<br> column.0.link.valueformat=val<br> column.0.linkedname=direct<br> column.0.listsort=string(name)<br> column.0.namekey=name.abbr<br> column.0.querysort=name<br> column.0.shortview=false<br> column.0.stretch=100<br> column.0.valuefield=name<br> column.0.valueformat=HTML<br> column.0.width=150<br> column.1.descriptionkey=assignedto<br> column.1.link.linkproperty.0.name=ID<br> column.1.link.linkproperty.0.valuefield=assignedTo:ID<br> column.1.link.linkproperty.0.valueformat=int<br> column.1.link.lookup=link.view<br> column.1.link.valuefield=assignedTo:objCode<br> column.1.link.valueformat=val<br> column.1.linkedname=assignedTo<br> column.1.listsort=nested(assignedTo)。string(name)<br> column.1.namekey=assignedto<br> column.1.querysort=assignedTo:name<br> column.1.shortview=false<br> column.1.stretch=0<br> column.1.valuefield=assignedTo:name<br> column.1.valueformat=HTML<br> column.1.width=150<br> column.2.description=分配給公司<br> column.2.displayname=已分配給公司<br> column.2.linkedname=assignedTo:company<br> column.2.listsort=nested(assignedTo:company)。string(name)<br> column.2.namekey=assignedto<br> column.2.querysort=assignedTo:company:名稱<br> column.2.shortview=false<br> column.2.stretch=0<br> column.2.valuefield=assignedTo:company:名稱<br> column.2.valueformat=HTML<br> column.2.width=150<br> column.3.description=分配給主組<br> column.3.displayname=已分配給主組<br> column.3.linkedname=assignedTo:homeGroup<br> column.3.listsort=nested(assignedTo:homeGroup)。string(name)<br> column.3.namekey=assignedto<br> column.3.querysort=assignedTo:homeGroup:名稱<br> column.3.shortview=false<br> column.3.stretch=0<br> column.3.valuefield=assignedTo:homeGroup:名稱<br> column.3.valueformat=HTML<br> column.3.width=150</pre>

1. 按一下 **儲存變更**.
