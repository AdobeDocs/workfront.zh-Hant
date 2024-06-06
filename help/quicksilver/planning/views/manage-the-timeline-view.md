---
title: 管理時間表檢視
description: 存取Adobe Workfront Planning中的記錄型別頁面時，您可以在時間軸檢視中顯示記錄。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: f348af7f-5bb9-4d88-9bcb-3bef7e8892dd
source-git-commit: a923d86f78e6dab4705289a8165c4b31ff68b5a2
workflow-type: tm+mt
source-wordcount: '1724'
ht-degree: 0%

---

# 管理時間表檢視

<!--
title: Manage the timeline view 
description: You can display records in a timeline view, when accessing the record type page in Adobe Workfront Planning. 
hidefromtoc: yes
hide: yes
author: Alina
feature: Work Management
role: User
-->

<!--update the metadata with real information when making this available in TOC and in the left nav-->

{{planning-important-intro}}

存取Adobe Workfront Planning中的記錄型別頁面時，您可以在時間軸檢視中顯示記錄。

如需有關記錄檢視的資訊，請參閱 [管理記錄檢視](/help/quicksilver/planning/views/manage-record-views.md).

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
   <td role="rowheader"><p>Adobe Workfront授權</p></td>
   <td>
   <p>任何</p> 
   <p>系統管理員只能存取他們建立或與他們共用的檢視。 </p>
  </td>
  </tr>

<tr>
   <td role="rowheader">存取層級設定</td>
   <td> <p>Adobe Workfront Planning沒有存取層級控制 </p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>權限</p></td>
   <td> <p>管理檢視的許可權</p>  
</td>
  </tr>

<tr>
   <td role="rowheader">版面配置範本</td>
   <td> <p>您的系統管理員必須在版面配置範本中新增Planning區域。 如需詳細資訊，請參閱 <a href="/help/quicksilver/planning/access/access-overview.md">存取權總覽</a>. </p>  
</td>
  </tr>
 </tbody>
</table>


## 管理時間表檢視 {#manage-a-timeline-view}

<!--insert screen shot of timeline view-->

建立時間表檢視時，所選記錄型別的所有記錄都會以時間順序時間表顯示。

請考量下列事項：

* 您至少有兩個日期欄位與記錄型別相關聯時，才能建立時間表檢視。 當您有一個或沒有與記錄型別相關聯的日期欄位時，時間軸檢視選項會變暗。

  您可以從記錄日期欄位中選取，或從連線的記錄或物件型別中查詢日期欄位。
* 根據與記錄關聯的日期，在下列情況下，某些記錄可能不會顯示在時間軸檢視中：

   * 當開始和結束日期沒有值時
   * 當「開始」或「結束」日期沒有值時
   * 當開始日期在結束日期之後時

若要管理時間表檢視：

1. 移至您要檢視其時間軸的記錄型別頁面。
1. 建立時間表檢視，如文章所述 [管理記錄檢視](/help/quicksilver/planning/views/manage-record-views.md).

   ![](assets/timeline-view-example.png)

   與您選取的記錄型別相關聯的記錄會在時間軸中顯示為長條，並依其開始日期的時間順序依預設排序。

   >[!TIP]
   >
   >    時間軸中記錄的排序在壓縮檢視中不可見。


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

1. 執行下列動作以快速尋找符合關鍵字的記錄：

   1. 按一下 **搜尋** 圖示 ![](assets/search-icon.png) 並開始輸入與畫面上所顯示之記錄的任何欄位相關聯的關鍵字。 正確相符的數目會顯示在搜尋專案旁邊，而具有正確相符專案的記錄會反白顯示。

      ![](assets/search-box-and-results-timeline-view.png)

      您可以使用熒幕上可見的任何文字或特殊字元。

      您無法使用與未顯示在時間表檢視中的欄位關聯的關鍵字。

   1. 在鍵盤上按Enter鍵以移至下一個找到的欄位。
   1. （選擇性）如果有多個相符專案，請按一下搜尋關鍵字右邊的向上和向下箭頭，以尋找表格中的所有相符專案。
   1. 按一下 **x** 圖示來清除搜尋關鍵字。

