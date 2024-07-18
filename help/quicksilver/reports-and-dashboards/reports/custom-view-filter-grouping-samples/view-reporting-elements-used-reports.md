---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 「檢視：報表中使用的報表元素」
description: 當您在報告清單中使用每個報告時，此檢視會顯示用來在Adobe Workfront中建立每個報告的檢視、篩選和分組。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 67f86523-e136-4768-af93-586a107b106f
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '370'
ht-degree: 1%

---

# 檢視：報表中使用的報表元素

當您在報告清單中使用每個報告時，此檢視會顯示用來在Adobe Workfront中建立每個報告的檢視、篩選和分組。

您可以看到

```
valuefields
```

或

```
valueexpressions
```

用於報告的每個元素。

![report_with_elements_definitions.png](assets/report-with-elements-definitions-350x130.png)

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

## 檢視報告中使用的報告元素

1. 前往報告清單。
1. 從&#x200B;**檢視**&#x200B;下拉式功能表中，選取&#x200B;**新增檢視**。

1. 在&#x200B;**資料行預覽**&#x200B;區域中，排除除一個資料行以外的所有資料行。
1. 按一下剩餘欄的標題，然後按一下&#x200B;**切換到文字模式**。
1. 將滑鼠移到文字模式區域上，然後按一下&#x200B;**按一下以編輯文字**。
1. 移除您在&#x200B;**文字模式**&#x200B;方塊中找到的文字，並取代為下列程式碼：
   <pre>column.0.descriptionkey=name<br>column.0.link.linkproperty.0.name=ID<br>column.0.link.linkproperty.0.valuefield=ID<br>column.0.link.linkproperty.0.valueformat=string<br>column.0.link.lookup=link.run<br>column.0.link.value=val(objCode)<br>column.0.listsort=string(name)<br>column.0.name=name.abbr<br>column.0.querysort=name<br>column.column.0.valuefield=name<br>column.0.valueformat=HTML<br>column.0.width=200<br>column.1.descriptionkey=objecttype<br>column.1.listsort=nested(view)。string(uiObjCode)<br>column.1.namekey=objecttype.abbr<br>column.1.querysort=uiObjCode<br>column.1 valueformat=objCodeMessage<br>column.1.width=80<br>column.2.descriptionkey=enteredby<br>column.2.listsort=nested(enteredBy)。string(lastName)<br>column.2.namekey=enteredby.abbr<br>column.2.querysort=enteredBy：lastName<br>column.2.valuefield=enteredBy：name<br>column.2.valueformat=HTML<br>column 2.width=130<br>column.3.displayname=Filter definition<br>column.3.textmode=true<br>column.3.valuefield=filter：definition<br>column.3.valueformat=HTML<br>column.4.displayname=View definition<br>column.4.textmode=true<br>column.4.valuefield=view<br>column.5.displayname=HTML{disgrouedefinition<br>.5.textmode=true<br>column.5.valuefield=groupBy：definition<br>column.5.valueformat=HTML<br><br><br></pre>

1. 按一下「**儲存視圖**」。
