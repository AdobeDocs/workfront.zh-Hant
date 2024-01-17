---
title: 管理記錄檢視
description: 使用「Adobe大師」時，您可以在表格或時間軸檢視中顯示記錄。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 77342724-0182-4134-903b-4428d54cdceb
source-git-commit: daa195b0273a232692fe47691a2926579b87ba6b
workflow-type: tm+mt
source-wordcount: '800'
ht-degree: 0%

---

# 管理記錄檢視

<!--update the metadata with real information when making this available in TOC and in the left nav-->

>[!IMPORTANT]
>
>本文資訊是指Adobe Maestro，這是Adobe Workfront的新產品。
>
>目前，Adobe大師是測試版計畫的一部分，向有限數量的客戶開放。 您必須是Workfront客戶才能使用Maestro功能。
>
>如需加入Maestro測試版計畫的詳細資訊，請聯絡您的客戶代表。
>
>如需詳細資訊，請參閱 [Adobe大師概觀](../maestro-overview.md).

在「Adobe大師」中選取記錄型別後，您可以在下列檢視中顯示該型別的所有記錄：

* 表格

  如需詳細資訊，請參閱 [管理表格檢視](../views/manage-the-table-view.md).
* 時間表

  如需詳細資訊，請參閱 [管理時間表檢視](../views/manage-the-timeline-view.md).

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
   <td role="rowheader">存取層級設定</td>
   <td> <p>Maestro沒有存取層級控制項</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>權限</p></td>
   <td> <p>管理檢視的許可權</p>  
</td>
  </tr>

<tr>
   <td role="rowheader">版面配置範本</td>
   <td> <p>您的系統管理員必須在您的版面配置範本中新增Maestro區域。 如需詳細資訊，請參閱 <a href="../access/access-overview.md">存取權總覽</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

## 使用Maestro檢視時的注意事項

* Maestro中的檢視是記錄型別專屬檢視。 您不能將相同的檢視套用至兩種不同的記錄型別。
* 您建立的檢視只對您和共用檢視的使用者可見。
* 建立作業記錄型別的檢視與建立分類記錄型別的檢視相同。
* 當您修改或刪除檢視時，該檢視會被修改並刪除，以供擁有該檢視許可權的所有使用者使用。
* Maestro中每個檢視都有以下獨特元素：

   * 篩選器
   * 分組
   * 排序

  <!-- some of these are not available in all of the views - edit above-->

  例如，在表格檢視中建立篩選時，篩選結果只會顯示在選取的檢視中，而不會顯示在「檢視」下拉式選單中列出的所有檢視中。

  >[!NOTE]
  >
  > 由於Maestro目前處於Beta版狀態，因此某些檢視元素可能無法用於這兩個檢視。

本文說明有關Maestro檢視的下列資訊：