1. 更新下列檢視元素，如下列子區段所述：
   * [篩選器](#add-filters)
   * [分組](#add-grouping)
   * [設定](#edit-the-timeline-view-settings)
     <!--* [Sort](#add-sort) not sure if this is present in timeline views?!; also check the anchor and make sure it's correct-->

### 新增篩選器

您可以使用篩選器來減少熒幕上顯示的資訊量。

在時間軸檢視中使用篩選器時，請考量下列事項：

<!-- this list is almost identical to the one for the table view - update both-->

* 您為時間軸檢視建立的篩選器與套用至相同記錄型別之任何其他檢視中的篩選器是獨立運作的。

* 這些篩選器對於您選取的檢視而言是唯一的。 相同記錄型別的兩個時間軸檢視可以套用不同的篩選器。

* 檢視相同時間表檢視的兩個使用者會看到目前套用的相同篩選器。

* 您無法為您為時間表檢視建置的篩選器命名。

* 移除篩選器會將篩選器從存取與您相同記錄型別以及顯示與您相同檢視的任何人移除。

* 在時間軸檢視中新增濾鏡，與在表格檢視中新增濾鏡相同。

  如需詳細資訊，請參閱文章中的「新增篩選器」一節 [管理表格檢視](/help/quicksilver/planning/views/manage-the-table-view.md).

* 您可以依已連線的記錄欄位或查詢欄位進行篩選，但不能針對允許連結至多個記錄的欄位進行篩選。

### 新增分組

<!-- groupings are almost identical between this view and table  but they display a little differently, so I kept the steps for both; update in both places if they make changes to groupings-->

將群組套用至檢視時，您可以依照類似的資訊來群組記錄。

在時間軸檢視中新增群組，類似於在表格檢視中新增群組。

在時間軸檢視中使用群組時，請考量下列事項：

* 您可以在表格和時間軸檢視中套用群組。 表格檢視的分組與相同記錄型別之時間軸檢視中的群組是獨立的。
* 您可以在檢視中套用3個群組層級。 記錄會依照您選取的群組順序進行分組。
* 使用API時，您最多可以套用4個層級的群組。
* 群組對於您選取的檢視而言是唯一的。 相同記錄型別的兩個時間軸檢視可套用不同的群組。 檢視相同時間表檢視的兩個使用者會看到目前套用的相同分組。
* 您無法為時間表檢視建立的分組命名。
* 移除群組會將群組從存取與您相同記錄型別以及顯示與您相同檢視的任何人中移除。
* 您可以依已連線的記錄欄位或查詢欄位來分組，但不能針對允許連結至多個記錄的欄位進行分組。

若要在時間表檢視中新增群組：

1. 如文章所述，為記錄型別建立時間表檢視 [管理記錄檢視](/help/quicksilver/planning/views/manage-record-views.md).
1. 按一下 **分組** 位於時間軸檢視的右上角。

   ![](assets/grouping-ui-timeline-view-with-linked-fields.png)

1. 按一下其中一個建議欄位，或按一下 **選擇其他欄位**，搜尋其他欄位，然後在清單中顯示時按一下該欄位。

   分組會自動套用至時間軸，且記錄會顯示在分組方塊內。

   <!-- add a step that you can rearrange the groupings here, when this will be possible-->

1. （可選）重複上述步驟以新增最多3個群組。

   為分組選取的欄位數會顯示在「分組」圖示旁。

   <!-- update screen shot with view redesign-->

   ![](assets/grouping-applied-in-timeline-view.png)

1. （選用）內部 **記錄分組依據** 方塊中，按一下 **x** 圖示在選取要移除分組的欄位右側

   或

   按一下 **全部清除** 以移除所有欄位。

1. 按一下 **記錄分組依據** 方塊以關閉它。
1. （選用）按一下 **設定**，然後 **顏色** 至色彩程式碼群組。 如需詳細資訊，請參閱 [編輯時間軸檢視設定](#edit-the-timeline-view-settings) 一節。

<!-- 

### Add sort

this is not possible right now; if this is the same functionality as the table view, document it there and link from here. 

-->

### 編輯時間軸檢視設定 {#edit-the-timeline-view-settings}

更新時間軸檢視設定，以指示要在檢視的時間軸區段中顯示哪些資訊及顯示方式。

1. 如文章所述，為記錄型別建立時間表檢視 [管理記錄檢視](/help/quicksilver/planning/views/manage-record-views.md).
1. 按一下 **設定**.
1. 按一下 **日期和時間** 在左側面板中，然後選取 **開始日期** 和 **結束日期** 以在時間軸上顯示。 您可以選擇預設的「開始」和「結束」日期，也可以選擇任何可用的日期欄位。 代表記錄的長條圖，其開始日期為您為「開始」日期指定的日期，結束日期為您與「結束」日期對應的日期。

   >[!NOTE]
   >
   >沒有開始或結束日期值或開始日期晚於結束日期的記錄不會顯示在時間軸檢視中。

1. 按一下 **橫條樣式** 在左側面板中，指定您要在記錄列上顯示的欄位。

   依預設，會選取「名稱」欄位。 <!--adjust this when the primary field is released??-->

1. （選擇性和條件性）如果您將縮圖新增至記錄，請選取「縮圖」選項，以顯示與其記錄列中的記錄相關聯的影像。

   >[!NOTE]
   >
   >    您必須先在表格檢視中新增縮圖，才能在時間軸檢視中顯示它們。 如需詳細資訊，請參閱 [新增縮圖至記錄](/help/quicksilver/planning/records/add-thumbnails-to-records.md).

1. 按一下 **新增欄位** 以新增最多4個欄位到記錄列。
1. 按一下 **搜尋欄位** 方塊，然後按一下您要新增的欄位。

   >[!TIP]
   >
   >   * 您必須先建立欄位，才能將其新增到記錄列。
   > 
   >   * 您必須至少選取一個欄位。 **名稱** 預設為選取。

   右側會顯示時間軸上長條圖的外觀。

   ![](assets/record-details-panel-timeline-settings-with-preview.png)

1. 按一下 **顏色** 在左側面板中，自訂時間軸中記錄和群組的顏色。

   ![](assets/color-tab-timeline-view.png)

1. （條件式與選擇性）如果您將群組新增至時間軸檢視，請從下列選項中選取，以設定群組中的顏色 **設定群組顏色** 區段：

   * **預設（灰色）**：群組的顏色會設定為灰色。 這是預設值。
   * **欄位值**：分組的顏色符合您分組依據的欄位顏色。
您只能將群組的顏色與具有顏色編碼選項的欄位配對。

   例如，多選或單選欄位可以有顏色編碼的選項。

   如果您依據沒有顏色編碼選項的欄位分組，則分組顏色保持灰色。

   >[!TIP]
   >
   >如果您未將群組新增至時間軸檢視，則不會顯示此區段。

1. 在 **設定記錄顏色** 區段中，從下列選項中選取，以設定記錄的顏色：

   * **記錄型別**：記錄的顏色符合您選取的記錄型別的顏色。 這是預設選項。
   * **欄位值**：記錄的顏色與您指定的欄位顏色相符。 繼續進行步驟10。 <!--ensure this stays accurate-->
   * **分組**：記錄的顏色符合您為分組指定的顏色。 當您未將群組套用到時間軸檢視時，此選項會變暗。
   * **無**：記錄會以白色列顯示。

1. （視條件而定）如果您已選取 **欄位值** 對於記錄顏色，從 **比對記錄顏色** 下拉式功能表。

   ![](assets/field-selector-drop-down-menu-timeline-view.png)

   下拉式選單中只會顯示具有色彩編碼選項的欄位。

   例如，多選或單選欄位可以有顏色編碼的選項。

   如果選取的記錄型別沒有包含顏色編碼選項的欄位，則此選項會變暗。

1. 按一下「**儲存**」。

   記錄會以您所選取的規格顯示在時間軸檢視中。
