---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: 檢視：指派使用者的公司和主群組
description: 此任務檢視會顯示任務之主要擁有者的公司和主群組。 這些值在標準介面中無法使用，但可透過文字模式存取。
author: Nolan
feature: Reports and Dashboards
exl-id: 818c1f3a-4e82-4dc3-af86-4f9dcf5c11a4
source-git-commit: ecce7484423419823effa2cb41da892ba3fb207c
workflow-type: tm+mt
source-wordcount: '255'
ht-degree: 0%

---

# 檢視：指派使用者的公司和主群組

<!--Audited: 11/2024-->

此任務檢視會顯示任務之主要擁有者的公司和主群組。 這些值在標準介面中無法使用，但可透過文字模式存取。

![](assets/view--assigned-user-s-company-and-home-group-350x80.png)

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

## 檢視指派使用者的公司和主群組

1. 前往工作清單。
1. 從&#x200B;**檢視**&#x200B;下拉式功能表中，選取&#x200B;**新增檢視**。

1. 在&#x200B;**資料行預覽**&#x200B;區域中，排除除一個資料行以外的所有資料行。
1. 按一下剩餘欄的標題，然後按一下&#x200B;**切換到文字模式**。
1. 按一下&#x200B;**編輯文字模式**。
1. 移除您在&#x200B;**編輯文字模式**&#x200B;方塊中找到的文字，並取代為下列程式碼：

   ```
   column.0.descriptionkey=name
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
   column.0.shortview=false
   column.0.stretch=100
   column.0.valuefield=name
   column.0.valueformat=HTML
   column.0.width=150
   column.1.descriptionkey=assignedto
   column.1.link.linkproperty.0.name=ID
   column.1.link.linkproperty.0.valuefield=assignedTo:ID
   column.1.link.linkproperty.0.valueformat=int
   column.1.link.lookup=link.view
   column.1.link.valuefield=assignedTo:objCode
   column.1.link.valueformat=val
   column.1.linkedname=assignedTo
   column.1.listsort=nested(assignedTo).string(name)
   column.1.namekey=assignedto
   column.1.querysort=assignedTo:name
   column.1.shortview=false
   column.1.stretch=0
   column.1.valuefield=assignedTo:name
   column.1.valueformat=HTML
   column.1.width=150
   column.2.description=Assigned To Company
   column.2.displayname=Assigned To Company
   column.2.linkedname=assignedTo:company
   column.2.listsort=nested(assignedTo:company).string(name)
   column.2.namekey=assignedto
   column.2.querysort=assignedTo:company:name
   column.2.shortview=false
   column.2.stretch=0
   column.2.valuefield=assignedTo:company:name
   column.2.valueformat=HTML
   column.2.width=150
   column.3.description=Assigned To Home Group
   column.3.displayname=Assigned To Home Group
   column.3.linkedname=assignedTo:homeGroup
   column.3.listsort=nested(assignedTo:homeGroup).string(name)
   column.3.namekey=assignedto
   column.3.querysort=assignedTo:homeGroup:name
   column.3.shortview=false
   column.3.stretch=0
   column.3.valuefield=assignedTo:homeGroup:name
   column.3.valueformat=HTML
   column.3.width=150
   ```

1. 按一下&#x200B;**完成** > **儲存檢視**。
1. （選擇性）更新檢視名稱，然後按一下&#x200B;**儲存檢視**。
