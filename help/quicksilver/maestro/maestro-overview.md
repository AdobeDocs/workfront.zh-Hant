---
title: Adobe大師概觀
description: Adobe大師是Adobe Workfront的新產品。 您可以建立可完全自訂的工作區，以定義符合企業內每個組織單位需求的工作流程。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: b1d6e0b3-e6d4-46d1-a6a2-4b8b73f7d3f7
source-git-commit: f4ef463ebdc9a4a7a0802e5394d7820ebc447aa9
workflow-type: tm+mt
source-wordcount: '1818'
ht-degree: 1%

---

# Adobe大師概觀

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

<!--see the separate article I wrote to have the PMs vet it for this: https://adobe-my.sharepoint.com/personal/alinaw_adobe_com/_layouts/15/doc.aspx?sourcedoc={79f94807-3d73-4015-afc0-5c016fc63cfc}&action=edit-->

<!--all the links are hidden for now, so I can share this with customer zero. Activate the links before making this public. -->

<!-- remove the references to closed beta from the entire article-->

<!--update the video in the IMPORTANT below, when we have something better, especially after Open Beta - remove it-->

>[!IMPORTANT]
>
>目前，Adobe大師是測試版計畫的一部分，向有限數量的客戶開放。
>
>如需加入Maestro測試版計畫的詳細資訊，請聯絡您的客戶代表。
>[觀看Adobe大師的影片展示](https://video.tv.adobe.com/v/3424253/){target=_blank}

## Adobe Maestro簡介

Adobe大師是Adobe Workfront的新產品。 Maestro的目的在於全面掌握組織的營運細節，並回答工作管理生命週期各階段的關鍵業務問題。

團隊和領導力需要這些問題的明確答案，例如：

* 第4季我們在EMEA執行多少次行銷活動？
* 並行行銷活動之間是否有任何對象重疊？
* 認識計畫目前表現如何？
* 特定行銷活動的資產看起來如何？ 其中哪些仍須核准？

若要回答這些問題，領導力需要一個解決方案，針對從規劃到執行、從交付到結果衡量的每個工作階段，提供整體檢視。 目前，組織擁有可涵蓋程式某些部分的工具，但許多工具無法與所有工作階段建立良好的連線，也無法可靠地提供結果。

以下是Maestro的部分主要功能：

* 解決跨所有階段以及參與工作流程的所有利害關係人管理工作的問題。
* 完全自訂您的工作流程，從決定您的組織使用哪些物件型別（或記錄型別），到設定這些物件如何彼此連結。
* 從其他系統連結到物件型別，為所有流程建立一致的架構。

## 在封閉Beta版計畫期間使用Maestro所需的存取權

>[!IMPORTANT]
>
>目前，沒有與使用者或Maestro中的資訊相關聯的存取層級或許可權。 所有使用者都可以檢視、編輯和刪除任何其他使用者新增至Maestro的所有資訊。

如需使用Maestro所需存取權的詳細資訊，請參閱 [Adobe大師存取概觀](../maestro/access/access-overview.md).

<!-- hidden the table after I moved the content to the Access overview article: 

You must have the following access to use Adobe Maestro: 

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Adobe product</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the Adobe Maestro closed beta program. Contact your account representative to inquire about this new offering. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license</p></td>
   <td>
   <p>Any</p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader">Access level</td>
   <td> <p>Any</p>  
</td>
  </tr>

<tr>
   <td role="rowheader">Layout template</td>
   <td> <p>Your system administrator must add the Maestro area in your layout template. For information, see <a href="../maestro/access/grant-access.md">Grant access to Adobe Maestro</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

************* Activate note when going to GA: 

>[!NOTE]
>
>If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). 
-->

## Maestro術語

雖然Maestro是Workfront的一部分，但是它隨附了專屬的概念和術語。 開始為貴組織設定Maestro之前，請務必熟悉Maestro的概念。

Maestro的架構是完全可自訂的。 您可以建立所有記錄型別、其屬性以及與其相關聯的任何欄位，以符合您組織的確切需求。

以下是主要的Maestro物件和概念：

* **工作區**：定義特定組織作業生命週期的記錄型別和分類之集合。 工作區是組織單位的工作框架。

  一個Workfront例項最多可以有1,000個工作區。

  ![](assets/marketing-workspace-with-record-type-taxonomies-opening-page.png)

  如需詳細資訊，請參閱 [建立工作區](../maestro/architecture-and-fields/create-workspaces.md).