* [建立及編輯檢視](#create-or-edit-record-views)
* [刪除檢視](#delete-views)
  <!--* [Duplicate a view](#duplicate-views)-->
  <!--* [Add a view as a favorite](#add-a-view-as-a-favorite) - not possible yet-->
* [共用檢視](#share-a-view)

## 表格和時間表檢視之間的異同

下表顯示Maestro中的表格檢視與時間表檢視之間的異同：

<!--some of these are NOT available right now; if you make this public, comment out the ones not there-->

| 功能 | 表格檢視 | 時間表檢視 |
|-----------------------------------------------------------------------|------------|---------------|
| 在清單或表格中顯示記錄 | ✓ (A) |              |
| 預設將所有欄位顯示為表格中的欄 | ✓ (A) |              |
| 隱藏或顯示欄位 | ✓ (A) |               |
| 編輯每個記錄的欄位值 | ✓ (A) |               |
| 在檢視中將記錄新增為新列 | ✓ (A) |               |
| 在檢視中新增欄位作為新欄 | ✓ (A) |               |
| 從外部清單複製列並將它們貼到表格中 | ✓ (A) |               |
| 在時間軸中顯示記錄 |            | ✓ (A) |
| 篩選記錄 | ✓ (A) | ✓ (A) |
| 群組記錄 | ✓ (A) | ✓ (A) |
| 排序記錄 | ✓ (A) |              |
| 色彩代碼記錄 |           | ✓ (A) |
| Color-code分組 |           | ✓ (A) |
| 搜尋特定記錄 | ✓ (A) | ✓ (A) |
| 共用檢視 | ✓ (A) | ✓ (A) |
| 從檢視開啟記錄的「詳細資訊」頁面 | ✓ (A) | ✓ (A) |

## 建立或編輯檢視 {#create-or-edit-views}

{{step1-to-maestro}}


您上次存取的工作區預設會開啟。 如需有關建立工作區的資訊，請參閱 [建立工作區](../architecture/create-workspaces.md).
1. 按一下記錄型別卡。 如需有關建立記錄型別的資訊，請參閱 [建立記錄型別](../architecture/create-record-types.md).

   依預設，選取型別的所有記錄都會顯示在表格檢視中。

1. 按一下 **檢視** 下拉式功能表，並選取現有的 **表格檢視** ![](assets/table-view-icon.png) 或按一下 **建立檢視>表格** 建立表格檢視

   或

   選取現有 **時間表檢視** ![](assets/timeline-view-icon.png) 檢視或按一下 **建立檢視>時間表** 以建立時間表檢視。

   ![](assets/view-types-drop-down-from-record-type-list.png)

   >[!NOTE]
   >
   >    若要建立時間表檢視，您為其建立檢視的記錄型別必須至少有兩個日期欄位。 否則，「時間軸」選項會變暗。

1. （可選）更新檢視的名稱，然後按一下 **建立** 以儲存。

   依預設，Maestro會將檢視命名為「表格&lt;數字>」或「時間軸&lt;數字>」。 數字是自動產生的增量。

1. （選擇性）若要在建立檢視後重新命名，請按一下檢視下拉式功能表，然後按一下 **更多** 功能表 ![](assets/more-menu.png) > **重新命名** 以更新檢視名稱。 <!--ensure there is not another saving step here?!-->
1. （可選）若要管理特定型別的檢視，請參閱下列文章：

   * [管理表格檢視](../views/manage-the-table-view.md)
   * [管理時間表檢視](../views/manage-the-timeline-view.md)


## 刪除檢視

{{step1-to-maestro}}

您上次存取的工作區預設會開啟。 如需有關建立工作區的資訊，請參閱 [建立工作區](../architecture/create-workspaces.md).

1. 按一下記錄型別卡。

   如需有關建立記錄型別的資訊，請參閱 [建立記錄型別](../architecture/create-record-types.md).

   依預設，選取型別的所有記錄都會顯示在表格檢視中。

1. 按一下「檢視」下拉式功能表，將滑鼠停留在清單中的其中一個檢視上，然後按一下 **更多** 功能表 ![](assets/more-menu.png) > **刪除**.
1. 按一下 **刪除** 以確認。 <!--ensure there is not another saving step here?!-->

   所有可以存取Maestro區域的使用者都將刪除該檢視，且無法復原該檢視。

## 共用檢視

如需關於共用檢視的資訊，請參閱 [共用檢視](/help/quicksilver/maestro/access/share-views.md).

<!--## Add a view as a favorite - this is not possible yet-->

<!--not possible yet - August 30, 2023: 

## Duplicate views

If you want to keep multiple versions of a view and make slight changes between the version, you can duplicate a view. Duplicating a view creates identical copies of an existing view. 

1. From the **Main Menu**, click **Maestro**. 
    The workspace you last accessed opens by default. For information about creating workspaces, see [Create workspaces](../architecture/create-workspaces.md).
1. Click a record type. For information about creating a record type, see [Create record types](../architecture/create-record-types.md). 

    By default, all the records of the type selected display in the table view. 

1. Click the view drop-down menu, then click the **More** menu ![](assets/more-menu.png) to the right of the view name > **Duplicate**. (**********ensure there is not another saving step here?! also, add how this view is named; the button to duplicate was there but not the functionality yet************)
    
    The view is duplicated and visible to all users who can access the Maestro area. 

-->
