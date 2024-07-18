---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 「檢視：任務和專案的原始問題詳細資訊」
description: 當問題轉換為任務或專案時，會在任務或專案與問題之間建立解決物件關係。 此檢視表會顯示任務或專案完成時自動完成的問題欄位。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 5fefb174-3a18-408f-aa12-3f4aff23acfa
source-git-commit: bcafa607da733b89747f6b448dd295d9b906d060
workflow-type: tm+mt
source-wordcount: '343'
ht-degree: 4%

---

# 檢視：任務和專案的原始問題詳細資訊

當問題轉換為任務或專案時，會在任務或專案與問題之間建立解決物件關係。 此檢視表會顯示任務或專案完成時自動完成之問題的下列欄位：

* 姓名
* 輸入日期
* 規劃完成日期
* 實際完成日期
* 請求類型
* 建立者名稱
* 指派給使用者

![task_with_resolving_issue_fields.png](assets/task-with-resolving-issue-fields-350x38.png)

如需詳細資訊，另請參閱[檢視：在任務與專案清單上顯示原始問題資訊](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-display-original-issue-info-task-project-list.md)。

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

## 檢視任務和專案的原始問題詳細資訊

1. 前往任務清單或專案清單。
1. 從&#x200B;**檢視**&#x200B;下拉式功能表中，選取&#x200B;**新增檢視**。

1. 在&#x200B;**資料行預覽**&#x200B;區域中，排除除一個資料行以外的所有資料行。
1. 按一下剩餘欄的標題，然後按一下&#x200B;**切換到文字模式**。
1. 將滑鼠移到文字模式區域上，然後按一下&#x200B;**按一下以編輯文字**。
1. 移除您在&#x200B;**文字模式**&#x200B;方塊中找到的文字，並取代為下列程式碼：

   <!-- [Copy](javascript:void(0);) -->
   <pre><code>column.0.textmode=false<br>column.0.valuefield=name<br>column.0.valueformat=HTML<br>column.0.descriptionkey=name<br>column.0.linkedname=direct<br>column.0.listsort=string(name)<br>column.0.namekey=name<br>column.0.querysort=name<br>column.0.shortview=false<br>column.0.stretch=100<br>column.0.width=150<br>column.1.displayname=Resolvables (Issues)<br>column.1.listdelimiter=<br><br>column.1.listmethod=nested(resolvables).lists<br>column.1.textmode=true<br>column.1.type=iterate<br>column.1.valueexpression={name}<br>column.1.valueformat=HTML<br>column.2.displayname=Resolvables Entry Date<br>column.2.listdelimiter=<br><br>column.2.listmethod=nested(resolvables).lists<br>column.2.textmode=true<br>column.2.type=iterate<br>column.2.valueexpression={entryDate}<br>column.2.valueformat=HTML<br>column.3.displayname=Resolvables Due Date<br>column.3.listdelimiter=<br><br>column.3.listmethod=nested(resolvables).lists<br>column.3.textmode=true<br>column.3.type=iterate<br>column.3.valueexpression={plannedCompletionDate}<br>column.3.valueformat=HTML<br>column.4.displayname=Resolvables Actual Completion Date<br>column.4.listdelimiter=<br><br>column.4.listmethod=nested(resolvables).lists<br>column.4.textmode=true<br>column.4.type=iterate<br>column.4.valueexpression={actualCompletionDate}<br>column.4.valueformat=HTML<br>column.5.displayname=Resolvables Request Type<br>column.5.listdelimiter=<br><br>column.5.listmethod=nested(resolvables).lists<br>column.5.textmode=true<br>column.5.type=iterate<br>column.5.valueexpression={opTaskType}<br>column.5.valueformat=HTML<br>column.6.displayname=Resolvables Originator<br>column.6.listdelimiter=<br><br>column.6.listmethod=nested(resolvables).lists<br>column.6.textmode=true<br>column.6.type=iterate<br>column.6.valueexpression={owner}.{name}<br>column.6.valueformat=HTML<br>column.7.descriptionkey=assignedto<br>column.7.linkedname=assignedTo<br>column.7.listsort=nested(assignedTo).string(name)<br>column.7.namekey=assignedto<br>column.7.querysort=assignedTo:name<br>column.7.shortview=false<br>column.7.stretch=0<br>column.7.textmode=true<br>column.7.valuefield=assignedTo:name<br>column.7.valueformat=HTML<br>column.7.width=150</code></pre>

1. 按一下「**儲存視圖**」。
