---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 「檢視：核准資訊的問題」
description: 以下問題檢視顯示核准流程、步驟、核准者名稱和授予核准前問題的狀態。 有些欄位無法透過標準介面產生器存取。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 4e123844-a0d6-474b-87fb-d30ed391ad07
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '464'
ht-degree: 0%

---

# 檢視：核准資訊的問題

以下問題檢視顯示核准流程、步驟、核准者名稱和授予核准前問題的狀態。 有些欄位無法透過標準介面產生器存取。

![custom_issue_view_with_approval_info.png](assets/custom-issue-view-with-approval-info-350x46.png)

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

## 檢視核准資訊的問題

1. 前往問題清單。
1. 從&#x200B;**檢視**&#x200B;下拉式功能表中，選取&#x200B;**新增檢視**。

1. 在&#x200B;**資料行預覽**&#x200B;區域中，排除除一個資料行以外的所有資料行。
1. 按一下剩餘欄的標題，然後按一下&#x200B;**切換到文字模式**。
1. 將滑鼠移到文字模式區域上，然後按一下&#x200B;**按一下以編輯文字**。
1. 移除您在&#x200B;**文字模式**&#x200B;方塊中找到的文字，並取代為下列程式碼：
   <pre style="font-style: normal;">column.0.descriptionkey=name<br>column.0.link.linkproperty.0.name=ID<br>column.0.link.linkproperty.0.valuefield=ID<br>column.0.link.linkproperty.0.valueformat=int<br>column.0.link.lookup=link.view<br>column.0.link.valuefield=objCode<br>column.0.link.valueformat=val<br>column.0.link.dname=direct<br>column.0.listort=string(name){name)<br>column.0.namekey=name.abbr<br>column.0.querysort=name<br>column.0.shortview=false<br>column.0.stretch=40<br>column.0.valuefield=name<br>column.0.valueformat=HTML<br>column.0.width=220<br>column.1.descriptionkey=assignedto<br>column.1.listort=nestalled(assignedTo){stringTo)。string(name)。string(name) 18}column.1.namekey=assignedto<br>column.1.querysort=assignedTo：name<br>column.1.shortview=true<br>column.1.stretch=0<br>column.1.valuefield=assignedTo：name<br>column.1.valueformat=HTML<br>column.1.width=150<br>column.2.descriptionkey=role<br>column.2.linkedname=role{role<br>column.2.2.linkedname=role{role{role{role<br>column.2.2.2.listsort role)。string(name)<br>column.2.namekey=role<br>column.2.querysort=role：name<br>column.2.shortview=false<br>column.2.stretch=25<br>column.2.valuefield=name<br>column.2.valueformat=HTML<br>column.2.width=150<br>column.3.description=批准流程名稱<br>column.3.linkedname=direct<br>column.3.listsort=string （名稱）<br>column.3.name=批准流程名稱<br>column.3.querysort=name<br>column.3.shortview=false<br>column.3.stretch=35<br>column.3.valuefield=approvalProcess：name<br>column.3.valueformat=HTML<br>column.3.width=220<br>column.4.description=批准步驟名稱<br>column.linkedname=direct<br>column.listort.string=direct{direct{direct<br>column.listort （名稱）<br>column.4.name=批准步驟名稱<br>column.4.querysort=name<br>column.4.shortview=false<br>column.4.stretch=0<br>column.4.valuefield=currentApprovalStep：name<br>column.4.valueformat=HTML<br>column.4.width=220<br>column.5.description=Previous<br>column.5.linkedname=direct<br>column.5.listort(direct（字串） name)<br>column.5.name=Previous Status<br>column.5.querysort=name<br>column.5.shortview=false<br>column.5.stretch=0<br>column.5.valuefield=previousStatus<br>column.5.valueformat=HTML<br>column.5.width=220<br>column.6.linkedname=direct<br>column.6.listort=HTML(approvers){approvers7}column.6.namekey=approkey ver.plural.abbr<br>column.6.querysort=approversString<br>column.6.shortview=false<br>column.6.stretch=0<br>column.6.valuefield=approversString<br>column.6.valueformat=HTML<br>column.6.viewalias=approver.plural<br>column.6.width=200<br><br></pre>

1. 按一下「**儲存視圖**」。
