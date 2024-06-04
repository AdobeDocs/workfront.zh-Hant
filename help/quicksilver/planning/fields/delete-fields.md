---
title: 刪除欄位
description: 在Adobe Workfront規劃中，您可以刪除不再相關的自訂欄位。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: ec48db42-2395-4439-97ae-e4f5242170b7
source-git-commit: 160bcc8796666c9615ebe8ead18813b96be26a71
workflow-type: tm+mt
source-wordcount: '323'
ht-degree: 0%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!---
title: Delete fields
description: In Adobe Planning, you can delete custom fields that are no longer relevant.
hidefromtoc: yes
hide: yes
author: Alina
feature: (*******************WE NEED A NEW ONE*******************)
role: User, Administrator (************is this right???************)
recommendations: noDisplay, noCatalog
--->

# 刪除欄位

{{planning-important-intro}}

在Adobe Workfront Planning中，您可以建立自訂欄位來儲存有關記錄的資訊。

如需有關在Workfront Planning中建立自訂欄位的資訊，請參閱 [建立欄位](/help/quicksilver/planning/fields/create-fields.md).

您可以刪除不再相關的Workfront規劃欄位。

## 刪除Workfront Planning欄位的相關考量事項：

* 您只能在記錄型別表格檢視中刪除欄位。
* 您無法刪除記錄的主要欄位。
* 儲存在欄位中的任何資訊都會被刪除且無法復原。
* 當您刪除連結的記錄欄位時，所有連結的查閱欄位也會從您連結的記錄型別中刪除。 您連結到的記錄型別的連結記錄欄位不會被刪除。

  如需詳細資訊，請參閱 [連線記錄型別](/help/quicksilver/planning/architecture/connect-record-types.md).

<!-- this is not possible yet, since fields cannot be shared yet; maybe move this up a bit, in this bullet list: * When you delete a field, it is deleted from all records associated with the field.-->

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
   <td role="rowheader"><p>Adobe Workfront授權</p></td>
   <td>
   <p>任何</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>存取層級設定</p></td>
   <td> <p>Workfront Planning沒有存取層級控制</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>版面配置範本</p></td>
   <td> <p>您的Workfront或群組管理員必須在版面配置範本中新增Planning區域。 如需詳細資訊，請參閱 <a href="/help/quicksilver/planning/access/access-overview.md">存取權總覽</a>. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>權限</p></td>
   <td> <p>管理工作區的許可權</a> </p>  
   <p>系統管理員擁有所有工作區的許可權，包括他們未建立的工作區</p>
</td>
  </tr>
 </tbody>
</table>



<!--Maybe enable this at GA - but Planning is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

## 刪除欄位

<!--When they release the sharing of fields between other records, revise this section.  -->

{{step1-to-planning}}

這會開啟上次在Workfront Planning中存取的工作區。
1. 按一下要刪除其欄位的記錄型別的卡片。
1. （視條件而定）選取 **表格檢視** 從 **檢視** 記錄型別頁面右上角的下拉式功能表。
1. 在欄標題中尋找要刪除的欄位，並將滑鼠游標停留在欄標題上，然後按一下欄位名稱后面的向下箭頭。

   ![](assets/arrow-menu-after-name-of-field-in-table-header-highlighted.png)

1. 按一下 **刪除**. <!-- check this: they might replace it with **Delete field**-->

   <!--insert screen shot when finalized-->

1. 按一下 **刪除** 以確認。

   欄位已刪除、無法復原，且無法再與任何記錄相關聯。
