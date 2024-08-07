---
title: 建立記錄
description: 使用Adobe Workfront Planning時，記錄是記錄型別的例項。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: c7de4b1f-674b-424b-af64-a6df62fb738f
source-git-commit: bda3dc43828032fd5a8862b12d851c56cf9b6cbd
workflow-type: tm+mt
source-wordcount: '930'
ht-degree: 0%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->

# 建立記錄

{{planning-important-intro}}

在Adobe Workfront Planning中，記錄是記錄型別的例項。

您可以執行下列其中一項作業來建立記錄：

* 從記錄型別頁面新增它們
* 從外部清單複製並貼上記錄清單
* 複製它們

本文會介紹如何建立記錄。 如需有關管理表格或時間表檢視中的記錄的資訊，請參閱下列文章：

* [管理表格檢視](/help/quicksilver/planning/views/manage-the-table-view.md)
* [管理時間表檢視](/help/quicksilver/planning/views/manage-the-timeline-view.md)

## 存取需求

+++ 展開以檢視Workfront Planning的存取需求。

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
   <p>新增：標準</p>
   <p>目前：計畫</p>  
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>存取層級設定</p></td>
   <td> <p>Adobe Workfront Planning沒有存取控制 </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>權限</p></td>
   <td> <p>Contribute或更高的工作區許可權</a> </p>  
   <p>系統管理員擁有所有工作區的許可權，包括他們未建立的工作區</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>版面配置範本</p></td>
   <td> <p>您的Workfront或群組管理員必須在版面配置範本中新增Planning區域。 如需詳細資訊，請參閱<a href="/help/quicksilver/planning/access/access-overview.md">存取總覽</a>。 </p>  
</td>
  </tr>

</tbody>
</table>

