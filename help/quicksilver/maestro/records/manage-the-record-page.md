---
title: 管理記錄頁面
description: 您可以在Adobe Workfront Planning中編輯管理記錄方塊和頁面的配置。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: 02d20209b8bf53c84308707a89a5abf399494b64
workflow-type: tm+mt
source-wordcount: '800'
ht-degree: 0%

---

<!--update the metadata with real information when making this avilable in TOC and in the left nav-->

# 管理記錄頁面

{{maestro-important-intro}}

您可以在Adobe Workfront Planning中編輯管理記錄方塊和頁面的配置。 您可以在記錄檢視中顯示記錄方塊。

記錄方塊是顯示在記錄型別檢視中的記錄頁面的較小檢視。

當您變更記錄方塊和頁面的版面配置時，方塊和頁面會針對相同型別的所有記錄而變更。

您必須先建立記錄型別和記錄，才能開始編輯記錄頁面。

如需詳細資訊，請參閱下列文章：

* [建立記錄型別](../architecture/create-record-types.md)

* [建立記錄](/help/quicksilver/maestro/records/create-records.md)

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
   <td role="rowheader"><p>Adobe Workfront授權*</p></td>
   <td>
   <p>新增：淺色或更高</p>
   或
   <p>目前：工作或以上</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>存取層級設定</p></td>
   <td> <p>Adobe Workfront Planning沒有存取控制</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>權限</p></td>
   <td> <p>管理工作區或更高的許可權</a> </p>  
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

*如需詳細資訊，請參閱 [Workfront檔案中的存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## 編輯記錄頁面的考量事項

* 重新排列記錄方塊或頁面中的欄位會重新排列該型別所有記錄的欄位以及存取這些記錄的所有使用者。
* 新增封面影像到記錄不是記錄方塊或頁面的整體配置的一部分。 您可以將唯一的封面影像新增到每張記錄中。

## 重新排列記錄方塊或頁面中的欄位

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

1. 在記錄方塊或頁面中，按一下抓取圖示 ![](assets/grab-icon.png) 至欄位名稱的左側，然後將其拖放到所需的位置。

   對於檢視記錄的所有使用者，相同型別的所有記錄之方塊和頁面中的欄位新位置都會更新。

   記錄方塊或頁面配置的所有變更都會自動儲存。


## 新增封面影像至記錄方塊或頁面

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

   所有變更會立即生效。

