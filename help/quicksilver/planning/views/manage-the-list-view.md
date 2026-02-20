---
title: 在Adobe Workfront規劃中管理清單檢視
description: 在Adobe Workfront Planning中，存取記錄之「連線記錄」頁面中的物件時，您可以在清單檢視中顯示物件及其欄位。 本文說明如何在記錄的「連線記錄」頁面中建立或編輯清單檢視。
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 1c7e6973-6e9e-4c93-9d3b-89ed90df9d14
source-git-commit: a5f33f914dabaa9368dea919510375bcb6ee03e2
workflow-type: tm+mt
source-wordcount: '1001'
ht-degree: 0%

---


# 在Adobe Workfront Planning中管理清單檢視

<!--<span class="preview">The information highlighted on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

在Adobe Workfront Planning中，存取記錄之「連線記錄」頁面中的物件時，您可以在清單檢視中顯示物件及其欄位。

本文說明如何在記錄的「連線記錄」頁面中建立或編輯清單檢視，以及如何編輯檢視中的物件。

## 存取權要求

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
   <td role="rowheader"><p>Adobe Workfront 封裝</p></td> 
   <td> 
<p>任何Workfront和任何Planning套件</p>
<p>任何工作流程與任何Planning套件</p>
<p>如需每個Workfront Planning套件所含內容的詳細資訊，請聯絡您的Workfront客戶代表。 </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront授權</p></td> 
   <td><p> 建立和刪除檢視的標準</p>
   <p>更新檢視元素的投稿人或更新者</p>
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

如需Workfront存取需求的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++ 

## 關於清單檢視的考量事項

* 您無法在清單檢視中檢視記錄型別頁面中的記錄。 當您在記錄的「連線的記錄」頁面中檢視下列物件時，只能在清單檢視中顯示這些物件：

   * Workfront專案

  如需有關建立連線記錄頁面的資訊，請參閱[新增連線記錄頁面至記錄](/help/quicksilver/planning/records/add-a-connected-records-page-to-a-record.md)。
* 您必須先將Workfront專案與Planning記錄型別連線，才能在記錄的已連線記錄頁面中檢視清單檢視。 如需詳細資訊，請參閱[連線記錄型別](/help/quicksilver/planning/architecture/connect-record-types.md)。
* 清單檢視類似於增強型清單。 如需詳細資訊，請參閱[使用增強型清單](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md)。


## 管理清單檢視 {#manage-a-list-view}

如需在Workfront中管理清單檢視的詳細資訊，請參閱[使用增強型清單](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md)。

{{step1-to-planning}}

1. 按一下工作區卡片，然後按一下記錄型別卡片。
1. 從任何檢視中，按一下記錄名稱以開啟記錄的預覽或詳細資訊頁面。
1. 依照文章&#x200B;**新增連線的記錄頁面**&#x200B;中的說明，為連線的專案新增[連線的記錄頁面](/help/quicksilver/planning/records/add-a-connected-records-page-to-a-record.md)。

   「連線的記錄」頁面會顯示清單檢視中連線至記錄的專案。

   <!--add new screen shot when they release Row colors/ special formatting for rows-->

   在清單檢視中![連線記錄頁面上的專案](assets/projects-on-connected-records-page-list-view.png)

