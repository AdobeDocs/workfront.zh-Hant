---
title: 管理記錄頁面配置
description: 您可以在Adobe Workfront Planning中編輯記錄預覽和頁面的版面。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: c044b4df-f61d-48e0-be9b-e9fa151b092b
source-git-commit: 567fa8c960f7db47279d6cde1f5e90dc7f38ae79
workflow-type: tm+mt
source-wordcount: '2133'
ht-degree: 1%

---


# 管理記錄頁面配置

<!--<span class="preview">The information highlighted on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

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

+++ 展開以檢視存取需求。

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
<p>貴組織的Workfront例項必須上線至Adobe Unified Experience，才能存取Workfront Planning。</p>
<p>如需詳細資訊，請參閱<a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">適用於Workfront的Adobe Unified Experience</a>。 </p>
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
   <p>貢獻或更高的許可權至工作區和記錄型別</a> </p>  
   <p>系統管理員擁有所有工作區的許可權，包括他們未建立的工作區</p> 
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

   從表格檢視中，按一下第一欄中的&#x200B;**開啟詳細資料**&#x200B;圖示![在表格名稱欄位中開啟詳細資料圖示](assets/open-details-icon-in-table-name-field.png)。

   記錄的預覽會在檢視中開啟。

   ![詳細資訊方塊](assets/details-box.png)

1. （選擇性）按一下記錄預覽右上角的&#x200B;**在新索引標籤中開啟**&#x200B;圖示![在新索引標籤中開啟詳細資料](assets/open-details-in-a-new-tab-icon.png)，以在新索引標籤中開啟記錄頁面。

   記錄頁面隨即開啟。 依預設，詳細資訊標籤會開啟。

   ![詳細資料頁面](assets/details-page.png)

