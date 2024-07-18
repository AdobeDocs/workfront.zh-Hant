---
content-type: reference
product-area: reporting;projects;portfolios;programs
navigation-topic: custom-view-filter-and-grouping-samples
title: 「檢視：在任務檢視中顯示計畫和Portfolio資訊」
description: 此任務檢視會顯示與任務專案關聯的方案和Portfolio。 建立任務檢視時，Report Builder中不提供此資訊。 只有文字模式才有此資訊。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: cdd5a1e9-3cbf-4951-b803-fca544b2519a
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '485'
ht-degree: 0%

---

# 檢視：在作業檢視中顯示程式和Portfolio資訊

此任務檢視會顯示與任務專案關聯的方案和Portfolio。 建立任務檢視時，Report Builder中不提供此資訊。 只有文字模式才有此資訊。

檢視也會提供工作清單中的專案、方案和Portfolio連結。

![](assets/view--program-and-portfolio-350x116.png)

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

## 在任務檢視中顯示程式和Portfolio資訊

若要將此檢視套用至工作清單：

1. 前往工作清單。
1. 從&#x200B;**檢視**&#x200B;下拉式功能表中，選取&#x200B;**新增檢視**。

1. 在&#x200B;**資料行預覽**&#x200B;區域中，排除除一個資料行以外的所有資料行。
1. 按一下剩餘欄的標題，然後按一下&#x200B;**切換到文字模式**。
1. 將滑鼠移到文字模式區域上，然後按一下&#x200B;**按一下以編輯文字**。
1. 移除您在&#x200B;**文字模式**&#x200B;方塊中找到的文字，並取代為下列程式碼：
   <pre>column.0.descriptionkey=name<br>column.0.link.linkproperty.0.name=ID<br>column.0.link.linkproperty.0.valuefield=ID<br>column.0.link.linkproperty.0.valueformat=int<br>column.0.link.lookup=link.view<br>column.0.link.valuefield=objCode<br>column.0.link.valueformat=val<br>column.0.link.dname=direct<br>column.0.listort=string(name){name)<br>column.0.namekey=name.abbr<br>column.0.querysort=name<br>column.0.shortview=false<br>column.0.stretch=100<br>column.0.valuefield=name<br>column.0.valueformat=HTML<br>column.0.width=150<br>column.1.descriptionkey=project<br>column.1.link.link.name.0.name=ID<br>column.link.link.0.valuefield.valuefield.0.valuefield.valuefield=project ID<br>column.1.link.linkproperty.0.valueformat=int<br>column.1.link.lookup=link.view<br>column.1.link.valuefield=project：objCode<br>column.1.link.valueformat=val<br>column.1.linkedname=project<br>column.1.listsort=nested(project)。string(name)<br>column.1.namekey=project<br>column.1.querysort=project<br>column.1.project：name{project：{name<br>column.1.column .shortview=false<br>column.1.stretch=0<br>column.1.valuefield=project：name<br>column.1.valueformat=HTML<br>column.1.width=150<br>column.2.descriptionkey=program<br>column.2.displayname=Program<br>column.2.linkproperty.0.name=ID<br>column.2.link.0.valuefield=project:program:ID<br>列2 LINK.LINKPROPERTY.0.VALUEFORMAT=INT<br>COLUMN.2.LINK.LOOKUP=LINK.VIEW<br>COLUMN.2.LINK.VALUEFIELD=PROJECT:program:OBJCoDE<br>COLUMN.2.LINKEDNAME=PROJECT<br>COLUMN.2.LISTSORT=NESTED(PROJECT：PROGRAM)。STRING(NAME)<br>COLUMN.2.NAMEKEY=PROJECT<br>COLUMN.2.QUERYSORT=PROJECT:program:NAME<br>COLUMN.2 VIEW=FALSE<br>COLUMN.2.STRETCH=0<br>COLUMN.2.VALUEFIELD=PROJECT:program:NAME<br>COLUMN.2.VALUEFORMAT=HTML<br>COLUMN.2.WIDTH=150<br>COLUMN.3.DESCRIPTIONKEY=PORTFOLIO<br>COLUMN.3.DISPLAYNAME=Portfolio<br>COLUMN.3.LINKPROPERTY.0.NAME=ID<br>column.3.link.0.valuefield=project:portfolio:ID<br>COLUMN 3.LINK.LINKPROPERTY.0.VALUEFORMAT=INT<br>COLUMN.3.LINK.LOOKUP=LINK.VIEW<br>COLUMN.3.LINK.VALUEFIELD=PROJECT:portfolio:OBJCoDE<br>COLUMN.3.LINK.VALUEFORMAT=VAL<br>COLUMN.3.LINKEDNAME=PROJECT<br>COLUMN.3.LISTSORT=NESTED(PROJECT：PORTFOLIO)。STRING(NAME)<br>COLUMN.3.NAMEKEY=PROJECT<br>COLUMN.3.QUERYSORT=PROJECT<br>NAME{PROJECT{PROJECT}NAME.3.QUERYSORT=PROJECT{PROJECT:portfolio:NAME{PROJECT3}.SHORTVIEW=FALSE<br>COLUMN.3.STRETCH=0<br>COLUMN.3.VALUEFIELD=PROJECT:portfolio:NAME<br>COLUMN.3.VALUEFORMAT=HTML<br>COLUMN.3.WIDTH=150 </pre>

1. 按一下&#x200B;**儲存檢視**。
