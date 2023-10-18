---
title: 管理時間表檢視
description: 存取Adobe Maestro中的記錄型別頁面時，您可以在時間軸檢視中顯示記錄。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: f348af7f-5bb9-4d88-9bcb-3bef7e8892dd
source-git-commit: b02c81873d84946f8db54bcf9a1a464de38781de
workflow-type: tm+mt
source-wordcount: '1093'
ht-degree: 1%

---

# 管理時間表檢視

<!--
title: Manage the timeline view in Adobe Maestro
description: You can display records in a timeline view, when accessing the record type page in Adobe Maestro. 
hidefromtoc: yes
hide: yes
author: Alina
feature: Work Management
role: User
-->

<!--update the metadata with real information when making this available in TOC and in the left nav-->

>[!IMPORTANT]
>
>本文資訊是指Adobe Maestro，這是Adobe的新產品。
>
>目前，Adobe大師是測試版計畫的一部分，向有限數量的客戶開放。
>
>如需加入Maestro測試版計畫的詳細資訊，請聯絡您的客戶代表。
>
>如需詳細資訊，請參閱 [Adobe大師概觀](../maestro-overview.md).

存取Adobe Maestro中的記錄型別頁面時，您可以在時間軸檢視中顯示記錄。

如需Maestro檢視的相關資訊，請參閱 [在Adobe大師中管理記錄檢視](../views/manage-record-views.md).

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto">
 <col>
 <tbody>
<td>
   <p> Adobe產品</p> </td>
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
   <td role="rowheader">存取層級</td>
   <td> <p>任何</p>  
</td>
  </tr>
<tr>
   <td role="rowheader">版面配置範本</td>
   <td> <p>您的系統管理員必須在您的版面配置範本中新增Maestro區域。 如需詳細資訊，請參閱 <a href="../access/grant-access.md">授與Adobe大師的存取權</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->

## 管理時間表檢視 {#manage-a-timeline-view}

<!--insert screen shot of timeline view-->

建立時間表檢視時，所選記錄型別的所有記錄都會以時間順序時間表顯示。

請考量下列事項：

* 您至少有兩個日期欄位與記錄型別相關聯時，才能建立時間表檢視。 當您有一個或沒有與記錄型別相關聯的日期欄位時，時間軸檢視選項會變暗。
* 根據與記錄關聯的日期，在下列情況下，某些記錄可能不會顯示在時間軸檢視中：

   * 當開始和結束日期沒有值時
   * 當「開始」或「結束」日期沒有值時
   * 當開始日期在結束日期之後時

<!--these are NOT available now because there won't be a table for the timeline view for the near future, per Andy: 
* The records displayed in the timeline view also display in a view-only table to the left of the timeline. 
* Each row in the table and each bar on the timeline represent the same record. 
* Each column in the table is a record field. The columns of this table are preconfigured and cannot be customized. 
* Only a limited number of fields (or columns) display in the timeline view table. 
* You cannot do the following in a timeline view:
     * Add rows or records
     * Add columns or fields
     * Edit record information
-->

建立時間軸檢視時，依預設，所選記錄型別的所有記錄都會在時間軸中顯示為長條。

若要管理時間表檢視：

1. 移至您要檢視其時間軸的記錄型別頁面。
1. 建立時間表檢視，如文章所述 [管理記錄檢視](../views/manage-record-views.md).

   ![](assets/timeline-view-example.png)

   與您選取的記錄型別相關聯的記錄會以時間軸的方式顯示為長條。

1. 執行下列任一項作業來瀏覽時間軸：

   * 按一下左右圖示，或使用水準捲動在時間軸中前後移動。
   * 按一下 **今天** 將時間軸置中到今天的日期。
   * 從時間範圍下拉式選單中選取下列其中一個選項，以更新時間增量：

      * 年
      * 季度
      * 月
1. 按一下 **切換至標準** 檢視以個別行顯示記錄 <!--check to see if they updated the name of the setting here-->

   或

   按一下 **切換至精簡檢視** 顯示日期在同一行上不相交的記錄。 <!--check to see if they updated the name of the setting here-->

   預設情況下，記錄會顯示在「壓縮」檢視中。

