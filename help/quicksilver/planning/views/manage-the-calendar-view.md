---
title: 管理行事曆檢視
description: 您可以在行事曆檢視中顯示記錄及其欄位。 本文說明如何建立行事曆檢視，以及如何編輯或刪除現有檢視。
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 45b5be81-703c-45d5-a08c-60cb8ec5b103
source-git-commit: 5b9b1f397c76afa2e2ae550e0ce62a6038b8bd86
workflow-type: tm+mt
source-wordcount: '1895'
ht-degree: 4%

---

# 管理行事曆檢視

<span class="preview">本頁醒目提示的資訊指出尚未普遍可用的功能。 它僅在預覽環境中可供所有客戶使用。 每月發行至生產環境後，生產環境中為啟用快速發行的客戶也提供相同的功能。</span>

<span class="preview">如需快速發行資訊，請參閱[為您的組織啟用或停用快速發行](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>

{{planning-important-intro}}

您可以從記錄型別頁面，在行事曆檢視中顯示記錄及其欄位。

如需Adobe Workfront Planning檢視的詳細資訊及管理方式，請參閱[管理記錄檢視](/help/quicksilver/planning/views/manage-record-views.md)。

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
<ul><li>選擇</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>舊版Workfront計畫不提供Workfront計畫</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront規劃套件*</p></td> 
   <td> 
<p>任何 </p> 
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
    <td role="rowheader"><p>Adobe Workfront授權*</p></td> 
   <td><p> 建立和刪除檢視的標準</p>
   <p>更新檢視元素的投稿人或更新者</p>
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
   <td>   <p>管理檢視的許可權</p>  
   <p>檢視許可權以暫時變更檢視設定或複製檢視</p> </td> 
  </tr> 
<tr>
   <td role="rowheader"><p>版面配置範本</p></td>
   <td> 必須為具有輕度或貢獻者授權的使用者指派包含Planning的版面配置範本。
   <p>標準使用者和系統管理員預設會啟用Planning區域。</p></div></li></ul>
</td>
  </tr>

</tbody> 
</table>

*如需Workfront存取需求的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++   

## 管理行事曆檢視 {#manage-a-calendar-view}

<!--insert screen shot of calendar view-->

請考量下列事項：

* 只有當您至少有兩個日期欄位與記錄型別相關聯時，才能建立「行事曆」檢視。 當您有一個或沒有與記錄型別相關聯的日期欄位時，「行事曆」檢視選項會變暗。

  您可以從記錄日期欄位中選取，或從連線的記錄或物件型別中查詢日期欄位。
* 存在下列情況：

   * 當「開始」與「結束」日期都沒有值時，記錄不會顯示在行事曆上
   * 當「開始」或「結束」日期沒有值時，記錄會顯示為單日事件
   * 當開始日期晚於結束日期時，記錄不會顯示在行事曆上。

若要管理行事曆檢視：

1. 移至您要檢視其行事曆的記錄型別頁面。
1. 建立行事曆檢視，如文章[管理記錄檢視](/help/quicksilver/planning/views/manage-record-views.md)中所述。

   ![行事曆檢視範例](assets/calendar-view-example.png)

   與您選取的記錄型別相關聯的記錄會在行事曆中顯示為長條。 依預設，長條的顏色與記錄圖示的顏色相符。

1. 執行下列任一項作業來瀏覽行事曆：

   * 按一下日曆左上角的左右圖示，或使用水準捲動在日曆中前後移動。
   * 按一下右上角的&#x200B;**今天**，將行事曆置中到今天的日期。
   * 從時間範圍下拉式選單中選取下列其中一個選項，以更新時間增量：

      * **月**：記錄會顯示在每月行事曆中。

      * **周**：記錄會顯示在下列區域中：

         * 橫跨多天的記錄會顯示在行事曆的頂端。
         * 持續一天或更短的記錄，會顯示在行事曆檢視的下半部分。 如果您選取顯示開始與結束日期的小時，則記錄會在記錄發生的當天的適當時間顯示。

1. <span class="preview">（選擇性）按一下&#x200B;**全熒幕**&#x200B;圖示![開啟全熒幕圖示](assets/open-full-screen-icon.png)以全熒幕開啟檢視，然後按一下&#x200B;**退出全熒幕**&#x200B;圖示![退出全熒幕圖示](assets/exit-full-screen-icon.png)或鍵盤上的Escape以退出全熒幕。 </span>

1. <span class="preview">若要在行事曆檢視中建立記錄或編輯其日期，請執行下列其中一個動作：</span>

   * <span class="preview">連按兩下行事曆上的任何位置以建立記錄。</span>

     <span class="preview">如需詳細資訊，請參閱[建立記錄](/help/quicksilver/planning/records/create-records.md)。</span>

   * <span class="preview">按一下記錄列的左邊界或右邊界，然後將其拖放到新位置。 調整記錄列的大小會立即更新其開始或結束日期。</span>

   * <span class="preview">拖放記錄列以更新其位置和日期。 移動記錄列會立即更新其開始和結束日期。</span>

     <span class="preview">如需詳細資訊，請參閱[編輯記錄](/help/quicksilver/planning/records/edit-records.md)。</span>

1. 更新下列檢視元素，如下列子區段所述：
   * [篩選器](#add-filters)
   * <span class="preview">[資料列高度](#modify-row-height)</span>
   * [設定](#edit-the-calendar-view-settings)

   <!--* [Grouping](#add-grouping)-->
   <!--* [Sort](#add-sort) not sure if this is present in calendar views?!; also check the anchor and make sure it's correct-->

### 新增篩選器

您可以使用篩選器來減少熒幕上顯示的資訊量。

在行事曆檢視中使用篩選器時，請考慮下列事項：

<!-- this list is almost identical to the one for the table view - update both-->

* 您為行事曆檢視建立的篩選器與套用至相同記錄型別之任何其他檢視中的篩選器分開運作。

* 這些篩選器對於您選取的檢視而言是唯一的。 相同記錄型別的兩個行事曆檢視可以套用不同的篩選器。

* 檢視相同行事曆檢視的兩個使用者會看到目前套用的相同篩選器。

* 您無法命名您為行事曆檢視建立的篩選器。

* 移除篩選器會將篩選器從存取與您相同記錄型別以及顯示與您相同檢視的任何人移除。

* 您可以依已連線的記錄欄位或查詢欄位進行篩選。

* 您可以依顯示多個值的查閱欄位進行篩選。

若要將篩選器新增至行事曆檢視：

1. 建立記錄型別頁面的行事曆檢視，如文章[管理記錄檢視](/help/quicksilver/planning/views/manage-record-views.md)中所述。
1. 選取行事曆檢視，然後按一下行事曆工具列中的&#x200B;**篩選器**。
1. 按一下&#x200B;**新增條件**&#x200B;並新增下列資訊：

   * **選取您要依**&#x200B;篩選的欄位<!-- the tip below might change-->

   * **選取選項** （或篩選修飾元）以定義欄位必須符合何種條件

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

   ![篩選器UI資料表檢視](assets/filter-ui-table-view.png)

   您可以新增的篩選條件數量沒有限制。

1. （選擇性）按一下&#x200B;**新增條件**&#x200B;以新增另一個篩選選項，並重複上述步驟。 套用的篩選器數會顯示在「篩選器」圖示的左側。
1. 按一下下列運運算元，指示如何聯結及套用篩選條件：

   * **AND**：必須符合所有指定的條件。
   * **OR**：必須符合任何指定的條件。 這是預設選項。

   1. （選用）在多個條件群組之間新增其他&#x200B;**AND**&#x200B;或&#x200B;**OR**&#x200B;運運算元。

      ![檢視中的多重層級篩選器](assets/multi-tiered-filters-in-views.png)

   系統會自動篩選記錄清單。 <!--at this time, you can't name and save the filter - but will this change?!-->
   <!-- asked on the task for the simple filters whether there is a limitation for how many statements a filter can have?!-->

1. （選擇性）按一下&#x200B;**x**&#x200B;圖示以移除篩選條件。
1. （選擇性）按一下&#x200B;**篩選器**&#x200B;以關閉篩選器方塊。<!--right now you cannot "clear all" for filters, but this might come later-->

<span class="preview">

### 修改列高

您可以修改行事曆儲存格的列高，以增加或減少您在每個儲存格中顯示的記錄列數目。

行事曆中顯示的記錄數會依您在記錄列上顯示的欄位數目而有所不同。

>[!TIP]
>
>此設定僅在依月份檢視行事曆時可用。


1. 建立記錄型別頁面的行事曆檢視，如文章[管理記錄檢視](/help/quicksilver/planning/views/manage-record-views.md)中所述。
1. （視條件而定）依月份顯示行事曆檢視，然後按一下行事曆工具列中的&#x200B;**列高**。
1. 從下列選項中選擇：

   <table>
    <thead>
    <tr>
        <th><b>列高選項</b></th>
        <th><b>預設最大記錄數</b></th>
    </tr>
    </thead>
    <tbody>
    <tr>
        <td>短</td>
        <td><p>包含：</p>

   <ul><li>2筆記錄顯示1個欄位</li>
    <li>顯示超過1個欄位的1筆記錄</li></ul>
        </td>
    </tr>
    <tr><td>標準</td>
        <td><p>包含：</p>

   <ul><li>4個記錄顯示1個欄位</li>
    <li>顯示超過1個欄位的2筆記錄</li></ul>
        </td>
    </tr>
    <tr>
        <td>媒體</td>
        <td><p>包含：</p>

   <ul><li>8筆記錄顯示1個欄位</li>
    <li>顯示超過1個欄位的4筆記錄</li></ul>
        </td>
    </tr>
    <tr>
        <td>高</td>
        <td><p>包含：</p>

   <ul><li>顯示1個欄位的12筆記錄</li>
    <li>顯示超過1個欄位的6筆記錄</li></ul>
        </td>
    </tr>
    <tr>
        <td>符合內容</td>
        <td><p>所有記錄皆可見，最多500筆記錄</p></td>
    </tr>
    </tbody>
    </table>

1. （選擇性）如果行事曆中有看不見的記錄，請按一下&#x200B;**更多**。

</span>

### 編輯行事曆檢視設定

更新行事曆檢視設定以指示檢視中顯示的資訊和方式。

1. 建立記錄型別的行事曆檢視，如文章[管理記錄檢視](/help/quicksilver/planning/views/manage-record-views.md)中所述。
1. 按一下&#x200B;**設定**。
1. 按一下左側面板中的&#x200B;**日期和時間**，然後選取要在行事曆上顯示的&#x200B;**開始日期**&#x200B;和&#x200B;**結束日期**。 您可以選擇預設的「開始」和「結束」日期，也可以選擇任何可用的日期欄位。

   代表記錄的長條圖，其開始日期為您為「開始」日期指定的日期，結束日期為您與「結束」日期對應的日期。

   >[!NOTE]
   >
   >* 沒有開始或結束日期值或開始日期晚於結束日期的記錄不會顯示在行事曆檢視中。
   >
   >* 如果您使用「劃分」選項顯示其他記錄，則「開始」與「結束」日期為主要記錄的日期。 您無法在此區域選擇連線記錄的「開始」和「結束」日期。

1. 按一下左側面板中的&#x200B;**長條樣式**，以指示您要在記錄長條上顯示的資訊。

   預設會選取記錄的主要欄位（或標題），如記錄的表格檢視中所定義。
   <!--adjust this when the primary field is released??-->

1. （選擇性和條件性）如果您在記錄中新增縮圖，請選取&#x200B;**縮圖**&#x200B;選項，以顯示與其記錄列中的記錄相關聯的影像。

   >[!NOTE]
   >
   >    您必須先在表格檢視中新增縮圖，才能在行事曆檢視中顯示它們。 如需詳細資訊，請參閱[新增縮圖至記錄](/help/quicksilver/planning/records/add-thumbnails-to-records.md)。

1. 按一下&#x200B;**新增欄位**，然後按一下&#x200B;**搜尋欄位**&#x200B;方塊內部，再按一下您要新增的欄位。

   >[!TIP]
   >
   >   * 您必須先建立欄位，才能將其新增到記錄列。
   > 
   >   * 您必須至少選取一個欄位。 預設會選取&#x200B;**名稱**。
   >
   >   * 您最多可以新增5個欄位。

   右邊顯示的行事曆上長條圖預覽。

   行事曆檢視設定中的![長條樣式區段](assets/bar-style-section-in-calendar-view-settings-with-preview.png)

1. 按一下左側面板中的&#x200B;**色彩**，以自訂行事曆上記錄的色彩。

   行事曆檢視設定上的![顏色面板](assets/color-panel-on-calendar-view-settings.png)

1. 在&#x200B;**將記錄顏色設定為**&#x200B;區段中，從下列選項中選取，以設定記錄的顏色：

   * **記錄型別**：行事曆中記錄列的色彩符合您選取的記錄型別。 這是預設選項。
   * **欄位值**：記錄的顏色符合您指定的欄位顏色。
   * **無**：記錄以白色列顯示。

1. （視條件而定）如果您為記錄顏色選取&#x200B;**欄位值**，請從&#x200B;**將記錄顏色與**&#x200B;下拉式功能表中選取欄位。

   ![行事曆檢視的欄位選擇器下拉式功能表](assets/field-selector-drop-down-menu-calendar-view.png)

   下拉式選單中只會顯示具有色彩編碼選項的欄位。

   例如，多選或單選欄位可以有顏色編碼的選項。

   如果選取的記錄型別沒有包含顏色編碼選項的欄位，則此選項會變暗。


1. 按一下「**儲存**」。

   記錄會以您所選取的規格顯示在行事曆檢視中。