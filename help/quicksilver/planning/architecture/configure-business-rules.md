---
title: 設定記錄型別商業規則
description: 您可以設定記錄型別商業規則，定義如何在Adobe Workfront Planning中管理該型別的記錄。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
source-git-commit: 159b845c7b755117197d18f8474c01d4b19d53b8
workflow-type: tm+mt
source-wordcount: '249'
ht-degree: 4%

---


# 設定記錄型別商業規則

{{planning-important-intro}}

<!--
<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the release to Preview, the same features are also available monthly in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

您可以設定記錄型別商業規則，定義如何在Adobe Workfront Planning中管理該型別的記錄。

## 存取權要求

+++ 展開以檢視存取需求，以執行本文中的步驟：  

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront 封裝</p></td> 
   <td> 
<ul> 
<li><p>具有Planning套件的任何Workfront或工作流程</p></li>
或
<li><p>以獨立產品形式購買時的任何Planning套件</p></li></ul>
   </td> </tr>
  <tr> 
   <td role="rowheader"><p>Adobe Workfront授權</p></td> 
   <td><p>Workflow Standard</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Adobe計畫授權</p></td> 
   <td><p>規劃標準</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>存取層級設定</p></td> 
   <td> <p>擁有Workflow和Planning套件時，您必須將Workflow和Planning授權型別新增到存取層級</p>   
</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>物件許可權</p></td> 
   <td>   <p>管理工作區和記錄型別的許可權</p>  
   <p>系統管理員擁有所有工作區的許可權，包括他們未建立的工作區</p>  </td> 
  </tr>  
</tbody> 
</table>

如需Workfront存取需求的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 設定商業規則時的注意事項

* 您可以設定何時可編輯或刪除記錄的規則。
* 建立記錄時，您無法設定規則。 擁有記錄型別管理許可權的所有人都可以建立記錄。
* 您可以為商業規則建立條件，該條件會參考以下欄位型別以外的所有欄位型別：
  * 公式欄位
  * 查詢欄位
  * 參考欄位

## 設定商業規則

1. 移至記錄型別。
1. 按一下記錄型別名稱右側的&#x200B;**更多**&#x200B;功能表![更多功能表](assets/more-menu.png)，然後按一下「商業規則」。



