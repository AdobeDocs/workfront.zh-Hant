---
title: 管理表格檢視
description: 存取Adobe Maestro中的記錄型別頁面時，您可以在表格檢視中顯示記錄及其欄位。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 0dd723b5-d674-4626-8fc2-7da41f3b7f35
source-git-commit: 7614652b57c57e1176dfb48058f890fd4e5c942e
workflow-type: tm+mt
source-wordcount: '1687'
ht-degree: 4%

---

# 管理表格檢視

<!--
title: Manage the table view
description: You can display records in a table view when using Adobe Maestro. 
hidefromtoc: yes
author: Alina
feature: Work Management
role: User
hide: yes
-->

<!--update the metadata with real information when making this available in TOC and in the left nav-->

>[!IMPORTANT]
>
>目前，Adobe大師是測試版計畫的一部分，向有限數量的客戶開放。
>
>如需加入Maestro測試版計畫的詳細資訊，請聯絡您的客戶代表。
>
>如需詳細資訊，請參閱 [Adobe大師概觀](../maestro-overview.md).

存取Adobe Maestro中的記錄型別頁面時，您可以在表格檢視中顯示記錄及其欄位。

有關Maestro檢視以及如何管理檢視的資訊，請參閱 [管理記錄檢視](../views/manage-record-views.md).

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

## 管理表格檢視 {#manage-a-table-view}

<!--insert screen shot of table view-->

建立表格檢視時，選取型別的所有記錄都會顯示在表格中。 每一列都是唯一的記錄，每一欄都是一個記錄欄位。 預設會顯示所有欄位和所有記錄。

若要管理表格檢視：

1. 建立表格檢視，如文章所述 [管理記錄檢視](../views/manage-record-views.md).

   ![](assets/table-view-example.png)

