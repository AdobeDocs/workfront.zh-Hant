---
title: 刪除記錄
description: 您可以刪除您或其他使用者建立的記錄。 您無法復原已刪除的記錄。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 3f7a3667-8a9f-462a-b706-cf15850a0d1c
source-git-commit: 5f3d5c93c2fc721dda2dd04adac22190ef6a3f29
workflow-type: tm+mt
source-wordcount: '543'
ht-degree: 1%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->

# 刪除記錄

>[!IMPORTANT]
>
>本文資訊是指Adobe Maestro，這是Adobe Workfront的新產品。
>
>目前，Adobe大師是測試版計畫的一部分，向有限數量的客戶開放。 您必須是Workfront客戶才能使用Maestro功能。
>
>如需加入Maestro測試版計畫的詳細資訊，請聯絡您的客戶代表。
>
>如需詳細資訊，請參閱 [Adobe大師概觀](../maestro-overview.md).

您可以刪除Adobe Maestro中不再相關的記錄。

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
<p>貴組織必須註冊AdobeMaestro封閉測試版計畫。 請聯絡您的客戶代表以查詢此新產品/服務。 </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront計畫</p></td>
   <td>
<p>任何</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront授權</p>
   </td>
   <td>
   <p>任何</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>存取層級設定</p></td>
   <td> <p>Maestro沒有存取層級控制項 </p>  
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
   <td> <p>您的Workfront或群組管理員必須在您的版面配置範本中新增Maestro區域。 如需詳細資訊，請參閱 <a href="../access/access-overview.md">存取權總覽</a>. </p>  
</td>
  </tr>

</tbody>
</table>


<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

## 刪除記錄的相關考量事項

* 您可以刪除您或其他使用者建立的記錄。
* 您無法復原已刪除的記錄。 <!--the above statements (and in the metadata description) will change with access levels and recycle bin??-->
* 如果刪除的記錄連結到其他記錄，則連結的記錄不會被刪除，但是已刪除的記錄中的資訊也會被刪除。
* 您無法大量刪除記錄。 <!--this will probably change-->
* 您無法從時間表檢視中刪除記錄。
* 您無法刪除從其他應用程式連結的記錄型別。 例如，如果您將Maestro記錄連結至Workfront物件，則無法從Workfront物件記錄頁面刪除Workfront物件。

## 刪除記錄

您可以從下列區域刪除記錄：

* [從記錄的詳細資訊頁面](#delete-a-record-from-the-records-details-page)
* [從記錄型別的表格檢視](#delete-a-record-from-the-record-type-table-view)

### 從記錄的「詳細資訊」頁面中刪除記錄

{{step1-to-maestro}}

您上次存取的工作區會開啟。

1. 按一下記錄型別。

   記錄型別頁面隨即開啟。
1. 執行下列其中一項：

   * 在「表格」檢視中，按一下記錄名稱。
   * 在「表格」檢視中，暫留在記錄名稱上，然後按一下 **更多** 功能表 ![](assets/more-menu.png)，然後按一下 **檢視**

     ![](assets/contextual-menu-for-record-row.png)
   * 在「時間軸」檢視中，按一下記錄列。

   記錄 **詳細資料** 頁面隨即開啟。

1. 按一下 **更多** 功能表 ![](assets/more-menu.png) 在記錄名稱的右側，然後按一下 **刪除**，然後 **刪除** 再次確認。

   ![](assets/more-menu-options-from-record-details-page.png) <!--ensure the options have not changed or been renamed-->
記錄已刪除，無法復原。

### 從記錄型別表格檢視中刪除記錄

{{step1-to-maestro}}

您上次存取的工作區會開啟。

1. 按一下記錄型別。

   記錄型別頁面隨即開啟。
1. （視條件而定）從 **檢視** 在表格右上角的下拉式功能表中，選取「表格」檢視。 這應為預設檢視，除非您上次存取時間軸檢視時已檢視該記錄型別。

   與所選記錄型別相關聯的記錄會顯示在表格檢視中。
1. 以滑鼠右鍵按一下記錄列，然後按一下 **刪除**.

   ![](assets/contextual-menu-for-record-row.png)

   記錄已刪除，無法復原。

1. （可選）使用下列鍵盤快速鍵來復原或重做刪除記錄：

   * CTRL + Z (Mac為⌘ + Z)可復原變更
   * CTRL + Shift + Z (Mac為⌘ + Shift + Z)以重做變更
