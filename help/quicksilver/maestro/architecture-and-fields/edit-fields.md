---
title: 編輯欄位
description: 在Adobe大師，您可以編輯已建立欄位的欄位設定。
hidefromtoc: true
hide: true
source-git-commit: f058c369bdb3b991910d3a820895de73ea4709f0
workflow-type: tm+mt
source-wordcount: '427'
ht-degree: 1%

---


<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# 編輯欄位

>[!IMPORTANT]
>
>目前，Adobe大師是測試版計畫的一部分，向有限數量的客戶開放。
>
>如需加入Maestro測試版計畫的詳細資訊，請聯絡您的客戶代表。
>
>如需詳細資訊，請參閱 [Adobe大師概觀](../maestro-overview.md).

您可以編輯已建立欄位的欄位設定。

如需有關建立Adobe主要欄位的資訊，請參閱 [建立欄位](../architecture-and-fields/create-fields.md).

本文說明如何編輯Maestro欄位的設定。 如需有關編輯Maestro記錄欄位值的資訊，請參閱 [編輯記錄](../records/edit-records.md).

## 編輯欄位資訊的考量事項

* 您可以編輯您建立的欄位或其他使用者建立的欄位。 <!--this will change with access levels/ permissions-->
* 您可以在記錄型別表格中編輯欄位。
* 儲存欄位後，您無法編輯欄位型別。
* 如果先前選取的「數字」、「百分比」或「幣別」欄位在其附加的記錄中已有負值，則無法取消選取該欄位的「允許負數」設定。
<!--this is not true yet; one piece of it is true and I added it as the bullet above: 
* You cannot edit the options, or the special format of the following fields, after they are saved:

    * Allow negative numbers option from a Number, Percentage, or Currency field. 
    * The Options of a Single-select or a Multi-select field.
-->

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto">
 <col>
 <tbody>
<td>
   <p> Adobe產品</p> </td>
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
   <td role="rowheader"><p>Adobe Workfront授權</p></td>
   <td>
   <p>任何</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader">存取層級</td>
   <td> <p>任何</p>  
</td>
  </tr>
<tr>
   <td role="rowheader">版面配置範本</td>
   <td> <p>您的系統管理員必須在您的版面配置範本中新增Maestro區域。 如需詳細資訊，請參閱 <a href="../access/grant-access.md">授與Adobe大師的存取權</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->

## 編輯欄位

1. 按一下 **主要功能表** 圖示 ![](assets/main-menu-workfront.png) 在Workfront的右上角， <!---or the **Main menu** icon ![](assets/main-menu-shell.png)  in the upper-left corner, if available--> 然後按一下 **大師** ![](assets/maestro-icon.png).

   根據預設，上次存取的工作區應該會開啟。

1. （可選）展開現有工作區名稱右側的向下箭頭，並選取您要刪除記錄型別的工作區。

   工作區隨即開啟，並顯示與其關聯的記錄型別和分類法。
1. 按一下您要編輯其欄位的記錄型別或分類法的卡片。

   這會開啟記錄型別的頁面。
1. （視條件而定）選取 **表格檢視** 從 **檢視** 記錄型別頁面右上角的下拉式功能表。
1. 暫留在您要編輯的欄位之欄標題上，然後按一下欄位名稱后的向下箭頭。
1. 按一下 **編輯欄位**，然後更新欄位的相關資訊並按一下 **儲存**.

   <!--insert screen shot when finalized-->

   >[!TIP]
   >
   >儲存欄位後，您無法更新欄位型別。


1. （視條件而定）對於連結的記錄欄位，按一下 **編輯查閱欄位** 和從連結的記錄型別新增或移除任何欄位。

   如需詳細資訊，請參閱 [連線記錄型別](../architecture-and-fields/connect-record-types.md).