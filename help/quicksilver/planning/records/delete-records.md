---
title: 刪除記錄
description: 您可以刪除您或其他使用者建立的記錄。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 3f7a3667-8a9f-462a-b706-cf15850a0d1c
source-git-commit: 298c542afea902d9fc14ef6a4470c0bc1d9bd33c
workflow-type: tm+mt
source-wordcount: '681'
ht-degree: 2%

---


# 刪除記錄

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>  -->

{{planning-important-intro}}

您可以刪除Adobe Workfront Planning中不再相關的記錄。 刪除的記錄後，您可以在30天內復原這些記錄。 如需有關復原已刪除記錄的資訊，請參閱[復原已刪除的記錄](/help/quicksilver/planning/records/restore-deleted-records.md)。

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
   <td>   <p>貢獻或更高的許可權至工作區和記錄型別</a> </p>  
   <p>系統管理員擁有所有工作區的許可權，包括他們未建立的工作區</p> </td> 
  </tr> 
</tbody> 
</table>

*如需Workfront存取需求的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 刪除記錄的相關考量事項

* 您可以刪除您或其他使用者建立的記錄。
* 您可以復原您或其他人已刪除的記錄。
* 如果刪除的記錄連結到其他記錄，則連結的記錄不會被刪除，但是已刪除的記錄中的資訊也會被刪除。
* 您無法從時間軸或行事曆檢視中刪除記錄。

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
   * 在[資料表]檢視中，暫留在記錄名稱上，然後按一下[其他] **&#x200B;**&#x200B;[其他]功能表![ [其他]功能表](assets/more-menu.png)，然後按一下[檢視] **&#x200B;**

     ![記錄列](assets/contextual-menu-for-record-row.png)的內容相關功能表
   * 在「時間軸」檢視中，按一下記錄列。

   記錄頁面隨即開啟。

1. 按一下記錄名稱右側的&#x200B;**更多**&#x200B;功能表![更多功能表](assets/more-menu.png)，然後按一下&#x200B;**刪除**，再按一次&#x200B;**刪除**&#x200B;以進行確認。

   ![記錄詳細資料頁面中的更多功能表選項](assets/more-menu-options-from-record-details-page.png) <!--ensure the options have not changed or been renamed-->
記錄已刪除。
1. （選擇性）移至記錄頁面的表格檢視，然後按一下檢視右上角的&#x200B;**還原**&#x200B;圖示![還原圖示](assets/undo-icon.png)，然後按一下&#x200B;**最近刪除**&#x200B;以復原刪除的記錄。

如需有關復原已刪除記錄的資訊，請參閱[復原已刪除的記錄](/help/quicksilver/planning/records/restore-deleted-records.md)。

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
   * 按一下記錄名稱右邊的&#x200B;**更多**&#x200B;功能表![更多功能表](assets/more-menu.png)，然後按一下&#x200B;**刪除**。

     ![記錄列](assets/contextual-menu-for-record-row.png)的內容相關功能表

   * 按一下&#x200B;**開啟詳細資料**&#x200B;圖示![開啟資料表名稱欄位中的詳細資料圖示](assets/open-details-icon-in-table-name-field.png)以開啟包含記錄詳細資訊的方塊，然後按一下記錄名稱右側的&#x200B;**更多** ![更多功能表](assets/more-menu.png)，然後&#x200B;**刪除**。

   記錄已刪除。

1. （選擇性）執行下列任一項作業，以復原或重做刪除記錄：

   * 按一下&#x200B;**復原**&#x200B;圖示![復原圖示](assets/undo-icon.png)，然後按一下&#x200B;**最近刪除的**，復原刪除的記錄。 如需有關復原已刪除記錄的資訊，請參閱[復原已刪除的記錄](/help/quicksilver/planning/records/restore-deleted-records.md)。
   * 使用下列鍵盤快速鍵來復原或重做刪除記錄：

      * 按CTRL + Z (⌘ + Z代表Mac)以復原刪除記錄
      * 按CTRL + Shift + Z (⌘ + Shift + Z代表Mac)以重做刪除記錄




