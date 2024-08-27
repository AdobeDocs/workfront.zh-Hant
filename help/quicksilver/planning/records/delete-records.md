---
title: 刪除記錄
description: 您可以刪除您或其他使用者建立的記錄。 您無法復原已刪除的記錄。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 3f7a3667-8a9f-462a-b706-cf15850a0d1c
source-git-commit: cf42511263ec1cffd90d1e4bdcd43521b7fe6a30
workflow-type: tm+mt
source-wordcount: '599'
ht-degree: 2%

---


# 刪除記錄

{{planning-important-intro}}

您可以刪除Adobe Workfront Planning中不再相關的記錄。

## 存取需求

+++ 展開以檢視Workfront Planning的存取需求。

您必須具備下列專案才能存取Workfront Planning：

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
   <td role="rowheader"><p>Adobe Workfront規劃計畫*</p></td> 
   <td> 
<p>任何 </p> 
<p>如需每個Workfront Planning計畫包含哪些專案的詳細資訊，請參閱<a href="https://business.adobe.com/products/workfront/pricing.html">Adobe Workfront定價與封裝</a>。 </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront平台</p></td> 
   <td> 
<p>貴組織的Workfront例項必須加入Adobe統一體驗，才能存取Workfront規劃的所有功能。</p> 
<p>如需詳細資訊，請參閱<a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Workfront的Adobe統一體驗</a>。 </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront授權*</p></td> 
   <td><p> 標準</p>
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
   <td>   <p>Contribute或更高的工作區許可權</a> </p>  
   <p>系統管理員擁有所有工作區的許可權，包括他們未建立的工作區</p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>版面配置範本</p></td> 
   <td> <p>必須為所有使用者(包括Workfront管理員)指派一個版面配置範本，該範本包含主功能表中的Planning區域。 </p> </td> 
  </tr> 
</tbody> 
</table>

*如需Workfront存取需求的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++


<!--

OLD

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Product</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the early access stage for Workfront Planning </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license*</p>
   </td>
   <td>
   <p>New: Standard</p>
   <p>Current: Plan</p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level configurations</p></td>
   <td> <p>There are no access level controls for Adobe Workfront Planning </p>  
</td>
  </tr>

  <tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>Contribute or higher permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your Workfront or group administrator must add the Planning area in your layout template. For information, see <a href="/help/quicksilver/planning/access/access-overview.md">Access overview</a>. </p>  
</td>
  </tr>

 </tbody>
</table>

*For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

-->

## 刪除記錄的相關考量事項

* 您可以刪除您或其他使用者建立的記錄。
* 您無法復原已刪除的記錄。<!--the above statements (and in the metadata description) will change with access levels and recycle bin??-->
* 如果刪除的記錄連結到其他記錄，則連結的記錄不會被刪除，但是已刪除的記錄中的資訊也會被刪除。
* 您無法大量刪除記錄。<!--this will probably change-->
* 您無法從時間表檢視中刪除記錄。

## 刪除記錄

您可以從下列區域刪除記錄：

* [從紀錄的頁面](#delete-a-record-from-the-records-page)
* [從記錄型別的資料表檢視](#delete-a-record-from-the-record-type-table-view)

### 從記錄頁面刪除記錄

{{step1-to-planning}}

1. 按一下要刪除其記錄的工作區。

   工作區隨即開啟，且記錄型別會顯示為卡片。

1. 按一下記錄型別卡。

   記錄型別頁面隨即開啟。
1. 執行下列其中一項：

   * 在「表格」檢視中，按一下記錄名稱。
   * 在[資料表]檢視中，暫留在記錄名稱上，然後按一下&#x200B;**更多**&#x200B;功能表![](assets/more-menu.png)，然後按一下&#x200B;**檢視**

     ![](assets/contextual-menu-for-record-row.png)
   * 在「時間軸」檢視中，按一下記錄列。

   記錄頁面隨即開啟。

1. 按一下記錄名稱右側的&#x200B;**更多**&#x200B;功能表![](assets/more-menu.png)，然後按一下&#x200B;**刪除**，再按一次&#x200B;**刪除**&#x200B;以進行確認。

   ![](assets/more-menu-options-from-record-details-page.png) <!--ensure the options have not changed or been renamed-->
記錄已刪除，無法復原。

### 從記錄型別表格檢視中刪除記錄

{{step1-to-planning}}

1. 按一下要刪除其記錄的工作區。

   工作區隨即開啟，且記錄型別會顯示為卡片。

1. 按一下記錄型別卡。

   記錄型別頁面隨即開啟。
1. （視條件而定）從表格左上角的&#x200B;**檢視**&#x200B;下拉式功能表中，選取表格檢視。 這應為預設檢視，除非您上次存取時間軸檢視時已檢視該記錄型別。

   與所選記錄型別相關聯的記錄會顯示在表格檢視中。
1. 執行下列其中一項：

   * 以滑鼠右鍵按一下記錄列，然後按一下&#x200B;**刪除**。
   * 按一下記錄名稱右側的&#x200B;**更多**&#x200B;功能表![](assets/more-menu.png)，然後按一下&#x200B;**刪除**

     ![](assets/contextual-menu-for-record-row.png)

   * 按一下&#x200B;**開啟詳細資料**&#x200B;圖示![](assets/open-details-icon-in-table-name-field.png)以開啟包含記錄詳細資訊的方塊，然後按一下記錄名稱右側的&#x200B;**更多** ![](assets/more-menu.png)，然後&#x200B;**刪除**。

   記錄已刪除，無法復原。

1. （可選）使用下列鍵盤快速鍵來復原或重做刪除記錄：

   * CTRL + Z (Mac為⌘ + Z)可復原變更
   * CTRL + Shift + Z (Mac為⌘ + Shift + Z)以重做變更
