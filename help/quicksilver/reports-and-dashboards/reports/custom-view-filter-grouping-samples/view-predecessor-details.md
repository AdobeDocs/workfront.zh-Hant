---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '''檢視：前置項詳細資訊'
description: 此任務視圖使用集合視圖顯示任務的前置任務的詳細資訊。 在集合視圖中，可以顯示「一對多」關係中對象的資訊。 在這種情況下，每個任務（一個）可以有多個前置任務（多個）。 此視圖顯示任務的名稱及其前置任務的名稱、前置任務的項目名稱、前置任務的計畫完成日期和前置任務的狀態。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 0187da94-4895-47b1-914f-284fed9e0fd0
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '458'
ht-degree: 0%

---

# 查看：前置詳細資訊

此任務視圖使用集合視圖顯示任務的前置任務的詳細資訊。 在集合視圖中，可以顯示「一對多」關係中對象的資訊。 在這種情況下，每個任務（一個）可以有多個前置任務（多個）。 此視圖顯示任務的名稱及其前置任務的名稱、前置任務的項目名稱、前置任務的計畫完成日期和前置任務的狀態。

如需在報表中參考集合的相關資訊，請參閱 [在報表中參考集合](../../../reports-and-dashboards/reports/text-mode/reference-collections-report.md).

![png](assets/predecessor-details-task-view-350x34.png)

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

## 查看前置項詳細資訊

1. 轉到任務清單。
1. 從 **檢視** 下拉式功能表，選取 **新建視圖**.

1. 在&#x200B;**欄預覽** 區域中，除一列外，刪除所有列。
1. 按一下剩餘欄的標題，然後按一下 **切換到文本模式**.
1. 將滑鼠移到文字模式區域上，然後按一下 **按一下「 」以編輯文字**.
1. 移除您在 **文字模式** 框中，並將其替換為以下代碼：
   <pre>column.0.displayname=<br>column.0.linkedname=direct<br>column.0.namekey=name<br>column.0.querysort=name<br>column.0.valuefield=name<br>column.0.valueformat=HTML<br>column.1.displayname=前置詞編號和名稱<br>column.1.listdelimiter=<br><br>column.1.listmethod=nested(precessions)。lists<br>column.1.textmode=true<br>column.1.type=iterate<br>column.1.valueexpression=CONCAT({pacisoment})。{taskNumber},' - ',{pacivestment}。{name})<br>column.1.valueformat=HTML<br>column.2.displayname=前置項目名稱<br>column.2.listdelimiter=<br><br>column.2.listmethod=nested(precessions)。lists<br>column.2.textmode=true<br>column.2.type=iterate<br>column.2.valueexpression={pacepress}。{專案}.{name}<br>column.2.valueformat=HTML<br>column.3.displayname=前置完成日期<br>column.3.listdelimeter=<br><br>column.3.listmethod=nested(precessions)。lists<br>column.3.textmode=true<br>column.3.type=iterate<br>column.3.valueexpression={pacepression}。{plannededCompletionDate}<br>column.3.valueformat=HTML<br>column.4.displayname=前置狀態<br>column.4.listdelimeter=<br><br>column.4.listmethod=nested(precessions)。lists<br>column.4.textmode=true<br>column.4.type=iterate<br>column.4.valueexpression={pacepression}。{status}<br>column.4.valueformat=HTML</pre>

1. 按一下 **保存視圖**.
