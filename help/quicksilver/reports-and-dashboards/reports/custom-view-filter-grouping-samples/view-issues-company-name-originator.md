---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: 「檢視：建立者的公司名稱問題」
description: 此問題檢視會顯示與提交問題之使用者相關聯的公司名稱。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: e628f7cf-4a7b-4125-bea6-348c72477bd7
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '407'
ht-degree: 0%

---

# 檢視：建立者的公司名稱問題

此問題檢視會顯示與提交問題之使用者相關聯的公司名稱。

![custom_view_for_issues_with_originator_company_name.png](assets/custom-view-for-issues-350x33.png)

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

## 檢視建立者的公司名稱問題

若要套用此檢視：

1. 前往問題清單。
1. 從&#x200B;**檢視**&#x200B;下拉式功能表中，選取&#x200B;**新增檢視**。

1. 在&#x200B;**資料行預覽**&#x200B;區域中，排除除一個資料行以外的所有資料行。
1. 按一下剩餘欄的標題，然後按一下&#x200B;**切換到文字模式**。
1. 將滑鼠移到文字模式區域上，然後按一下&#x200B;**按一下以編輯文字**。
1. 移除您在&#x200B;**文字模式**&#x200B;方塊中找到的文字，並取代為下列程式碼：
   <pre>column.0.descriptionkey=name<br>column.0.link.linkproperty.0.name=ID<br>column.0.link.linkproperty.0.valuefield=ID<br>column.0.link.linkproperty.0.valueformat=val<br>column.0.link.lookup=link.view<br>column.0.link.value=val(objCode)<br>column.0.listsort=string(name)<br>column.0.name=name<br>column.0.querysort=name<br>column.valuname.0.valuuuuename.valuum.valuuuuue efield=name<br>column.0.valueformat=HTML<br>column.0.width=140<br>column.1.descriptionkey=originator<br>column.1.link.linkproperty.0.name=ID<br>column.1.link.linkproperty.0.valuefield=ownerID<br>column.1.link.link.lookup=link.view<br>column.link.valuefield=owner ：objCode<br>column.1.link.valueformat=val<br>column.1.listsort=nested(owner)。string(name)<br>column.1.namekey=originator.abbr<br>column.1.querysort=owner：name<br>column.1.valueformat=HTML<br>column.1.width=151<br>column.2.descriptionkey=entrydate<br>column.lim.2 stsort=atDateAsAtDate(entryDate)<br>column.2.namekey=entrydate.abbr<br>column.2.querysort=entryDate<br>column.2.valuefield=entryDate<br>column.2.valueformat=atDate<br>column.2.width=75<br>column.3.descriptionkey=age<br>column.doubleAsDouble(age)<br>column.3.name key=age<br>column.3.querysort=age<br>column.3.valuefield=howOld<br>column.3.valueformat=val<br>column.3.width=80<br>column.4.viewalias=statusicons<br>column.4.displayname=Flags<br>column.4.linkedname=direct<br>column.4.namekey=statusicons<br>column.4.valuefield=<br>column.4.valueformat=HTML <br>column.4.querysort=<br>column.4.tile.name=component.issuestatusicons<br>column.4.tile.pdfcomponent=issueStatusIcons<br>column.4.delimiter=<br>column.4.tile.template=/WEB-INF/jsp/lists/components/issueStatusIcons.jsp<br>column.5.description=Originator的公司名稱<br>column.5.link.link.0.name=ID<br>column.link.linkproperty.0.valuefield=owner.0.valuefield=owner：companyID{5 2}column.5.link.linkproperty.0.valueformat=int<br>column.5.link.lookup=link.view<br>column.5.link.valuefield=owner:company:objCode<br>column.5.link.valueformat=val<br>column.5.listsort=nested(owner：company)。string(name)<br>column.5.name=Originator公司<br>column.5.querysort=owwner:company:name<br>name{name{name.5.valuefield.valuefield所有者:company:name<br>column.5.valueformat=HTML<br>column.5.width=151<br><br><br></pre>

1. 按一下「**儲存視圖**」。
