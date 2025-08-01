---
title: 刪除欄位
description: 在Adobe Workfront規劃中，您可以刪除不再相關的自訂欄位。
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
author: Alina
exl-id: ec48db42-2395-4439-97ae-e4f5242170b7
source-git-commit: 298c542afea902d9fc14ef6a4470c0bc1d9bd33c
workflow-type: tm+mt
source-wordcount: '467'
ht-degree: 1%

---



# 刪除欄位

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

在Adobe Workfront Planning中，您可以建立自訂欄位來儲存有關記錄的資訊。

如需有關在Workfront Planning中建立自訂欄位的資訊，請參閱[建立欄位](/help/quicksilver/planning/fields/create-fields.md)。

您可以刪除不再相關的Workfront規劃欄位。

## 刪除Workfront Planning欄位的相關考量事項：

* 您只能在記錄型別表格檢視中刪除欄位。
* 您無法刪除記錄的主要欄位。
* 儲存在欄位中的任何資訊都會被刪除且無法復原。
* 當您刪除連線的記錄欄位時，所有連線的查閱欄位也會從您連線的記錄型別中刪除。 您所連線之記錄型別的連線記錄欄位也會從您所連線的記錄中刪除。

  例如，當您將行銷活動連結到另一個記錄型別「產品」，並從行銷活動刪除「已連結產品」欄位和「產品狀態」查詢欄位時，以下專案即被刪除：

   * 來自行銷活動的已連線產品欄位
   * 來自行銷活動的產品狀態查詢欄位
   * 產品中的「已連線促銷活動」欄位。

  如需詳細資訊，請參閱[連線記錄型別](/help/quicksilver/planning/architecture/connect-record-types.md)。

<!-- this is not possible yet, since fields cannot be shared yet; maybe move this up a bit, in this bullet list: * When you delete a field, it is deleted from all records associated with the field.-->

## 存取需求

+++ 展開以檢視存取需求。

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> 產品</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront規劃<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront計畫*</p></td> 
   <td> 
<p>下列任一Workfront計畫：</p> 
<ul><li>選取</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>舊版Workfront計畫不提供Workfront計畫</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront規劃套件*</p></td> 
   <td> 
<p>任何 </p> 
<p>如需每個Workfront計畫包含內容的詳細資訊，請聯絡您的Workfront客戶經理。 </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront平台</p></td> 
   <td> 
<p>貴組織的Workfront例項必須上線至Adobe Unified Experience，才能存取Workfront Planning。</p> 
<p>如需詳細資訊，請參閱<a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">適用於Workfront的Adobe Unified Experience</a>。 </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront授權*</p></td> 
   <td><p> 標準 </p>
   <p>Workfront計畫不適用於舊版Workfront授權</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>存取層級設定</p></td> 
   <td> <p>Adobe Workfront Planning沒有存取層級控制</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>物件許可權</p></td> 
   <td>   <p>管理工作區與記錄型別</a>的許可權 </p>  
   <p>系統管理員擁有所有工作區的許可權，包括他們未建立的工作區</p></td> 
  </tr> 
</tbody> 
</table>

*如需Workfront存取需求的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 刪除欄位

<!--When they release the sharing of fields between other records, revise this section.  -->

{{step1-to-planning}}

1. 按一下要刪除其記錄欄位的工作區。

   工作區隨即開啟，且記錄型別隨即顯示。

1. 按一下記錄型別的卡片。

1. （視條件而定）如果尚未選取，請按一下記錄型別頁面上&#x200B;**資料表檢視**&#x200B;的索引標籤。

   與記錄型別關聯的所有現有記錄都會顯示在表格檢視的列中。

1. 在欄標題中尋找要刪除的欄位，並將滑鼠游標停留在欄標題上，然後按一下欄位名稱后面的向下箭頭。

   在表格標題中反白顯示的欄位名稱后面的![箭頭選單](assets/arrow-menu-after-name-of-field-in-table-header-highlighted.png)

1. 按一下&#x200B;**刪除**。<!-- check this: they might replace it with **Delete field**-->

   <!--insert screen shot when finalized-->

1. 按一下&#x200B;**刪除**&#x200B;確認。

   欄位已刪除、無法復原，且無法再與任何記錄相關聯。
