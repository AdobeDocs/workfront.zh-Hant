---
title: 新增縮圖至記錄
description: 您可以在Adobe Workfront Planning中編輯記錄資訊，並將每個記錄與個別縮圖建立關聯，以便輕鬆識別。
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: b22c4955-c3f2-4841-a278-bb40e8890ed9
source-git-commit: e26a3d0e283182e08902c263252c8d067838c23a
workflow-type: tm+mt
source-wordcount: '812'
ht-degree: 0%

---


# 新增縮圖至記錄

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->


{{planning-important-intro}}

您可以在Adobe Workfront Planning中將記錄與唯一縮圖建立關聯，以便輕鬆識別。

您必須先建立記錄型別，才能開始建立和編輯記錄。
如需詳細資訊，請參閱[建立記錄型別](/help/quicksilver/planning/architecture/create-record-types.md)。

## 存取需求

<!--************double-check permissions here - asking Isk and Lilit what permissions users need for adding thumbnails-->

+++ 展開以檢視本文中功能的存取需求。 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront套件</p></td> 
   <td> 
<p>任何Workfront和任何Planning套件</p> <p>任何工作流程與任何Planning套件</p>
<p>如需每個Workfront Planning套件所含內容的詳細資訊，請聯絡您的Workfront客戶代表。 </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront授權</p></td> 
   <td><p>標準</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>物件許可權</p></td> 
   <td>   <p>貢獻或更高的許可權到工作區和記錄型別  </p>  
   <p>系統管理員擁有所有工作區的許可權，包括他們未建立的工作區</p> </td> 
  </tr>   
</tbody> 
</table>

如需Workfront存取需求的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++   

<!--Old:

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Products</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront plan*</p></td> 
   <td> 
<p>Any of the following Workfront plans:</p> 
<ul><li>Select</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning is not available for legacy Workfront plans</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront Planning package*</p></td> 
   <td> 
<p>Any </p> 
<p>For more information about what is included in each Workfront Planning plan, contact your Workfront account manager. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront platform</p></td> 
   <td> 
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access Workfront Planning.</p> 
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license*</p></td> 
   <td><p> Standard </p>
   <p>Workfront Planning is not available for legacy Workfront licenses</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Access level configuration</p></td> 
   <td> <p>There are no access level controls for Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>   <p>Contribute or higher permissions to a workspace and record type  </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p> </td> 
  </tr> 
</tbody> 
</table> -->


## 有關記錄縮圖的考量事項

若要在視覺上區分表格檢視中的記錄，您可以將唯一的縮圖影像與每個記錄建立關聯。

請考量下列事項：

* 縮圖只適用於一筆記錄，不會套用至相同型別的所有記錄。
* 您只能將影像檔案新增為縮圖。
  <!--above: when you know exactly what type of files are allowed, add the exact extensions above-->
* 您可以將縮圖影像新增至表格檢視中的個別記錄，或是從記錄的頁面或預覽方塊新增縮圖影像。
* 每次建立記錄時，Workfront都會自動上傳縮圖影像。 您稍後可以修改此影像。
* 縮圖屬於記錄資訊，且會顯示在記錄顯示的區域中。 例如，縮圖會與記錄資訊一起顯示在下列區域中：

   * 表格檢視中記錄的主要欄位
   * 時間軸檢視中的記錄列。
   * 記錄的詳細資料預覽和頁面。

## 新增縮圖至記錄

您可以透過下列方式新增縮圖：

