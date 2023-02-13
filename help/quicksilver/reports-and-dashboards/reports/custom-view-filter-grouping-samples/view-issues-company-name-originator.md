---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: '''檢視：創作者的公司名稱問題'
description: 此問題視圖顯示與提交問題的用戶關聯的公司名稱。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: e628f7cf-4a7b-4125-bea6-348c72477bd7
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '464'
ht-degree: 0%

---

# 查看：創作者的公司名稱問題

此問題視圖顯示與提交問題的用戶關聯的公司名稱。

![custom_view_for_issues_with_originator_company_name.png](assets/custom-view-for-issues-350x33.png)

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

## 查看創始方的公司名稱問題

要應用此視圖，請執行以下操作：

1. 前往問題清單。
1. 從 **檢視** 下拉式功能表，選取 **新建視圖**.

1. 在&#x200B;**欄預覽** 區域中，除一列外，刪除所有列。
1. 按一下剩餘欄的標題，然後按一下 **切換到文本模式**.
1. 將滑鼠移到文字模式區域上，然後按一下 **按一下「 」以編輯文字**.
1. 移除您在 **文字模式** 框中，並將其替換為以下代碼：
   <pre>column.0.descriptionkey=name<br>column.0.link.linkproperty.0.name=ID<br>column.0.link.linkproperty.0.valuefield=ID<br>column.0.link.linkproperty.0.valueformat=val<br>column.0.link.lookup=link.view<br>column.0.link.value=val(objCode)<br>column.0.listsort=string(name)<br>column.0.namekey=name<br>column.0.querysort=name<br>column.0.valuefield=name<br>column.0.valueformat=HTML<br>column.0.width=140<br>column.1.descriptionkey=originator<br>column.1.link.linkproperty.0.name=ID<br>column.1.link.linkproperty.0.valuefield=ownerID<br>column.1.link.linkproperty.0.valueformat=int<br>column.1.link.lookup=link.view<br>column.1.link.valuefield=owner:objCode<br>column.1.link.valueformat=val<br>column.1.listsort=nested(owner)。string(name)<br>column.1.namekey=originator.abbr<br>column.1.querysort=owner:name<br>column.1.valuefield=owner:name<br>column.1.valueformat=HTML<br>column.1.width=151<br>column.2.descriptionkey=entrydate<br>column.2.listsort=atDateAsAtDate(entryDate)<br>column.2.namekey=entrydate.abbr<br>column.2.querysort=entryDate<br>column.2.valuefield=entryDate<br>column.2.valueformat=atDate<br>column.2.width=75<br>column.3.descriptionkey=age<br>column.3.listsort=doubleAsDouble(age)<br>column.3.namekey=age<br>column.3.querysort=age<br>column.3.valuefield=howOld<br>column.3.valueformat=val<br>column.3.width=80<br>column.4.viewalias=statusicons<br>column.4.displayname=Flags<br>column.4.linkedname=direct<br>column.4.namekey=statusicons<br>column.4.valuefield=<br>column.4.valueformat=HTML<br>column.4.querysort=<br>column.4.tile.name=component.issuestatusicons<br>column.4.tile.pdfcomponent=issueStatusIcons<br>column.4.delimiter=<br>column.4.tile.template=/WEB-INF/jsp/lists/components/issueStatusIcons.jsp<br>column.5.description=創作者的公司名稱<br>column.5.link.linkproperty.0.name=ID<br>column.5.link.linkproperty.0.valuefield=owner:companyID<br>column.5.link.linkproperty.0.valueformat=int<br>column.5.link.lookup=link.view<br>column.5.link.valuefield=owner:company:objCode<br>column.5.link.valueformat=val<br>column.5.listsort=nested(owner:company)。string(name)<br>column.5.name=Originator公司<br>column.5.querysort=owner:company:名稱<br>column.5.valuefield=owner:company:名稱<br>column.5.valueformat=HTML<br>column.5.width=151</pre>

1. 按一下 **保存視圖**.
