---
title: 新增連線的記錄頁面至記錄
description: 您可以將「連線記錄」頁面的索引標籤新增至記錄，以檢視連線記錄或物件的資訊。 這會將表格檢視中的連線記錄新增至索引標籤。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
source-git-commit: 66d59467e7e9857ca5573b819d51da839ddbd4f7
workflow-type: tm+mt
source-wordcount: '2743'
ht-degree: 0%

---


# 將「連線的記錄」頁面新增至記錄

<span class="preview">本頁醒目提示的資訊指出尚未普遍可用的功能。 它僅在預覽環境中可供所有客戶使用。 每月發行至生產環境後，生產環境中為啟用快速發行的客戶也提供相同的功能。</span>

<span class="preview">如需快速發行資訊，請參閱[為您的組織啟用或停用快速發行](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>

您可以在Adobe Workfront Planning中將連線記錄頁面的頁簽新增至記錄，以檢視連線記錄或物件的資訊。 這會將表格檢視中的連線記錄新增至索引標籤。

將「連線的記錄」頁面新增至記錄時，請考量下列事項：

* 將記錄或物件型別從其表格檢視中連線至記錄型別後，您可以將「已連線的記錄」頁面新增至記錄。

* 您可以從記錄的預覽區域或記錄的頁面新增「連線記錄」頁面。

* <span class="preview">您只能有一個特定記錄型別的連線記錄頁面。</span>

  <span class="preview">例如，如果您為行銷活動建立連線記錄頁面，並且想要顯示其連線角色，則角色只能有一個連線記錄頁面。</span>

* 「連線的記錄」頁面只會顯示連線的物件或來自一個物件或記錄型別的記錄。 頁面不會顯示該型別的所有記錄。

* 視您在連線的記錄頁面中顯示的物件或記錄型別而定，您可以使用下列檢視來顯示它們：

   * 您可在下列檢視中顯示連線的Planning記錄：
      * 表格
      * <span class="preview">時間表</span>
      * <span class="preview">行事曆</span>
   * 您可以在清單檢視中顯示連線的Workfront專案。

* 您可以為下列連線記錄或物件型別新增「連線記錄」頁面：

   * Workfront Planning記錄型別
   * Workfront專案

     即使您無權在Workfront中存取Workfront專案，仍可檢視這些連線的專案。

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

在將連線的記錄頁面新增到記錄之前，您必須先將記錄型別與其他記錄型別或Workfront專案連線。

1. 按一下記錄名稱，從記錄型別頁面的任何檢視中開啟記錄。
1. 從下列其中一個區域按一下&#x200B;**新增頁面**：

   * 記錄的預覽視窗
   * 記錄的詳細資訊頁面，在按一下預覽頁面右上角的&#x200B;**在新索引標籤中開啟**&#x200B;圖示![在新索引標籤中開啟詳細資訊](assets/open-details-in-a-new-tab-icon.png)之後。

   **建立頁面**&#x200B;方塊開啟。

   ![新增連線記錄頁面模組](assets/add-connection-view-page-modal.png)

1. 新增&#x200B;**頁面名稱**，按一下&#x200B;**頁面型別**&#x200B;的&#x200B;**連線記錄頁面**，然後按一下&#x200B;**建立**。
1. （選擇性）按一下清單中連線記錄或物件型別的名稱，或搜尋它，然後在清單中顯示時按一下它，以建立該記錄或物件型別的頁面。

   >[!TIP]
   >
   ><span class="preview">您可以為每個記錄型別建立一個連線記錄頁面。 如果連線的記錄型別已經有頁面，則不再顯示為選項。</span>
   >

1. （選擇性和條件性）如果您要建置頁面的記錄或物件型別有多個連線的欄位，請從&#x200B;**選取參考欄位**&#x200B;清單中，按一下要在連線的記錄頁面中顯示其記錄或物件的欄位。

   ![選取參考欄位清單](assets/select-reference-field-list-on-connected-records-page.png)

   下列其中一個頁面已新增至「連線記錄」頁面：

   * 記錄型別的表格檢視
   * 專案物件型別的清單檢視

   連線至目前記錄的記錄或專案會顯示在表格或清單檢視中。

   >[!TIP]
   >
   >您必須先在記錄的表格或「詳細資訊」區域中新增連線的記錄，才能在連線的記錄頁面中顯示它們。 否則，表格或清單為空白。

   依預設，會顯示連線記錄的前五個欄位。 依預設，不會顯示任何查閱欄位。

   ![行銷活動詳細資料下的對象已連線資料表檢視](assets/audience-connected-table-view-under-campaign-details-page.png)

1. （視條件而定）請根據您在連線記錄頁面中顯示的記錄型別，執行下列其中一項作業：

   * 管理Planning記錄
如需相關資訊，請參閱本文章的[管理Planning記錄的連線記錄頁面](#manage-the-connected-records-page-for-planning-records)一節。
   * 管理Workfront專案
如需詳細資訊，請參閱本文章的[管理Workfront專案的連線記錄頁面](#manage-the-connected-records-page-for-workfront-projects)一節。

1. （選擇性）連按兩下&#x200B;**連線記錄頁面**&#x200B;索引標籤的名稱

   或

   暫留在索引標簽名稱上，然後按一下[其他] **&#x200B;**&#x200B;![&#x200B; [其他]功能表](assets/more-menu.png)，然後按一下[重新命名] **以重新命名為新的連線記錄頁面索引標籤。**

1. （選擇性）將游標暫留在連線記錄頁面索引標簽名稱上，按一下&#x200B;**更多** ![更多功能表](assets/more-menu.png)，然後按一下&#x200B;**刪除**&#x200B;以移除至索引標籤。

### 管理Planning記錄的連線記錄頁面

根據您使用的環境，管理Planning記錄的連線記錄頁面會有所不同。

#### 管理生產環境中Planning記錄的連線記錄頁面

當您在「生產」環境中建立連線Planning記錄的連線記錄頁面時，請執行下列動作： <!--or AEM Assets--> <!--AEM is not available yet?? see note below-->

1. 移至記錄型別頁面，然後按一下記錄名稱。 這會開啟記錄的預覽頁面。
1. 按一下顯示Planning記錄的連線記錄頁面頁標。
與您選取的記錄連線的記錄會顯示在表格檢視中。
1. 按一下表格檢視底部的&#x200B;**連線**&#x200B;以連線現有記錄，從連線方塊中選取記錄，然後按一下方塊外部以關閉記錄。 這些記錄會自動新增到表格中，並連線到您選取的記錄。 在新增記錄之前，記錄必須存在。

   如需詳細資訊，請參閱[連線記錄](/help/quicksilver/planning/records/connect-records.md)。

1. 編輯內嵌在表格檢視中之連線記錄的任何資訊。
1. 將游標暫留在已連線的記錄名稱上，然後按一下&#x200B;**更多**&#x200B;功能表![更多](assets/more-menu.png)

   或

   選取其中一個記錄，然後按一下清單底部藍色列中的下列選項之一：

   * **檢視**&#x200B;以在新索引標籤中開啟記錄頁面
   * **複製連結**&#x200B;以複製記錄頁面的連結
   * **編輯縮圖**&#x200B;以開啟&#x200B;**錄製縮圖**&#x200B;方塊並編輯錄製的縮圖影像
   * **複製**&#x200B;以複製連線的記錄。 重複的記錄也連線到目前的記錄。
   * **在上方或下方插入記錄**&#x200B;以將新記錄新增至連線的記錄型別。 新增至此的新記錄也會連線至目前的記錄。 在表格中選取記錄時，此選項在藍色列中無法使用。
   * **刪除**&#x200B;以刪除記錄。 刪除連線的記錄會將其從記錄型別以及記錄連線的位置刪除。 刪除的記錄移至其記錄型別的&#x200B;**最近刪除的**&#x200B;資料匣。

     如需有關編輯表格檢視中記錄的資訊，請參閱[編輯記錄](/help/quicksilver/planning/records/edit-records.md)。

     >[!TIP]
     >
     >您可以選取多個記錄或物件來刪除它們。
     >

1. 在「連線記錄」頁面上的表格中，內聯編輯任何記錄。
1. 在連線的記錄頁面的工具列中使用下列任何檢視元素來管理表格檢視：

   * **篩選器**
   * **排序**
   * **群組**
   * **欄位**，以顯示、隱藏或重新排列欄位
   * **資料列高度**
   * **搜尋**

   如需詳細資訊，請參閱[管理資料表檢視](/help/quicksilver/planning/views/manage-the-table-view.md)。

   >[!NOTE]
   >
   >您無法在已連線記錄之索引標籤的表格檢視中建立、編輯或刪除欄位。
   >

<div class="preview">

#### 在預覽環境中管理Planning記錄的連線記錄頁面

當您在「預覽」環境中建立連線Planning記錄的連線記錄頁面時，請執行下列動作： <!--or AEM Assets--> <!--AEM is not available yet?? see note below-->

1. 移至記錄型別頁面，然後按一下記錄名稱。 這會開啟記錄的預覽頁面。
1. 按一下顯示Planning記錄的連線記錄頁面頁標。
與您選取的記錄連線的記錄會顯示在表格檢視中。
1. 按一下連線記錄頁面右上角的&#x200B;**連線記錄**。若要連線現有記錄，請從連線方塊中選取記錄，然後按一下方塊外部以關閉記錄。 這些記錄會自動新增到表格中，並連線到您選取的記錄。 在新增記錄之前，記錄必須存在。

   如需詳細資訊，請參閱[連線記錄](/help/quicksilver/planning/records/connect-records.md)。

1. 按一下表格底部的&#x200B;**新列**&#x200B;以新增記錄。 新記錄會自動連線到您選取的記錄。
1. 編輯內嵌在表格檢視中之連線記錄的任何資訊。
1. 將游標暫留在已連線的記錄名稱上，然後按一下&#x200B;**更多**&#x200B;功能表![更多](assets/more-menu.png)

   或

   選取其中一個記錄，然後按一下清單底部藍色列中的下列選項之一：

   * **檢視**&#x200B;以在新索引標籤中開啟記錄頁面
   * **複製連結**&#x200B;以複製記錄頁面的連結
   * **編輯縮圖**&#x200B;以開啟&#x200B;**錄製縮圖**&#x200B;方塊並編輯錄製的縮圖影像
   * **複製**&#x200B;以複製連線的記錄。 重複的記錄也連線到目前的記錄。
   * **在上方或下方插入記錄**&#x200B;以將新記錄新增至連線的記錄型別。 新增至此的新記錄也會連線至目前的記錄。 在表格中選取記錄時，此選項在藍色列中無法使用。
   * **刪除**&#x200B;以刪除記錄。 刪除連線的記錄會將其從記錄型別以及記錄連線的位置刪除。 刪除的記錄移至其記錄型別的&#x200B;**最近刪除的**&#x200B;資料匣。

     如需有關編輯表格檢視中記錄的資訊，請參閱[編輯記錄](/help/quicksilver/planning/records/edit-records.md)。

     >[!TIP]
     >
     >您可以選取多個記錄或物件來刪除它們。

1. 在「連線記錄」頁面上的表格中，內聯編輯任何記錄。
1. 在連線的記錄頁面的工具列中使用下列任何檢視元素來管理表格檢視：

   * **篩選器**
   * **排序**
   * **群組**
   * **欄位**，以顯示、隱藏或重新排列欄位
   * **資料列高度**
   * **搜尋**

   如需詳細資訊，請參閱[管理資料表檢視](/help/quicksilver/planning/views/manage-the-table-view.md)。

   >[!NOTE]
   >
   >您無法在已連線記錄之索引標籤的表格檢視中建立、編輯或刪除欄位。
   >

1. 按一下[檢視]下拉式功能表，然後按一下[新檢視] **，為頁面新增檢視，然後執行下列動作：**

   1. 新增&#x200B;**檢視名稱**。
   1. 從&#x200B;**檢視型別**&#x200B;區域，選取下列檢視型別之一：

      * 表格
如需詳細資訊，請參閱[管理資料表檢視](/help/quicksilver/planning/views/manage-the-table-view.md)
      * 時間表
如需詳細資訊，請參閱[管理時間表檢視](/help/quicksilver/planning/views/manage-the-timeline-view.md)。
      * 行事曆
如需詳細資訊，請參閱[管理行事曆檢視](/help/quicksilver/planning/views/manage-the-calendar-view.md)。

        如需詳細資訊，請參閱本文中的[從連線的記錄頁面](#manage-multiple-views-from-the-connected-records-page)管理多個檢視一節。

   1. 按一下&#x200B;**建立**。
新檢視會新增至「檢視」下拉式功能表。

   1. （選擇性）將游標停留在您建立的檢視名稱上，按一下&#x200B;**更多**&#x200B;功能表![更多](assets/more-menu.png)，然後按一下下列其中一個選項：

      * **重新命名**，以新增檢視的名稱。
      * **共用**

        如需詳細資訊，請參閱[共用檢視](/help/quicksilver/planning/access/share-views.md)。

        >[!NOTE]
        >
        >您無法分享Workfront建立的系統檢視。

      * **刪除**
如需詳細資訊，請參閱[刪除記錄檢視](/help/quicksilver/planning/views/delete-record-views.md)。

        ![](assets/view-more-menu-projects-connected-records-page.png)

</div>

### 管理Workfront專案的連線記錄頁面

當您為連線的Workfront專案建立連線記錄頁面時，請執行下列動作：

1. 移至記錄型別頁面，然後按一下記錄名稱。 這會開啟記錄的預覽頁面。
1. 按一下顯示Workfront專案的已連線記錄頁面標籤。
與您選取的記錄連線的專案會顯示在清單檢視中。
1. 按一下連線記錄頁面右上角的&#x200B;**連線記錄**&#x200B;以連線現有的專案。

   如需詳細資訊，請參閱[連線記錄](/help/quicksilver/planning/records/connect-records.md)。
1. 在表格中內聯編輯專案資訊。
1. 按一下&#x200B;**新增列**&#x200B;以建立沒有範本的專案。 新專案會自動連線到目前的記錄。

   如需詳細資訊，請參閱[當您將Workfront物件連線至記錄時，從Workfront Planning建立物件](/help/quicksilver/planning/records/create-workfront-objects-from-workfront-planning.md)。

1. 將滑鼠停留在清單中的專案名稱上，然後按一下&#x200B;**更多**&#x200B;功能表[更多](assets/more-menu.png)

   或

   選取一或多個專案，並注意清單底部的藍色列，然後按一下下列其中一項：

   * **刪除**&#x200B;以刪除專案。 刪除專案會中斷專案與記錄的連線，並將其移至Workfront的「資源回收筒」。 Workfront管理員可在刪除已刪除的專案後30天內復原這些專案。
   * **中斷連線**&#x200B;以中斷專案與記錄的連線。 中斷專案的連線會從目前記錄中移除該專案及其查閱欄位的所有值。

     >[!TIP]
     >
     >您可以選取多個專案來中斷連線或予以刪除。
     >

1. 按一下[檢視]下拉式功能表，然後按一下[新檢視] **，為頁面新增檢視，然後執行下列動作：**

   1. 新增&#x200B;**檢視名稱**。
   1. 從&#x200B;**檢視型別**&#x200B;區域選取&#x200B;**清單**。
   1. 按一下&#x200B;**建立**。
新的清單檢視會新增至「檢視」下拉式功能表。

      如需詳細資訊，請參閱本文中的[從連線的記錄頁面](#manage-multiple-views-from-the-connected-records-page)管理多個檢視一節。

   1. （選擇性）將游標停留在您建立的檢視名稱上，按一下&#x200B;**更多**&#x200B;功能表![更多](assets/more-menu.png)，然後按一下下列其中一個選項：
      * **重新命名**，以新增檢視的名稱。
      * <span class="preview">**共用**</span>

        如需詳細資訊，請參閱[共用檢視](/help/quicksilver/planning/access/share-views.md)。

        >[!NOTE]
        >
        >您無法分享Workfront建立的系統檢視。

      * **刪除**
如需詳細資訊，請參閱[刪除記錄檢視](/help/quicksilver/planning/views/delete-record-views.md)。

        ![](assets/view-more-menu-projects-connected-records-page.png)

   1. 按一下&#x200B;**篩選器**&#x200B;圖示![篩選器圖示](assets/filter-icon.png)，然後使用該篩選器來顯示特定專案。

      >[!TIP]
      >
      ><span class="preview">針對人員型別欄位，例如&#x200B;**所有者**&#x200B;或&#x200B;**贊助者**，您可以使用萬用字元來顯示將登入使用者指派給這些角色的專案。</span>
      >
      >![使用使用者萬用字元篩選專案連線記錄頁面](assets/filter-with-user-wildcard-project-connected-records-page.png)
      >

   1. 按一下&#x200B;**欄**&#x200B;圖示![欄圖示](assets/columns-icon.png)以隱藏或顯示清單中的欄。
   1. 按一下表格檢視右上角的&#x200B;**+**&#x200B;圖示，將現有欄位新增至表格。 欄位必須先存在，您才能新增它們。

      **資料行管理員**&#x200B;方塊開啟。 請執行下列動作：

      1. 搜尋&#x200B;**可用**&#x200B;欄位中的現有物件欄位，然後按一下欄位名稱右側的&#x200B;**+**，將其新增至&#x200B;**已選取**&#x200B;欄。

         您選取的欄位會新增至連線記錄頁面的表格檢視中。
      1. 按一下&#x200B;**已選取**&#x200B;資料行中欄位右側的&#x200B;**-**，將其從資料表檢視中移除。
      1. 按一下&#x200B;**儲存**&#x200B;以儲存連線的記錄頁面資料表檢視。


<div class="preview">

## 從連線的記錄頁面管理多個檢視

您可以從記錄的已連線記錄頁面新增及管理多個檢視型別。

您在記錄型別的「連線記錄」頁面中建立的檢視，在Workfront Planning中顯示該記錄型別頁面的任何地方都可以使用。 在Workfront Planning中任何地方為相同記錄型別建立的檢視，也可在該記錄型別的所有已連線記錄頁面中存取。

若要從連線的記錄頁面管理多個檢視：

1. 從記錄的已連線記錄頁面中，按一下檢視名稱右側的下拉式功能表，然後按一下[新增檢視] **以新增檢視，然後從下列選項中選取：**

   * **資料表**。 如需詳細資訊，請參閱[管理資料表檢視](/help/quicksilver/planning/views/manage-the-table-view.md)。
   * **時間表**。 如需詳細資訊，請參閱[管理時間表檢視](/help/quicksilver/planning/views/manage-the-timeline-view.md)。
   * **行事曆**。 如需詳細資訊，請參閱[管理行事曆檢視](/help/quicksilver/planning/views/manage-the-calendar-view.md)。

1. （選擇性）將游標暫留在「連線的記錄」頁面中的檢視名稱上，然後按一下&#x200B;**更多**&#x200B;功能表![更多](assets/more-menu.png)，然後按一下下列其中一項：

   * **重新命名**
   * **共用**。 如需詳細資訊，請參閱[共用檢視](/help/quicksilver/planning/access/share-views.md)。

   >[!TIP]
   >
   >共用「連線記錄」頁面的檢視可讓使用者存取Workfront Planning中顯示檢視的所有區域。
   >此外，如果從Workfront Planning的任何其他區域共用檢視，則在「連線的記錄」頁面中也可讓相同的使用者使用。

   * **匯出**
   * **重複**。 如需詳細資訊，請參閱[重複的記錄檢視](/help/quicksilver/planning/views/duplicate-record-views.md)。

     >[!TIP]
     >
     >從「連線的記錄」頁面複製檢視，可在檢視相同記錄型別時，於Workforce計畫的所有其他區域使用。

</div>

<!--No longer possible: 1. (Optional and conditional) When you create a connected records page for the following Workfront object types:
         * Portfolios
         * Programs
         * Groups
         * Companies
      Do any of the following in the table view of the connected records page: 
      * Click the name of a object. This opens the object's page in a new tab. 
      * Click **Connect** at the bottom of the table view to connect existing objects, select them from the connection box, then click outside the box to close it. The objects are automatically added to the table. The objects must exist before you can add them.
      For more information, see [Connect records](/help/quicksilver/planning/records/connect-records.md).
      * Select one of the objects in the table view, then click one of the following options in the blue bar at the bottom of the list: 
      * **View** to open the record page in a new tab
      * **Copy link** to copy a link to the record page
      * **Disconnect** to disconnect the object from the record you are viewing. 
      TIP      
      You can select more than one record or object to disconnect them.
      -->