1. 在記錄預覽或頁面的&#x200B;**詳細資料**&#x200B;索引標籤中，將滑鼠移至欄位左側的空白區域，然後按一下&#x200B;**新增區段**&#x200B;圖示![新增區段圖示](assets/add-section-icon.png)以新增區段。
1. 按一下區段名稱內部，將&#x200B;**未命名的區段**&#x200B;取代為名稱，然後按一下[輸入]。 在區段下顯示的欄位會自動成為新區段的一部分。
1. 開始將欄位拖放至新區段，如本文中記錄預覽或詳細資訊頁面[中的區段](#rearrange-fields-in-the-record-preview-or-details-page)重新排列欄位中所述。

1. （選擇性）將滑鼠停留在區段名稱上，然後按一下&#x200B;**更多**&#x200B;功能表![更多](assets/more-menu.png)。

   記錄頁面![上區段的](assets/more-menu-options-for-section-on-record-page.png)更多功能表選項
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

1. （選擇性）按一下區段名稱左側的&#x200B;**抓取**&#x200B;圖示![抓取圖示](assets/grab-icon.png)，然後將其拖放到所需位置。

   對於檢視記錄的所有使用者，區段的新位置會在相同型別的所有記錄預覽和頁面中更新。

   對區段和欄位順序的所有變更會自動儲存。

1. （選擇性）按一下記錄詳細資料頁面中的&#x200B;**匯出**&#x200B;功能表![匯出圖示](assets/export-icon-in-record-details-page.png)，將[詳細資訊]索引標籤匯出至Word或PDF檔案。 如需詳細資訊，請參閱[匯出記錄的詳細資料](/help/quicksilver/planning/records/export-the-record-page.md)。

1. （選擇性）按一下&#x200B;**詳細資料**&#x200B;標籤旁的&#x200B;**連線**&#x200B;標籤。 您必須先按一下&#x200B;**更多**，再按一下&#x200B;**連線**&#x200B;索引標籤。

   所有與所選記錄連線的記錄或物件都會顯示在記錄型別或其所屬應用程式的名稱下。

   在Workfront Planning中記錄的![連線標籤](assets/connections-tab-on-record-in-workfront-planning.png)

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

   從表格檢視中，按一下第一欄中的&#x200B;**開啟詳細資料**&#x200B;圖示![在表格名稱欄位中開啟詳細資料圖示](assets/open-details-icon-in-table-name-field.png)。

   記錄的預覽會在檢視中開啟。

   ![詳細資訊方塊](assets/details-box.png)

1. （選擇性）按一下記錄預覽右上角的&#x200B;**在新索引標籤中開啟**&#x200B;圖示![在新索引標籤圖示中開啟詳細資訊方塊](assets/open-details-in-a-new-tab-icon.png) <!--check the icon; they are changing it-->，以在新索引標籤中開啟記錄的頁面。

   記錄的&#x200B;**詳細資料**&#x200B;索引標籤預設會開啟。

   ![詳細資料頁面](assets/details-page.png)

1. 在記錄&#x200B;**詳細資料**&#x200B;索引標籤中，按一下欄位名稱左側的&#x200B;**抓取**&#x200B;圖示![抓取圖示](assets/grab-icon.png)，然後將其拖放到所要的位置。

   >[!TIP]
   >
   >您可以將欄位拖放至另一個區段。
   >區段中必須至少有一個欄位。
   >

   對於檢視記錄的所有使用者，相同型別的所有記錄預覽和頁面中的欄位新位置都會更新。

   對記錄預覽或頁面儲存的版面配置所做的所有變更都會自動完成。

## 將「連線的記錄」頁面新增至記錄

您可以將「連線記錄」頁面的索引標籤新增至記錄，以檢視連線記錄或物件的資訊。

可以在表格檢視中編輯來自已連線記錄的資訊。 從另一個應用程式連線的物件資訊在表格檢視中無法編輯。

將「連線的記錄」頁面新增至記錄時，請考量下列事項：

* 從記錄型別的表格檢視中，將記錄或物件型別連線至記錄型別後，您可以將「已連線的記錄」頁面新增至記錄。

* 您無法將「連線的記錄」頁面新增至記錄的預覽區域。<!--take this out when we release connected record pages to the record preview area-->

* 「連線的記錄」頁面在表格檢視中只會顯示連線的物件或來自一個物件或記錄型別的記錄。 頁面不會在表格檢視中顯示該型別的所有記錄。

* 將「連線的記錄」頁面新增到記錄後，可從記錄的預覽區域看到頁面標籤，但為空白。 您必須移至完整頁面，才能檢視連線記錄的表格檢視。 &lt;！ — 這將隨著將連結的頁面發行到預覽區域而改變 — 檢查並取消免責宣告 — >

* 您可以為下列連線記錄或物件型別新增「連線記錄」頁面：

   * Workfront Planning記錄型別
   * Workfront專案、方案、投資組合、群組或公司。 即使您沒有在Workfront中存取Workfront物件的許可權，仍可檢視連線物件。

  >[!NOTE]
  >
  >   您無法新增已連線AEM Assets記錄的「已連線記錄」頁面。

若要新增「連線的記錄」頁面：

<!--replace the first 2 steps with these steps when we release connected record page to the record preview area, if this goes both to Preview and Prod: 

1. Click the name of the record to open it. 
1. Click **Add page** from one of the following areas: 

   * The record's preview window
   * The record's details page, after clicking the **Open in new tab** icon ![Open details in a new tab icon](assets/open-details-in-a-new-tab-icon.png) in the upper-right corner of the preview page.  

-->

1. 從記錄頁面檢視中，按一下記錄名稱以開啟它，然後按一下預覽頁面右上角的&#x200B;**在新索引標籤中開啟**&#x200B;圖示![在新索引標籤中開啟詳細資料](assets/open-details-in-a-new-tab-icon.png)。
1. 按一下&#x200B;**新增頁面**。

   **建立頁面**&#x200B;方塊開啟。

   ![新增連線記錄頁面模組](assets/add-connection-view-page-modal.png)

1. 新增&#x200B;**頁面名稱**，按一下&#x200B;**連線記錄頁面**，然後按一下&#x200B;**建立**。

   新索引標籤將新增到記錄的頁面。
1. 搜尋或按一下清單中連線記錄或物件型別的名稱。
您選取的記錄型別表格檢視會顯示在新頁面中，而連線的記錄會顯示在表格檢視中。
已連線記錄的所有欄位都會顯示在已連線記錄之索引標籤的表格檢視中。

   依預設，連線的記錄表格的前五個欄位會顯示出來。 依預設，不會顯示任何查閱欄位。

   <!--replace screen shot below when additional capabilities come to the table view - Fields, etc-->

   ![行銷活動詳細資料下的對象已連線資料表檢視](assets/audience-connected-table-view-under-campaign-details-page.png)

1. （選擇性）在連線記錄的表格檢視中，執行下列任一項作業：

   * 按一下記錄名稱。 這會在新索引標籤中開啟記錄頁面。

     這會開啟記錄的預覽頁面。 按一下右上角的&#x200B;**在新索引標籤中開啟**&#x200B;圖示![在新索引標籤中開啟](assets/open-details-in-a-new-tab-icon.png)以開啟連線記錄的頁面。

   * 按一下[連線]**連線**&#x200B;以連線更多記錄，然後按一下連線方塊外部以關閉連線。 新記錄會自動新增到表格中。
   * 編輯表格檢視內連線記錄的任何資訊。

   * 將游標停留在連線記錄的名稱上，然後按一下&#x200B;**更多**&#x200B;功能表![更多](assets/more-menu.png)，然後按一下下列其中一個選項：
      * 檢視
      * 複製連結
      * 編輯縮圖
      * 複製
      * 在上方或下方插入記錄
      * 刪除
   * 選取其中一個記錄，然後按一下畫面底部藍色列中的下列選項之一：
      * 檢視
      * 複製連結
      * 編輯縮圖
      * 複製
      * 刪除。 當您選取多個記錄時，「刪除」是唯一可用的選項。

     如需有關編輯表格檢視中記錄的資訊，請參閱[編輯記錄](/help/quicksilver/planning/records/edit-records.md)。

   * 在「連線的記錄」頁面上，內聯編輯表格中的任何記錄。 Workfront物件會以唯讀表格檢視顯示，且您無法加以編輯。

1. （選擇性）連按兩下「連線記錄」頁面標籤的名稱

   或

   將游標暫留在索引標簽名稱上，然後按一下[其他] **** ![ [其他]功能表](assets/more-menu.png)，然後按一下[重新命名] **以重新命名為新的[連線檢視]索引標籤。**
1. （可選）使用工具列中的下列任何檢視元素來管理表格檢視：

   * 篩選器
   * 排序
   * 分組
   * 欄位，以顯示、隱藏或重新排列欄位

   如需詳細資訊，請參閱[管理資料表檢視](/help/quicksilver/planning/views/manage-the-table-view.md)。

   >[!NOTE]
   >
   >   您無法在已連線記錄之索引標籤的表格檢視中建立、編輯或刪除欄位。
   >

1. 按一下&#x200B;**連線**&#x200B;以新增或移除記錄。 如需詳細資訊，請參閱[連線記錄](/help/quicksilver/planning/records/connect-records.md)
1. （選擇性）將游標暫留在[連線的記錄]頁面索引標簽名稱上，按一下[其他] **** ![ [其他]功能表](assets/more-menu.png)，然後按一下[刪除] ****&#x200B;以移除索引標籤。




<!--
## Add a Brief page to a record's page

You can add a Brief page to the record's preview or pages. 

Brief pages contain the same information as the Details tab, in a read-only format. <!--edit this when we can remove fields from this page-->

<!--
1. From a record's page view, click the name of a record to open its preview or page.
1. Click **Add page** > **Brief**. 
1. Add the **Page name**, then click **Create**. 
-->



