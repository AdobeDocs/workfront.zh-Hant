---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 檢視與群組：顯示依群組中平均值彙總的專案實際期間
description: 您可以在專案報表中新增下列欄，以顯示分組中彙總為平均的實際期間。
author: Nolan
feature: Reports and Dashboards
exl-id: 31794fe9-a04a-437d-8d2e-40e0cb6e6104
source-git-commit: ecce7484423419823effa2cb41da892ba3fb207c
workflow-type: tm+mt
source-wordcount: '278'
ht-degree: 1%

---

# 檢視與分組：顯示依分組中平均值彙總的專案實際期間

<!--Audited: 11/2024-->

您可以在專案檢視中新增下列欄，以顯示分組中彙總為平均的實際期間。

![project_with_aggregate_actual_duration_in_grouping_view.png](assets/project-with-aggregate-actual-duration-in-grouping-view-350x65.png)

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> 
    <p>新增：</p>
   <ul><li><p>修改篩選器的貢獻者 </p></li>
   <li><p>用於修改報告的標準</p></li> </ul>

<p>目前：</p>
   <ul><li><p>請求修改篩選器 </p></li>
   <li><p>計畫修改報表</p></li> </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>編輯報告、儀表板、行事曆的存取權以修改報告</p> <p>編輯篩選器、檢視和群組的存取權以修改篩選器</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>管理報表的許可權</p>  </td> 
  </tr> 
 </tbody> 
</table>

*如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 顯示依分組中平均值彙總的專案實際期間

若要將此欄新增至專案檢視：

1. 前往專案清單。
1. （必要）若要檢視專案實際期間彙總的平均值，您必須將群組新增至專案清單。\
   如需建立群組的詳細資訊，請參閱文章[Adobe Workfront中的群組概觀](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)。
1. 展開&#x200B;**檢視**&#x200B;下拉式功能表，然後選取&#x200B;**自訂檢視**。
1. 按一下「**新增欄**」。
1. 按一下&#x200B;**切換到文字模式**，然後按一下&#x200B;**編輯文字模式**。
1. 移除&#x200B;**編輯文字模式**&#x200B;方塊中的所有文字，並以下列程式碼取代：

   ```
   aggregator.displayformat=compound 
   aggregator.function=AVG 
   aggregator.namekey=view.relatedcolumn 
   aggregator.namekeyargkey=actualduration 
   aggregator.valuefield=actualDurationMinutes 
   aggregator.valueformat=val 
   displayname=Project Actual Duration 
   durationunitfield=durationUnit.value 
   linkedname=project 
   namekey=actualduration 
   namekeyargkey=actualduration 
   querysort=actualDurationMinutes 
   textmode=true 
   valuefield=actualDurationMinutes 
   valueformat=compound#M:D 
   viewalias=actualduration
   ```

1. 按一下&#x200B;**完成**，然後按一下&#x200B;**儲存檢視**。
1. （選擇性）更新檢視名稱，然後按一下&#x200B;**儲存檢視**。
