---
content-type: reference
product-area: reporting;projects;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: 「檢視：具有工作角色的專案使用者清單」
description: 您可以在專案清單或報告中套用此檢視，以顯示與專案相關聯的使用者清單，以及他們在專案上執行的工作角色清單。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: a3f59f69-7f39-4814-bd2f-7734d620081e
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '449'
ht-degree: 0%

---

# 檢視：具有工作角色的專案使用者清單

您可以在專案清單或報告中套用此檢視，以顯示與專案相關聯的使用者清單，以及他們在專案上執行的工作角色清單。

此報告中的資訊也可在專案的「人員」區域中找到。

>[!TIP]
>
>如果沒有為使用者列出工作角色，但您知道他們與其使用者設定檔中的工作角色相關聯，這可能表示他們被指派到任務和問題，但他們可能未與任務或問題上的工作角色相關聯，或者報告中列出的使用者不是任務和問題的受指派人，但履行專案上的其他角色（例如，所有者或贊助者）。

![project_with_user_and_role_information_report.png](assets/project-with-user-and-role-information-report-350x100.png)

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

## 檢視具有工作角色的專案使用者清單

1. 前往專案清單。
1. 從&#x200B;**檢視**&#x200B;下拉式功能表中，選取&#x200B;**新增檢視**。

1. 在&#x200B;**資料行預覽**&#x200B;區域中，排除除一個資料行以外的所有資料行。
1. 按一下剩餘欄的標題，然後按一下&#x200B;**切換到文字模式**。
1. 將滑鼠移到文字模式區域上，然後按一下&#x200B;**按一下以編輯文字**。
1. 移除您在&#x200B;**文字模式**&#x200B;方塊中找到的文字，並取代為下列程式碼：
   <pre>column.0.link.valueformat=val<br>column.0.linkedname=direct<br>column.0.listsort=string(name)<br>column.0.namekey=name.abbr<br>column.0.querysort=name<br>column.0.section=0<br>column.0.shortview=false<br>column.0.stretch=100<br>column.0.valuefield=name<br>column.0.width=HTML{10001Displayname專案使用者<br>column.1.listdelimiter=&lt;br&gt;<br>column.1.listmethod=nested(projectUsers)。lists<br>column.1.textmode=true<br>column.1.type=iterate<br>column.1.valueexpression={user}。<br><br>{name}<br>column.1.valueformat=HTML<br>column.2.displayname=專案角色<br>column.2.listdelimiter=&lt;br&gt;<br>column.2.listmethod=nested(projectUserRoles)。lists<br>column.2.textmode=true<br>column.2.type=iterate<br>column.2.valueexpression={role}。{name}<br>column.2.valueformat=HTML</pre>

1. 按一下「**儲存視圖**」。
