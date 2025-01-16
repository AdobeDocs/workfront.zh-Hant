---
title: 管理記錄頁面配置
description: 您可以在Adobe Workfront Planning中編輯記錄預覽和頁面的版面。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: c044b4df-f61d-48e0-be9b-e9fa151b092b
source-git-commit: ba17bd824717f61e72fb9a73c8b90fbe755e20d8
workflow-type: tm+mt
source-wordcount: '1624'
ht-degree: 0%

---


# 管理記錄頁面配置

<!--<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

您可以在Adobe Workfront Planning中編輯記錄預覽和頁面的版面。

記錄預覽是顯示在記錄型別檢視中的記錄頁面的較小檢視。

當您變更記錄預覽和頁面的版面時，變更會影響相同型別的所有記錄的預覽方塊和詳細資訊頁面。

本文說明如何變更記錄預覽方塊或記錄頁面的版面配置和外觀。 如需有關編輯記錄的資訊，請參閱[編輯記錄](/help/quicksilver/planning/records/edit-records.md)。

您必須先建立記錄型別和記錄，才能開始編輯記錄頁面。

如需詳細資訊，請參閱下列文章：

* [建立記錄型別](/help/quicksilver/planning/architecture/create-record-types.md)

* [建立記錄](/help/quicksilver/planning/records/create-records.md)

## 存取需求

+++ 展開以檢視Workfront Planning的存取需求。

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
   <ul><li><p> Adobe Workfront</p></li>
   <li><p> Adobe Workfront規劃<p></li></ul></td>
  </tr>  
 <tr>
   <td role="rowheader"><p>Adobe Workfront計畫*</p></td>
   <td>
<p>下列任一Workfront計畫：</p>
<ul><li>選取</li>
<li>Prime</li>
<li>Ultimate</li></ul>
<p>舊版Workfront計畫不提供Workfront計畫</p>
   </td>

<tr>
   <td role="rowheader"><p>Adobe Workfront規劃套件*</p></td>
   <td>
<p>任何</p>
<p>如需每個Workfront計畫包含內容的詳細資訊，請聯絡您的Workfront客戶經理。 </p>
   </td>

<tr>
   <td role="rowheader"><p>Adobe Workfront平台</p></td>
   <td>
<p>貴組織的Workfront例項必須加入Adobe統一體驗，才能存取Workfront規劃的所有功能。</p>
<p>如需詳細資訊，請參閱<a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Workfront的Adobe統一體驗</a>。 </p>
   </td>

</tr>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront授權*</p></td>
   <td>
   <p>標準</p>
   <p>Workfront計畫不適用於舊版Workfront授權</p>
  </td>
  </tr>
  <tr>
   <td role="rowheader"><p>存取層級設定</p></td>
   <td> <p>Adobe Workfront Planning沒有存取層級控制</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>物件許可權</p></td>
   <td>
   <p>管理工作區</a>的許可權 </p>  
   <p>系統管理員擁有所有工作區的許可權，包括他們未建立的工作區</p> 
  </td>
  </tr>
<tr>
   <td role="rowheader"><p>版面配置範本</p></td>
   <td> <p>必須為所有使用者(包括Workfront管理員)指派一個版面配置範本，該範本包含主功能表中的「規劃」區域，以及專案、投資組合和方案的「規劃」區域。 </p> 如需詳細資訊，請參閱<a href="/help/quicksilver/planning/access/access-overview.md">Adobe計畫存取總覽</a>。 </p>  </p>  
</td>
  </tr>
 </tbody>
</table>

*如需Workfront存取需求的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 編輯記錄頁面的考量事項

* 依預設，記錄的詳細資訊和預覽頁面會顯示與記錄關聯的所有欄位。

* 您無法在預覽或詳細資訊頁面中為記錄新增欄位。 您必須在表格檢視中新增欄位，才能在預覽和詳細資訊頁面中顯示它們。

* 您可以將區段新增到記錄預覽或詳細資訊頁面，以根據通用條件組織資訊並使其更容易找到。

* 下列變更會影響相同型別的所有記錄，而且存取這些記錄的所有使用者都可以看到這些變更：

   * 重新排列欄位
   * 新增或移除截面

* 顯示在記錄預覽中所做的變更會立即顯示在記錄詳細資訊頁面中。 在記錄頁面中所做的變更也會顯示在記錄預覽方塊中。

* 將封面影像或縮圖新增至記錄，不屬於記錄預覽或頁面的整體配置。 您可以新增唯一的封面影像或縮圖到每筆記錄。 如需詳細資訊，請參閱[新增封面影像至記錄](/help/quicksilver/planning/records/add-a-cover-image-to-a-record.md)和[新增縮圖至記錄](/help/quicksilver/planning/records/add-thumbnails-to-records.md)。

