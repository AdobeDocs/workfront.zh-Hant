---
title: 編輯記錄
description: 您可以在Adobe Maestro中編輯記錄資訊。 您必須先建立記錄型別，才能開始建立和編輯記錄。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 981b8e44-b548-4f94-bf89-5f5dec3a6166
source-git-commit: 1ae60512c337d778939ef6c48fd2eda8b279dcce
workflow-type: tm+mt
source-wordcount: '875'
ht-degree: 1%

---

<!--update the metadata with real information when making this avilable in TOC and in the left nav-->

# 編輯記錄

>[!IMPORTANT]
>
>本文資訊是指Adobe Maestro，這是Adobe Workfront的新產品。
>
>目前，Adobe大師是測試版計畫的一部分，向有限數量的客戶開放。 您必須是Workfront客戶才能使用Maestro功能。
>
>如需加入Maestro測試版計畫的詳細資訊，請聯絡您的客戶代表。
>
>如需詳細資訊，請參閱 [Adobe大師概觀](../maestro-overview.md).

您可以在Adobe Maestro中編輯記錄資訊。 您必須先建立記錄型別，才能開始建立和編輯記錄。
如需詳細資訊，請參閱 [建立記錄型別](../architecture/create-record-types.md).

&lt;! — 在此提及，詳細資訊檢視中的欄位與表格檢視中的欄位相同 — 本文從「管理記錄」檢視連結，其中一個參考此資訊 — >

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
   <td role="rowheader"><p>Adobe Workfront授權</p></td>
   <td>
   <p>任何</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>存取層級設定</p></td>
   <td> <p>Maestro沒有存取控制 </p>  
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

## 編輯記錄的相關考量事項

* 您可以編輯您或其他使用者建立的記錄。 <!--will change with access levels-->
* 您無法編輯從其他記錄連結的欄位或包含計算的欄位。
* 如果顯示的記錄連結到其他記錄，則您正在編輯的記錄的新資訊會反映在連結的記錄上。
* 您無法大量編輯記錄。 <!--this will probably change-->
* URL只有以下列專案開頭時，才會被識別為單行文字欄位型別中的連結： http://、https://、ftp://或www。.
* 編輯段落型別欄位時，您可以使用下列RTF格式選項：

   * 粗體
   * 斜體
   * 底線
   * 新增連結
   * 新增專案符號清單
   * 新增編號清單

## 編輯記錄

您可以從下列區域編輯記錄：

* [從記錄的詳細資訊頁面](#edit-a-record-from-the-records-details-page)
* [從記錄型別的表格檢視](#edit-a-record-from-the-record-type-table-view)

### 從記錄的「詳細資訊」頁面編輯記錄

{{step1-to-maestro}}

您上次存取的工作區會開啟。

1. （可選）按一下工作區名稱右側的向下箭頭，以選取您要更新其記錄的工作區。
1. 執行下列其中一項：

   * 在「表格」檢視中，按一下記錄名稱。
   * 在「表格」檢視中，暫留在記錄名稱上，然後按一下 **更多** 功能表 ![](assets/more-menu.png)，然後按一下 **檢視**

     ![](assets/contextual-menu-for-record-row.png)
   * 在「時間軸」檢視中，按一下記錄列。

   記錄 **詳細資料** 頁面隨即開啟。

1. 按一下 **更多** 功能表 ![](assets/more-menu.png) 在記錄名稱的右側，然後按一下 **編輯**

   或

   按一下「詳細資訊」頁面上的任何可編輯欄位以編輯資訊。

   ![](assets/more-menu-options-from-record-details-page.png) <!--ensure the options have not changed or been renamed-->

1. 按一下 **儲存變更**. <!--logged a bug for this - this needs to be "Save"-->

### 從記錄型別的表格檢視中編輯記錄

{#step1-to-maestro}

您上次存取的工作區會開啟。

1. （可選）按一下工作區名稱右側的向下箭頭，以選取您要更新其記錄的工作區。
1. 按一下記錄型別卡。

   記錄型別頁面隨即開啟。
1. （視條件而定）從 **檢視** 在表格右上角的下拉式功能表中，選取 **表格** 檢視。 這應為預設檢視，除非您上次存取時間軸檢視時已檢視該記錄型別。

   與所選記錄型別相關聯的記錄會顯示在表格檢視中。
1. 在記錄列內按一下，開始編輯有關內嵌記錄的資訊。

   ![](assets/edit-record-paragraph-field-with-formatting-table-view.png)
1. 按下 **輸入** 使用鍵盤或按一下資料列外部以儲存變更。 變更會自動儲存。 已儲存的指標會短暫顯示在表格檢視的右上角，顯示變更已儲存。

   >[!NOTE]
   >
   >  您無法編輯下列欄位的資訊，因為這些欄位是唯讀欄位，且Workfront會自動更新它們：
   >  
   >  * 透過連線記錄型別建立的連結欄位。 如需詳細資訊，請參閱 [連線記錄型別](../architecture/connect-record-types.md).
   >  * 下列型別的欄位：建立者、建立日期、上次修改者、上次修改日期


1. （可選）複製欄位的一或多個現有值，然後貼到另一筆記錄中相同型別的欄位中，然後按一下 **輸入** 以儲存變更。

   >[!NOTE]
   >
   >請考量下列事項：
   >
   >* 您無法從其他來源複製資訊，除了與貼上資訊的欄位型別相同的Maestro欄位之外。
   >
   >* 您無法在記錄的詳細資訊區域中複製和貼上欄位值。 只有在記錄型別的表格檢視中才支援此功能。
   >* 您無法複製和貼上下列欄位型別的欄位值：
   >
   >
   >    * 透過連線記錄型別建立的連結欄位。 您可以複製並貼上連結的記錄欄位。 如需詳細資訊，請參閱 [連線記錄型別](../architecture/connect-record-types.md).
   >    * 下列型別的欄位：建立者、建立日期、上次修改者、上次修改日期

1. （可選）使用下列鍵盤快速鍵來復原或重做編輯或複製和貼上記錄資訊：

   * **還原**： CTRL/CMD + Z
   * **取消復原**：CTRL/CMD + Shift + Z