* **記錄型別**：Maestro主要物件型別。

  與Workfront預先定義物件型別不同，在Maestro中，您可以建立自己的物件型別。

  例如，在Workfront中，已建立方案、Portfolio、專案、任務或問題的物件型別。

  在Maestro中，您可以建立符合組織工作流程的任何記錄型別。 稍後，您可以定義記錄型別如何相互關聯或表單相依性。

  如需詳細資訊，請參閱 [作業記錄型態與分類的概要](../maestro/architecture-and-fields/overview-of-record-types-and-taxonomies.md).

  Maestro有下列記錄型別：

   * **作業記錄型別**：代表策略性計畫、方案或已執行工作的記錄型別。

     ![](assets/operational-record-type-blank.png)

     例如，促銷活動、活動、方案可以是作業記錄型別。

     如需詳細資訊，請參閱 [建立記錄型別](../maestro/architecture-and-fields/create-record-types.md).

   * **分類法**：擷取操作記錄型別相關屬性的記錄型別。

     ![](assets/taxonomy-record-type-blank.png)

     雖然建立分類與建立作業記錄型別相同，但Maestro會區分作業記錄型別與分類記錄型別。 分類法的用途是增強作業記錄型別。 <!--this is no longer true, but might be later?!: A taxonomy is a record without dates, like a static list of attributes.-->

     例如，「對象」、「區域」或「地址」可以是分類型別的記錄型別。

     如需詳細資訊，請參閱 [建立分類記錄型別](../maestro/architecture-and-fields/create-a-taxonomy.md).

* **記錄**：Maestro記錄型別的例項。 記錄可以參考作業記錄型別或分類法。

  ![](assets/records-highlighted-in-campaign-record-type-list.png)
  ![](assets/records-highlighted-in-region-taxonomy-type-list.png)

  將記錄型別新增至工作區後，您就可以開始在記錄型別的頁面上新增該型別的記錄。

  例如，「Campaign」可以是作業記錄型別，「Summer Campaign for EMEA」是Campaign記錄型別的記錄

  或

  「地區」是分類法型別的記錄，而「美洲 — 拉丁美洲」或「EMEA — 中歐」是分類法記錄。

  如需詳細資訊，請參閱 [建立記錄](../maestro/records/create-records.md).

* **工作區範本**：您可以使用預先定義的範本建立工作區。 您可以使用範本中預先定義的記錄型別、分類和欄位，也可以新增您自己的記錄型別、分類和欄位。

  ![](assets/workspaces-page-with-templates-thumbnails.png)

  Maestro隨附銷售、行銷和產品管理工作區範本。

  如需詳細資訊，請參閱 [建立工作區](../maestro/architecture-and-fields/create-workspaces.md).

* **欄位**：欄位是可新增至作業或分類記錄型別的屬性，這些記錄型別包含有關記錄型別的資訊。 <!--check the shot below, "Connection" needs to be in lowercase-->

  ![](assets/drop-down-list-of-record-fields.png)

  有關Maestro欄位的注意事項：

   * 您為記錄型別新增的欄位會自動與該型別的所有記錄相關聯，並可用於擷取有關這些記錄的資料。

   * 在套用至記錄型別頁面的「表格」檢視中，欄位會顯示為欄。 它們也會顯示在記錄的詳細資訊頁面中。

   * 欄位對記錄型別是唯一的，不會從一種記錄型別轉移到另一種記錄型別。

   * Maestro欄位完全可自訂，僅可在Maestro中存取。 您無法從Workfront存取Maestro欄位。

  如需詳細資訊，請參閱 [建立欄位](../maestro/architecture-and-fields/create-fields.md)

  依預設，新的作業記錄型態與下列預先定義的欄位相關聯：

   * 名稱
   * 說明
   * 開始日期
   * 結束日期
   * 狀態

  依預設，新的分類記錄型別與「名稱」欄位相關聯。

  您可以建立下列型別的自訂欄位：

   * 單行文字
   * 段落
   * 多選
   * 單選
   * 日期
   * 數字
   * 百分比
   * 貨幣
   * 核取方塊

* **連結的記錄型別**， **連結的記錄**、和 **連結的記錄欄位**：您可以在下列實體之間建立連線：

   * 兩種Maestro記錄型別
   * Maestro記錄型別和Workfront專案、方案、投資組合、公司或群組物件型別。

  ![](assets/new-connection-tab-with-workfront-option.png)

  在記錄型別之間建立連線之後，可以將這些型別的個別記錄彼此連線。 記錄之間的連線會顯示為連結的記錄欄位。

