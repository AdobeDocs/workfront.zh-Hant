---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '''查看：顯示最多4層的父任務'
description: 此任務視圖顯示第一列中的任務名稱，並且（如果存在）同一清單中單獨列中最多4個父任務。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 66b45d64-794d-4adc-b208-2ded0dc9c5dc
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '594'
ht-degree: 0%

---

# 視圖：顯示最多4層的父任務

此任務視圖顯示第一列中的任務名稱，並且（如果存在）同一清單中單獨列中最多4個父任務。

![parent_tasks_4_levels_deep_png](assets/parent-tasks-4-levels-deep-350x29.png)

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

## 將父任務顯示到4個級別

1. 轉到任務清單。
1. 從 **視圖** 下拉菜單，選擇 **新建視圖**。

1. 在&#x200B;**列預覽** 框中，刪除除一個列之外的所有列。
1. 按一下其餘列的標題，然後按一下 **切換到文本模式**。
1. 將滑鼠移到文本模式區域上，然後按一下 **按一下可編輯文本**。
1. 刪除在中查找的文本 **文本模式** 框，並用以下代碼替換它：

   ```
   column.0.descriptionkey=name
   ```

   <pre>column.0.link.linkproperty.0.name=ID<br>column.0.link.linkproperty.0.valuefield=ID<br>column.0.link.linkproperty.0.valueformat=int<br>column.0.link.lookup=link.view<br>column.0.link.valuefield=objCode<br>column.0.link.valueformat=val<br>column.0.linkedname=direct<br>column.0.listsort=string(name)<br>column.0.namekey=name.abbr<br>column.0.querysort=name<br>column.0.shortview=false<br>column.0.valuefield=name<br>column.0.valueformat=HTML<br>column.0.width=150<br>column.1.descriptionkey=parent<br>column.1.link.linkproperty.0.name=ID<br>column.1.link.linkproperty.0.valuefield=parent:ID<br>column.1.link.linkproperty.0.valueformat=int<br>column.1.link.lookup=link.view<br>column.1.link.valuefield=parent:objCode<br>column.1.link.valueformat=val<br>column.1.linkedname=parent<br>column.1.listsort=nested(parent)。string(name)<br>column.1.namekey=parent<br>column.1.querysort=parent:name<br>column.1.shortview=false<br>column.1.stretch=0<br>column.1.valuefield=parent:name<br>column.1.valueformat=HTML<br>column.1.width=150<br>column.2.description=父代<br>column.2.link.linkproperty.0.name=ID<br>column.2.link.linkproperty.0.valuefield=parent:parent:ID<br>column.2.link.linkproperty.0.valueformat=int<br>column.2.link.lookup=link.view<br>column.2.link.valuefield=parent:parent:obj代碼<br>column.2.link.valueformat=val<br>column.2.linkedname=parent<br>column.2.listsort=nested(parent:parent)。string(name)<br>column.2.name=父代<br>column.2.querysort=parent:parent:名稱<br>column.2.shortview=false<br>column.2.strt.0<br>column.2.valuefield=parent:parent:名稱<br>column.2.valueformat=HTML<br>column.2.width=150<br>column.3.description=父代父代<br>column.3.link.linkproperty.0.name=ID<br>column.3.link.linkproperty.0.valuefield=parent:parent:父級：ID<br>column.3.link.linkproperty.0.valueformat=int<br>column.3.link.lookup=link.view<br>column.3.link.valuefield=parent:parent:父代：obj代碼<br>column.3.link.valueformat=val<br>column.3.linkedname=parent<br>column.3.listsort=nested（父級）:parent:parent)。string(name)<br>column.3.name=父代父代<br>column.3.querysort=parent:parent:父級：名稱<br>column.3.shortview=false<br>column.3.strt.0<br>column.3.valuefield=parent:parent:父級：名稱<br>column.3.valueformat=HTML<br>column.3.width=150<br>column.4.description=父代父代<br>column.4.link.linkproperty.0.name=ID<br>column.4.link.linkproperty.0.valuefield=parent:parent:父:parent:ID<br>column.4.link.linkproperty.0.valueformat=int<br>column.4.link.lookup=link.view<br>column.4.link.valuefield=parent:parent:父:parent:obj代碼<br>column.4.link.valueformat=val<br>column.4.linkedname=parent<br>column.4.listsort=nested（父級）:parent:parent:parent)。string(name)<br>column.4.name=父代父代<br>column.4.querysort=parent:parent:父:parent:名稱<br>column.4.shortview=false<br>column.4.stretch=100<br>column.4.valuefield=parent:parent:父:parent:名稱<br>column.4.valueformat=HTML<br>column.4.width=150</pre>

1. 按一下 **保存視圖**。

   任務的名稱顯示在第一列中，如果任務有任何父項，則最多4個父項顯示在其餘列中。
