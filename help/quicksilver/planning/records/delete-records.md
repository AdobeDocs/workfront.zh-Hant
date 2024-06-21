---
title: 刪除記錄
description: 您可以刪除您或其他使用者建立的記錄。 您無法復原已刪除的記錄。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 3f7a3667-8a9f-462a-b706-cf15850a0d1c
source-git-commit: f5430d81f1914a3717130de3af54b4b84e0e2d06
workflow-type: tm+mt
source-wordcount: '507'
ht-degree: 2%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->

# 刪除記錄

{{planning-important-intro}}

您可以刪除Adobe Workfront Planning中不再相關的記錄。

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

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
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront合約</p></td>
   <td>
<p>您的組織必須處於Workfront Planning的早期存取階段中註冊 </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront計畫</p></td>
   <td>
<p>任何</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront授權*</p>
   </td>
   <td>
   <p>新增：標準</p>
   <p>目前：計畫</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>存取層級設定</p></td>
   <td> <p>Adobe Workfront Planning沒有存取層級控制 </p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>權限</p></td>
   <td> <p>貢獻或更高的工作區許可權</a> </p>  
   <p>系統管理員擁有所有工作區的許可權，包括他們未建立的工作區</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>版面配置範本</p></td>
   <td> <p>您的Workfront或群組管理員必須在版面配置範本中新增Planning區域。 如需詳細資訊，請參閱 <a href="/help/quicksilver/planning/access/access-overview.md">存取權總覽</a>. </p>  
</td>
  </tr>

</tbody>
</table>


<!--Maybe enable this at GA - but Planning is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

## 刪除記錄的相關考量事項

* 您可以刪除您或其他使用者建立的記錄。
* 您無法復原已刪除的記錄。 <!--the above statements (and in the metadata description) will change with access levels and recycle bin??-->
* 如果刪除的記錄連結到其他記錄，則連結的記錄不會被刪除，但是已刪除的記錄中的資訊也會被刪除。
* 您無法大量刪除記錄。 <!--this will probably change-->
* 您無法從時間表檢視中刪除記錄。

## 刪除記錄

您可以從下列區域刪除記錄：

* [從紀錄的頁面](#delete-a-record-from-the-records-page)
* [從記錄型別的表格檢視](#delete-a-record-from-the-record-type-table-view)

### 從記錄頁面刪除記錄

{{step1-to-planning}}

1. 按一下要刪除其記錄的工作區。

   工作區隨即開啟，且記錄型別會顯示為卡片。

1. 按一下記錄型別卡。

   記錄型別頁面隨即開啟。
1. 執行下列其中一項：

   * 在「表格」檢視中，按一下記錄名稱。
   * 在「表格」檢視中，暫留在記錄名稱上，然後按一下 **更多** 功能表 ![](assets/more-menu.png)，然後按一下 **檢視**

     ![](assets/contextual-menu-for-record-row.png)
   * 在「時間軸」檢視中，按一下記錄列。

   記錄頁面隨即開啟。

1. 按一下 **更多** 功能表 ![](assets/more-menu.png) 在記錄名稱的右側，然後按一下 **刪除**，然後 **刪除** 再次確認。

   ![](assets/more-menu-options-from-record-details-page.png) <!--ensure the options have not changed or been renamed-->
記錄已刪除，無法復原。

### 從記錄型別表格檢視中刪除記錄

{{step1-to-planning}}

1. 按一下要刪除其記錄的工作區。

   工作區隨即開啟，且記錄型別會顯示為卡片。

1. 按一下記錄型別卡。

   記錄型別頁面隨即開啟。
1. （視條件而定）從 **檢視** 在表格左上角的下拉式功能表中，選取「表格」檢視。 這應為預設檢視，除非您上次存取時間軸檢視時已檢視該記錄型別。

   與所選記錄型別相關聯的記錄會顯示在表格檢視中。
1. 執行下列其中一項：

   * 以滑鼠右鍵按一下記錄列，然後按一下 **刪除**.
   * 按一下 **更多** 功能表 ![](assets/more-menu.png) 在記錄名稱的右側，然後按一下 **刪除**

     ![](assets/contextual-menu-for-record-row.png)

   * 按一下 **開啟詳細資料** 圖示 ![](assets/open-details-icon-in-table-name-field.png) 開啟包含記錄詳細資訊的方塊，然後按一下 **更多** ![](assets/more-menu.png) 在記錄名稱的右側，然後 **刪除**.

   記錄已刪除，無法復原。

1. （可選）使用下列鍵盤快速鍵來復原或重做刪除記錄：

   * CTRL + Z (Mac為⌘ + Z)可復原變更
   * CTRL + Shift + Z (Mac為⌘ + Shift + Z)以重做變更
