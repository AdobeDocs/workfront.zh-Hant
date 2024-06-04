---
title: 管理表格檢視
description: 存取Adobe Workfront Planning中的記錄型別頁面時，您可以在表格檢視中顯示記錄及其欄位。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 0dd723b5-d674-4626-8fc2-7da41f3b7f35
source-git-commit: 6c50746c4c230d7f9fa2c73b66d13c8b02153b89
workflow-type: tm+mt
source-wordcount: '2394'
ht-degree: 3%

---

# 管理表格檢視

<!--
title: Manage the table view
description: You can display records in a table view when using Adobe Workfront Planning. 
hidefromtoc: yes
author: Alina
feature: Work Management
role: User
hide: yes
-->

<!--update the metadata with real information when making this available in TOC and in the left nav-->

{{planning-important-intro}}

存取Adobe Workfront Planning中的記錄型別頁面時，您可以在表格檢視中顯示記錄及其欄位。

如需有關記錄檢視以及如何管理檢視的資訊，請參閱 [管理記錄檢視](/help/quicksilver/planning/views/manage-record-views.md).

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
   <td> <p>AdobeWorkfront計畫沒有存取層級控制項</p>  
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

## 管理表格檢視 {#manage-a-table-view}

<!--insert screen shot of table view-->

建立表格檢視時，選取型別的所有記錄都會顯示在表格中。 每一列都是唯一的記錄，每一欄都是一個記錄欄位。 預設會顯示所有欄位和所有記錄。

若要管理表格檢視：

1. 建立表格檢視，如文章所述 [管理記錄檢視](/help/quicksilver/planning/views/manage-record-views.md).

   ![](assets/table-view-example.png)

1. （選用）按一下 **列高**，然後從下列選項中選取，以修改表格列的高度：
   * 短
   * 中
   * 高

