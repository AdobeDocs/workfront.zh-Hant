---
title: 新增連線的記錄頁面至記錄
description: 您可以將「連線記錄」頁面的索引標籤新增至記錄，以檢視連線記錄或物件的資訊。 這會將表格檢視中的連線記錄新增至索引標籤。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
source-git-commit: 1f1db1c9184a6a8a2abcd3139e4e4e61d2f08bc4
workflow-type: tm+mt
source-wordcount: '1139'
ht-degree: 1%

---


# 將「連線的記錄」頁面新增至記錄

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

您可以將「連線記錄」頁面的索引標籤新增至記錄，以檢視連線記錄或物件的資訊。 這會將表格檢視中的連線記錄新增至索引標籤。

將「連線的記錄」頁面新增至記錄時，請考量下列事項：

* 從記錄型別的表格檢視中，將記錄或物件型別連線至記錄型別後，您可以將「已連線的記錄」頁面新增至記錄。

* 您可以從記錄的預覽區域或記錄的頁面新增「連線記錄」頁面。

* 「連線的記錄」頁面在表格檢視中只會顯示連線的物件或來自一個物件或記錄型別的記錄。 頁面不會顯示該型別的所有記錄。

* 您可以為下列連線記錄或物件型別新增「連線記錄」頁面：

   * Workfront Planning記錄型別
   * Workfront專案、方案、投資組合、群組或公司。 即使您沒有在Workfront中存取Workfront物件的許可權，仍可檢視連線物件。

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
<td> 
   <p> 其他產品</p> </td> 
   <td> 
   <p> 除了Adobe Workfront之外，如果您想要從下列應用程式為物件新增連線的記錄頁面，也必須具備下列專案：</p>
   <ul><li><p>Adobe Experience Manager Assets授權及AEM Assets與Workfront之間的整合，用於連結AEM資產與Planning記錄型別。</p>
   <p>如需詳細資訊，請參閱<a href="/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/workfront-for-aem-asset-essentials.md">適用於Experience Manager Assets和Assets Essentials的Adobe Workfront：文章索引</a>。 </p></li>
   <li><p> 連線記錄型別與GenStudio Brands的Adobe GenStudio for Performance Marketing授權</p>
   <p>如需詳細資訊，請參閱<a href="https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/get-started">開始使用Adobe GenStudio for Performance Marketing</a>。</p></li></ul>
   </td> 
  </tr>

<tr> 
   <td role="rowheader"><p>Adobe Workfront授權</p></td> 
   <td><p>標準</p>
   </td> 
  </tr> 
  <tr>
   <td role="rowheader"><p>物件許可權</p></td>
   <td>
   <p>貢獻或更高的許可權到工作區和記錄型別 </p>  
   <p>系統管理員擁有所有工作區的許可權，包括他們未建立的工作區</p> 
  </td>
  </tr>   
</tbody> 
</table>

如需Workfront存取需求的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++   


## 將「連線的記錄」頁面新增至記錄

1. 按一下記錄名稱，從記錄型別頁面的任何檢視中開啟記錄。
1. 從下列其中一個區域按一下&#x200B;**新增頁面**：

   * 記錄的預覽視窗
   * 記錄的詳細資訊頁面，在按一下預覽頁面右上角的&#x200B;**在新索引標籤中開啟**&#x200B;圖示![在新索引標籤中開啟詳細資訊](assets/open-details-in-a-new-tab-icon.png)之後。

   **建立頁面**&#x200B;方塊開啟。

   ![新增連線記錄頁面模組](assets/add-connection-view-page-modal.png)

1. 新增&#x200B;**頁面名稱**，按一下&#x200B;**連線記錄頁面**，然後按一下&#x200B;**建立**。

   新的連線記錄頁面會新增為記錄頁面的新索引標籤。

   連線至目前記錄的記錄會顯示在表格檢視中。

   >[!TIP]
   >
   >您必須先在記錄的表格或「詳細資訊」區域中新增連線的記錄，才能在連線的記錄頁面中顯示它們。

   <!--All fields of the connected record display in the table view of the connected record's tab.-->

   依預設，會顯示連線記錄的前五個欄位。<!--No lookup fields display by default.-->

   ![行銷活動詳細資料下的對象已連線資料表檢視](assets/audience-connected-table-view-under-campaign-details-page.png)

1. （選擇性）搜尋或按一下清單中連線記錄或物件型別的名稱。