* [從表格檢視新增縮圖至記錄](#add-a-thumbnail-to-a-record-from-the-table-view)
* [從詳細資訊頁面新增縮圖至記錄](#add-a-thumbnail-to-a-record-from-the-details-page)

### 從表格檢視新增縮圖至記錄

{{step1-to-planning}}

1. 按一下您要新增縮圖之記錄的工作區，然後按一下記錄型別卡。

   這會開啟記錄型別頁面。
1. 從&#x200B;**檢視**&#x200B;下拉式功能表中選取表格檢視。 您所選取型別的所有記錄都會顯示在表格中。
1. 暫留在主要欄位資訊上，按一下&#x200B;**更多**&#x200B;功能表![更多](assets/more-menu.png)，然後按一下&#x200B;**縮圖**。

   ![其他錄製功能表已展開](assets/record-more-menu-expanded.png)

   >[!TIP]
   >
   >   主要欄位是顯示在表格檢視第一欄中的欄位。 主要欄位一律凍結，不能隱藏或重新定位。 主要欄位為公式欄位時，「更多」選單中的「縮圖」選項無法使用。

   **上傳**&#x200B;索引標籤預設會在&#x200B;**錄製縮圖**&#x200B;方塊中開啟。

   如需有關上傳縮圖的詳細資訊，請參閱本文章中[從詳細資訊頁面](#add-a-thumbnail-to-a-record-from-the-details-page)新增縮圖至記錄一節，從步驟6開始。<!--see if this is accurate-->

<!--
   ![Record thumbnail box for upload](assets/record-thumbnail-box-for-upload.png) 

  *****update screen shot with correct casing****

1. Drag and drop a file to add as a thumbnail
   
   Or
   
   Click **Browse images**, then browse for an image file to add. The file must be saved on your computer. 
1. (Optional) After the image uploads in the **Record thumbnail** box, use the sizing tool to crop and resize the image.
1. (Optional) Click the **Upload new image** icon ![Upload new image icon](assets/upload-new-image-icon.png) to upload another image. 
1. (Optional) To remove a thumbnail before it is saved, click  **Remove uploaded image** icon ![Remove image icon](assets/remove-image-icon.png) to the right of the image. 
1. (Optional) Click the **Gallery** tab, then click an image. The gallery of images cannot be modified.

   ![Record thumbnail box for gallery](assets/record-thumbnail-box-for-gallery.png)
1. Click **Use image** to add the image as a thumbnail. 
   This closes the **Record thumbnail** box.
   The thumbnail displays in areas of Workfront Planning where the record displays. 

   >[!TIP]
   >
   >   You must enable the Thumbnail field in the table view to display thumbnails in this view. It is disabled by default.

1. (Optional) To remove the thumbnail after it is saved, hover over the primary field and click the **More** menu ![More menu](assets/more-menu.png)> **Thumbnail** > the **Remove** icon ![Remove image icon](assets/remove-image-icon.png), then click **Save changes**. -->

### 從詳細資訊頁面新增縮圖至記錄

{{step1-to-planning}}

1. 按一下您要新增縮圖之記錄的工作區，然後按一下記錄型別卡。

   這會開啟記錄型別頁面。
1. 從任何檢視中，按一下記錄以開啟它。

   詳細資訊預覽方塊隨即顯示。
1. （選擇性）按一下右上角的&#x200B;**在新標籤中開啟**&#x200B;圖示![在新標籤圖示中開啟詳細資料](assets/open-details-in-a-new-tab-icon.png)。

   記錄的詳細資訊頁面隨即開啟。

1. （視條件而定）在記錄預覽或詳細資訊頁面中，將滑鼠指標暫留在詳細資訊頁面上的縮圖影像或圖示![記錄縮圖圖示](assets/record-thumbnail-icon-on-details-page.png)上，然後將滑鼠指標暫留在記錄名稱上方的空格上，然後按一下&#x200B;**新增縮圖**&#x200B;或&#x200B;**編輯縮圖**。

   **上傳**&#x200B;索引標籤預設會在&#x200B;**錄製縮圖**&#x200B;方塊中開啟。

   ![錄製上傳的縮圖方塊](assets/record-thumbnail-box-for-upload.png)

1. 拖放檔案以新增為縮圖

   或

   按一下&#x200B;**瀏覽影像**，然後瀏覽以新增影像檔案。 檔案必須儲存在電腦上。

1. （選擇性）在&#x200B;**錄製縮圖**&#x200B;方塊中上傳影像後，使用大小調整工具來裁切影像並調整影像大小。
1. （選擇性）按一下&#x200B;**上傳新影像**&#x200B;圖示![上傳新影像圖示](assets/upload-new-image-icon.png)以上傳另一個影像。
1. （選擇性）按一下&#x200B;**相簿**&#x200B;標籤，然後按一下影像。 無法修改影像庫。

   ![錄製相簿的縮圖方塊](assets/record-thumbnail-box-for-gallery.png)

1. （選擇性）若要在儲存縮圖之前移除縮圖，請按一下影像右側的&#x200B;**移除**&#x200B;圖示![移除影像圖示](assets/remove-image-icon.png)。

1. 按一下&#x200B;**使用影像**將影像新增為縮圖。
這會關閉**錄製縮圖**方塊。
縮圖會顯示在Workfront Planning中記錄顯示的區域中。

   >[!TIP]
   >
   >   您必須啟用表格檢視中的縮圖欄位，才能在此檢視中顯示縮圖。 預設為停用。

1. （選擇性）若要在儲存縮圖後移除縮圖，請按一下任何檢視中的記錄以開啟詳細資料頁面，然後將滑鼠游標停留在縮圖影像上，然後按一下&#x200B;**更多**&#x200B;功能表![更多功能表圖示](assets/more-menu.png)> **移除**&#x200B;圖示![移除圖示](assets/remove-image-icon.png)。 縮圖影像即會移除。


<!--
### Generate a thumbnail for a record

{{step1-to-planning}}

1. Click the workspace for whose records you want to add thumbnails, then click the record type card. 

   This opens the record type page. 
1. Select a table view from the **View** drop-down menu. All records of the type you selected display in a table. 
1. Hover over the primary field information, click the **More** menu ![More menu](assets/more-menu.png), then click **Thumbnail**. 

   ![Record more menu expanded](assets/record-more-menu-expanded.png)

      >[!TIP]
      >
      >   The primary field is the field that displays in the first column of a table view. The primary field is always frozen and cannot be hidden or relocated. 

   The **Record thumbnail** box opens.

(*************** update the screenshot below*************)
   ![Record thumbnail box for upload](assets/record-thumbnail-box-for-upload.png) 

1. Click the **Generate** tab, and type a prompt describing the type of image you want to add in the space provided. 
1. Click **Generate**. 

   A set of four suggested images displays. 

1. Click an image to select it, then click **Use image**. 

   The Record thumbnail box closes and the thumbnail is attached to the record. All users who can view the records can now see the selected thumbnail. 
1. (Optional) Click the **More** menu ![More menu](assets/more-menu.png) to the right of the record name in the table view, then click **Thumbnail**. 

   The generated image opens in the **Upload** tab where you can modify or remove it, as described in the section [Upload a thumbnail to a record](#upload-a-thumbnail-to-a-record) in this article. 
-->
