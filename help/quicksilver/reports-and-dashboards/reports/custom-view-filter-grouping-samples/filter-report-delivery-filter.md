---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 篩選器：顯示已排程傳送的報告
description: 此報告篩選器會顯示所有排程在Adobe Workfront中自動傳送的報告。 最好搭配標準檢視使用。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 7b937384-80c9-4bc7-94be-5573cf86b35b
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '179'
ht-degree: 1%

---

# 篩選器：顯示排程傳送的報表

<!--Audited: 10/2024-->

此報告篩選器會顯示所有排程在Adobe Workfront中自動傳送的報告。 最好搭配標準檢視使用。

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
   <p>修改篩選器的貢獻者或請求 </p>
   <p>要修改報告的標準或計畫</p>
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

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 報告傳遞篩選器

若要套用此篩選：

1. 前往報告清單。

1. 從&#x200B;**篩選器**&#x200B;下拉式功能表中，選取&#x200B;**新增篩選器**。

1. 按一下&#x200B;**切換到文字模式**。

1. 在&#x200B;**設定報表**&#x200B;的篩選規則區域中，複製並貼上下列程式碼：

   ```
   scheduledReportID=0
   scheduledReportID_Mod=notnull
   ```

1. 按一下「**儲存篩選器**」。
