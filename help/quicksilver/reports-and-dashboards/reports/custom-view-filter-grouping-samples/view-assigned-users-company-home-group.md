---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: 「查看：已分配用戶的公司和家庭組」
description: 此任務視圖顯示任務的主要所有者的公司和家庭組。 這些值在標準介面中不可用，但可以通過文本模式訪問。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 818c1f3a-4e82-4dc3-af86-4f9dcf5c11a4
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '478'
ht-degree: 0%

---

# 視圖：已分配用戶的公司和家庭組

此任務視圖顯示任務的主要所有者的公司和家庭組。 這些值在標準介面中不可用，但可以通過文本模式訪問。

![](assets/view--assigned-user-s-company-and-home-group-350x80.png)

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

## 查看分配的用戶的公司和主組

1. 轉到任務清單。
1. 從 **視圖** 下拉菜單，選擇 **新建視圖**。

1. 在&#x200B;**列預覽** 框中，刪除除一個列之外的所有列。
1. 按一下其餘列的標題，然後按一下 **切換到文本模式**。
1. 將滑鼠移到文本模式區域上，然後按一下 **按一下可編輯文本**。
1. 刪除在中查找的文本 **文本模式** 框，並用以下代碼替換它：
   <pre>column.0.descriptionkey=name<br> column.0.link.linkproperty.0.name=ID<br> column.0.link.linkproperty.0.valuefield=ID<br> column.0.link.linkproperty.0.valueformat=int<br> column.0.link.lookup=link.view<br> column.0.link.valuefield=objCode<br> column.0.link.valueformat=val<br> column.0.linkedname=direct<br> column.0.listsort=string(name)<br> column.0.namekey=name.abbr<br> column.0.querysort=name<br> column.0.shortview=false<br> column.0.stretch=100<br> column.0.valuefield=name<br> column.0.valueformat=HTML<br> column.0.width=150<br> column.1.descriptionkey=assignedto<br> column.1.link.linkproperty.0.name=ID<br> column.1.link.linkproperty.0.valuefield=assignedTo:ID<br> column.1.link.linkproperty.0.valueformat=int<br> column.1.link.lookup=link.view<br> column.1.link.valuefield=assignedTo:objCode<br> column.1.link.valueformat=val<br> column.1.linkedname=assignedTo<br> column.1.listsort=nested（已分配給）。string(name)<br> column.1.namekey=已分配到<br> column.1.querysort=assignedTo:name<br> column.1.shortview=false<br> column.1.stretch=0<br> column.1.valuefield=assignedTo:name<br> column.1.valueformat=HTML<br> column.1.width=150<br> column.2.description=分配給公司<br> column.2.displayname=已分配給公司<br> column.2.linkedname=assignedTo:company<br> column.2.listsort=nested（已分配給：company）。string(name)<br> column.2.namekey=已分配到<br> column.2.querysort=assignedTo:company:名稱<br> column.2.shortview=false<br> column.2.strt.0<br> column.2.valuefield=assignedTo:company:名稱<br> column.2.valueformat=HTML<br> column.2.width=150<br> column.3.description=分配給主組<br> column.3.displayname=已分配給主組<br> column.3.linkedname=assignedTo:homeGroup<br> column.3.listsort=nested（已分配給：homeGroup）。string(name)<br> column.3.namekey=已分配到<br> column.3.querysort=assignedTo:homeGroup:名稱<br> column.3.shortview=false<br> column.3.strt.0<br> column.3.valuefield=assignedTo:homeGroup:名稱<br> column.3.valueformat=HTML<br> column.3.width=150</pre>

1. 按一下 **保存更改**。
