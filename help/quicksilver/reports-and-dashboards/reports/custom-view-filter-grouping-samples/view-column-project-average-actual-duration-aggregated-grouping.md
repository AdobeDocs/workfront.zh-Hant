---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '''查看和分組：顯示按分組中的平均值匯總的項目實際持續時間'
description: 您可以在專案報表中新增下列欄，將匯總的實際持續時間顯示為分組中的平均值。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 31794fe9-a04a-437d-8d2e-40e0cb6e6104
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '341'
ht-degree: 0%

---

# 查看和分組：顯示按分組中的平均值匯總的項目實際持續時間

您可以在專案報表中新增下列欄，將匯總的實際持續時間顯示為分組中的平均值。

![project_with_aggregate_actual_duration_in_grouping_view_png](assets/project-with-aggregate-actual-duration-in-grouping-view-350x65.png)

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

## 顯示按分組中的平均值匯總的項目實際持續時間

要將此列添加到項目視圖：

1. （建議）為獲得最佳結果，並查看「實際持續時間」的匯總平均值，您必須在專案清單或報表中新增「分組」。\
   如需建立群組的詳細資訊，請參閱文章 [Adobe Workfront中的群組概觀](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. 前往現有的專案檢視。
1. 展開「檢視」下拉式功能表，然後選取 **自訂檢視**.
1. 按一下 **添加列**.
1. 按一下 **切換到文本模式**.
1. 將滑鼠移至 **顯示在此列中** 按一下 **按一下「 」以編輯文字**.

1. 移除「文字模式」方塊中的所有文字，並以下列程式碼取代：

   <pre>aggreator.displayformat=compound <br>aggregator.function=AVG <br>aggreator.namekey=view.relatedcolumn <br>aggerator.namekeyargkey=actualduration <br>aggregator.valuefield=actualDurationMinutes <br>aggregator.valueformat=val <br>displayname=項目實際持續時間 <br>durationunitfield=durationUnit.value <br>linkedname=project <br>namekey=actualduration <br>namekeyargkey=actualduration <br>querysort=actualDurationMinutes <br>textmode=true <br>valuefield=actualDurationMinutes <br>valueformat=compound#M:D <br>viewalias=actualduration</pre>

1. 按一下 **保存視圖**.