1. （選擇性和條件性）在連線記錄頁面的表格檢視中，檢視連線的Planning記錄或任何Workfront物件（專案除外）時，請執行下列任一動作： <!--or AEM Assets--> <!--AEM is not available yet?? see note below-->

   * 按一下記錄名稱。 這會在新索引標籤中開啟記錄頁面。

   * 按一下表格檢視底部的&#x200B;**連線**&#x200B;以連線更多記錄，然後按一下連線方塊外部以關閉它。 新記錄會自動新增到表格中。

     如需詳細資訊，請參閱[連線記錄](/help/quicksilver/planning/records/connect-records.md)。
   * 編輯內嵌在表格檢視中之連線記錄的任何資訊。

   * 將游標暫留在已連線的記錄名稱上，然後按一下&#x200B;**更多**&#x200B;功能表![更多](assets/more-menu.png)

     或

     選取其中一個記錄，然後按一下清單底部藍色列中的下列選項之一：

      * **檢視**&#x200B;以在新索引標籤中開啟記錄頁面
      * **複製連結**&#x200B;以複製記錄頁面的連結
      * **編輯縮圖**&#x200B;以開啟&#x200B;**錄製縮圖**&#x200B;方塊並編輯錄製的縮圖影像
      * **複製**&#x200B;以複製連線的記錄。 重複的記錄也連線到目前的記錄。
      * **在上方或下方插入記錄**&#x200B;以將新記錄新增至連線的記錄型別。 新增至此的新記錄也會連線至目前的記錄。 在表格中選取記錄時，此選項在藍色列中無法使用。
      * **刪除**&#x200B;以刪除記錄。 刪除連線的記錄會將其從記錄型別以及記錄連線的位置刪除。

     如需有關編輯表格檢視中記錄的資訊，請參閱[編輯記錄](/help/quicksilver/planning/records/edit-records.md)。

     >[!TIP]
     >
     >您可以選取多個記錄或物件來刪除它們。

   * 在「連線的記錄」頁面上的表格中，內聯編輯任何Planning記錄。

     所有其他Workfront物件都會以唯讀表格檢視顯示，且您無法加以編輯。

1. （選擇性和條件性）檢視連線的Workfront專案時，請在「連線記錄」頁面的表格檢視中執行下列任一項作業：

   * 按一下連線記錄頁面右上角的&#x200B;**連線記錄**&#x200B;以連線現有的專案。

   如需詳細資訊，請參閱[連線記錄](/help/quicksilver/planning/records/connect-records.md)。
   * 在表格中內聯編輯專案資訊。
   * 按一下&#x200B;**新增列**&#x200B;以建立沒有範本的專案。 新專案會立即連線到目前的記錄。

     如需詳細資訊，請參閱[當您將Workfront物件連線至記錄時，從Workfront Planning建立物件](/help/quicksilver/planning/records/create-workfront-objects-from-workfront-planning.md)
   * 將滑鼠停留在專案上，然後按一下&#x200B;**更多**&#x200B;功能表[更多](assets/more-menu.png)

     或

     選取一或多個專案，並注意清單底部的藍色列，然後按一下下列其中一項：

      * **刪除**&#x200B;以刪除專案。 刪除專案會中斷專案與記錄的連線，並將其移至Workfront的「資源回收筒」。
      * **中斷連線**&#x200B;以中斷專案與記錄的連線。 中斷專案的連線會從目前記錄中移除該專案及其查閱欄位的所有值。

1. （選擇性）連按兩下&#x200B;**連線記錄頁面**&#x200B;索引標籤的名稱

   或

   將游標暫留在索引標簽名稱上，然後按一下[其他] **** ![ [其他]功能表](assets/more-menu.png)，然後按一下[重新命名] **以重新命名為新的[連線檢視]索引標籤。**
1. （選擇性）在連線的記錄頁面的工具列中使用下列任何檢視元素來管理表格檢視：

   * 篩選器
   * 排序
   * 分組
   * 欄位，以顯示、隱藏或重新排列欄位
   * 列高
   * 搜尋

   如需詳細資訊，請參閱[管理資料表檢視](/help/quicksilver/planning/views/manage-the-table-view.md)。

   >[!NOTE]
   >
   >您無法在已連線記錄之索引標籤的表格檢視中建立、編輯或刪除欄位。

   <!--1. <span class="preview">(Optional) Click the dropdown menu to the right of the view name, then click **New view** to add a view. For more information, see the section [Manage multiple views from the connected records page](#manage-multiple-views-from-the-connected-records-page) in this article. </span>-->

1. （選擇性）將游標暫留在[連線的記錄]頁面索引標簽名稱上，按一下[其他] **** ![ [其他]功能表](assets/more-menu.png)，然後按一下[刪除] ****&#x200B;以移除索引標籤。

<!--
<div class="preview">

## Manage multiple views from the connected records page

You can add and manage views from the connected records page of a record. 

1. From the connected records page of a record, click the dropdown menu to the right of the view name, then click **New view** to add a view, then select from the following options: 

   * **Table**. For more information, see [Manage the table view](/help/quicksilver/planning/views/manage-the-table-view.md). 
   * **Timeline**. For more information, see [Manage the timeline view](/help/quicksilver/planning/views/manage-the-timeline-view.md).
   * **Calendar**. For more information, see [Manage the calendar view](/help/quicksilver/planning/views/manage-the-calendar-view.md). 

1. (Optional) Hover over the name of a view in the Connected records page, then click the **More** menu ![More menu](assets/more-menu.png), then click one of the following: *************check to make sure these are all possible*********

   * **Rename**
   * **Share**. For more information, see [Share views](/help/quicksilver/planning/access/share-views.md).

   >[!TIP]
   >
   >Sharing views from Connected records pages makes them accessible to users in all areas of Workfront Planning where the view displays. 
   >Also, if a view is shared from any other area of Workfront Planning, it is also available to the same users in Connected records pages. 

   * **Export** 
   * **Duplicate**. For more information, see [Duplicate record views](/help/quicksilver/planning/views/duplicate-record-views.md).

      >[!TIP]
      >
      >Duplicating a view from Connected records pages makes it available in all other areas of Workfornt planning, when viewing the same record types. 

</div> -->