---
title: 建立記錄
description: 使用Adobe Workfront規劃功能時，記錄是記錄型別的例項。 在建立個別記錄之前，您必須先建立記錄型別。 建立分類記錄與建立作業記錄相同。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: c7de4b1f-674b-424b-af64-a6df62fb738f
source-git-commit: b795ceccb3f72eb64269062823199be9c8511860
workflow-type: tm+mt
source-wordcount: '809'
ht-degree: 0%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->

# 建立記錄

{{maestro-important-intro}}

在Adobe Workfront規劃功能中，記錄是記錄型別的例項。

您可以擁有下列記錄型別：

* **作業記錄**：代表工作相關物件。 例如，針對名為「行銷活動」的營運記錄，您可以為「每月電子報」或「夏季銷售」等記錄命名。
* **分類法記錄**：它們代表可與作業記錄關聯的屬性。 例如，針對名為「頻道」的分類法記錄型別，您可以命名分類法，例如「電子郵件」、「社群媒體」或「廣告」。

建立作業記錄與建立分類記錄相同。

您可以執行下列其中一項作業來建立記錄：

* 手動為記錄型別建立它們
  <!-- not possible anymore: * Connect them to records from other applications-->
* 從外部清單複製並貼上資訊，以建立記錄。

本文會介紹如何建立記錄。 如需有關管理表格或時間表檢視中的記錄的資訊，請參閱下列文章：

* [管理表格檢視](/help/quicksilver/maestro/views/manage-the-table-view.md)
* [管理時間表檢視](/help/quicksilver/maestro/views/manage-the-timeline-view.md)

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
<p>貴組織必須註冊Adobe Workfront規劃功能封閉測試版計畫。 請聯絡您的客戶代表以查詢此新產品/服務。 </p>
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
   <td> <p>Adobe Workfront規劃功能沒有存取控制 </p>  
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

<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

## 手動將記錄新增至記錄型別以建立記錄 <!--in a record type table (I don't think you can create them elsewhere right now)-->

您可以在記錄型別頁面的表格檢視中建立記錄。

如需有關編輯記錄資訊的資訊，請參閱 [編輯記錄](/help/quicksilver/maestro/records/edit-records.md).

{#step1-to-maestro}

您上次存取的工作區預設會開啟。 如需有關建立工作區的資訊，請參閱 [建立工作區](../architecture/create-workspaces.md).
1. 按一下記錄型別卡。 如需有關建立記錄型別的資訊，請參閱 [建立記錄型別](../architecture/create-record-types.md).

   記錄型別頁面會在您上次存取的檢視中開啟。 依預設，會在表格檢視中開啟記錄型別頁面。
所選型別的所有記錄都會顯示在表格檢視中。

1. （視條件而定）如果記錄型別頁面未在表格檢視中開啟，請按一下 **檢視** 下拉式功能表，並選取現有的 **表格檢視** ![](assets/table-view-icon.png) 或按一下 **建立檢視>表格** 以建立表格檢視。

<!--Replace the above with this when we release the tabbed views: 
1. (Conditional) If the record type page does not open in the table view, click the tab of a table view, or click **+ View** to create a table view. -->

1. 若要新增記錄，請按一下 **新記錄** 在表格的最後一列

   或

   按一下 **Shift + Enter** 從表格的任一欄或列移至鍵盤上。 這會新增空白列。

   ![](assets/adding-a-new-campaign-in-table-row.png)

1. 開始在新列輸入有關新記錄的資訊。

   >[!NOTE]
   >
   >  * 記錄沒有必填欄位。 不過，我們建議您為記錄新增「名稱」，因為將記錄連結至彼此時，有助於識別記錄。
   >
   >  * 參考其他記錄型別或計算欄位的欄位為唯讀欄位。

1. 繼續新增每一列的資訊，然後按一下 **輸入** 以儲存變更。

<!--Or 
    
    Click the new record's name or the **Open details** icon ![](assets/open-details-icon-in-table-name-field.png) to the left of the record name. The **Details** box opens in the table. 

      >[!TIP]
      >
      >    You can access the Details box only from the name field of the record when the Name field is a primary field. 

  1. Start editing the record's information in the Details box. Workfront automatically saves your changes. 
  1. (Optional) Click the **Open in new tab** icon ![](assets/open-details-in-a-new-tab-icon.png) in the upper-right corner of the Details box to open the record's **Details** page in a new tab. Continue editing the record on the Details page.
    -->

1. （可選）使用下列鍵盤快速鍵來復原或重做新增記錄：

   * CTRL + Z (Mac為⌘ + Z)可復原變更
   * CTRL + Shift + Z (Mac為⌘ + Shift + Z)以重做變更

<!-- this is not possible anymore: 

## Create records by connecting them from another application

You can import records from other applications by linking them to existing records. This creates a linked record for the other application's connected object. 

1. Create a record type, as described in the [Create record types](../architecture/create-record-types.md).

1. Create records for the record type you created in the previous step. For information, see the section [Create records by manually adding them to a record type](#create-records-by-manually-adding-them-to-a-record-type) in this article. 

1. Create a connection to an object type from another application for the record type you created. For information, see [Connect record types](../architecture/connect-record-types.md).

1. Add objects from another application to the records you created above using the linked record field you created in the previous step. For information, see [Connect records](../records/connect-records.md). 

    The following items are created in Maestro:

    * A read-only Maestro record type that refers to the other application's record type you linked to in the connected record field. 

      For example, if you connect a Maestro record type to Workfront project, a read-only record type named "Workfront project" is created in the same workspace. You can access the read-only Workfront record types from the table view of the Maestro records you're linking from. 
   
-->

## 從外部清單複製並貼上資訊，以建立記錄

1. 開始在「表格」檢視中建立記錄（如區段所述） [手動將記錄新增至記錄型別以建立記錄](#create-records-by-manually-adding-them-to-a-record-type) 本文章內容。

   確定表格檢視具有您要填入新記錄資訊的欄（或欄位）。

1. 按一下 **新&lt;記錄型別名稱>** 在表格的最後一列，新增任意數目的新資料列至表格。

   例如，如果要從另一個應用程式貼上10筆新記錄的資訊，請將10列新增到表格檢視中。

1. 在另一個應用程式中，建立您要匯入的記錄清單。

   例如，您可以使用Excel試算表來建立清單。

   清單應包含表格格式的資訊。

   >[!TIP]
   >
   > 清單的欄應包含您在Workfront中擁有的現有欄位資訊。
   >
   > 確定您已在Workfront中建立所需欄位，且工作表中的資訊以符合Workfront中每個欄位資訊的正確格式顯示。

1. 從另一個應用程式中，選取數個列和欄，然後將資訊貼到記錄型別表格檢視中，從第一個新記錄開始。

   下列資訊會匯入Workfront規劃功能區域：

   * 列包含新記錄
   * 欄會填入記錄欄位的資訊。