1. 更新下列檢視元素，如下列子區段所述：
   * [欄（或欄位）](#add-columns-or-fields)
   * [列（或記錄）](#add-rows-or-records)
   * [篩選器](#add-filters)
   * [分組](#add-groupings)
   * [排序](#add-a-sort)


### 新增欄（或欄位） {#add-columns}

表格檢視的欄標題會顯示與檢視中記錄相關聯的欄位。 表格檢視中顯示的相同欄位也會顯示在記錄的「詳細資訊」區段中。 如需詳細資訊，請參閱 [編輯記錄](/help/quicksilver/planning/records/edit-records.md).

<!--this is not available yet:You can display record fields (or columns) in both a table and a timeline view. However, the number of columns displayed in the table of the timeline view is limited and you cannot add columns in addition to those selected by default.-->

將欄新增至檢視與將欄位新增至記錄型別相同。

您可以在表格檢視中新增最多500個欄位（或欄）。

1. 移至記錄型別頁面並選取 **表格** 從「檢視」下拉式選單中檢視。

   <!-- replace above with this when view redesign: Go to a record type page and click a table view tab, or click **+ View **to add a new view, then choose **Table**. -->
1. 開始新增欄位（或欄），如文章所述 [建立欄位](/help/quicksilver/planning/fields/create-fields.md).

   您新增的欄對存取記錄型別的所有使用者可見，並作為記錄頁面的新欄位新增。

1. 執行下列任一項作業，重新排序表格中的欄：

   * 抓取欄標題，並將其拖放到所需位置。 您移動的欄會短暫地以藍色背景顯示，直到您對表格進行其他調整為止。

   * 按一下 **欄位** 在表格工具列中，依所需順序拖放欄位，然後按一下 **欄位可見度和順序** 方塊以關閉它。

     ![](assets/fields-setting-table-view-toolbar-expanded.png)


     >[!TIP]
     >
     >* 依預設，「名稱」欄位永遠是表格檢視中的第一個欄位。 系統會將此視為主要欄位。
     >
     >* 除非您指定其他欄位作為主要欄位，否則您無法將「名稱」欄位移至其他位置。 如需詳細資訊，請繼續進行步驟4。 <!--accurate?-->
     >
     >* 您無法隱藏或刪除主要欄位。
     >
     >* 主要欄位已凍結，不是水準捲動的一部分。

   * 變更主要欄位，以其他欄位取代第一欄中的欄位。 如需詳細資訊，請繼續步驟4。 <!--accurate?-->

1. （選擇性）將滑鼠游標停留在任何未顯示在表格第一欄之欄位的欄位標題中，按一下欄位名稱右側的向下箭頭，然後按一下 **設為主要欄位**.

   ![](assets/set-as-primary-field-option-table-view.png)

1. 按一下 **設定欄位** 以確認。

   該欄位會變成主要欄位，表示它會顯示為表格檢視的第一欄。 前一個主要欄位會移至第二欄。

   >[!NOTE]
   >
   >   * 只有下列型別的欄位才能為主要欄位：
   >
   >       * 單行文字
   >       * 數字
   >       * 公式
   >
   >   * 主要欄位一律凍結且無法移動。 如果需要將主要欄位移至其他位置，您可以選取其他欄位來取代主要欄位。
   >
   >   * 變更表格檢視中的主要欄位會影響其他所有選擇檢視的使用者的檢視。
   >
   >   * 變更表格檢視中的主要欄位會影響所有表格檢視。
   >
   >   * 您無法刪除或隱藏主要欄位。
   >
   >   * 主要欄位中列出的值一律會以超連結方式連結至記錄的頁面。

1. 按一下並拖曳欄分隔線，並將它們拖曳到所需的位置以增加欄寬。

   >[!TIP]
   >
   >您對欄寬和順序所做的變更是永久性的，並且所有存取該記錄型別的使用者都可以看到。

1. 將游標停留在欄標題上，按一下向下箭頭，然後按一下 **隱藏欄位**

   或

   按一下 **欄位** ，並停用與您要隱藏的欄位或欄位相關聯的切換。 此 **欄位可見度和順序** 方塊隨即顯示。

   >[!TIP]
   >
   >隱藏欄位數會顯示在工具列的「欄位」圖示左側。


1. 按一下 **欄位** 圖示並啟用與您要顯示在表格欄位中的欄位相關聯的切換。 預設會顯示所有欄位。

1. 執行下列動作以快速尋找符合關鍵字的記錄：

   1. 按一下 **搜尋** 圖示 ![](assets/search-icon.png) 並開始輸入與畫面上所顯示之記錄的任何欄位相關聯的關鍵字。 正確相符的數目會顯示在搜尋專案旁邊，而具有正確相符專案的欄位會反白顯示。

      ![](assets/search-box-with-results-blue-outline-table-view.png)

      您可以使用熒幕上可見的任何文字或特殊字元。

      您無法使用與表格檢視中隱藏之欄位關聯的關鍵字。

   1. 按下 **輸入** 前往下一個找到的欄位。

   1. （選擇性）如果有多個相符專案，請按一下搜尋關鍵字右邊的向上和向下箭頭，以尋找表格中的所有相符專案。

   1. 按一下 **x** 圖示來清除搜尋關鍵字。


### 新增列（或記錄） {#add-rows}

表格檢視的列會顯示所選記錄型別的個別記錄。

記錄型別最多可以有50,000筆記錄（或列）。

1. 移至記錄型別頁面並選取 **表格** 從「檢視」下拉式選單中檢視。

<!-- replace above with this when view redesign: Go to a record type page and click a table view tab, or click **+ View **to add a new view, then choose **Table**. -->
1. 開始新增記錄（或列），如文章所述 [建立記錄](/help/quicksilver/planning/records/create-records.md).

   您在表格檢視中新增的記錄會立即儲存，且所有擁有工作區檢視或更高許可權的使用者皆可看到。

1. （可選）新增縮圖至每筆記錄，然後按一下 **欄位** 在表格的右上角，然後選取 **縮圖** 欄位，在主欄位左側顯示。 預設會取消選取它。

   如需詳細資訊，請參閱 [新增縮圖至記錄](/help/quicksilver/planning/records/add-thumbnails-to-records.md).

1. （選擇性）選取一列中的一或多個記錄，然後拖放 **控點** 圖示 ![](assets/handle-icon.png) 記錄名稱左側，以重新排序列。

   >[!NOTE]
   >
   >如果您對表格檢視至少套用一種排序，則無法重新排序列。

   <!-- this is not possible right now:

    1. To reorder the rows, click the row header, drag and drop it in the desired location. 

        The changes you make to the row order are permanent and visible to all users who access the record type
    -->

<!-- this section below links from the timeline view; consider splitting them if they become different-->

### 新增篩選器 {#add-filters}

篩選器可協助您減少熒幕上顯示的資訊量。

在表格檢視中使用篩選器時，請考量下列事項：
<!-- this list is almost identical to the one for the table view - update both-->

* 您為表格檢視建立的篩選器在套用至相同記錄型別時，會與時間軸檢視中的篩選器分開運作。

* 這些篩選器對於您選取的檢視而言是唯一的。 相同記錄型別的兩個表格檢視可以套用不同的篩選器。 檢視相同表格檢視的兩個使用者會看到目前套用的相同篩選器。

* 您無法為您建立並套用至表格檢視的篩選器命名。

* 移除篩選器會將其從存取與您相同記錄型別的任何人中移除，並使用與您使用的相同檢視。

* 將濾鏡新增至表格檢視與將濾鏡新增至時間軸檢視相同。

* 您可以依已連線的記錄欄位或查詢欄位進行篩選，但不能針對允許連結至多個記錄的欄位進行篩選。

若要將篩選器新增至表格檢視：

1. 建立記錄型別頁面的表格檢視，如文章所述 [管理記錄檢視](/help/quicksilver/planning/views/manage-record-views.md).
1. 選取表格檢視，然後按一下 **篩選器** 在表格的右上角。
1. 按一下 **新增條件** 並新增下列資訊：

   * 選取您要作為篩選依據的欄位 <!-- the tip below might change-->

   * 選取選項（或篩選修飾元）以定義欄位必須符合何種條件

     下表顯示每種欄位型別的可用修飾元。

     <table>
        <thead>
        <tr>
            <th><b>欄位類型</b></th>
            <th><b>修飾元</b></th>
        </tr>
        </thead>
        <tbody>
        <tr>
            <td>單行，段落，公式 </td>
            <td><p>包含</p>
            <p>不包含</p>
            <p>是</p>
            <p>不是</p>
            <p>是空的</p>
            <p>不是空的</p></td>
        </tr>
        <tr><td>單選</td>
            <td><p>是</p>
            <p>不是</p>
            <p>屬於任一</p>
            <p>不屬於</p>
            <p>是空的</p>
            <p>不是空的</p></td>
        </tr>
        <tr>
            <td>多選，人員</td>
            <td><p>具有任一</p>
            <p>具有所有</p>
            <p>完全符合</p>
            <p>不具有</p>
            <p>是空的</p>
            <p>不是空的</p></td>
        </tr>
        <tr>
            <td>數字、百分比、貨幣</td>
            <td><p>=</p>
            <p>≠</p>
            <p> &lt; </p>
            <p>&gt;</p>
            <p>≤</p>
            <p>≥</p>
            <p>是空的</p>
            <p>不是空的</p></td>
        </tr>
        <tr>
            <td>日期</td>
            <td><p>是</p>
            <p>不是</p>
            <p>晚於</p>
            <p>早於</p>
            <p>介於</p><p>不介於</p>
            <p>是空的</p><p>不是空的</p></td>
        </tr>

     <tr>
            <td>核取方塊</td>
            <td><p>是</p>
        </tr>
        </tbody>
        </table>

   * 選取所選欄位的值。

   ![](assets/filter-ui-table-view.png)

   您可以新增的篩選條件數量沒有限制。

1. （選用）按一下 **新增條件** 以新增另一個篩選選項，並重複上述步驟。 套用的篩選器數會顯示在「篩選器」圖示的左側。
1. 按一下下列運運算元，指示如何聯結及套用篩選條件：

   * **與**：必須符合所有指定的條件。
   * **或**：必須符合任何指定的條件。 這是預設選項。

   系統會自動篩選記錄清單。  <!--at this time, you can't name and save the filter - but will this change?!-->
   <!-- asked on the task for the simple filters whether there is a limitation for how many statements a filter can have?!-->

1. （選用）按一下 **篩選器**，然後按一下 **x** 圖示以移除篩選器。 <!--right now you cannot "clear all" for filters, but this might come later-->

### 新增群組 {#add-groupings}

<!--this section exists in the timeline view too, but the display is slightly different, so I kept both steps; consider updating both sections if any updates to groupings are introduced-->

將群組套用至檢視時，您可以依照類似的資訊來群組記錄。

在表格檢視中新增群組，類似於在時間軸檢視中新增群組。

請考量下列事項：

* 您可以在表格和時間軸檢視中套用群組。 表格檢視的分組與相同記錄型別之時間軸檢視中的群組是獨立的。
* 您可以在檢視中套用3個群組層級。 記錄會依照您選取的群組順序進行分組。
&lt;!—*使用API時，您最多可以套用4個層級的群組。  — 現在正在檢查此專案 — >
* 群組對於您選取的檢視而言是唯一的。 相同記錄型別的兩個表格檢視可以套用不同的群組。 檢視相同表格檢視的兩個使用者會看到目前套用的相同分組。
* 您無法為表格檢視建立的分組命名。
* 移除群組會將群組從存取與您相同記錄型別以及顯示與您相同檢視的任何人中移除。
* 您可以編輯列在群組下的記錄。
* 您可以依已連線的記錄欄位或查詢欄位來分組，但不能針對允許連結至多個記錄的欄位進行分組。
<!--checking into this: * You can apply up to 4 levels of grouping when using the API. -->
<!-- checking also into this: * You cannot group by a Paragraph-type field.-->

若要新增群組：

1. 如文章所述，為記錄型別建立時間表檢視 [管理記錄檢視](/help/quicksilver/planning/views/manage-record-views.md).
1. 按一下 **分組** 表格檢視的右上角。

   ![](assets/grouping-ui-table-view-with-linked-fields.png)

1. 按一下其中一個建議欄位，或按一下 **選擇其他欄位**，搜尋其他欄位，然後在清單中顯示時按一下該欄位。

   此分組會自動套用至表格，且記錄會顯示在分組分隔行下方。

1. （可選）重複上述步驟以新增最多3個群組。

   為分組選取的欄位數會顯示在「分組」圖示旁。

   ![](assets/grouping-applied-in-table-view.png)

1. （選用）內部 **記錄分組依據** 方塊中，按一下 **x** 圖示在選取要移除分組的欄位右側

   或

   按一下 **全部清除** 以移除所有欄位。

1. 按一下 **記錄分組依據** 方塊以關閉它。
1. （選用）按一下 **+新增&lt;記錄型別名稱>** 在任何群組結束時新增記錄，然後重新整理您的頁面以將新記錄新增到適當的群組。 <!--this might need to be changed when they add the Refresh button on the toolbar of the table view-->

### 新增排序 {#sort-information}

透過套用排序，您可以依指定順序組織資訊。

您可以排序下列資訊：

* 表格檢視中的所有記錄。 <!--or timeline view. ***********verify this is the case for the timeline view*********************-->
  <!--* All groupings. - this is not available yet-->

在表格檢視中排序記錄時，請考量下列事項：

<!-- if this is available for the timeline view, update both when you update one-->

* 排序對您選取的檢視而言是唯一的。 相同記錄型別的兩個表格檢視可套用不同的排序標準。 檢視相同表格檢視的兩個使用者會看到目前套用的相同排序。

* 您無法命名您建置並套用至表格檢視的排序。

* 當您導覽到其他位置時，您建立的排序會保留。

* 您可以依顯示在記錄型別表格檢視中的欄位數量來排序。

* 僅當連結欄位允許單一值，或允許選取了彙總選項（總和、平均、最大值、最小值）的多重選取值時，連結欄位才可排序。

* 移除排序標準會將它們從存取與您相同記錄型別的任何人中移除，並使用與您使用的相同檢視。

* 您可以依已連線的記錄欄位或查詢欄位排序，但不能針對允許連結至多個記錄的欄位進行排序。

排序 <!--ungrouped (add this when sorting for groupings will be available--> 記錄，請執行下列動作：

1. 建立表格檢視，如文章所述 [管理記錄檢視](/help/quicksilver/planning/views/manage-record-views.md).
1. 按一下 **排序** 圖示 ![](assets/sort-icon.png) 在表格的右上角

   或

   暫留在表格檢視中的欄名稱上，按一下欄標題名稱右側的向下箭頭，然後按一下 **依此欄位排序**. 欄位會在表格檢視右上角的「排序」圖示中新增為排序選取專案。

1. 在 **記錄排序依據** 方塊中，按一下其中一個建議的欄位，或按一下 **選擇其他欄位** 並搜尋其他欄位，然後在清單中顯示時按一下該欄位。

   排序會自動套用至表格檢視，且記錄會依您選取的條件排序。

   <!-- add a step that you can rearrange the sorting fields here, when this will be possible-->

1. （選用）重複上述步驟，依其他欄位排序。

   排序依據的欄位數會顯示在工具列右上角的「排序」圖示左側。 您只能選擇顯示在表格檢視欄中的欄位。

1. （選用）在 **記錄排序依據** 方塊中，按一下 **x** 圖示在排序欄位右側以移除排序

   或

   按一下 **全部清除** 以移除排序中的所有欄位。

1. 按一下 **記錄排序依據** 方塊以關閉它。

   ![](assets/sorting-in-table-view.png)

   表格中顯示的資訊會根據您選取的條件排序。

   為排序選取的欄位會顯示排序圖示，後面跟著數字，表示套用排序的順序。

<!-- this is not available yet: 

To sort grouped records: 

1. Create a view, as described in [Create or edit record views](#create-or-edit-record-views). 
1. ************************* add steps here for sorting grouped records****************

-->