* **連結的欄位** （或查詢欄位）：在兩個記錄型別之間建立連線並將個別記錄連結在一起後，您可以在要連線的記錄上參考連結記錄的欄位。

  ![](assets/add-lookup-fields-modal.png)

  如需連結記錄型別、記錄和建立連結欄位的相關資訊，請參閱下列文章：

   * [連線記錄型別](../maestro/architecture-and-fields/connect-record-types.md)
   * [連線記錄](../maestro/records/connect-records.md)

<!--not yet:* Fields are reusable across Record Types.  -->

* **檢視**：記錄會顯示在不同檢視型別的個別記錄型別頁面下。

  ![](assets/view-types-drop-down-from-record-type-list.png)

  檢視包含特定檢視型別的個人化設定，例如欄位清單（欄）、記錄清單（列）、其順序（排序）、套用或適用的篩選和分組。

  以下是您可以套用至記錄型別頁面的檢視型別：

   * **表格檢視**：以表格格式顯示記錄及其欄位。 表格的列是個別記錄，欄是記錄欄位。 這是預設檢視。

     ![](assets/table-view-example.png)

   * **時間表檢視**：在時間軸中顯示至少有兩個日期欄位的記錄。

     ![](assets/grouping-applied-in-timeline-view.png)

  如需詳細資訊，請參閱 [管理記錄檢視](../maestro/views/manage-record-views.md).


## Maestro物件限制

下表顯示您可以在Maestro中建立多少物件的限制。 當我們進入Maestro開發的下一個階段時，限制可能會有所變更。

| Maestro物 | 限制 |
|-------------------------------------------------------------------------------|:---------------------------------------------------------------------------------------------------------------:|
| 一個Workfront例項的工作區數 | 1,000 |
| 一個工作區的記錄型別數 | 1,000 （這包括工作區的分類，或從協力廠商應用程式匯入的物件） |
| 一種記錄型別的記錄數 | 10,000 |
| 一種記錄型別或分類法的欄位數 | 500 |
| 文字欄位的字元數 | 1,000個字元 |
| 您可以在記錄型別表格中貼上的檔案大小 | 1MB |
| 您可以透過記錄型別表格的API匯入的檔案大小 | 1.5MB |
| 提出API要求的速率 | 每分鐘200個請求 |
| 您可在表格中匯入的Excel檔案CSV大小 | 5MB |

## 為您的Workfront執行個體中的使用者啟用Maestro

貴組織必須註冊AdobeMaestro封閉測試版計畫，您才能存取Maestro。 如需註冊Beta版計畫的相關資訊，請聯絡客戶代表。

如需有關授予存取權以及允許其他人使用Maestro的詳細資訊，請參閱 [授與Adobe大師的存取權](../maestro/access/grant-access.md).

<!--hidden this after moved it to a separate article

After your organization has been enrolled in the Maestro beta program, you can add the Maestro area for other users by using a layout template. 

To share the Maestro area using a layout template: 

1. Log in to Workfront as a system administrator.  

1. Add the Maestro icon to the Main Menu using a Layout Template. For information, see [Customize the Main Menu using a layout template](../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md). 

1. Assign the  layout template to the users that you want to have access to Maestro.For information, see [Assign users to a layout template](../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md).

    All users who can access Maestro in their Main Menu can start creating workspaces, records types, records, and fields.  
  -->


## 找到Maestro

確保貴組織已獲得Maestro的存取權，且您的系統或群組管理員已將Maestro區域新增至您的主功能表。

若要尋找Maestro：

1. 登入Adobe Workfront。

1. 按一下 **主要功能表** ![](assets/main-menu-workfront.png) 或按一下 **主要功能表** ![](assets/main-menu-shell.png) 左上角（如果有的話）。

1. 按一下 **大師** ![](assets/maestro-icon.png).

   「Maestro工作區」區域隨即開啟。

1. （可選用且建議使用）繼續下列部分動作，以在Maestro中建置您的工作結構：

   1. 從頭開始或使用範本建立工作區。

   1. 將記錄型別新增至新工作區。

   1. 將分類新增至新工作區。

   1. 按一下記錄型別的名稱以開啟記錄的頁面。 依預設，記錄頁面會在「表格」檢視中開啟。

   1. 執行下列任一項作業來自訂「表格」檢視：

      * 按一下「 」以新增更多欄位至記錄型別 **+** 圖示加以顯示。 檢視中的欄是與記錄型別相關聯的欄位。
      * 按一下 **+** 圖示重新整理。 檢視中的列是所選記錄型別的唯一記錄。
      * 按一下 **篩選器** 以篩選您顯示在記錄型別頁面上的資訊。

   1. 按一下記錄名稱，在記錄的「詳細資訊」頁面中檢視更多資訊。

   1. 從建立時間表檢視 **檢視** 記錄型別頁面右上角的下拉式功能表。

   1. 透過更新篩選器、群組或設定來自訂時間軸檢視。

