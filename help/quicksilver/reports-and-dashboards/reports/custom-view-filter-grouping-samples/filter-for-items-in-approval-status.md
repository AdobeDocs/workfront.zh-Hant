---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '''篩選：僅顯示處於批准狀態的項目'
description: 您只能顯示當前處於「待批准」狀態的特定狀態的項目。 對於具有批准狀態的任何其他對象，這同樣適用。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: c1de5193-d3d5-406c-aa68-e6ba6d6751ae
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '298'
ht-degree: 1%

---

# 篩選：僅顯示處於批准狀態的項目

您只能顯示當前處於「待批准」狀態的特定狀態的項目。 對於具有批准狀態的任何其他對象，這同樣適用。

您可以將以下對象置於批准狀態：

* 任務
* 問題
* 專案

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

## 僅顯示處於批准狀態的項目

1. 移至您要自訂的篩選器，以取得專案清單。
1. 按一下 **新增篩選規則** 針對 **狀態** 清單對象的欄位。\
   例如，在專案報表中，新增 **狀態均等計畫**，而只顯示狀態為 **計畫 — 待批准**.

1. 按一下 **切換到文本模式**.
1. 修改

   ```
   status
   ```

   加行 **:A** 狀態為3個字母的鍵：
   <pre>status=PLN:A<br>status_Mod=in</pre>

1. 按一下 **完成**，然後 **儲存篩選**.

   清單僅顯示處於「計畫 — 待批准」狀態的項目。
