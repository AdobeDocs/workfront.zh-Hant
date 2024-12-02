---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 群組：依輸入日期排列的專案
description: 在此自訂專案分組中，您可以顯示按其輸入日期值分組的專案。
author: Nolan
feature: Reports and Dashboards
exl-id: 511faad5-b5bd-4e2d-8daa-3fcde49a502c
source-git-commit: a6874c3a2dfda02b8a25f78056767d8c59c888e9
workflow-type: tm+mt
source-wordcount: '234'
ht-degree: 0%

---

# 群組：依輸入日期排列的專案

<!--Audited: 10/2024-->

在此自訂專案分組中，您可以顯示按其輸入日期值分組的專案。

每個群組會顯示具有輸入日期的專案，範圍如下：

* 過去30天
* 30-60天
* 60天以上

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

## 依輸入日期將專案分組

若要套用此群組：

1. 前往現有的專案報告，或建立新的專案報告。\
   如需有關建立報告的詳細資訊，請參閱文章[建立自訂報告](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)。
1. 按一下&#x200B;**報告動作** > **編輯**。
1. 從&#x200B;**群組**&#x200B;索引標籤中，按一下&#x200B;**新增群組**。
1. 按一下&#x200B;**切換到文字模式**。
1. 移除&#x200B;**依**&#x200B;分組區域中的文字。
1. 將文字取代為下列程式碼：


   ```
   group.0.linkedname=direct
   group.0.name=Project Entry
   group.0.valueexpression=IF(ABS(DATEDIFF({entryDate},$$TODAY))<=30,"Last 30 Days",IF(ABS(DATEDIFF({entryDate},$$TODAY))>30&&ABS(DATEDIFF({entryDate},$$TODAY))<=60,"30-60 Days","Older than 60 days"))
   group.0.valueformat=atDateAsMonthString
   textmode=true
   ```

1. 按一下&#x200B;**完成** > **儲存群組**。
1. （選擇性）更新群組的名稱，然後按一下&#x200B;**儲存群組**。
