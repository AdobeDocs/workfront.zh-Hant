---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 篩選：顯示您目前的擱置核准專案
description: 下列專案篩選器會顯示處於目前 — 未決核准狀態的專案，其中登入的使用者是專案贊助者或Portfolio經理。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 32045aec-acc5-44d2-bad5-7759dc797414
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '197'
ht-degree: 0%

---

# 篩選：顯示您目前的擱置核准專案

<!--Audited: 10/2024-->

下列專案篩選器會顯示處於目前 — 未決核准狀態的專案，其中登入的使用者是專案贊助者或Portfolio經理。

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

## 篩選目前擱置核准的專案

若要套用此篩選：

1. 前往專案清單。
1. 從&#x200B;**篩選器**&#x200B;下拉式功能表中，選取&#x200B;**新增篩選器**。

1. 按一下&#x200B;**文字模式**。
1. 在顯示的區域中，複製並貼上下列程式碼：
   <pre>status=CUR：A<br>sponnerID=$$USER.ID<br>或:a:status=CUR：A<br>或:a:投資組合：ownerID=$$USER.ID</pre>

1. 按一下&#x200B;**套用** > **另存新檔**。
