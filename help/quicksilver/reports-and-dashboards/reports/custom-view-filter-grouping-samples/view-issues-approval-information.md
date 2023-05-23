---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '''查看：與批准資訊一起發佈'
description: 以下發行視圖顯示批准流程、步驟、批准者的名稱以及批准之前的發行狀態。 某些欄位無法通過標準介面生成器訪問。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 4e123844-a0d6-474b-87fb-d30ed391ad07
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '534'
ht-degree: 0%

---

# 視圖：發佈審批資訊

以下發行視圖顯示批准流程、步驟、批准者的名稱以及批准之前的發行狀態。 某些欄位無法通過標準介面生成器訪問。

![custom_issue_view_with_approval_info_png](assets/custom-issue-view-with-approval-info-350x46.png)

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

## 查看包含審批資訊的問題

1. 轉到問題清單。
1. 從 **視圖** 下拉菜單，選擇 **新建視圖**。

1. 在&#x200B;**列預覽** 框中，刪除除一個列之外的所有列。
1. 按一下其餘列的標題，然後按一下 **切換到文本模式**。
1. 將滑鼠移到文本模式區域上，然後按一下 **按一下可編輯文本**。
1. 刪除在中查找的文本 **文本模式** 框，並用以下代碼替換它：
   <pre style="font-style: normal;">column.0.descriptionkey=name<br>column.0.link.linkproperty.0.name=ID<br>column.0.link.linkproperty.0.valuefield=ID<br>column.0.link.linkproperty.0.valueformat=int<br>column.0.link.lookup=link.view<br>column.0.link.valuefield=objCode<br>column.0.link.valueformat=val<br>column.0.linkedname=direct<br>column.0.listsort=string(name)<br>column.0.namekey=name.abbr<br>column.0.querysort=name<br>column.0.shortview=false<br>column.0.strect=40<br>column.0.valuefield=name<br>column.0.valueformat=HTML<br>column.0.width=220<br>column.1.descriptionkey=assignedto<br>column.1.linkedname=assignedTo<br>column.1.listsort=nested（已分配給）。string(name)<br>column.1.namekey=已分配到<br>column.1.querysort=assignedTo:name<br>column.1.shortview=true<br>column.1.stretch=0<br>column.1.valuefield=assignedTo:name<br>column.1.valueformat=HTML<br>column.1.width=150<br>column.2.descriptionkey=role<br>column.2.linkedname=role<br>column.2.listsort=nested(role)。string(name)<br>column.2.namekey=role<br>column.2.querysort=role:name<br>column.2.shortview=false<br>column.2.strect=25<br>column.2.valuefield=role:name<br>column.2.valueformat=HTML<br>column.2.width=150<br>column.3.description=審批流程名稱<br>column.3.linkedname=direct<br>column.3.listsort=string(name)<br>column.3.name=批准進程名稱<br>column.3.querysort=name<br>column.3.shortview=false<br>column.3.strect=35<br>column.3.valuefield=approvalProcess:name<br>column.3.valueformat=HTML<br>column.3.width=220<br>column.4.description=批准步驟名稱<br>column.4.linkedname=direct<br>column.4.listsort=string(name)<br>column.4.name=批准步驟名稱<br>column.4.querysort=name<br>column.4.shortview=false<br>column.4.stretch=0<br>column.4.valuefield=currentApprovalStep:name<br>column.4.valueformat=HTML<br>column.4.width=220<br>column.5.description=上一狀態<br>column.5.linkedname=direct<br>column.5.listsort=string(name)<br>column.5.name=上一狀態<br>column.5.querysort=name<br>column.5.shortview=false<br>column.5.strt.0<br>column.5.valuefield=previousStatus<br>column.5.valueformat=HTML<br>column.5.width=220<br>column.6.linkedname=direct<br>column.6.listsort=HTML(approversString)<br>column.6.namekey=approver.plurar.abbr<br>column.6.querysort=approvers字串<br>column.6.shortview=false<br>column.6.strt.0<br>column.6.valuefield=approversString<br>column.6.valueformat=HTML<br>column.6.viewalias=approver.plur<br>column.6.width=200<br></pre>

1. 按一下 **保存視圖**。
