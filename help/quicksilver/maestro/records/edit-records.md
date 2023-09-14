---
title: 編輯記錄
description: 您可以在Adobe Maestro中編輯記錄資訊。 您必須先建立記錄型別，才能開始建立和編輯記錄。
hidefromtoc: true
hide: true
source-git-commit: f058c369bdb3b991910d3a820895de73ea4709f0
workflow-type: tm+mt
source-wordcount: '545'
ht-degree: 2%

---


<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# 編輯記錄

>[!IMPORTANT]
>
>目前，Adobe大師是測試版計畫的一部分，向有限數量的客戶開放。
>
>如需加入Maestro測試版計畫的詳細資訊，請聯絡您的客戶代表。
>
>如需詳細資訊，請參閱 [Adobe大師概觀](../maestro-overview.md).

您可以在Adobe Maestro中編輯記錄資訊。 您必須先建立記錄型別，才能開始建立和編輯記錄。
如需詳細資訊，請參閱 [建立記錄型別](../architecture-and-fields/create-record-types.md).

&lt;! — 在此提及，詳細資訊檢視中的欄位與表格檢視中的欄位相同 — 本文從「管理記錄」檢視連結，其中一個參考此資訊 — >

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

## 編輯記錄的相關考量事項

* 您可以編輯您或其他使用者建立的記錄。 <!--will change with access levels-->
* 如果編輯的記錄連結到其他記錄，則您正在編輯的記錄的新資訊會反映在連結的記錄上。
* 您無法大量編輯記錄。 <!--this will probably change-->

## 編輯記錄

您可以從下列區域編輯記錄：

* [從記錄的詳細資訊頁面](#edit-a-record-from-the-records-details-page)
* [從記錄型別的表格檢視](#edit-a-record-from-the-record-type-table-view)

### 從記錄的「詳細資訊」頁面編輯記錄

1. 按一下 **主要功能表** ![](assets/main-menu-workfront.png) 位於右上角，或 **主要功能表** ![](assets/main-menu-shell.png) 如果可用，請按一下「Maestro」。

   您上次存取的工作區會開啟。
1. 執行下列任一項作業：

   * 在「表格」檢視中，按一下記錄名稱。
   * 在「表格」檢視中，暫留在記錄名稱上，然後按一下 **更多** 功能表 ![](assets/more-menu.png)，然後按一下 **檢視**

     ![](assets/contextual-menu-for-record-row.png)
   * 在「時間軸」檢視中，按一下記錄列。

   記錄 **詳細資料** 頁面隨即開啟。

1. 按一下 **更多** 功能表 ![](assets/more-menu.png) 在記錄名稱的右側，然後按一下 **編輯**

   或

   按一下「詳細資訊」頁面上的任何可編輯欄位以編輯資訊。

   ![](assets/more-menu-options-from-record-details-page.png) <!--ensure the options have not changed or been renamed-->

   >[!NOTE]
   >
   >    包含計算或由系統產生的連結欄位或欄位無法編輯。


1. 按一下 **儲存變更**. <!--logged a bug for this - this needs to be "Save"-->

### 從記錄型別表格檢視編輯記錄

1. 按一下 **主要功能表** ![](assets/main-menu-workfront.png) 在右上角， <!--or the **Main Menu** ![](assets/main-menu-shell.png) in the upper-left corner, if it is available,--> 然後按一下 **大師** ![](assets/maestro-icon.png).

   您上次存取的工作區會開啟。
1. 按一下記錄型別卡。

   記錄型別頁面隨即開啟。
1. （視條件而定）從 **檢視** 在表格右上角的下拉式功能表中，選取「表格」檢視。 這應為預設檢視，除非您上次存取時間軸檢視時已檢視該記錄型別。

   與所選記錄型別相關聯的記錄會顯示在表格檢視中。
1. 按一下記錄列內部，開始編輯內嵌記錄的相關資訊，然後按下 **輸入** 以儲存變更。 變更會自動儲存。

   >[!TIP]
   >
   >連結的欄位不可編輯。 這些欄位的資訊會自動從連結的記錄中填入。 如需詳細資訊，請參閱 [連線記錄型別](../architecture-and-fields/connect-record-types.md).



