---
title: 管理記錄頁面配置
description: 您可以在Adobe Workfront Planning中編輯記錄預覽和頁面的版面。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: c044b4df-f61d-48e0-be9b-e9fa151b092b
source-git-commit: 869a1f9e4fd7e3b65591050530b96d6dae9e230c
workflow-type: tm+mt
source-wordcount: '1066'
ht-degree: 0%

---

<!--update the metadata with real information when making this avilable in TOC and in the left nav-->

# 管理記錄頁面配置

{{planning-important-intro}}

您可以在Adobe Workfront Planning中編輯記錄預覽和頁面的版面。

記錄預覽是顯示在記錄型別檢視中的記錄頁面的較小檢視。

當您變更記錄預覽和頁面的版面時，變更會影響相同型別的所有記錄的預覽方塊和詳細資訊頁面。

本文說明如何變更記錄預覽方塊或記錄頁面的版面配置和外觀。 如需有關編輯記錄的資訊，請參閱 [編輯記錄](/help/quicksilver/planning/records/edit-records.md).

您必須先建立記錄型別和記錄，才能開始編輯記錄頁面。

如需詳細資訊，請參閱下列文章：

* [建立記錄型別](/help/quicksilver/planning/architecture/create-record-types.md)

* [建立記錄](/help/quicksilver/planning/records/create-records.md)

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
   <td> <p>您的Workfront或群組管理員必須在版面配置範本中新增Planning區域。 如需詳細資訊，請參閱 <a href="/help/quicksilver/planning/access/access-overview.md">存取權總覽</a>. </p>  
</td>
  </tr>

</tbody>
</table>

*如需詳細資訊，請參閱 [Workfront檔案中的存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## 編輯記錄頁面的考量事項

* 依預設，記錄的詳細資訊和預覽頁面會顯示與記錄關聯的所有欄位。

* 您無法在預覽或詳細資訊頁面中為記錄新增欄位。 您必須在表格檢視中新增欄位，才能在預覽和詳細資訊頁面中顯示它們。

* 您可以將區段新增到記錄預覽或詳細資訊頁面，以根據通用條件組織資訊並使其更容易找到。

* 下列變更會影響相同型別的所有記錄，而且存取這些記錄的所有使用者都可以看到這些變更：

   * 重新排列欄位
   * 新增或移除截面

* 顯示在記錄預覽中所做的變更會立即顯示在記錄詳細資訊頁面中。 在記錄頁面中所做的變更也會顯示在記錄預覽方塊中。

* 將封面影像或縮圖新增至記錄，不屬於記錄預覽或頁面的整體配置。 您可以新增唯一的封面影像或縮圖到每筆記錄。 如需詳細資訊，請參閱 [新增封面影像至記錄](/help/quicksilver/planning/records/add-a-cover-image-to-a-record.md) 和 [新增縮圖至記錄](/help/quicksilver/planning/records/add-thumbnails-to-records.md).

## 新增區段到記錄預覽或頁面

將區段新增至記錄頁面時，請考量下列事項：

* 一個頁面上可以擁有的區段數沒有限制。
* 不能有空白區段。 區段中必須至少有一個欄位。
* 您可以將欄位從一個區段拖放至另一個區段。 如需詳細資訊，請參閱區段 [重新排列記錄預覽或詳細資訊頁面中的欄位](#rearrange-fields-in-the-record-preview-or-details-page) 本文章內容。
* 當您從區段移除所有欄位時，該區段會自動刪除且無法復原。

若要將區段新增至記錄預覽或頁面：

{{step1-to-planning}}

1. 按一下工作區的卡片。

   工作區隨即開啟，且記錄型別會顯示為卡片。

1. 按一下記錄型別卡。

   記錄型別頁面隨即開啟。

1. 從任何型別的檢視中，按一下記錄的名稱

   或

   從表格檢視中，按一下 **開啟詳細資料** 圖示 ![](assets/open-details-icon-in-table-name-field.png) 在第一欄中。

   記錄的預覽會在檢視中開啟。

   ![](assets/details-box.png)

1. （可選）按一下 **在新標籤中開啟** 圖示 ![](assets/open-details-in-a-new-tab-icon.png) 在記錄預覽的右上角，以在新索引標籤中開啟記錄頁面。

   記錄頁面隨即開啟。

   ![](assets/details-page.png)

1. 在記錄預覽或頁面中，暫留在欄位左側的空白區域上，然後按一下 **新增區段** 圖示 ![](assets/add-section-icon.png) 以新增區段。
1. 在區段名稱內按一下並取代 **未命名的區段** 名稱，然後按一下Enter。 在區段下顯示的欄位會自動成為新區段的一部分。
1. 開始將欄位拖放至新區段，如區段所述 [重新排列記錄預覽或詳細資訊頁面中的欄位](#rearrange-fields-in-the-record-preview-or-details-page) 本文章內容。

1. （可選）將游標停留在區段名稱上，然後按一下 **更多** 功能表 ![](assets/more-menu.png).

   ![](assets/more-menu-options-for-section-on-record-page.png)
1. （可選）執行下列任一項作業來編輯區段：

   * 按一下 **重新命名** 重新命名截面

     >[!TIP]
     >
     > 您可以按一下名稱，以內嵌方式重新命名截面。

   * 按一下 **上移** 將區段向上移動一個位置

     或

     按一下 **下移** 將區段下移一個位置。
區段中的所有欄位會隨著區段移動。

   * 按一下 **刪除** 以刪除區段。 該區段已刪除且無法復原。 所有存取此型別記錄的使用者將不再檢視已刪除的區段。

1. 按一下區段名稱左側的向下箭頭可將其摺疊，按一下向右箭頭可將其展開。
依預設，所有截面都會展開。

1. （可選）按一下 **抓取** 圖示 ![](assets/grab-icon.png) 將區段名稱左側，然後將其拖放到所需位置。

   對於檢視記錄的所有使用者，區段的新位置會在相同型別的所有記錄預覽和頁面中更新。

   對區段和欄位順序的所有變更會自動儲存。

## 重新排列記錄預覽或詳細資訊頁面中的欄位

{{step1-to-planning}}

1. 按一下工作區的卡片。

   工作區隨即開啟，且記錄型別會顯示為卡片。

1. 按一下記錄型別卡。

   記錄型別頁面隨即開啟。

1. 從任何型別的檢視中，按一下記錄的名稱

   或

   從表格檢視中，按一下 **開啟詳細資料** 圖示 ![](assets/open-details-icon-in-table-name-field.png) 在第一欄中。

   記錄的預覽會在檢視中開啟。

   ![](assets/details-box.png)

1. （可選）按一下 **在新標籤中開啟** 圖示 ![](assets/open-details-in-a-new-tab-icon.png) <!--check the icon; they are changing it--> 在記錄預覽的右上角，以在新索引標籤中開啟記錄頁面。

   記錄頁面隨即開啟。

   ![](assets/details-page.png)

1. 在記錄預覽或頁面中，按一下 **抓取** 圖示 ![](assets/grab-icon.png) 至欄位名稱的左側，然後將其拖放到所需的位置。 <!--You can drag and drop fields to another section. You must have at least one field in a section.-->

   對於檢視記錄的所有使用者，相同型別的所有記錄預覽和頁面中的欄位新位置都會更新。

   對記錄預覽或頁面儲存的版面配置所做的所有變更都會自動完成。

