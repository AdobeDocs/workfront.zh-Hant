---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 篩選：僅顯示處於核准狀態的專案
description: 您只能顯示目前處於「未決核准」之特定狀態的專案。 對於任何其他具有核准狀態的物件，其運作方式都相同。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: c1de5193-d3d5-406c-aa68-e6ba6d6751ae
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '265'
ht-degree: 1%

---

# 篩選：僅顯示處於核准狀態的專案

<!--Audited: 10/2024-->

您只能顯示目前處於「未決核准」之特定狀態的專案。 對於任何其他具有核准狀態的物件，其運作方式都相同。

您可以將下列物件置於核准狀態：

* 任務
* 問題
* 專案

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

## 僅顯示處於核准狀態的專案

1. 前往專案清單。
1. 從&#x200B;**篩選器**&#x200B;下拉式功能表中，選取&#x200B;**新增篩選器**。
1. 選擇依&#x200B;**專案篩選：狀態**，然後從清單中選取您要篩選的狀態。

   例如，在專案報告中，如果您只想顯示處於&#x200B;**計畫 — 未決核准**&#x200B;狀態的專案，請新增&#x200B;**狀態等於計畫**。
1. 按一下&#x200B;**文字模式**。
1. 將`status`加入狀態的3字母索引鍵中，以修改&#x200B;**:A**&#x200B;行：
   <pre>status=PLN：A<br>status_Mod=in</pre>

1. 按一下&#x200B;**套用** > **另存新檔**。

   此清單只會顯示處於「計畫 — 未決核准」狀態的專案。
