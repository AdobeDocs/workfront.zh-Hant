---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 「檢視」：任務 檢視同一欄中超過計劃工時的實際小時數”
description: 在此任務 視圖中，任務上記錄的實際小時數顯示在每個任務的計劃小時數。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: c1179283-dc2e-40d3-b8e0-4b1b79f83ad3
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '376'
ht-degree: 1%

---

# 檢視：任務 檢視同一欄中超過計劃小時數的實際小時數

在此任務檢視中，任務上記錄的實際時數會顯示在針對每個任務計畫的時數中。

![actual_vs_planned_in_task_report.png](assets/actual-vs-planned-in-task-report-350x58.png)

## 存取需求

您必須具有以下存取權限才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Systems工作台計劃*</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Systems Workfront 許可證*</td> 
   <td> <p>請求修改視圖 </p>
   <p>計劃修改報表</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取等級設定*</td> 
   <td> <p>編輯存取報表、控制面板、日曆以修改報表</p> <p>編輯對篩選器、檢視、群組的存取權以修改檢視</p> <p><b>附註</b>

如果您仍然沒有訪問許可權，請詢問您的 Workfront 管理員是否在您的訪問許可權級別中設置了其他限制。 有關 Workfront 管理員如何修改存取權限等級的資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自定義訪問級別</a>。</p> </td>
</tr>  
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>管理報表的許可權</p> <p>有關請求其他存取權限的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對物件 </a>的存取權限 。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要瞭解您擁有的計劃、許可證類型或訪問許可權，請聯繫您的 Workfront 管理員。

## 檢視任務 視圖中超過計劃小時數的實際小時數

若要套用此視圖：

1. 轉到任務清單。
1. 從&#x200B;**檢視**&#x200B;下拉式功能表中，選取&#x200B;**新增檢視**。

1. 在&#x200B;**資料行預覽**&#x200B;區域中，排除除一個資料行以外的所有資料行。
1. 按兩下剩餘欄的標題，然後按下 **切換到文字模式**。
1. 將滑鼠移到文字模式區域，然後按下按兩下 **以編輯文字**。
1. 移除在「文字模式&#x200B;**」**&#x200B;框中找到的文字，並將其替換為以下代碼：
   <pre>column.0.descriptionkey=name column.0.連結.linkproperty.0.name=ID<br>column.0.連結.linkproperty.0.valuefield=ID<br>column.0.連結.linkproperty.0.valueformat=int<br>column.0.連結.lookup=連結.視圖<br>column.0.連結.valuefield=objCode<br>column.0.連結.valueformat=val<br>column.0.linkedName=direct column.0.listsort=string（name）column.0.namekey=name.abbr<br>column.0.querysort=name<br>column.0.shortview=false<br>column.0.stretch<br>=<br><br>100 column.0.valuefield=name column.0.valueformat=HTML column.0.width=150<br>column.1.viewalias=assignments column.1.displayname=column.1.linkedname=direct column.1.namekey=assignments column.1.valuefield=assignmentsListString column.1.valueformat=HTML column.1.tile.name=component.assignmentslist<br>column.2.displayname=實際/計劃工時<br>column.2.linkedname=direct<br>column.2.namekey<br>=<br><br><br><br><br><br><br><br>actualworkrequired<br>column.2.querysort=actualWork<br>column.2.textMode=true<br>column.2.valueexpression=CONCAT（{actualWorkRequired}/60，' / '，{workRequired}/60）<br>column.2.valuefield=actualWorkRequired<br>column.2.valueformat=compound<br>column.2.viewalias=actualworkrequired<br>column.3.aggregator.function=SUM<br>column.3.aggregator.valueexpression=SUB（{actualWork}， {workRequired}）<br>column.3.aggregator.valueformat=compound<br>column.3.displayname=Hours Variance<br>column.3.linkedname=direct<br>column.3.textMode=true<br>column.3.valueexpression=SUB（{actualWork}， {workRequired}）/60<br>column.3.valueformat=customNumberAsString</pre>

1. 按一下「**儲存視圖**」。