## Maestro目前可用的功能

下表說明Maestro中可用的主要功能，及其可用時間軸。 此清單並未包含所有功能。

| 功能 | 現在可用 | 即將推出 | 研究中 |
|----------------------------------------------------|:-----------------------------:|:--------------------------------:|:----------------:|
| 建立工作區 | ✓ (A) |                                  |                  |
| 建立作業記錄型別 | ✓ |                                  |                  |
| 建立分類 | ✓ |                                  |                  |
| 建立個別具名記錄和分類法 | ✓ |                                  |                  |
| 建立記錄自訂欄位 | ✓ |                                  |                  |
| 使用Excel或CSV檔案匯入記錄型別和欄位 | ✓ |                                  |                  |
| 連結記錄 | ✓ |                                  |                  |
| 檢視表格中的記錄 | ✓ |                                  |                  |
| 在時間軸中檢視記錄 | ✓ |                                  |                  |
| 篩選記錄 | ✓ |                                  |                  |
| 在時間軸檢視中將記錄分組 | ✓ |                                  |                  |
| 在表格檢視中將記錄分組 |                               | ✓ |                  |
| 排序表格檢視中的記錄 | ✓ |                                 |                  |
| 在時間軸檢視中排序記錄 |                               | ✓ |                  |
| 在表格檢視中排序群組 |                               | ✓ |                  |
| 在時間軸檢視中排序群組 |                               | ✓ |                  |
| 連線工作區 |                               | ✓ |                  |
| 連線主要記錄和分類法 | ✓ |
| 在表格檢視中搜尋記錄 | ✓ |   |
| 將Maestro記錄連線至Workfront專案、計畫、投資組合、公司、群組 | ✓ |                                 |                  |
| 記錄詳細資訊頁面 | ✓ |                                  |                  |
| 更新記錄詳細資訊頁面的版面 |                               | ✓ |                  |
| 存取層級和許可權 | | ✓ |  |
| 提交請求 |                               |                                  | ✓ |
| 創意簡報 |                               |                                  | ✓ |
| 自訂記錄的顏色和圖示 | ✓ |                                  |                 |

## Maestro發行活動

我們定期為Maestro發佈新功能。 如需最新已發行功能清單，請參閱 [Adobe大師發行活動](../maestro/release-activity.md).

<!--moved the contents of this whole section to its own article: release-activity.md, in the same folder

This section lists the features and patches that have been released after the launch of the Maestro closed beta program, on May 22, 2023. 

The features are released weekly and are listed in the order of their release, with the most recent first. Customers who are participating in the Maestro closed beta program can access all features in their Preview and Production environments. 

### Week of September 4, 2023

#### Connect Maestro records with Workfront companies and groups

Preview and production: September 5, 2023  

You can now connect a Maestro record with Workfront companies and groups. You must first create a connection between a Maestro record type and the Workfront companies and groups object types. Then, you can connect a single Maestro record of the selected record type to individual Workfront companies and groups.  

Consider the following:  

* You must create a connection between Maestro record types and Workfront companies and groups for each Workspace.  

* You cannot connect taxonomy record types with Workfront object types. 

* You can connect multiple Maestro records to the same Workfront company or group, and multiple companies or groups to the same Maestro record.  

* You cannot edit companies or groups in Maestro. All company or group changes performed in Workfront are visible in Maestro, when reviewing the Maestro linked records.  

#### URL support for single-line text fields 

Preview and production: September 7, 2023 

For better visibility when working with links in the Table view, we have added support for URLs in single-line text fields. Using URLs to other websites or external drives when updating a single-line text field, now identifies them as links and allows you to click them from the table.  

### Week of August 28, 2023

#### Field visibility menu for the Table View toolbar

Preview and production: August 31, 2023

To display the right information on a given set of records, especially if you intend to share the view with others who need to see some but not all fields of a record type, you can now select which fields (or columns) to display and which to hide in the Table view.  

You can hide or show individual fields, from each header of the field columns, or you can manage all fields of the record type from a setting in the table view toolbar.  