1. （選擇性）執行下列任一項作業來修改清單檢視：

   1. 展開清單右上角的下拉式檢視功能表，以選取其他檢視，或按一下&#x200B;**新增檢視**&#x200B;並建立另一個檢視。

      檢視會在整個系統中共用。 如果您為一個記錄型別建立「專案」檢視，則可以在顯示已連線專案的其他記錄型別上檢視它。

   1. 將滑鼠停留在現有檢視的名稱上，然後按一下&#x200B;**更多**&#x200B;功能表![更多](assets/more-menu.png)，然後按一下下列其中一項：
      * **重新命名**，為檢視提供新名稱
      * **共用**，與其他人共用檢視
      * **刪除**，以刪除檢視。

      >[!NOTE]
      >
      >* 您必須擁有檢視的管理許可權才能編輯、共用或刪除檢視。
      >
      >* 您無法修改系統檢視。
      >
      <!--* <span class="preview">You can reset a view that was shared with you after you modified it to restore its original preferences, or you can copy it with your changes and share the copy. For more information, see [Use enhanced lists](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md). </span>
        -->
   1. 按一下&#x200B;**篩選器**&#x200B;圖示![篩選器圖示](assets/filter-icon.png)將篩選器新增至檢視。 結果會立即在清單中篩選。 您無法儲存並命名篩選器。 日後存取頁面時會記住篩選器，這些篩選器也是共用檢視的一部分。
   1. 按一下&#x200B;**欄**&#x200B;圖示![欄圖示](assets/columns-icon.png)以選取要在檢視中顯示或隱藏的欄。
   1. 暫留在欄名稱上，然後按一下欄名稱左側的向下箭頭，然後按一下下列其中一項：
      * **重新命名**，為資料行新增&#x200B;**自訂標籤**。 Workfront中原始欄位的名稱不會變更。
      * **排序**，依選取的欄位排序清單。 表示排序方向的排序圖示會新增至欄標題。
   1. 按一下清單右上角的&#x200B;**+**&#x200B;圖示，新增或移除清單中的欄，然後按一下&#x200B;**儲存**。

      **資料行管理員**&#x200B;開啟。

      您只能將現有欄位新增到清單檢視。
您不能移除在第一欄顯示的清單檢視中的主要欄位。


   <!--
    1. <span class="preview">Click **Row colors** <!-insert icon and edit the name of the icon if they changed it->. The **Format** box opens. <!-change the name of the box when they update it-></span>
        <span class="preview">Do the following: </span>
        <div class="preview">
        1. Define the formatting conditions in the **If** area by clicking **Add condition**, then select a field you want to format by and choose a field value. 
            >[!TIP]
            >
            >Only field visible in the list view are available for conditional formatting.
        1. (Optional) Click **Add condition** in the If area to add more conditions. 
        1. Click the **Or** connector between conditions to change to **And**. **Or** is the default connector.  
        1. In the **Format** area, select a field to indicate which column will be formatted. <!-edit this area, if it changes names???->
        1. Click on the color circle to expand and choose another color.
        1. Turn on the **Apply to row** setting to apply the formatting to the entire row that meets the conditions. 
        1. (Optional) Click **Clear all** to remove all formatting.
            The formatting is applies immediately.
        1. Click outside the **Format** box to close it. 
            This returns you to the list view. There is a blue dot next to the **Row colors** icon to indicate that the view has special formatting applied. <!-might need to edit the icon name and get a screen shot of the icon with the dot and insert it here->
        </div>
    -->

1. （可選）在清單右上角的搜尋方塊中新增關鍵字，以搜尋專案。


   符合搜尋字詞的專案會在清單中反白顯示。
1. （選擇性）若要新增更多專案至清單，並自動將其連線至選取的記錄，請執行下列其中一項作業：

   * 按一下清單右上角的&#x200B;**連線記錄**&#x200B;以新增現有專案。
   * 按一下清單底部的&#x200B;**新列**&#x200B;以新增專案。
1. 按一下清單中連線專案的名稱，以在其他瀏覽器標籤中開啟它。
1. 在清單的儲存格內按兩下以編輯欄位的資訊，然後按下Enter以儲存變更。

   有些欄位是唯讀的。 例如，專案的完成百分比是由系統計算的欄位，您無法手動進行編輯。

1. 將滑鼠懸停在清單中專案的名稱上，然後按一下&#x200B;**更多**&#x200B;功能表[更多](assets/more-menu.png)，然後按一下&#x200B;**檢視**&#x200B;以在另一個索引標籤中開啟專案

   或

   選取一或多個專案，並注意清單底部的動作列，然後按一下下列其中一項：

   * **刪除**&#x200B;以刪除專案。 刪除專案會中斷專案與記錄的連線，並將其移至Workfront的「資源回收筒」。 Workfront管理員可在刪除已刪除的專案後30天內復原這些專案。
   * **中斷連線**&#x200B;以中斷專案與記錄的連線。 中斷專案的連線會從目前記錄中移除該專案及其查閱欄位的所有值。

   連線記錄頁面清單檢視中的![動作列](assets/actions-bar-connected-records-page-list-view.png)

