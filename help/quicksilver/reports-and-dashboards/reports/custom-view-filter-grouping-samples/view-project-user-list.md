---
content-type: reference
product-area: reporting;projects;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: '''查看：具有作業角色的項目用戶清單'
description: 您可以在項目清單或報告中應用此視圖，以顯示與項目關聯的用戶清單以及他們正在項目上執行的作業角色清單。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: a3f59f69-7f39-4814-bd2f-7734d620081e
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '477'
ht-degree: 0%

---

# 視圖：具有作業角色的項目用戶清單

您可以在項目清單或報告中應用此視圖，以顯示與項目關聯的用戶清單以及他們正在項目上執行的作業角色清單。

此報告中的資訊也可在項目的「人員」區域找到。

>[!TIP]
>
>如果沒有為用戶列出作業角色，但您知道這些角色與其用戶配置檔案中的作業角色相關聯，這可能意味著它們被分配給任務和問題，但可能不與任務或問題上的作業角色相關聯，或者報告中列出的用戶不是任務和問題的任務負責人，而是在項目上履行其他角色（例如，所有者或贊助人）。

![project_with_user_and_role_information_report_png](assets/project-with-user-and-role-information-report-350x100.png)

## 訪問要求

您必須具有以下訪問權限才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront許可證*</td> 
   <td> <p>請求修改視圖 </p>
   <p>計畫修改報表</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>編輯對報表、儀表板、日曆的訪問以修改報表</p> <p>編輯對篩選器、視圖、分組的訪問以修改視圖</p> <p><b>附註</b>

如果您仍然沒有訪問權限，請詢問您的Workfront管理員是否在您的訪問級別設定了其他限制。 有關Workfront管理員如何修改您的訪問級別的資訊，請參見 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自定義訪問級別</a>。</p> </td>
</tr>  
  <tr> 
   <td role="rowheader">對象權限</td> 
   <td> <p>管理對報表的權限</p> <p>有關請求附加訪問的資訊，請參見 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求訪問對象 </a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要瞭解您擁有的計畫、許可證類型或訪問權限，請與您的Workfront管理員聯繫。

## 查看具有作業角色的項目用戶清單

1. 轉到項目清單。
1. 從 **視圖** 下拉菜單，選擇 **新建視圖**。

1. 在&#x200B;**列預覽** 框中，刪除除一個列之外的所有列。
1. 按一下其餘列的標題，然後按一下 **切換到文本模式**。
1. 將滑鼠移到文本模式區域上，然後按一下 **按一下可編輯文本**。
1. 刪除在中查找的文本 **文本模式** 框，並用以下代碼替換它：
   <pre>column.0.link.valueformat=val<br>column.0.linkedname=direct<br>column.0.listsort=string(name)<br>column.0.namekey=name.abbr<br>column.0.querysort=name<br>column.0.section=0<br>column.0.shortview=false<br>column.0.stretch=100<br>column.0.valuefield=name<br>column.0.valueformat=HTML<br>column.0.width=200<br>column.1.displayname=項目用戶<br>column.1.listdelimiter=&lt;br&gt;<br>column.1.listmethod=nested(projectUsers)。lists<br>column.1.textmode=true<br>column.1.type=iterate<br>column.1.valueexpression={user}。{name}<br>column.1.valueformat=HTML<br>column.2.displayname=項目角色<br>column.2.listdelimiter=&lt;br&gt;<br>column.2.listmethod=nested(projectUserRoles)。lists<br>column.2.textmode=true<br>column.2.type=iterate<br>column.2.valueexpression={role}。{name}<br>column.2.valueformat=HTML</pre>

1. 按一下 **保存視圖**。
