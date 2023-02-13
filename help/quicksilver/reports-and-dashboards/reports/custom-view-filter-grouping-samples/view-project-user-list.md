---
content-type: reference
product-area: reporting;projects;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: '''檢視：具有作業角色的項目用戶清單'
description: 您可以在項目清單或報告中應用此視圖，以顯示與項目關聯的用戶清單，以及他們在項目上執行的作業角色清單。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: a3f59f69-7f39-4814-bd2f-7734d620081e
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '460'
ht-degree: 0%

---

# 查看：具有作業角色的項目用戶清單

您可以在項目清單或報告中應用此視圖，以顯示與項目關聯的用戶清單，以及他們在項目上執行的作業角色清單。

此報告中的資訊也可在專案的「人員」區域找到。

>[!TIP]
>
>如果沒有為用戶列出任務角色，但您知道這些角色與其用戶配置檔案中的任務角色相關聯，則這可能意味著它們被分配給任務和問題，但它們可能不與任務或問題上的任務角色相關聯，或者報表中列出的用戶不是任務和問題的受分配者，而是履行項目上的其他角色（例如「所有者」或「發起人」）。

![project_with_user_and_role_information_report_png](assets/project-with-user-and-role-information-report-350x100.png)

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

## 查看具有作業角色的項目用戶清單

1. 前往專案清單。
1. 從 **檢視** 下拉式功能表，選取 **新建視圖**.

1. 在&#x200B;**欄預覽** 區域中，除一列外，刪除所有列。
1. 按一下剩餘欄的標題，然後按一下 **切換到文本模式**.
1. 將滑鼠移到文字模式區域上，然後按一下 **按一下「 」以編輯文字**.
1. 移除您在 **文字模式** 框中，並將其替換為以下代碼：
   <pre>column.0.link.valueformat=val<br>column.0.linkedname=direct<br>column.0.listsort=string(name)<br>column.0.namekey=name.abbr<br>column.0.querysort=name<br>column.0.section=0<br>column.0.shortview=false<br>column.0.stretch=100<br>column.0.valuefield=name<br>column.0.valueformat=HTML<br>column.0.width=200<br>column.1.displayname=Project用戶<br>column.1.listdelimiter=&lt;br&gt;<br>column.1.listmethod=nested(projectUsers)。lists<br>column.1.textmode=true<br>column.1.type=iterate<br>column.1.valueexpression={user}。{name}<br>column.1.valueformat=HTML<br>column.2.displayname=項目角色<br>column.2.listdelimiter=&lt;br&gt;<br>column.2.listmethod=nested(projectUserRoles)。lists<br>column.2.textmode=true<br>column.2.type=iterate<br>column.2.valueexpression={role}。{name}<br>column.2.valueformat=HTML</pre>

1. 按一下 **保存視圖**.
