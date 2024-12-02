---
content-type: reference
product-area: reporting;projects;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: 檢視：具有工作角色的專案使用者清單
description: 您可以在專案清單或報告中套用此檢視，以顯示與專案相關聯的使用者清單，以及他們在專案上執行的工作角色清單。
author: Nolan
feature: Reports and Dashboards
exl-id: a3f59f69-7f39-4814-bd2f-7734d620081e
source-git-commit: 6405c01c8b1d842a4175f9caa18a7ed31316a3a1
workflow-type: tm+mt
source-wordcount: '356'
ht-degree: 0%

---

# 檢視：具有工作角色的專案使用者清單

<!--Audited: 11/2024-->

您可以在專案清單或報告中套用此檢視，以顯示與專案相關聯的使用者清單，以及他們在專案上執行的工作角色清單。

此報告中的資訊也可在專案的「人員」區域中找到。

>[!TIP]
>
>如果沒有為使用者列出工作角色，但您知道他們與其使用者設定檔中的工作角色相關聯，這可能表示他們被指派到任務和問題，但他們可能未與任務或問題上的工作角色相關聯，或者報告中列出的使用者不是任務和問題的受指派人，但履行專案上的其他角色（例如，所有者或贊助者）。

![project_with_user_and_role_information_report.png](assets/project-with-user-and-role-information-report-350x100.png)

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


## 檢視具有工作角色的專案使用者清單

1. 前往專案清單。
1. 從&#x200B;**檢視**&#x200B;下拉式功能表中，選取&#x200B;**新增檢視**。
1. 在&#x200B;**資料行預覽**&#x200B;區域中，排除除一個資料行以外的所有資料行。
1. 按一下剩餘欄的標題，然後按一下&#x200B;**切換到文字模式** > **編輯文字模式**。
1. 移除您在&#x200B;**編輯文字模式**&#x200B;方塊中找到的文字，並取代為下列程式碼：

   ```
   column.0.link.valueformat=val
   column.0.linkedname=direct
   column.0.listsort=string(name)
   column.0.namekey=name.abbr
   column.0.querysort=name
   column.0.section=0
   column.0.shortview=false
   column.0.stretch=100
   column.0.valuefield=name
   column.0.valueformat=HTML
   column.0.width=200
   column.1.displayname=Project Users
   column.1.listdelimiter=<br>
   column.1.listmethod=nested(projectUsers).lists
   column.1.textmode=true
   column.1.type=iterate
   column.1.valueexpression={user}.{name}
   column.1.valueformat=HTML
   column.2.displayname=Project Roles
   column.2.listdelimiter=<br>
   column.2.listmethod=nested(projectUserRoles).lists
   column.2.textmode=true
   column.2.type=iterate
   column.2.valueexpression={role}.{name}
   column.2.valueformat=HTML
   ```

1. 按一下&#x200B;**完成** > **儲存檢視**。
