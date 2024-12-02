---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 篩選：僅顯示處於核准狀態的專案
description: 您只能顯示目前處於「未決核准」之特定狀態的專案。 對於任何其他具有核准狀態的物件，其運作方式都相同。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: c1de5193-d3d5-406c-aa68-e6ba6d6751ae
source-git-commit: a19668ac2238448010b5a177120f936ef7ba5bba
workflow-type: tm+mt
source-wordcount: '280'
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

## 僅顯示處於核准狀態的專案

1. 前往專案清單。
1. 從&#x200B;**篩選器**&#x200B;下拉式功能表中，選取&#x200B;**新增篩選器**。
1. 選擇依&#x200B;**專案篩選：狀態**，然後從清單中選取您要篩選的狀態。

   例如，在專案報告中，如果您只想顯示處於&#x200B;**計畫 — 未決核准**&#x200B;狀態的專案，請新增&#x200B;**狀態等於計畫**。
1. 按一下&#x200B;**文字模式**。
1. 將&#x200B;**：A**&#x200B;加入狀態的3字母索引鍵中，以修改`status`行：
   <pre>status=PLN：A<br>status_Mod=in</pre>

1. 按一下&#x200B;**套用** > **另存新檔**。

   此清單只會顯示處於「計畫 — 未決核准」狀態的專案。
