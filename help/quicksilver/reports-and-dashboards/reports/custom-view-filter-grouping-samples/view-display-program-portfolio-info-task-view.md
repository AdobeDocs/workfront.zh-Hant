---
content-type: reference
product-area: reporting;projects;portfolios;programs
navigation-topic: custom-view-filter-and-grouping-samples
title: '''查看：在任務視圖中顯示程式和Portfolio資訊'
description: 此任務視圖顯示與任務項目關聯的程式和Portfolio。 生成任務視圖時，報表生成器中不提供此資訊。 此資訊僅在文本模式下可用。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: cdd5a1e9-3cbf-4951-b803-fca544b2519a
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '555'
ht-degree: 0%

---

# 視圖：在任務視圖中顯示程式和Portfolio資訊

此任務視圖顯示與任務項目關聯的程式和Portfolio。 生成任務視圖時，報表生成器中不提供此資訊。 此資訊僅在文本模式下可用。

該視圖還提供從任務清單到項目、項目群和Portfolio的連結。

![](assets/view--program-and-portfolio-350x116.png)

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

## 在任務視圖中顯示程式和Portfolio資訊

要將此視圖應用於任務清單：

1. 轉到任務清單。
1. 從 **視圖** 下拉菜單，選擇 **新建視圖**。

1. 在&#x200B;**列預覽** 框中，刪除除一個列之外的所有列。
1. 按一下其餘列的標題，然後按一下 **切換到文本模式**。
1. 將滑鼠移到文本模式區域上，然後按一下 **按一下可編輯文本**。
1. 刪除在中查找的文本 **文本模式** 框，並用以下代碼替換它：
   <pre>column.0.descriptionkey=name<br>column.0.link.linkproperty.0.name=ID<br>column.0.link.linkproperty.0.valuefield=ID<br>column.0.link.linkproperty.0.valueformat=int<br>column.0.link.lookup=link.view<br>column.0.link.valuefield=objCode<br>column.0.link.valueformat=val<br>column.0.linkedname=direct<br>column.0.listsort=string(name)<br>column.0.namekey=name.abbr<br>column.0.querysort=name<br>column.0.shortview=false<br>column.0.stretch=100<br>column.0.valuefield=name<br>column.0.valueformat=HTML<br>column.0.width=150<br>column.1.descriptionkey=project<br>column.1.link.linkproperty.0.name=ID<br>column.1.link.linkproperty.0.valuefield=project:ID<br>column.1.link.linkproperty.0.valueformat=int<br>column.1.link.lookup=link.view<br>column.1.link.valuefield=project:objCode<br>column.1.link.valueformat=val<br>column.1.linkedname=project<br>column.1.listsort=nested(project.string(name))<br>column.1.namekey=project<br>column.1.querysort=項目：名稱<br>column.1.shortview=false<br>column.1.stretch=0<br>column.1.valuefield=project.name<br>column.1.valueformat=HTML<br>column.1.width=150<br>column.2.descriptionkey=program<br>column.2.displayname=程式<br>column.2.link.linkproperty.0.name=ID<br>column.2.link.linkproperty.0.valuefield=project:program:ID<br>column.2.link.linkproperty.0.valueformat=int<br>column.2.link.lookup=link.view<br>column.2.link.valuefield=project:program:obj代碼<br>column.2.link.valueformat=val<br>column.2.linkedname=project<br>column.2.listsort=nested(project:program)。string(name)<br>column.2.namekey=project<br>column.2.querysort=project:program:名稱<br>column.2.shortview=false<br>column.2.strt.0<br>column.2.valuefield=project:program:名稱<br>column.2.valueformat=HTML<br>column.2.width=150<br>column.3.descriptionkey=portforio<br>column.3.displayname=Portfolio<br>column.3.link.linkproperty.0.name=ID<br>column.3.link.linkproperty.0.valuefield=project:portfolio:ID<br>column.3.link.linkproperty.0.valueformat=int<br>column.3.link.lookup=link.view<br>column.3.link.valuefield=project:portfolio:obj代碼<br>column.3.link.valueformat=val<br>column.3.linkedname=project<br>column.3.listsort=nested(project:portfolio)。string(name)<br>column.3.namekey=project<br>column.3.querysort=project:portfolio:名稱<br>column.3.shortview=false<br>column.3.strt.0<br>column.3.valuefield=project:portfolio:名稱<br>column.3.valueformat=HTML<br>column.3.width=150 </pre>

1. 按一下 **保存視圖**。