*如需詳細資訊，請參閱[Workfront檔案的存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

<!--Maybe enable this at GA - but Planning is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](/help/quicksilver/planning/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

## 將記錄新增至記錄型別<!--in a record type table (I don't think you can create them elsewhere right now)-->以建立記錄

您可以在記錄型別頁面的表格檢視中建立記錄。

如需有關編輯記錄資訊的資訊，請參閱[編輯記錄](/help/quicksilver/planning/records/edit-records.md)。

{{step1-to-planning}}

1. 按一下您要新增記錄的工作區。

   工作區隨即開啟，且記錄型別會顯示為卡片。

1. 按一下記錄型別卡。 如需有關建立記錄型別的資訊，請參閱[建立記錄型別](/help/quicksilver/planning/architecture/create-record-types.md)。

   記錄型別頁面會在您上次存取的檢視中開啟。 依預設，會在表格檢視中開啟記錄型別頁面。
所選型別的所有記錄都會顯示在檢視中。

1. （視條件而定）視您顯示的檢視而定，請執行下列其中一項作業：

   * 從表格檢視中：

      * 在表格的最後一列按一下&#x200B;**新增記錄**

      * 在表格的任何欄或列按一下鍵盤上的&#x200B;**Shift + Enter**。 這會在您開始的記錄底下新增一個空白列。
      * 暫留在記錄的主要欄位上，按一下欄位右邊的&#x200B;**更多**&#x200B;功能表![](assets/more-menu.png)，然後按一下&#x200B;**在上方插入記錄**&#x200B;或&#x200B;**在下方插入記錄**。

     ![](assets/adding-a-new-campaign-in-table-row.png)

   * 從任何檢視：

      * 按一下頁面右上角的&#x200B;**新增記錄**。 記錄預覽方塊開啟。

     Workfront會自動上傳縮圖和封面影像至每張新記錄。 您稍後可以修改這些影像。 如需詳細資訊，請參閱下列文章：

      * [新增封面影像至記錄](/help/quicksilver/planning/records/add-a-cover-image-to-a-record.md)
      * [新增縮圖至記錄](/help/quicksilver/planning/records/add-thumbnails-to-records.md)

1. 開始在您在預覽方塊中看到的欄位中輸入有關新記錄的資訊。

   >[!NOTE]
   >
   >  * 記錄沒有必填欄位。 不過，我們建議您為記錄的主要欄位新增資訊，因為將記錄連結至彼此時，識別記錄會很有幫助。 如需主要欄位的詳細資訊，請參閱[管理資料表檢視](/help/quicksilver/planning/views/manage-the-table-view.md)和[主要欄位概述](/help/quicksilver/planning/fields/primary-field-overview.md)。
   >
   >  * 參考其他記錄型別或計算欄位的欄位為唯讀欄位。

1. （視條件而定）在表格中新增記錄時，請繼續在每一列新增資訊，然後在鍵盤上按一下&#x200B;**Enter**&#x200B;以儲存變更。

   或

   按一下新記錄名稱或記錄名稱左側的&#x200B;**開啟詳細資料**&#x200B;圖示![](assets/open-details-icon-in-table-name-field.png)。 含有記錄詳細資訊的預覽會在表格中開啟。

   >[!TIP]
   >
   >當「名稱」欄位是主要欄位時，您只能從記錄的名稱欄位存取&#x200B;**開啟詳細資料**&#x200B;圖示。

1. 開始編輯記錄預覽中的記錄資訊。 Workfront會自動儲存您的變更。
1. （選擇性）按一下記錄預覽右上角的&#x200B;**在新索引標籤中開啟**&#x200B;圖示![](assets/open-details-in-a-new-tab-icon.png)，以在新索引標籤中開啟記錄的頁面。 繼續編輯記錄頁面上的記錄。 如需詳細資訊，請參閱[編輯記錄](/help/quicksilver/planning/records/edit-records.md)。

1. （可選）在表格檢視中新增記錄或其資訊時，請使用下列鍵盤快速鍵來復原或重做新增記錄或其資訊：

   * CTRL + Z (Mac為⌘ + Z)可復原變更
   * CTRL + Shift + Z (Mac為⌘ + Shift + Z)以重做變更

<!-- this is not possible anymore: 

## Create records by connecting them from another application

You can import records from other applications by linking them to existing records. This creates a linked record for the other application's connected object. 

1. Create a record type, as described in the [Create record types](/help/quicksilver/planning/architecture/create-record-types.md).

1. Create records for the record type you created in the previous step. For information, see the section [Create records by manually adding them to a record type](#create-records-by-manually-adding-them-to-a-record-type) in this article. 

1. Create a connection to an object type from another application for the record type you created. For information, see [Connect record types](/help/quicksilver/planning/architecture/connect-record-types.md).

1. Add objects from another application to the records you created above using the linked record field you created in the previous step. For information, see [Connect records](/help/quicksilver/planning/records/connect-records.md). 

    The following items are created in Workfront Planning:

    * A read-only record type that refers to the other application's record type you linked to in the connected record field. 

      For example, if you connect a Planning record type to Workfront project, a read-only record type named "Workfront project" is created in the same workspace. You can access the read-only Workfront record types from the table view of the Planning records you're linking from. 
   
-->

## 從外部清單複製並貼上記錄，以建立記錄

1. 開始在[資料表]檢視中建立記錄，如本文[將記錄手動新增至記錄型別](#create-records-by-manually-adding-them-to-a-record-type)以建立記錄一節中所述。

   確定表格檢視具有您要填入新記錄資訊的欄（或欄位）。

1. 在表格的最後一列按一下&#x200B;**新增&lt;記錄型別名稱>**，新增您想要的新記錄至表格的所有新列。

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

   下列資訊會匯入Workfront Planning區域：

   * 列包含新記錄
   * 欄會填入記錄欄位的資訊。


## 複製記錄以建立記錄

如需複製記錄的資訊，請參閱[複製記錄](/help/quicksilver/planning/records/copy-or-duplicate-records.md)。