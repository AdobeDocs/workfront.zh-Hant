---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '''查看：前置項詳細資訊'
description: 此任務視圖使用集合視圖顯示任務的前置任務的詳細資訊。 在集合視圖中，可以顯示有關「一對多」關係中的對象的資訊。 在這種情況下，每個任務（一個）可以具有多個前置任務（多個）。 該視圖顯示任務的名稱，以及其前置任務名稱、前置任務項目名稱、前置任務計畫完成日期和前置任務狀態。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 0187da94-4895-47b1-914f-284fed9e0fd0
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '475'
ht-degree: 0%

---

# 視圖：前置任務詳細資訊

此任務視圖使用集合視圖顯示任務的前置任務的詳細資訊。 在集合視圖中，可以顯示有關「一對多」關係中的對象的資訊。 在這種情況下，每個任務（一個）可以具有多個前置任務（多個）。 該視圖顯示任務的名稱，以及其前置任務名稱、前置任務項目名稱、前置任務計畫完成日期和前置任務狀態。

有關在報表中引用集合的資訊，請參見 [報表中的引用集合](../../../reports-and-dashboards/reports/text-mode/reference-collections-report.md)。

![前置任務_詳細資訊_任務_視圖_png](assets/predecessor-details-task-view-350x34.png)

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

## 查看前置任務詳細資訊

1. 轉到任務清單。
1. 從 **視圖** 下拉菜單，選擇 **新建視圖**。

1. 在&#x200B;**列預覽** 框中，刪除除一個列之外的所有列。
1. 按一下其餘列的標題，然後按一下 **切換到文本模式**。
1. 將滑鼠移到文本模式區域上，然後按一下 **按一下可編輯文本**。
1. 刪除在中查找的文本 **文本模式** 框，並用以下代碼替換它：
   <pre>column.0.displayname=<br>column.0.linkedname=direct<br>column.0.namekey=name<br>column.0.querysort=name<br>column.0.valuefield=name<br>column.0.valueformat=HTML<br>column.1.displayname=前置任務編號和名稱<br>column.1.listdelimiter=<br><br>column.1.listmethod=nested(precessers)。lists<br>column.1.textmode=true<br>column.1.type=iterate<br>column.1.valueexpression=CONCAT({pacisent})。{taskNumber},' — 「，{pacestive}。{name})<br>column.1.valueformat=HTML<br>column.2.displayname=前置任務項目名稱<br>column.2.listdelimiter=<br><br>column.2.listmethod=nested(precessers)。lists<br>column.2.textmode=true<br>column.2.type=iterate<br>column.2.valueexpression={pacisment}。{專案}.{name}<br>column.2.valueformat=HTML<br>column.3.displayname=前置任務完成日期<br>column.3.listdelimiter=<br><br>column.3.listmethod=nested(precessers)。lists<br>column.3.textmode=true<br>column.3.type=iterate<br>column.3.valueexpression={pacistment}。{planedCompletionDate}<br>column.3.valueformat=HTML<br>column.4.displayname=前置任務狀態<br>column.4.listdelimiter=<br><br>column.4.listmethod=nested(precessers)。lists<br>column.4.textmode=true<br>column.4.type=iterate<br>column.4.valueexpression={pacistment}。{status}<br>column.4.valueformat=HTML</pre>

1. 按一下 **保存視圖**。
