---
title: 新增縮圖至記錄
description: 您可以在「Adobe大師」中編輯記錄資訊，並將每個記錄與個別縮圖建立關聯，以便輕鬆識別。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: 4016ba2c1b94ba84037612bdc9c1136267513fd5
workflow-type: tm+mt
source-wordcount: '539'
ht-degree: 0%

---

<!--update the metadata with real information-->

# 新增縮圖至記錄

{{maestro-important-intro}}

您可以在Adobe Maestro中將記錄與唯一縮圖建立關聯，以便輕鬆識別。

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
   <td> <p>貢獻或更高的工作區許可權 </p>  
   <p>系統管理員擁有所有工作區的許可權，包括他們未建立的工作區</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>版面配置範本</p></td>
   <td>  <p>必須為所有使用者(包括Workfront管理員)指派一個版面配置範本，該範本包含主功能表中的Maestro區域。 </p> <p>如需詳細資訊，請參閱 <a href="/help/quicksilver/maestro/access/access-overview.md">存取權總覽</a>. </p>  
</td>
  </tr>

</tbody>
</table>

## 有關記錄縮圖的考量事項

若要在視覺上區分表格檢視中的記錄，您可以將唯一的縮圖影像與每個記錄建立關聯。

請考量下列事項：

* 您只能將影像檔案新增為縮圖。
  <!--above: when you know exactly what type of files are allowed, add the exact extensions above-->
* 您可以在表格檢視中將縮圖影像新增至個別記錄。
* 縮圖屬於記錄資訊，且會顯示在記錄顯示的檢視中。 例如，縮圖會與記錄資訊一起顯示在下列區域中：

   * 表格檢視中記錄的主要欄位
   * 時間軸檢視中的記錄列。
* 您無法從記錄的「詳細資訊」頁面或時間軸檢視中新增記錄縮圖。
* 縮圖不會顯示在記錄的詳細資訊頁面中。

## 新增縮圖至記錄

{{step1-to-maestro}}

1. 選取您要新增縮圖之記錄的工作區，然後按一下記錄型別卡。

   這會開啟記錄型別頁面。
1. 從中選擇表格檢視 **檢視** 下拉式功能表。 您所選取型別的所有記錄都會顯示在表格中。
1. 暫留在主要欄位資訊上，按一下 **更多** 功能表 ![](assets/more-menu.png)，然後按一下 **縮圖**.

   ![](assets/record-more-menu-expanded.png)

   >[!TIP]
   >
   >   主要欄位是顯示在表格檢視第一欄中的欄位。 主要欄位一律凍結，不能隱藏或重新定位。

   此 **錄製縮圖** 方塊開啟。

   ![](assets/record-thumbnail-box-for-upload.png)

   <!--update screen shot with correct casing-->

1. 在 **上傳** 標籤，拖放檔案以新增為縮圖，或按一下 **選取以上傳**，然後瀏覽以新增影像檔案。 檔案必須儲存在電腦上。
1. （選用）使用大小調整工具來裁切影像和調整影像大小。
1. 按一下 **使用影像** 將影像新增為縮圖。
如此即會關閉 **錄製縮圖** 方塊。
1. （視條件而定）如果您至少擁有表格檢視的「貢獻」許可權，請按一下 **欄位** 表格檢視的右上角。
1. 選取 **縮圖** 切換即可顯示縮圖。 預設會取消選取此選項。

   ![](assets/thumbnail-toggle-in-fields-menu-deselected.png)

   縮圖會顯示在主要欄位值的左側。
1. （選擇性和條件性）如果您沒有Contribute或更高的檢視許可權，請從 **檢視** 下拉式功能表，或建立檢視。
1. （可選）若要移除縮圖，請將游標移至主要欄位上，然後按一下 **更多** 功能表 ![](assets/more-menu.png)> **縮圖** > **移除** 圖示 ![](assets/remove-image-icon.png)，然後按一下 **儲存變更**.
