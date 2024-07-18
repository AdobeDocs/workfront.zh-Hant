---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 「檢視：前置任務詳細資訊」
description: 此任務檢視使用集合檢視顯示任務前置任務的詳細資訊。 在集合檢視中，您可以顯示有關處於「一對多」關係中的物件的資訊。 在這種情況下，每個任務（一個）可以有多個前置任務（多個）。 該檢視顯示任務名稱，以及其前置任務名稱、前置任務專案名稱、前置任務計畫完成日期及前置任務狀態。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 0187da94-4895-47b1-914f-284fed9e0fd0
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '438'
ht-degree: 0%

---

# 檢視：前置任務詳細資訊

此任務檢視使用集合檢視顯示任務前置任務的詳細資訊。 在集合檢視中，您可以顯示有關處於「一對多」關係中的物件的資訊。 在這種情況下，每個任務（一個）可以有多個前置任務（多個）。 該檢視顯示任務名稱，以及其前置任務名稱、前置任務專案名稱、前置任務計畫完成日期及前置任務狀態。

如需在報表中參考集合的相關資訊，請參閱[報表中的參考集合](../../../reports-and-dashboards/reports/text-mode/reference-collections-report.md)。

![前置任務_詳細資料_任務_檢視.png](assets/predecessor-details-task-view-350x34.png)

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

## 檢視前置任務詳細資訊

1. 前往工作清單。
1. 從&#x200B;**檢視**&#x200B;下拉式功能表中，選取&#x200B;**新增檢視**。

1. 在&#x200B;**資料行預覽**&#x200B;區域中，排除除一個資料行以外的所有資料行。
1. 按一下剩餘欄的標題，然後按一下&#x200B;**切換到文字模式**。
1. 將滑鼠移到文字模式區域上，然後按一下&#x200B;**按一下以編輯文字**。
1. 移除您在&#x200B;**文字模式**&#x200B;方塊中找到的文字，並取代為下列程式碼：
   <pre>column.0.displayname=<br>column.0.linkedname=direct<br>column.0.namekey=name<br>column.0.querysort=name<br>column.0.valuefield=name<br>column.0.valueformat=HTML<br>column.1.displayname=前置任務數字和名稱<br>column.1.listdelimiter=<br><br>column.1.listmethod=nested（前置任務）。listers<br>column.1.textmode=true<br>column.1.type=iterate{1.1.valuterate{1.valuate{1.valustain.1.valuterate eexpression=CONCAT({predecessor}.<br>{taskNumber}，' - '，{predecessor}。{name})<br>column.1.valueformat=HTML<br>column.2.displayname=前置任務專案名稱<br>column.2.listdelimiter=<br><br>column.2.listmethod=nested(predecessors)。lists<br>column.2.textmode=true<br>column.2.type=iterate<br>column.2.valueexpression={predecessor}。{project}。{name}<br>column.2.valueformat=HTML<br>column.3.displayname=前置任務完成日期<br>column.3.listdelimiter=<br><br>column.3.listmethod=nested(predecessors)。lists<br>column.3.textmode=true<br>column.3.type=iterate<br>column.3.valueexpression={predecessor}。{plannedCompletionDate}<br>column.3.valueformat=HTML<br>column.4.displayname=前置任務狀態<br>column.4.listdelimiter=<br><br>column.4.listmethod=nested（前置任務）。lists<br>column.4.textmode=true<br>column.4.type=iterate<br>column.4.valueexpression={predecessor}。{status}<br>column.4.valueformat=HTML</pre>

1. 按一下「**儲存視圖**」。
