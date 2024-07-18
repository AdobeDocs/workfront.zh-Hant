---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 「檢視：顯示上層任務最多4層深」
description: 此任務檢視會在第一欄顯示任務名稱，並在相同清單的不同欄中顯示最多4個父系任務（如果存在）。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 66b45d64-794d-4adc-b208-2ded0dc9c5dc
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '513'
ht-degree: 0%

---

# 檢視：最多顯示4層深的父系任務

此任務檢視會在第一欄顯示任務名稱，並在相同清單的不同欄中顯示最多4個父系任務（如果存在）。

![parent_tasks_4_levels_deep.png](assets/parent-tasks-4-levels-deep-350x29.png)

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

## 顯示最多4層深的父系任務

1. 前往工作清單。
1. 從&#x200B;**檢視**&#x200B;下拉式功能表中，選取&#x200B;**新增檢視**。

1. 在&#x200B;**資料行預覽**&#x200B;區域中，排除除一個資料行以外的所有資料行。
1. 按一下剩餘欄的標題，然後按一下&#x200B;**切換到文字模式**。
1. 將滑鼠移到文字模式區域上，然後按一下&#x200B;**按一下以編輯文字**。
1. 移除您在&#x200B;**文字模式**&#x200B;方塊中找到的文字，並取代為下列程式碼：

   ```
   column.0.descriptionkey=name
   ```

   <pre>column.0.link.linkproperty.0.name=ID<br>column.0.link.linkproperty.0.valuefield=ID<br>column.0.link.linkproperty.0.valueformat=int<br>column.0.link.lookup=link.view<br>column.0.link.valuefield=objCode<br>column.0.link.valueformat=val<br>column.0.linkedname=direct<br>column.0.listort=string(name)<br>column.0.name.name=name.abbr.abbr<br>column.abbr 0.querysort=name<br>column.0.shortview=false<br>column.0.valuefield=name<br>column.0.valueformat=HTML<br>column.0.width=150<br>column.1.descriptionkey=parent<br>column.1.link.name=ID<br>column.1.link.property.0.valuefield.link.link.0.valueformat=int<br>.1.link.lookup=link.view<br>column.1.link.valuefield=parent：objCode<br>column.1.linkedname=parent<br>column.1.listsort=nested(parent)。string(name)<br>column.1.namekey=parent<br>column.1.querysort=parent：name<br>column.1.shortview=false<br>column.1.stretch=0<br>column.1.valuefield=0{parent.valuefield ：name<br>column.1.valueformat=HTML<br>column.1.width=150<br>column.2.description=Parent Parent<br>column.2.link.linkproperty.0.name=ID<br>column.2.link.linkproperty.0.valuefield=parent:parent:ID<br>column.2.link.link.lookup=link.view<br>column.link.valuefield :parent:objCode<br>column.2.link.valueformat=val<br>column.2.linkedname=parent<br>column.2.listsort=nested(parent：parent)。string(name)<br>column.2.name=Parent Parent<br>column.2.querysort=parent:parent:name<br>column.2.shortview=false<br>column.2.stretch=0<br>column.2.valuefield=parent:parent:name<br>name{name{valuevaluevaluevaluefield.2.valuefield.2.valuefield format=HTML<br>column.2.width=150<br>column.3.description=Parent Parent Parent<br>column.3.link.linkproperty.0.name=ID<br>column.3.link.linkproperty.0.valuefield=parent:parent:parent：ID<br>column.3.link.lookup=link.view<br>column.3.link.valuefield=parent:parent:obj代碼<br>column.3.link.valueformat=val<br>column.3.linkedname=parent<br>column.3.listsort=nested(parent:parent:parent)。string(name)<br>column.3.name=Parent Parent Parent<br>column.3.querysort=parent:parent:parent：name<br>column.3.short view=false<br>column.3.stretch=0<br>column.3.column.3.valuefield=parent:parent:parent{name<br>parent：name{valvalvalue.valuefield.column.3 ueformat=HTML<br>column.3.width=150<br>column.4.description=Parent Parent Parent<br>column.4.link.linkproperty.0.name=ID<br>column.4.linkproperty.0.valuefield=parent:parent:parent:parent:ID<br>column.4.linkproperty.0.valueformat=int<br>column.4.link.lookup.link=link.link.view{77 8}parent:parent:objCode<br>column.4.link.valueformat=val<br>column.4.linkedname=parent<br>column.4.listsort=nested(parent:parent:parent：parent)。string(name)<br>column.4.name=Parent Parent Parent Parent<br>column.4.querysort=parent:parent:name<br>column.4.short=false<br>column.4.stretch=10<br>column.4 valuefield=parent:parent:parent:parent:name<br>column.4.valueformat=HTML<br>column.4.width=150<br><br><br><br><br>:parent::parent:</pre>

1. 按一下「**儲存視圖**」。

   任務名稱會顯示在第一欄，如果任務有任何父系，則最多會在剩餘的欄中顯示4個父系。
