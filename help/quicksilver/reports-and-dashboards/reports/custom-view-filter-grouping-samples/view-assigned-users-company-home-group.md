---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: 「檢視：指派使用者的公司和主群組」
description: 此任務檢視會顯示任務之主要擁有者的公司和主群組。 這些值在標準介面中無法使用，但可透過文字模式存取。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 818c1f3a-4e82-4dc3-af86-4f9dcf5c11a4
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '426'
ht-degree: 0%

---

# 檢視：指派使用者的公司和主群組

此任務檢視會顯示任務之主要擁有者的公司和主群組。 這些值在標準介面中無法使用，但可透過文字模式存取。

![](assets/view--assigned-user-s-company-and-home-group-350x80.png)

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

## 檢視指派使用者的公司和主群組

1. 前往工作清單。
1. 從&#x200B;**檢視**&#x200B;下拉式功能表中，選取&#x200B;**新增檢視**。

1. 在&#x200B;**資料行預覽**&#x200B;區域中，排除除一個資料行以外的所有資料行。
1. 按一下剩餘欄的標題，然後按一下&#x200B;**切換到文字模式**。
1. 將滑鼠移到文字模式區域上，然後按一下&#x200B;**按一下以編輯文字**。
1. 移除您在&#x200B;**文字模式**&#x200B;方塊中找到的文字，並取代為下列程式碼：
   <pre>column.0.descriptionkey=name<br> column.0.link.linkproperty.0.name=ID<br> column.0.link.linkproperty.0.valuefield=ID<br> column.0.link.linkproperty.0.valueformat=int<br> column.0.link.lookup=link.view<br> column.0.link.valuefield=objCode<br> column.0.link.valueformat=val<br> column.0.linkdname=direct<br> column.0.listort=string(name){name)<br> column.0.namekey=name.abbr<br> column.0.querysort=name<br> column.0.shortview=false<br> column.0.stretch=100<br> column.0.valuefield=name<br> column.0.valueformat=HTML<br> column.0.width=150<br> column.1.descriptionkey=assignedto<br> column.1.link.link.name.name=ID<br> column.link.link.link.link.linkproperty.0.valueproperty.0.valuevalueproperty.valueid field=assignedTo：ID<br> column.1.link.linkproperty.0.valueformat=int<br> column.1.link.lookup=link.view<br> column.1.link.valuefield=assignedTo：objCode<br> column.1.link.valueformat=val<br> column.1.linkedname=assignedTo<br> column.1.listsort=nested(assignedTo)。string(name)<br> column(name)<br> column.1.querysort=assignedTo：name<br> column.1.shortview=false<br> column.1.stretch=0<br> column.1.valuefield=assignedTo：name<br> column.1.valueformat=HTML HTML<br> column.1.width=150<br> column.2.description=Assigned To Company<br> column.2.linkedname=assignedTo：company<br> column.liststable sort=nested(assignedTo：company)。string(name)<br> column.2.namekey=assignedto<br> column.2.querysort=assignedTo:company:name<br> column.2.shortview=false<br> column.2.stretch=0<br> column.2.valuefield=assignedTo:company:name<br> column.2.valueformat=150<br> column.column.description=分配給主組{4 5} column.3.displayname=分配給主組<br> column.3.linkedname=assignedTo：homeGroup<br> column.3.listsort=nested(assignedTo：homeGroup)。string(name)<br> column.3.namekey=assignedto<br> column.3.querysort=assignedTo:homeGroup:name<br> column.3.short=false<br> column.3.stretch=0<br> column=0<br> column 4}name<br> column.3.valueformat=HTML<br> column.3.width=150<br><br>:homeGroup:</pre>

1. 按一下「**儲存變更**」。
