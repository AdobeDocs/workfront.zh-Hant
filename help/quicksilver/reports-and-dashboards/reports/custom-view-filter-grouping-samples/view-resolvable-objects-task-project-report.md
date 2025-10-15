---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 檢視：任務或專案報表中的可解析物件
description: 您可以在專案、任務檢視或報告中顯示所有可解析物件的清單。
author: Nolan
feature: Reports and Dashboards
exl-id: 2b0d8e7c-9211-44e5-9d92-c87a2fe4336d
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '259'
ht-degree: 0%

---

# 檢視：任務或專案報告中的可解析物件

<!--Audited: 11/2024-->

您可以在專案、任務檢視或報告中顯示所有可解析物件的清單。

如需可解析物件的詳細資訊，請參閱文章[解析和可解析物件概觀](../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md)。

![list_of_resolvables_in_report.png](assets/list-of-resolvables-in-report-350x54.png)

套用此檢視對於任務和專案是相同的。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront套件</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td> 
   <p>投稿人或請求修改檢視 </p>
   <p>要修改報告的標準或計畫</p>
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>編輯報告、儀表板、行事曆的存取權以修改報告</p> <p>編輯對篩選器、檢視、群組的存取權以修改檢視</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>管理報表的許可權</p>  </td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。


+++

## 在任務或專案報告中檢視可解析物件

1. 前往已從問題轉換的任務或專案清單。
1. 從&#x200B;**檢視**&#x200B;下拉式功能表，按一下&#x200B;**新增檢視**。

1. 在&#x200B;**欄預覽**&#x200B;區域中，按一下&#x200B;**新增欄**。

1. 按一下新欄的標題，然後按一下&#x200B;**切換到文字模式** > **編輯文字模式**。
1. 移除您在&#x200B;**編輯文字模式**&#x200B;方塊中找到的文字，並取代為下列程式碼：

   ```
   displayname=Resolvables
   listdelimiter=<br>
   listmethod=nested(resolvables).lists
   textmode=true
   type=iterate
   valuefield=name
   valueformat=HTML
   ```

1. 按一下&#x200B;**完成** > **儲存檢視**。\
   新欄中會顯示所有「可解析物件」的清單。 清單中的物件名稱無法直接連結到物件。