1. 更新下列檢視元素，如下列子區段所述：
   * [欄（或欄位）](#add-columns-or-fields)
   * [列（或記錄）](#add-rows-or-records)
   * [篩選器](#add-filters)
   * [分組](#add-groupings)
   * [排序](#sort-information)


### 新增欄（或欄位） {#add-columns}

Maestro表格檢視的欄標題會顯示與檢視中記錄相關聯的欄位。 表格檢視中顯示的相同欄位也會顯示在Maestro記錄的「詳細資訊」區段中。 如需詳細資訊，請參閱 [編輯記錄](../records/edit-records.md).

<!-- this is not available yet:You can display record fields (or columns) in both a table and a timeline view. However, the number of columns displayed in the table of the timeline view is limited and you cannot add columns in addition to those selected by default. -->

將欄新增至檢視與將欄位新增至記錄型別相同。

您可以在表格檢視中新增最多500個欄位（或欄）。

1. 移至記錄型別頁面並選取 **表格** 從「檢視」下拉式選單中檢視。
1. 開始新增欄位（或欄），如文章所述 [建立欄位](../architecture-and-fields/create-fields.md).

   您新增的欄對存取記錄型別的所有使用者可見，並作為新欄位新增到所選記錄型別的記錄的「詳細資訊」頁面上。

1. 執行下列任一項作業，重新排序表格中的欄：

   * 抓取欄標題，並將其拖放到所需位置。 您移動的欄會短暫地以藍色背景顯示，直到您對表格進行其他調整為止。

   * 按一下 **欄位** 在表格工具列中，依所需順序拖放欄位，然後按一下 **欄位可見度和順序方塊** 以關閉它。

     ![](assets/fields-setting-table-view-toolbar-expanded.png)

   >[!TIP]
   >
   >* [名稱]欄位永遠是表格檢視中的第一個欄位。
   >
   >* 您無法將「名稱」欄位移至其他位置。
   >
   >* 您無法隱藏「名稱」欄位。
   >
   >* 「名稱」欄位已凍結，且不是水準捲動的一部分。

1. 按一下並拖曳欄分隔線，並將它們拖曳到所需的位置以增加欄寬。

   >[!TIP]
   >
   >您對欄寬和順序所做的變更是永久性的，並且所有存取該記錄型別的使用者都可以看到。

1. 將游標停留在欄標題上，按一下向下箭頭，然後按一下 **隱藏欄位**

   或

   按一下 **欄位** ，並停用與您要隱藏的欄位或欄位相關聯的切換。

   >[!TIP]
   >
   >隱藏欄位數會顯示在工具列的「欄位」圖示左側。


1. 按一下 **欄位** 設定並啟用與您要顯示在表格欄位中的欄位相關聯的切換按鈕。 預設會顯示所有欄位。

1. 執行下列動作以快速尋找符合關鍵字的記錄：

   1. 按一下 **搜尋** 圖示 ![](assets/search-icon.png) 並開始輸入與畫面上所顯示之記錄的任何欄位相關聯的關鍵字。 正確相符的數目會顯示在搜尋專案旁邊，而具有正確相符專案的欄位會以藍色反白顯示。

      您可以使用熒幕上可見的任何文字或特殊字元。

      您無法使用與表格檢視中隱藏之欄位關聯的關鍵字。

      ![](assets/search-box-with-results-blue-outline-table-view.png)

   1. （選擇性）如果有多個相符專案，請按一下搜尋關鍵字右邊的向上和向下箭頭，以尋找表格中的所有相符專案。

   1. 按一下 **X** 圖示來清除搜尋關鍵字。


### 新增列（或記錄） {#add-rows}

Maestro表格檢視的列會顯示所選記錄型別的個別記錄。

在Maestro中，記錄型別最多可以有10,000筆記錄（或列）。

1. 移至記錄型別頁面並選取 **表格** 從「檢視」下拉式選單中檢視。
1. 開始新增記錄（或列），如文章所述 [建立記錄](../records/create-records.md).

   您在表格檢視中新增的記錄會立即儲存，並且所有存取Maestro的使用者都能看到。 <!--this will change with permissions-->

1. （選擇性）選取一列中的一或多個記錄，然後拖放 **控點** 圖示 ![](assets/handle-icon.png) 記錄名稱左側，以重新排序列。

   >[!NOTE]
   >
   >如果您對表格檢視至少套用一種排序，則無法重新排序列。

<!-- this is not possible right now:

1. To reorder the rows, click the row header, drag and drop it in the desired location. 

    The changes you make to the row order are permanent and visible to all users who access the record type
-->

### 新增篩選器 {#add-filters}

<!-- this section links from the timeline view; consider splitting them if they become different-->

篩選器可協助您減少熒幕上顯示的資訊量。

在表格檢視中使用篩選器時，請考量下列事項：
<!-- this list is almost identical to the one for the table view - update both-->

* 您為表格檢視建立的篩選器在套用至相同記錄型別時，會與時間軸檢視中的篩選器分開運作。

* 這些篩選器對於您選取的檢視而言是唯一的。 相同記錄型別的兩個表格檢視可以套用不同的篩選器。 檢視相同表格檢視的兩個使用者會看到目前套用的相同篩選器。

* 您無法為您建立並套用至表格檢視的篩選器命名。

* 移除篩選器會將其從存取與您相同記錄型別的任何人中移除，並使用與您使用的相同檢視。

* 將濾鏡新增至表格檢視與將濾鏡新增至時間軸檢視相同。

若要將篩選器新增至表格檢視：

1. 建立記錄型別頁面的表格檢視，如文章所述 [管理記錄檢視](../views/manage-record-views.md).
1. 選取表格檢視，然後按一下 **篩選器** 在表格的右上角。
1. 按一下 **新增條件** 並新增下列資訊：

   * 選取您要作為篩選依據的欄位 <!-- the tip below might change-->

   * 選取選項（或篩選修飾元）以定義欄位必須符合何種條件

     下表顯示每種欄位型別的可用修飾元。

     >[!TIP]
     >
     > 您無法選取連結的欄位。 如需詳細資訊，請參閱 [建立欄位](../architecture-and-fields/create-fields.md).

     <table>
        <thead>
        <tr>
            <th><b>欄位類型</b></th>
            <th><b>修飾元</b></th>
        </tr>
        </thead>
        <tbody>
        <tr>
            <td>單行，段落 </td>
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
            <td>多選</td>
            <td><p>具有任一</p>
            <p>具有所有</p>
            <p>完全符合</p>
            <p>不具有</p>
            <p>是空的</p>
            <p>不是空的</p></td>
        </tr>
        <tr>
            <td>數值，百分比，貨幣</td>
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

<!-- this is not available yet

### Add groupings {#add-groupings}

*******************this section might link in the future from the timeline view; right now it's only documented there; also, check the steps below because this was not released to the table when they were written*****************

You can group records by similar information when applying  a grouping to a view.

You can apply groupings both in the table and timeline views. The groupings of the table view are independent from those in the timeline view of the same record type. 

Consider the following:

* You can apply 3 levels of grouping in a Maestro view. The records are grouped in the order of groupings that you select. (***************check on this; this might be true for timeline, but not for table??? One dev said in a demo that there are unlimited groupings in a table - check *********************)
* You can apply up to 4 levels of grouping when using the API. 

To add a grouping:

1. Create a view, as described in [Create or edit record views](#create-or-edit-record-views). 
1. (Conditional) To apply a grouping in the table view, do the following:
    
    1. ***************start adding steps for building a grouping - see if there it a global setting or just per column; also, see if the steps are different for a table vs a timeline view?!**********************
1. (Conditional) To apply a grouping in the timeline view, do the following:

    1. Go to a timeline view, then click **Group**. ************************did they rename this to "Grouping"?!****************************
        ******************insert screen shot***********
    1. Click one of the 5 suggested fields, or click **Choose a different field** to display all fields, then click one when it displays in the list. 
    
        >[!TIP]
        >
        > You cannot select linked fields. For information, see [Create fields](../architecture-and-fields/create-fields.md).  
    The grouping is applied automatically to the timeline and records display inside the grouping box.    <********************ensure this is correct functionality here*************
    
    1. (Optional) Click **Add grouping** to add up to 3 groupings. 

        The number of groupings applied displays to the left of the Grouping icon in the upper-right corner of the toolbar. **********ensure this says "grouping" and not "group"*****************
    
    1. (Optional) Click **Clear all** to remove all groupings.  

-->

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

* 移除排序標準會將它們從存取與您相同記錄型別的任何人中移除，並使用與您使用的相同檢視。

排序 <!--ungrouped (add this when sorting for groupings will be available--> 記錄，請執行下列動作：

1. 建立表格檢視，如文章所述 [管理記錄檢視](../views/manage-record-views.md).
1. 按一下 **排序** 圖示 ![](assets/sort-icon.png) 在表格的右上角

   或

   暫留在表格檢視中的欄名稱上，按一下欄標題名稱右側的向下箭頭，然後按一下 **依此欄位排序**. 欄位會在表格檢視右上角的「排序」圖示中新增為排序選取專案。
1. 在 **記錄排序依據** 方塊中，按一下其中一個建議的欄位，或按一下 **選擇其他欄位** 並搜尋其他欄位，然後在清單中顯示時按一下該欄位。

   排序會自動套用至表格檢視，且記錄會依您選取的條件排序。

   <!-- add a step that you can rearrange the sorting fields here, when this will be possible-->

1. （選用）重複上述步驟，依其他欄位排序。

   排序依據的欄位數會顯示在工具列右上角的「排序」圖示左側。 您只能選擇顯示在表格檢視欄中的欄位。

   >[!TIP]
   >
   > 您無法選取連結的欄位。 如需詳細資訊，請參閱 [建立欄位](../architecture-and-fields/create-fields.md).

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
