---
title: 編輯欄位
description: 在Adobe Workfront規劃中，您可以編輯已建立欄位的欄位設定。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 6c35c313-d6ed-428b-b70d-2ea242da4e8f
source-git-commit: a0f12a016ae8ac73136f05bf3255f9882e2ce6d4
workflow-type: tm+mt
source-wordcount: '440'
ht-degree: 0%

---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

<!---
title: Edit foelds
description: In Adobe Maestro, you can edit the field settings for fields that are already created.
hidefromtoc: yes
hide: yes
author: Alina
feature: (*******************WE NEED A NEW ONE*******************)
role: User, Administrator (************is this right???************)
recommendations: noDisplay, noCatalog
--->


# 編輯欄位

{{maestro-important-intro}}

您可以編輯已在Adobe Workfront規劃中建立的欄位之欄位設定。

如需有關建立Adobe Workfront規劃欄位的資訊，請參閱 [建立欄位](../fields/create-fields.md).

本文說明如何編輯Workfront規劃欄位的設定。 如需有關編輯記錄欄位值的資訊，請參閱 [編輯記錄](/help/quicksilver/maestro/records/edit-records.md).

## 編輯欄位資訊的考量事項

* 如果您擁有該欄位所屬工作區的管理許可權，您可以編輯您建立的欄位或其他使用者建立的欄位。
* 您可以在記錄型別表格中編輯欄位。
* 您無法在記錄的詳細資訊頁面或時間軸檢視中編輯欄位。
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
<p>貴組織必須註冊Adobe Workfront計畫Beta版計畫。 請聯絡您的客戶代表以查詢此新產品/服務。 </p>
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
   <td role="rowheader"><p>存取層級設定</p></td>
   <td> <p>Workfront計畫沒有存取控制</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>權限</p></td>
   <td> <p>管理工作區的許可權</a> </p>  
   <p>系統管理員擁有所有工作區的許可權，包括他們未建立的工作區</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>版面配置範本</p></td>
   <td> <p>您的Workfront或群組管理員必須在版面配置範本中新增Planning區域。 如需詳細資訊，請參閱 <a href="../access/access-overview.md">存取權總覽</a>. </p>  
</td>
  </tr>

</tbody>
</table>

<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

## 編輯欄位

{{step1-to-maestro}}

    根據預設，上次存取的工作區應該會開啟。

1. （可選）展開現有工作區名稱右側的向下箭頭，並選取您要刪除記錄型別的工作區。

   工作區隨即開啟，並顯示與其關聯的記錄型別。
1. 按一下您要編輯其欄位的記錄型別的卡片。

   這會開啟記錄型別的頁面。
1. （視條件而定）選取 **表格檢視** 從 **檢視** 記錄型別頁面右上角的下拉式功能表。
1. 將游標停留在您要編輯的欄位標題上，然後按一下欄位名稱后的向下箭頭，然後按一下 **編輯欄位**

   或

   連按兩下欄位的欄標題。

   ![](assets/arrow-menu-after-name-of-field-in-table-header-highlighted.png)

1. 更新欄位的相關資訊，然後按一下 **儲存**.

   <!--insert screen shot when finalized-->

   >[!TIP]
   >
   >儲存欄位後，您無法更新欄位型別。


1. （視條件而定）對於連結的記錄欄位，按一下 **編輯查閱欄位** 和從連結的記錄型別新增或移除任何欄位。

   如需詳細資訊，請參閱 [連線記錄型別](../architecture/connect-record-types.md).
