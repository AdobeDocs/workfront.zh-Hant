---
title: 新增封面影像至記錄
description: 編輯記錄時，您可以在Adobe Workfront Planning中將封面影像新增至記錄頁面，以個人化記錄。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 93c6bc15-d945-4cfc-8e87-f5b4e6fac2f4
source-git-commit: 2f8a5b2d2183090029966a13c7af37f20eb44fd0
workflow-type: tm+mt
source-wordcount: '563'
ht-degree: 0%

---


<!--update the metadata with real information-->

# 新增封面影像至記錄

{{maestro-important-intro}}

編輯記錄時，您可以在Adobe Workfront Planning中將封面影像新增至記錄頁面，以個人化記錄。

如需有關編輯記錄的資訊，請參閱 [編輯記錄](/help/quicksilver/maestro/records/edit-records.md).

您必須先建立記錄型別，才能開始建立和編輯記錄。

如需詳細資訊，請參閱 [建立記錄型別](../architecture/create-record-types.md).

## 存取需求

<!--************double-check permissions here - asking Isk and Lilit what permissions users need for adding thumbnails-->

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
<p>貴組織必須註冊Adobe Workfront Planning測試版計畫。 請聯絡您的客戶代表以查詢此新產品/服務。 </p>
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
   <td> <p>Workfront Planning沒有存取控制 </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>權限</p></td>
   <td> <p>貢獻或更高的工作區許可權 </p>  
   <p>系統管理員擁有所有工作區的許可權，包括他們未建立的工作區</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>版面配置範本</p></td>
   <td>  <p>必須為所有使用者(包括Workfront管理員)指派一個版面配置範本，該範本包含主功能表中的Planning區域。 </p> <p>如需詳細資訊，請參閱 <a href="/help/quicksilver/maestro/access/access-overview.md">存取權總覽</a>. </p>  
</td>
  </tr>

</tbody>
</table>

## 關於紀錄頁封面影像的考量事項

您可以新增封面影像以個人化記錄頁面。

請考量下列事項：

* 封面影像隻適用於一筆記錄，不適用於相同型別的所有記錄。
* 您只能將影像檔案新增為封面影像。
  <!--above: when you know exactly what type of files are allowed, add the exact extensions above-->
* 您可以從任何檢視的記錄方塊或記錄頁面，將封面影像新增至個別記錄。
* 您無法從任何記錄檢視中內嵌新增封面影像。

## 新增封面影像至記錄

您可以在記錄方塊或頁面頂端新增封面影像，以個人化記錄。

{{step1-to-maestro}}

您上次存取的工作區會開啟。

1. （可選）按一下工作區名稱右側的向下箭頭，以選取您要更新其記錄的工作區。

1. 按一下記錄型別卡。

   記錄型別頁面隨即開啟。

1. 從任何型別的檢視中，按一下記錄的名稱

   或

   從表格檢視中，按一下 **開啟詳細資料** 圖示 ![](assets/open-details-icon-in-table-name-field.png) 記錄名稱的左側。

   記錄的方塊會在檢視中開啟。

   ![](assets/details-box.png)

   >[!TIP]
   >
   >您可以檢視 **開啟詳細資料** 圖示至表格檢視中記錄之「名稱」欄位左邊的圖示（僅當「名稱」欄位為主要欄位時）。

1. （可選）按一下 **在新標籤中開啟** 圖示 ![](assets/open-details-in-a-new-tab-icon.png) <!--check the icon; they are changing it--> 在記錄方塊的右上角，以在新索引標籤中開啟記錄頁面。

   記錄頁面隨即開啟。

   ![](assets/details-page.png)

1. 在記錄方塊或頁面中，按一下 **新增封面**. <!--check the casing here; I logged a bug for this-->
此 **紀錄封面** 方塊開啟。

1. 按一下 **選取以上傳** 並瀏覽電腦上的圖片，以選取、新增圖片，然後按一下 **使用影像**.

   影像會上傳至記錄方塊或頁面頂端，且變更會自動儲存。

   ![](assets/record-page-with-cover-image.png)

1. （選用）將游標停留在影像上，然後按一下 **更多** 功能表 ![](assets/more-menu.png) 在封面影像的右下角，執行下列任一項作業：

   * 按一下 **上傳** 如果要取代封面影像，並重複步驟6以上傳和儲存新影像。
   * 按一下 **重新定位**，並使用 **重新定位** 工具 ![](assets/reposition-tool-icon.png) 將封面影像置中，然後按一下 **儲存** 完成時。
   * 按一下 **移除** 以移除封面影像。

   Workfront會自動儲存您的變更。