### Week of August 21, 2023

#### Connect Maestro records to programs and portfolios 

Preview and production: August 24, 2023

You can now connect a Maestro record with Workfront programs and portfolios. You must first create a connection between a Maestro record type and a program or portfolio which creates a connected field. Then, you can connect any Maestro records from all other record types within the same workspace to specific programs and portfolios which will create a read-only Workfront Program or Workfront Portfolio record type in the same workspace. Consider the following:

* Workfront connector record types are unique for each workspace. 
* You can connect multiple Maestro records to the same Workfront program or portfolio, and multiple programs and portfolios to the same Maestro record. 
* You cannot edit programs and portfolios in Maestro. All program and portfolio changes performed in Workfront are visible in Maestro, when reviewing the linked records. 

#### New sorting functionality for the table view

Preview and production: August 24, 2023

You can now sort records in the table view of a record type page. 
The following capabilities are now available: 

* Sorting at the table-level, where you can sort by multiple fields at the same time. 
* Sorting at the column or field-level, where you can sort by an individual field at a time.

#### Improvements to the timeline view: new look-and-feel for groupings and the Compact/ Standard view switch

Preview and production: August 24, 2023

We have introduced the following improvements to the timeline view: 

* You can now display the timeline view in the following modes:

    * Standard: Displays records in separate lines.
    * Compact: Display the records whose dates don't intersect on the same line. 

* We have changed the look-and-feel of the grouping lines in the timeline view to display above the timeline of the records they contain. Prior to this improvement, the grouping lines displayed across the entire length of the timeline.

### Week of August 14, 2023

#### Reorder columns in the table view

You can now reorder columns in the Maestro table view. Consider the following when reordering columns: 

* The Name field is always the first field in the table view of a record type page 

* You cannot move the Name field to another position 

* The Name field is frozen and is not part of the horizontal scroll. 

#### Horizontal scroll for timeline view

You can now scroll horizontally in the timeline view of a record type. 

### Week of August 7, 2023

#### Import record types from an Excel file 

Preview and production: August 10, 2023

You can now import an Excel file to create record types in a workspace. The sheets of the file become the record types, and the columns of the file become their respective fields.  

#### Improved experience for connecting record types and projects 

Preview and production: August 10, 2023

We have improved the way you connect record types, including connecting to Workfront projects. As part of this improvement, we made the following changes when adding a field for a record type from the table view:  

* Removed the Relationship-type field from the "New field" tab.  

* Add a "New connection" tab where you can directly select the record or object type you want to connect to, eliminating the need for a Relationship-type field. 

### Week of July 10, 2023

#### Update the appearance of a record type

Preview and production: July 13, 2023

You can now select a custom icon for a record type, as well as a custom color for the record type icon.  

#### New Checkbox field type

Preview and production: July 13, 2023 

You can now add a Checkbox field type to Maestro record types. You can use the Checkbox field type to add a single checkbox option to a record. You can use this field to indicate a specific attribute or status for that particular record. For example, you can use it as a flag for tracking completion, approval, or any other binary attribute for each record.  

### Week of June 26, 2023

#### Quick activation of the contextual menu in a table

Preview and production: June 28, 2023
 
We have enabled the ability to activate the contextual menu by right-clicking anywhere in a record row, when viewing the records in the table view or a record type. You can now quickly view, delete, or copy a link to the record's Details page when you access the contextual menu from anywhere in the table view of a record type. Prior to this enhancement, the contextual menu was accessible only from the More menu in the Name column of a record.  

### Week of June 19, 2023

#### Record field names are unique

We have introduced a requirement now that the field names of a Maestro record type should have unique names. Fields that belong to different record types do not have to have unique names.  

### Week of June 5, 2023

#### Connect Maestro records with Workfront projects

Preview and production: June 5, 2023

You can now connect a Maestro record with Workfront projects. You must first create a connector Maestro record type to establish the connection between Maestro records and Workfront projects. Then, you can connect any Maestro records from all other record types to the connector record using the Relationship field. Consider the following:

* You must have a connector record type for Workfront for each Workspace. 
* You can connect multiple Maestro records to the same Workfront project, and multiple projects to the same Maestro record. 
* You cannot edit projects in Maestro. All project changes performed in Workfront are visible in Maestro, when reviewing the linked records. 

### Week of May 29, 2023

#### Two-date requirement for creating a Timeline view

Preview and production: May 31, 2023  

You must have at least two date fields associated with a record type in order to create a Timeline view. 
-->