## 新增區段到記錄預覽或頁面

將區段新增至記錄頁面時，請考量下列事項：

* 一個頁面上可以擁有的區段數沒有限制。
* 不能有空白區段。 區段中必須至少有一個欄位。
* 您可以將欄位從一個區段拖放至另一個區段。 如需詳細資訊，請參閱本文中[重新排列記錄預覽或詳細資訊頁面](#rearrange-fields-in-the-record-preview-or-details-page)中的欄位。
* 當您從區段移除所有欄位時，該區段會自動刪除且無法復原。

若要將區段新增至記錄預覽或頁面：

{{step1-to-planning}}

1. 按一下工作區的卡片。

   工作區隨即開啟，且記錄型別會顯示為卡片。

1. 按一下記錄型別卡。

   記錄型別頁面隨即開啟。

1. 從任何型別的檢視中，按一下記錄的名稱

   或

   從表格檢視中，按一下第一欄中的&#x200B;**開啟詳細資料**&#x200B;圖示![](assets/open-details-icon-in-table-name-field.png)。

   記錄的預覽會在檢視中開啟。

   ![](assets/details-box.png)

1. （選擇性）按一下記錄預覽右上角的&#x200B;**在新索引標籤中開啟**&#x200B;圖示![](assets/open-details-in-a-new-tab-icon.png)，以在新索引標籤中開啟記錄的頁面。

   記錄頁面隨即開啟。 依預設，詳細資訊標籤會開啟。

   ![](assets/details-page.png)

1. 在記錄預覽或頁面的&#x200B;**詳細資料**&#x200B;索引標籤中，將滑鼠移至欄位左側的空白區域，然後按一下&#x200B;**新增區段**&#x200B;圖示![](assets/add-section-icon.png)以新增區段。
1. 按一下區段名稱內部，將&#x200B;**未命名的區段**&#x200B;取代為名稱，然後按一下[輸入]。 在區段下顯示的欄位會自動成為新區段的一部分。
1. 開始將欄位拖放至新區段，如本文中記錄預覽或詳細資訊頁面](#rearrange-fields-in-the-record-preview-or-details-page)中的區段[重新排列欄位中所述。

1. （選擇性）將滑鼠停留在區段名稱上，然後按一下&#x200B;**更多**&#x200B;功能表![](assets/more-menu.png)。

   ![](assets/more-menu-options-for-section-on-record-page.png)
1. （可選）執行下列任一項作業來編輯區段：

   * 按一下&#x200B;**重新命名**&#x200B;以重新命名區段

     >[!TIP]
     >
     > 您可以按一下名稱，以內嵌方式重新命名截面。

   * 按一下&#x200B;**向上移動**，將區段向上移動一個位置

     或

     按一下&#x200B;**下移**將區段下移一個位置。
區段中的所有欄位會隨著區段移動。

   * 按一下&#x200B;**刪除**&#x200B;以刪除區段。 該區段已刪除且無法復原。 所有存取此型別記錄的使用者將不再檢視已刪除的區段。

1. 按一下區段名稱左側的向下箭頭可將其摺疊，按一下向右箭頭可將其展開。
依預設，所有截面都會展開。

1. （選擇性）按一下區段名稱左側的&#x200B;**抓取**&#x200B;圖示![](assets/grab-icon.png)，然後將其拖放到所需的位置。

   對於檢視記錄的所有使用者，區段的新位置會在相同型別的所有記錄預覽和頁面中更新。

   對區段和欄位順序的所有變更會自動儲存。

1. （選擇性）按一下&#x200B;**匯出**&#x200B;功能表![](assets/export-icon-in-record-details-page.png)，將[詳細資料]索引標籤匯出至Word或PDF檔案。 如需詳細資訊，請參閱[匯出記錄的詳細資料](/help/quicksilver/planning/records/export-the-record-page.md)。

1. （選擇性）按一下&#x200B;**詳細資料**&#x200B;標籤旁的&#x200B;**連線**&#x200B;標籤。 您必須先按一下&#x200B;**更多**，再按一下&#x200B;**連線**&#x200B;索引標籤。

   所有與所選記錄連線的記錄或物件都會顯示在記錄型別或其所屬應用程式的名稱下。

   ![](assets/connections-tab-on-record-in-workfront-planning.png)

1. （選擇性）選取[連線]索引標籤右上角的&#x200B;**顯示所有記錄**&#x200B;設定。 所有連線的記錄型別都會顯示，包括尚未有任何連線記錄的型別。 依預設，會取消選取切換並隱藏沒有連線記錄的記錄型別。

1. （選擇性）按一下&#x200B;**連線**，將更多記錄新增至連線的記錄型別。 如需詳細資訊，請參閱[連線記錄](/help/quicksilver/planning/records/connect-records.md)。

1. （選擇性）將游標停留在記錄卡上，然後按一下中斷連線記錄圖示&#x200B;**-**，然後按一下&#x200B;**中斷連線**。 <!--this is copied to the Manage the Planning page in Workfront article; update in both articles-->
會發生下列情況：
   * 記錄不再連線至Workfront物件。
   * Workfront物件也會從Workfront Planning的記錄連線欄位中移除。
   * 連線至Planning記錄的Workfront查閱欄位值也會一併刪除。

## 重新排列記錄詳細資訊索引標籤中的欄位

{{step1-to-planning}}

1. 按一下工作區的卡片。

   工作區隨即開啟，且記錄型別會顯示為卡片。

1. 按一下記錄型別卡。

   記錄型別頁面隨即開啟。

1. 從任何型別的檢視中，按一下記錄的名稱

   或

   從表格檢視中，按一下第一欄中的&#x200B;**開啟詳細資料**&#x200B;圖示![](assets/open-details-icon-in-table-name-field.png)。

   記錄的預覽會在檢視中開啟。

   ![](assets/details-box.png)

1. （選擇性）按一下記錄預覽右上角的&#x200B;**在新索引標籤中開啟**&#x200B;圖示![](assets/open-details-in-a-new-tab-icon.png) <!--check the icon; they are changing it-->，以在新索引標籤中開啟記錄的頁面。

   記錄的&#x200B;**詳細資料**&#x200B;索引標籤預設會開啟。

   ![](assets/details-page.png)

1. 在記錄&#x200B;**詳細資料**&#x200B;索引標籤中，按一下欄位名稱左側的&#x200B;**抓取**&#x200B;圖示![](assets/grab-icon.png)，然後將其拖放到所要的位置。<!--You can drag and drop fields to another section. You must have at least one field in a section.-->

   對於檢視記錄的所有使用者，相同型別的所有記錄預覽和頁面中的欄位新位置都會更新。

   對記錄預覽或頁面儲存的版面配置所做的所有變更都會自動完成。

## 新增連線檢視頁面到記錄的頁面

將「連線」檢視新增至記錄頁面時，請考量下列事項：

* 您可以將連線檢視頁面新增到記錄的頁面。

* 您無法將[連線]檢視頁面新增到記錄的預覽區域。

* 連線檢視頁面會在表格檢視中顯示一個連線記錄頁面。 表格檢視是唯讀的。

* 您可以為每個連線的記錄型別新增一個連線檢視頁面。 <!--edit this when we can remove fields from this page-->

* 將「連線」檢視頁面新增到記錄頁面後，該頁面會從記錄的預覽區域可見。

若要新增「連線」檢視頁面：

1. 從記錄頁面檢視中，按一下記錄名稱以開啟它，然後按一下預覽頁面右上角的&#x200B;**在新索引標籤中開啟**&#x200B;圖示![](assets/open-details-in-a-new-tab-icon.png)。
1. 按一下&#x200B;**新增頁面** > **連線檢視**。

   ![](assets/add-connection-view-page-modal.png)
1. 新增&#x200B;**頁面名稱**，按一下&#x200B;**連線檢視**，然後按一下&#x200B;**建立**。

   新索引標籤將新增到記錄的頁面。
1. 搜尋或按一下清單中連線記錄或物件型別的名稱。
您選取之記錄型別的表格檢視會顯示，而連線的記錄會顯示在表格檢視中。
表格檢視是唯讀的。

   ![](assets/audience-connected-table-view-under-campaign-details-page.png)
1. （可選）按兩下標籤的名稱

   或

   將游標暫留在索引標簽名稱上，然後按一下[其他] **![](assets/more-menu.png)，然後按一下[重新命名]** **以重新命名為新的[連線檢視]索引標籤。**
1. （選擇性）使用工具列中的任何檢視元素來管理表格檢視。 如需詳細資訊，請參閱[管理資料表檢視](/help/quicksilver/planning/views/manage-the-table-view.md)。
1. （選擇性）將游標暫留在索引標簽名稱上，然後按一下&#x200B;**更多** ![](assets/more-menu.png)，然後按一下&#x200B;**刪除**&#x200B;以移除至新的「連線檢視」索引標籤。



<!--
## Add a Brief page to a record's page

You can add a Brief page to the record's preview or pages. 

Brief pages contain the same information as the Details tab, in a read-only format. <!--edit this when we can remove fields from this page-->

<!--
1. From a record's page view, click the name of a record to open its preview or page.
1. Click **Add page** > **Brief**. 
1. Add the **Page name**, then click **Create**. 
-->



