---
title: 管理記錄頁面配置
description: 您可以在Adobe Workfront Planning中編輯記錄預覽和頁面的版面。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: c044b4df-f61d-48e0-be9b-e9fa151b092b
source-git-commit: 48bfeb3b950ca1149a919aa204d77db6aa501e01
workflow-type: tm+mt
source-wordcount: '1384'
ht-degree: 0%

---


# 管理記錄頁面配置

<!--
<span class="preview">The information highlighted on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

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
<p>任何Workfront和任何Planning套件</p>
<p>任何工作流程與任何Planning套件</p>
<p>如需每個Workfront Planning套件所含內容的詳細資訊，請聯絡您的Workfront客戶代表。 </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront授權</p></td> 
   <td><p>標準</p>
   </td> 
  </tr> 
  <tr>
   <td role="rowheader"><p>物件許可權</p></td>
   <td>
   <p>貢獻或更高的許可權到工作區和記錄型別 </p>  
   <p>系統管理員擁有所有工作區的許可權，包括他們未建立的工作區</p> 
  </td>
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
<p>Any</p>
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
   <td>
   <p>Standard</p>
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
   <td>
   <p>Contribute or higher permissions to a workspace and record type </a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p> 
  </td>
  </tr>
 </tbody>
</table>-->

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

1. （選擇性）選取[連線]索引標籤右上角的&#x200B;**顯示所有記錄**&#x200B;設定。 所有連線的記錄型別都會顯示，包括尚未有任何連線記錄的型別。 依預設，切換會取消選取，且隱藏沒有連線記錄的記錄型別。

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

您可以將「連線記錄」頁面的索引標籤新增至記錄，以檢視連線記錄或物件的資訊。 這會將表格檢視中的連線記錄新增至索引標籤。

如需詳細資訊，請參閱[新增連線記錄頁面至記錄](/help/quicksilver/planning/records/add-a-connected-records-page-to-a-record.md)。

<!--this content has been moved to the page linked above
Consider the following when adding a Connected records page to a record: 

* You can add a Connected records page to a record after you connected record or object types to the record type from the table view of a record type.

* You can add a Connected records page from a record's preview area or the record's page.

* Connected records pages display only the connected objects or records from one object or record type in a table view. The page does not display all records of that type. 

* You can add Connected records pages for the following connected record or object types:

   * Workfront Planning record types
   * Workfront projects, programs, portfolios, groups, or companies. You can view the connected Workfront objects even when you do not have permissions to access them in Workfront. 

To add a Connected records page:

1. Click the name of the record to open it from any view of a record type page. 
1. Click **Add page** from one of the following areas: 

   * The record's preview window
   * The record's details page, after clicking the **Open in new tab** icon ![Open details in a new tab icon](assets/open-details-in-a-new-tab-icon.png) in the upper-right corner of the preview page.  

   The **Create page** box opens.

   ![Add Connected records page modal](assets/add-connection-view-page-modal.png) 

1. Add the **Page name**, click **Connected records page**, then click **Create**.

   A new connected records page is added as a new tab to the record's page.
   
   The records that are connected to the current record display in the table view.  

      >[!TIP]
      >
      >You must add connected records in the table or Details area of a record before you can display them in a connected records page.

   (^^^^^^All fields of the connected record display in the table view of the connected record's tab.^^^^^^^^)
   
   The first five fields of the connected records display by default. (^^^^No lookup fields display by default.^^^^^^^)

   ![Audience connected table view under campaign details](assets/audience-connected-table-view-under-campaign-details-page.png)

1. (Optional) Search for or click the name of a connected record or object type in the list.

1. (Optional and conditional) In the table view of the connected records page, do any of the following when viewing connected Planning records or any Workfront objects except for projects: 

   * Click the name of a record. This opens the record's page in a new tab. 

   * Click **Connect** at the bottom of the table view to connect more records, then click outside the connection box to close it. The new records are automatically added to the table. 

      For information, see [Connect records](/help/quicksilver/planning/records/connect-records.md).
   * Edit any information from the connected records inline in the table view. 

   * Hover over a connected record's name, then click the **More** menu ![More menu](assets/more-menu.png)
   
      Or 
      
      Select one of the records, then click one of the following options in the blue bar at the bottom of the list: 

      * **View** to open the record page in a new tab
      * **Copy link** to copy a link to the record page
      * **Edit thumbnail** to open the **Record thumbnail** box and edit the record's thumbnail image
      * **Duplicate** to duplicate the connected record. The duplicated record is also connected to the current record.
      * **Insert record above or below** to add new records to the connected record type. New records added here are also connected to the current record. This option is not available in the blue bar when selecting a record in the table.
      * **Delete** to delete the record. Deleting a connected record deletes it from its record type and from everywhere where the record is connected.

      For information about editing records in the table view, see [Edit records](/help/quicksilver/planning/records/edit-records.md). 

      >[!TIP]
      >
      >You can select more than one record or object to delete them.

   * Inline edit any of the Planning records in the table on the Connected records page. 
   
      All other Workfront objects display in a read-only table view and you cannot edit them. 
   
1. (Optional and conditional) In the table view of the connected records page, do any of the following when viewing connected Workfront projects:

     * Click **Connect records** in the upper-right corner of the connected record page to connect existing projects.

      For information, see [Connect records](/help/quicksilver/planning/records/connect-records.md).
     * Inline edit project information in the table.
     * Click **New row** to create a project without a template. The new project is connected to the current record immediately.

         For more information, see [Create Workfront objects from Workfront Planning as you connect them to records](/help/quicksilver/planning/records/create-workfront-objects-from-workfront-planning.md)
     * Hover over a project and click the **More** menu [More menu](assets/more-menu.png)
     
         Or

         Select one or more projects, and notice the blue bar at the bottom of the list, then click one of the following:
         
         * **Delete** to delete the project. Deleting a project disconnects it from the record and moves it to the Workfront's Recycle Bin. 
         * **Disconnect** to disconnect the project from the record. Disconnecting a project removes it and all the values of its lookup fields from the current record.
      
1. (Optional) Double-click the name of the **Connected records page** tab

   Or

   Hover over the name of the tab, then click **More** ![More menu](assets/more-menu.png), then click **Rename** to rename to new Connected view tab.
1. (Optional) Use any of the following view elements in the toolbar of a connected record page to manage the table view:

   * Filters
   * Sort
   * Grouping
   * Fields, to display, hide, or rearrange fields
   * Row height
   * Search

   For information, see [Manage the table view](/help/quicksilver/planning/views/manage-the-table-view.md). 

   >[!NOTE]
   >
   >You cannot create, edit, or delete fields in the table view of a connected record's tab.
   
1. (Optional)  Hover over the name of the Connected records page tab, click **More** ![More menu](assets/more-menu.png), then click **Delete** to remove to tab.-->


<!--
## Add a Brief page to a record

(^^^^^^^^^^move this content to its own article, like you did above - leave the header here with a link^^^^^^^^^^^^)

You can add a Brief page to the record's preview or pages. 

Brief pages contain the same information as the Details tab, in a read-only format. <!--edit this when we can remove fields from this page-->

<!--
1. From a record's page view, click the name of a record to open its preview or page.
1. Click **Add page** > **Brief**. 
1. Add the **Page name**, then click **Create**. 
-->



