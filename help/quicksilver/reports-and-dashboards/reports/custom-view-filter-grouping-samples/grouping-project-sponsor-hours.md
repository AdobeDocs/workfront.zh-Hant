---
content-type: reference
product-area: reporting;projects;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: 分組：時數的專案贊助者
description: 此小時分組按記錄小時數的專案贊助者組織小時。 時數分組的標準Report Builder介面不提供專案贊助者欄位的對應。 您必須使用文字模式介面才能存取此欄位。
author: Nolan
feature: Reports and Dashboards
exl-id: 6b35b0ef-18b7-4121-ae39-d7957d76c04b
source-git-commit: bc99e303047b989b972974b398420a9180e40874
workflow-type: tm+mt
source-wordcount: '248'
ht-degree: 0%

---

# 分組：時數的專案贊助者

<!--Audited: 10/2024-->

此小時分組按記錄小時數的專案贊助者組織小時。 時數分組的標準Report Builder介面不提供專案贊助者欄位的對應。 您必須使用文字模式介面才能存取此欄位。

![hour_report_grouped_by_sponner.png](assets/hour-report-grouped-by-sponsor-350x39.png)

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

## 按專案贊助者分組小時

若要套用此群組：

1. 前往時數清單。
1. 從&#x200B;**群組**&#x200B;下拉式功能表中，選取&#x200B;**新群組**。

1. 按一下&#x200B;**切換到文字模式**。
1. 移除顯示區域中的文字，並使用下列程式碼加以取代：

```
   group.0.linkedname=project:sponsor:name
   group.0.name=
   group.0.valuefield=project:sponsor:name
   group.0.valueformat=HTML
   textmode=true
```

1. 按一下&#x200B;**完成**。
1. 更新群組名稱，然後按一下[儲存群組]。**&#x200B;**
