---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 檢視：任務和專案的原始問題詳細資訊
description: 當問題轉換為任務或專案時，會在任務或專案與問題之間建立解決物件關係。 此檢視表會顯示任務或專案完成時自動完成的問題欄位。
author: Nolan
feature: Reports and Dashboards
exl-id: 5fefb174-3a18-408f-aa12-3f4aff23acfa
source-git-commit: 6405c01c8b1d842a4175f9caa18a7ed31316a3a1
workflow-type: tm+mt
source-wordcount: '310'
ht-degree: 3%

---

# 檢視：任務和專案的原始問題詳細資訊

<!--Audited: 11/2024-->

當問題轉換為任務或專案時，會在任務或專案與問題之間建立解決物件關係。 此檢視表會顯示任務或專案完成時自動完成之問題的下列欄位：

* 姓名
* 輸入日期
* 規劃完成日期
* 實際完成日期
* 請求類型
* 建立者名稱
* 指派給使用者

![task_with_resolving_issue_fields.png](assets/task-with-resolving-issue-fields-350x38.png)

如需詳細資訊，另請參閱[檢視：在任務或專案清單上顯示原始問題資訊](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-display-original-issue-info-task-project-list.md)。

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
   <td role="rowheader">Adobe Workfront授權</td> 
   <td> <p> 目前： 
   <ul>
   <li>請求修改檢視</li> 
   <li>計畫修改報表</li>
   </ul>
     </p>
     <p> 新增： 
   <ul>
   <li>修改檢視的貢獻者</li> 
   <li>用於修改報告的標準</li>
   </ul>
     </p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>編輯報告、儀表板、行事曆的存取權以修改報告</p> <p>編輯對篩選器、檢視、群組的存取權以修改檢視</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>管理報表的許可權</p> </td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 檢視任務和專案的原始問題詳細資訊

1. 前往任務清單或專案清單。
1. 從&#x200B;**檢視**&#x200B;下拉式功能表中，選取&#x200B;**新增檢視**。
1. 在&#x200B;**資料行預覽**&#x200B;區域中，排除除一個資料行以外的所有資料行。
1. 按一下剩餘欄的標題，然後按一下&#x200B;**切換到文字模式**，然後按&#x200B;**編輯文字模式**。
1. 移除您在&#x200B;**編輯文字模式**&#x200B;方塊中找到的文字，並取代為下列程式碼：

   ```
   column.0.textmode=false
   column.0.valuefield=name
   column.0.valueformat=HTML
   column.0.descriptionkey=name
   column.0.linkedname=direct
   column.0.listsort=string(name)
   column.0.namekey=name
   column.0.querysort=name
   column.0.shortview=false
   column.0.stretch=100
   column.0.width=150
   column.1.displayname=Resolvables (Issues)
   column.1.listdelimiter=
   column.1.listmethod=nested(resolvables).lists
   column.1.textmode=true
   column.1.type=iterate
   column.1.valueexpression={name}
   column.1.valueformat=HTML
   column.2.displayname=Resolvables Entry Date
   column.2.listdelimiter=
   column.2.listmethod=nested(resolvables).lists
   column.2.textmode=true
   column.2.type=iterate
   column.2.valueexpression={entryDate}
   column.2.valueformat=HTML
   column.3.displayname=Resolvables Due Date
   column.3.listdelimiter=
   column.3.listmethod=nested(resolvables).lists
   column.3.textmode=true
   column.3.type=iterate
   column.3.valueexpression={plannedCompletionDate}
   column.3.valueformat=HTML
   column.4.displayname=Resolvables Actual Completion Date
   column.4.listdelimiter=
   column.4.listmethod=nested(resolvables).lists
   column.4.textmode=true
   column.4.type=iterate
   column.4.valueexpression={actualCompletionDate}
   column.4.valueformat=HTML
   column.5.displayname=Resolvables Request Type
   column.5.listdelimiter=
   column.5.listmethod=nested(resolvables).lists
   column.5.textmode=true
   column.5.type=iterate
   column.5.valueexpression={opTaskType}
   column.5.valueformat=HTML
   column.6.displayname=Resolvables Originator
   column.6.listdelimiter=
   column.6.listmethod=nested(resolvables).lists
   column.6.textmode=true
   column.6.type=iterate
   column.6.valueexpression={owner}.{name}
   column.6.valueformat=HTML
   column.7.descriptionkey=assignedto
   column.7.linkedname=assignedTo
   column.7.listsort=nested(assignedTo).string(name)
   column.7.namekey=assignedto
   column.7.querysort=assignedTo:name
   column.7.shortview=false
   column.7.stretch=0
   column.7.textmode=true
   column.7.valuefield=assignedTo:name
   column.7.valueformat=HTML
   column.7.width=150
   ```

1. 按一下&#x200B;**完成** > **儲存檢視**。