1. 更新下列檢視元素，如下列子區段所述：
   * [篩選器](#add-filters)
   * [分組](#add-grouping)
     <!--* [Sort](#add-sort) not sure if this is present in timeline views?!; also check the anchor and make sure it's correct-->
   * [設定](#edit-the-timeline-view-settings)

### 新增篩選器

篩選器可協助您減少熒幕上顯示的資訊量。

在時間軸檢視中使用篩選器時，請考量下列事項：

<!-- this list is almost identical to the one for the table view - update both-->

* 您為時間軸檢視建立的篩選器套用至相同記錄型別時，會與表格檢視中的篩選器分開運作。

* 這些篩選器對於您選取的檢視而言是唯一的。 相同記錄型別的兩個時間軸檢視可以套用不同的篩選器。 檢視相同時間表檢視的兩個使用者會看到目前套用的相同篩選器。

* 您無法為您建立並套用至時間表檢視的篩選器命名。

* 移除篩選器會將其從存取與您相同記錄型別的任何人中移除，並使用與您使用的相同檢視。

在時間軸檢視中新增濾鏡，與在表格檢視中新增濾鏡相同。

如需詳細資訊，請參閱文章中的「新增篩選器」一節 [管理表格檢視](../views/manage-the-table-view.md).

### 新增分組

<!-- if groupings are identical between the table and the timeline, consider replacing this section with this: 

Adding groupings in the timeline view is identical to adding filters in the table view. 

For more information, see the "Add filters" section in the article [Manage the table view](../views/manage-the-table-view.md). -->


將群組套用至檢視時，您可以依照類似的資訊來群組記錄。

在時間軸檢視中使用群組時，請考量下列事項：

* 您可以在表格和時間軸檢視中套用群組。 表格檢視的分組與相同記錄型別之時間軸檢視中的群組是獨立的。
* 您可以在Maestro檢視中套用3個群組層級。 記錄會依照您選取的群組順序進行分組。
* 使用API時，您最多可以套用4個層級的群組。

若要新增群組：

1. 建立時間表檢視，如文章所述 [管理記錄檢視](../views/manage-record-views.md).
1. 按一下 **分組**.

   ![](assets/grouping-ui-timeline-view.png)

1. 按一下其中一個建議欄位，或按一下 **選擇其他欄位** 並搜尋其他欄位，然後在清單中顯示時按一下該欄位。

   >[!TIP]
   >
   >您無法選取連結的欄位。

   分組會自動套用至時間軸，且記錄會顯示在分組方塊內。 分組中的專案數會顯示在分組行上。

   <!-- add a step that you can rearrange the groupings here, when this will be possible-->

1. （可選）重複上述步驟以新增最多3個群組。

   套用的分組數會顯示在工具列右上角「分組」圖示的左側。

   ![](assets/grouping-applied-in-timeline-view.png)

1. （可選）按一下 **x** 圖示在群組右側以移除群組

   或

   按一下 **全部清除** 以移除所有群組。

1. 按一下 **記錄分組依據** 方塊以關閉它。

<!-- 

### Add sort

this is not possible right now; if this is the same functionality as the table view, document it there and link from here. 

-->

### 編輯時間軸檢視設定 {#edit-the-timeline-view-settings}

更新時間軸檢視設定，以指示檢視的時間軸區段中顯示哪些資訊。

1. 建立時間表檢視，如文章所述 [管理記錄檢視](../views/manage-record-views.md).
1. 按一下 **設定**.
1. 按一下 **日期和時間** 在左側面板中，然後選取 **開始日期** 和 **結束日期** 以在時間軸上顯示。 您可以選擇預設的「開始」和「結束」日期，也可以選擇任何可用的日期欄位。 代表記錄的長條圖，其開始日期為您為「開始」日期指定的日期，結束日期為您與「結束」日期對應的日期。

   >[!NOTE]
   >
   >    沒有開始或結束日期值或開始日期晚於結束日期的記錄不會顯示在時間軸檢視中。


1. 按一下 **記錄詳細資料** 以指示您要在記錄欄位上顯示的欄位。

   依預設，會選取「名稱」欄位。

1. 按一下 **新增欄位** 以新增最多4個欄位到記錄列。
1. 按一下 **搜尋欄位** 方塊，然後按一下您要新增的欄位。

   >[!TIP]
   >
   >   * 您必須先建立欄位，才能將其新增到記錄列。
   > 
   >   * 您必須至少選取一個欄位。 **名稱** 預設為選取。

   右側會顯示時間軸上長條圖的外觀。

   ![](assets/record-details-panel-timeline-settings-with-preview.png)

1. 按一下&#x200B;**儲存**。

   記錄會以您所選取的規格顯示在時間軸檢視中。
