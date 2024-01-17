---
title: 連線記錄
description: 在記錄型別之間建立連線後，可以將個別記錄彼此連線。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 17796cdc-6de8-4209-a5af-b255dc64d70a
source-git-commit: 5f3d5c93c2fc721dda2dd04adac22190ef6a3f29
workflow-type: tm+mt
source-wordcount: '2912'
ht-degree: 0%

---

<!--when you make this live, update the metadata above to this: 
---
title: Connect records and objects
description: In addition to connecting Maestro records to one another, you can also connect Maestro records to objects from other applications.  
topic: Architecture
role: User
hidefromtoc: yes
hide: yes
---
-->
<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!--if you change steps here, also update steps in the "Connect records" article-->

# 連線記錄

>[!IMPORTANT]
>
>本文資訊是指Adobe Maestro，這是Adobe Workfront的新產品。
>
>目前，Adobe大師是測試版計畫的一部分，向有限數量的客戶開放。 您必須是Workfront客戶才能使用Maestro功能。
>
>如需加入Maestro測試版計畫的詳細資訊，請聯絡您的客戶代表。
>
>如需詳細資訊，請參閱 [Adobe大師概觀](../maestro-overview.md).

您可以將AdobeMaestro記錄彼此連線，或連線到其他應用程式的物件。

您必須先將兩個記錄型別連線在一起，或將記錄型別連線到另一個應用程式的物件型別，然後可以使用記錄型別的「表格」檢視將記錄連線到另一個或記錄連線到其他物件。

如需有關將記錄型別相互連線或從其他應用程式連線到物件型別的資訊，請參閱 [連線記錄型別](../architecture/connect-record-types.md).

如需連線記錄型別的範例，請參閱 [連線記錄型別和記錄的範例](../architecture/example-connect-record-types-and-records.md).

您可以連線下列專案：

* Maestro作業記錄
* 將主要作業記錄轉換為分類記錄
* Maestro作業記錄和其他應用程式的物件。

  您可以從下列應用程式將Maestro記錄連線至下列型別的物件：

   * Adobe Workfront

      * 專案
      * 專案組合
      * 計劃
      * 公司
      * 群組

   * Adobe Experience Manager Assets

      * 影像檔案
      * 資料夾



  <!--when you add more objects, fix the Access Requirements below which right now refer only to projects-->

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
<td>產品</p> </td>
   <td>
   <p> Adobe Workfront</p> 
   <p>若要將Maestro記錄與Experience Manager Assets連線，您必須擁有Adobe Experience Manager Assets授權，且貴組織的Workfront執行個體必須上線至Adobe Business Platform或Adobe Admin Console。</p>
   </td>
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
   <td role="rowheader"><p>存取層級設定</p></td>
   <td> <p>Maestro沒有存取層級控制項</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>權限</p></td>
   <td> <p>管理工作區的許可權</a> </p>  
   <p>系統管理員擁有所有工作區的許可權，包括他們未建立的工作區</p>
</td>
  </tr>

<tr>
   <td role="rowheader"><p>版面配置範本</p></td>
   <td> <p>您的Workfront或群組管理員必須在您的版面配置範本中新增Maestro區域。 如需詳細資訊，請參閱 <a href="../access/access-overview.md">存取權總覽</a>. </p>  
</td>
  </tr>

</tbody>
</table>

<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

## 連線記錄

### 有關連線記錄的考量事項

* 在您連線記錄型別之後，連線的記錄型別會在它們所連結的記錄型別表格中顯示為連結的記錄欄位。
* 您可以從連結記錄欄位中瀏覽並新增連結記錄的記錄和物件以及物件型別。
* 您可以將連結的記錄型別的欄位新增至您正在連結的記錄型別的表格。
* 您無法手動更新連結來源記錄之連結欄位的值。

  連結記錄中連結欄位的值會填入您要從您設定的Maestro工作區或從第三方應用程式自動連結的Maestro記錄。

* 擁有工作區之Maestro存取權和「管理」許可權的所有人，都可以看到您在Maestro記錄之間或Maestro記錄與其他應用程式物件之間的連線。 使用者可檢視連線的記錄和物件，無論其對於您所連線的協力廠商應用程式的許可權為何。 <!--check with PM-->
* 如果您對連線記錄所在的工作區具有管理許可權，則可以檢視及編輯其他人的連線。
* 您可以將一個Maestro記錄連線到另一個應用程式的一個或多個物件。
* 若要將Maestro記錄與其他記錄或物件連結，您必須具備下列專案：

   * 至少有一個Maestro工作區、記錄型別和記錄。

     如需詳細資訊，請參閱下列文章：

      * [建立工作區](../architecture/create-workspaces.md)
      * [建立記錄型別](../architecture/create-record-types.md)
      * [建立記錄](../records/create-records.md)

   * 記錄型別之間的連線，或記錄型別與其他應用程式物件之間的連線。 如需詳細資訊，請參閱 [連線記錄型別](../architecture/connect-record-types.md)

### 連線大師記錄

{{step1-to-maestro}}

根據預設，上次存取的工作區應該會開啟。

1. （可選）展開現有工作區名稱右側的向下箭頭，並選取您要連線記錄的工作區。
1. 按一下記錄型別的卡片以開啟記錄型別頁面。
1. 選取 **表格** 從檢視 **檢視** 記錄型別頁面右上角的下拉式功能表。
1. （選擇性）將記錄新增至表格的新列，以將記錄新增至您選取的記錄型別。 如需詳細資訊，請參閱 [建立記錄](../../maestro/records/create-records.md).
1. 從表格檢視中列出的記錄，移至連結的記錄欄，並將游標停留在您要與其他記錄連結之記錄的對應儲存格上，然後按一下 **+** 圖示。

   此 **連線物件** 方塊隨即顯示。

   ![](assets/connected-objects-table-for-records.png)

1. 開始在搜尋方塊中輸入記錄名稱，然後在清單中顯示記錄時選取記錄

   或

   在方塊中選取一或多個記錄的名稱，然後按一下 **連線物件** 在「連線物件」方塊的右上角。

   新增下列專案：

   * 連結的記錄會顯示在您在步驟5中所選記錄的連結記錄欄位中。 <!--accurate?--> 更新連結的記錄會自動更新連結的記錄欄位。 您無法手動編輯連結的欄位。

     >[!TIP]
     >
     >* 我們會交替使用「連結欄位」和「查詢欄位」。
     >
     >* 如果您已啟用 **允許多筆記錄** 設定當您連線記錄型別時，多個所選物件的欄位值會以逗號分隔顯示，或根據您選擇的彙總器彙總。

1. （可選）關閉Maestro記錄型別頁面，然後移至您選取的工作區。
1. 按一下您所連結之記錄型別的卡片。

   例如，如果您已連線 **Campaign** 含有產品記錄的記錄，按一下 **產品** 卡片。

   記錄型別卡片應在「表格」檢視中開啟。 如果沒有，請選取表格檢視。

   請注意 **Campaign** 連結的記錄欄位會顯示您在「產品記錄型別」頁面中連結至產品的行銷活動名稱。 更新行銷活動資訊會自動更新產品記錄型別的行銷活動連結記錄欄位。

### 將Maestro記錄連線到Workfront物件

<!--when we will have more applications to link to from Maestro, change the title to soemthing like: Connect Maestro records to objects from other applications-->

在Maestro記錄型別和Workfront物件型別之間建立連線後，您可以將個別Maestro記錄連線到Workfront中的物件。 您連結的Workfront欄位會自動填入您連結物件的Maestro記錄中。

{{step1-to-maestro}}

根據預設，上次存取的工作區應該會開啟。

1. （可選）展開現有工作區名稱右側的向下箭頭，並選取您要連線記錄的工作區。
1. 按一下記錄型別的卡片以開啟記錄型別頁面。
1. 選取 **表格** 從檢視 **檢視** 記錄型別頁面右上角的下拉式功能表。

1. （選擇性）將個別記錄新增至表格的新列，以將個別記錄新增至您選取的記錄型別。 如需詳細資訊，請參閱 [建立記錄](../../maestro/records/create-records.md).
1. （視條件而定）如果您將選取的記錄型別與Workfront物件連線，請移至連結物件欄，將游標停留在您要與Workfront物件連結之記錄對應的儲存格上，然後按一下 **+** 圖示。

   此 **連線物件** 方塊隨即顯示。

   ![](assets/connect-objects-box-to-select-projects.png)

   如需有關將記錄型別與來自協力廠商應用程式的物件連線的詳細資訊，請參閱 [連線記錄型別](../architecture/connect-record-types.md).

1. 開始在搜尋方塊中輸入Workfront物件的名稱，然後在其顯示在清單中時選取它

   或

   在方塊中選取一或多個物件的名稱，然後按一下 **連線物件** 在「連線物件」方塊的右上角。

   新增下列專案：

   * 選取的Workfront物件會新增至連結的記錄欄位。
   * 如果您在使用Workfront連線記錄型別時新增這些欄位，則連結欄位（或查詢欄位）會自動填入Workfront中的資訊。
   * 名為「&lt; Workfront物件型別名稱>」的新記錄型別會建立在與您連結的Maestro記錄相同的工作區中。 物件的名稱是此記錄型別名稱的一部分。 例如，連結至Workfront專案會建立 **專案** Maestro中的記錄型別。

     這是唯讀記錄型別，它顯示在您從Maestro記錄建立的新連結物件欄位中選取的Workfront物件。 連結物件的連結欄位也會顯示在唯讀的連結Workfront記錄上。

     >[!IMPORTANT]
     >
     > 唯讀的Workfront物件記錄型別只會在個別專案新增到Maestro記錄時建立。 只是在Maestro記錄型別和Workfront物件型別之間建立連線，不會建立Workfront記錄型別。

     Workfront物件欄位中的任何現有資訊都會顯示在連結或查詢欄位中。

     >[!TIP]
     >
     >
     >* 如果您啟用「允許多筆記錄」設定，則多個物件的值會以逗號分隔顯示，或根據您選擇的彙總器彙總。
     >
     >* 在Workfront中，不會針對連結的Workfront物件建立連結至Maestro連結記錄的連結記錄欄位。


1. （可選）關閉Maestro記錄型別頁面，然後移至您選取的工作區。
1. （選用）按一下Workfront物件記錄型別的卡片。 例如，按一下 **專案** 卡片，如果您連結至Workfront專案。 唯讀Workfront記錄型別卡片應在表格檢視中開啟。

   Workfront記錄型別頁面中列出的記錄是已從Maestro記錄連結的唯讀Workfront物件。 從Workfront記錄型別連結的欄位也會顯示為唯讀欄，且在Workfront中填入欄位時自動填入。

1. （可選）若要在Maestro中開啟Workfront物件記錄「詳細資訊」頁面，請執行下列任一項作業：

   * 從您連結的記錄型別中，前往Workfront物件連結的記錄欄位，然後按一下Workfront物件的名稱。
   * 從 **表格** 檢視Workfront記錄型別頁面，按一下Workfront物件的名稱

     或

     按一下 **更多** Workfront物件名稱右側的功能表，然後按一下 **檢視**.

     ![](assets/workfront-object-more-menu-in-table-with-go-to-source-link.png)

   這會開啟連結Workfront物件的「Maestro詳細資訊」頁面。 這是唯讀頁面。

1. （可選）若要在Workfront中開啟連結的Workfront物件，請執行下列任一項作業：

   * 從 **表格** 檢視Workfront記錄型別頁面，按一下Workfront物件的名稱以在Maestro中開啟專案記錄

   或

   按一下 **更多** Workfront物件名稱右側的功能表，然後按一下 **移至來源**.

   ![](assets/workfront-project-maestro-details-page-with-go-to-source-link.png)

   這會開啟Workfront物件頁面。 如果您有許可權，可以編輯Workfront物件的相關資訊。

1. （可選）在Maestro的唯讀Workfront物件記錄頁面中，按一下 **新增欄位** 圖示 ![](assets/add-fields-icon.png) 在表格檢視的右上角，新增或移除Workfront記錄型別中的Workfront欄位。

   >[!NOTE]
   >
   >  您在Workfront物件記錄型別頁面中新增或移除的欄位，不會從連結至Workfront物件型別的Maestro記錄型別中新增或移除。 這些欄位僅在唯讀的Workfront記錄型別頁面上可見，因此您可以在Maestro中檢視它們。

1. （選擇性和條件性）如果您將至少兩個日期欄位新增至Workfront物件，請按一下 **檢視** Workfront物件記錄型別頁面中的下拉式功能表，然後選取 **時間表** 檢視或 **建立檢視** 以建立時間表檢視。  如需詳細資訊，請參閱 [管理時間表檢視](/help/quicksilver/maestro/views/manage-the-timeline-view.md).

   Workfront連結物件會顯示在時間軸檢視中。


### 將Maestro記錄連線到Adobe Experience Manager物件

<!--when we will have more applications to link to from Maestro, change the title to soemthing like: Connect Maestro records to objects from other applications-->

>[!IMPORTANT]
>
>您必須擁有Adobe Experience Manager Assets授權，且貴組織的Workfront執行個體必須上線至Adobe商業平台或Adobe Admin Console，才能將Maestro記錄連線至Adobe Experience Manager Assets。
>
>如果您對上線Adobe Admin Console有任何疑問，請參閱 [Adobe Unified Experience常見問題集](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/unified-experience-faq.md).

建立Maestro記錄型別與Adobe Experience Manager Assets之間的連線後，您可以將個別Maestro記錄連線至Experience Manager資產。 當您建立連線時，您從Experience Manager Assets連線的資產欄位會自動填入您連結的Maestro記錄型別中。

{{step1-to-maestro}}

根據預設，上次存取的工作區應該會開啟。

1. （可選）展開現有工作區名稱右側的向下箭頭，並選取您要連線記錄的工作區。
1. 按一下記錄型別的卡片以開啟記錄型別頁面。
1. 選取 **表格** 從檢視 **檢視** 記錄型別頁面右上角的下拉式功能表。

1. （選擇性）將個別記錄新增至表格的新列，以將個別記錄新增至您選取的記錄型別。 如需詳細資訊，請參閱 [建立記錄](../../maestro/records/create-records.md).
1. （視條件而定）如果您將選取的記錄型別與Experience Manager Assets連線，請移至連結物件欄，將游標停留在您要從Experience Manager連結其他物件的記錄所對應的儲存格上，然後按一下 **+** 圖示。

   此 **選取資產** 方塊隨即顯示。 <!--update screen shot with actual assets-->

   ![](assets/select-assets-box-for-aem-record-connections.png)

   如需有關將記錄型別與來自協力廠商應用程式的物件連線的詳細資訊，請參閱 [連線記錄型別](../architecture/connect-record-types.md).

1. 按一下以選取下列部分資產型別：

   * 影像
   * 資料夾

   您可以選取多個資產。

   >[!IMPORTANT]
   >
   > 您只能連線您有權在Experience Manager中檢視的資產。 連線之後，所有Maestro使用者都可以在Maestro中檢視資產，無論他們在Experience Manager Assets中是否具備存取權。

1. 按一下 **選取**.

   新增下列專案：

   * 選取的Experience Manager資產會新增至連結的記錄欄位。
   * 連結欄位（或查詢欄位）會填入Experience Manager連線資產的資訊。
   * 名為「Experience Manager Assets」的新記錄型別會建立在與您連結的Maestro記錄相同的工作區中。 <!--is this still added?-->

     這是唯讀的記錄型別，它顯示在您從Maestro記錄建立的新連結物件欄位中選取的Experience Manager資產。 連結物件的連結欄位也會顯示在唯讀的連結Experience Manager記錄上。

     >[!IMPORTANT]
     >
     > 唯讀的Experience Manager Assets記錄型別只會在個別資產新增到Maestro記錄時建立。 只是在Maestro記錄型別和Experience Manager Assets之間建立連線，不會建立Experience Manager Assets記錄型別。

     Experience Manager資產欄位中的任何現有資訊都會顯示在連結或查詢欄位中。

     >[!TIP]
     >
     >
     >* 如果您啟用「允許多筆記錄」設定，則會以逗號分隔多個物件的值。
     >
     >* 在Experience Manager Assets應用程式中，不會針對連結的Experience Manager資產建立連結至Maestro連結記錄的連結記錄欄位。


1. （可選）關閉Maestro記錄型別頁面，然後移至您選取的工作區。
1. 按一下Experience Manager Assets記錄型別的卡片。 唯讀Experience Manager Assets記錄型別卡片應在表格檢視中開啟。

   Experience Manager Assets記錄型別頁面中列出的記錄為唯讀資產。 從Experience Manager Assets記錄型別連結的欄位也會顯示為唯讀欄，並在以Experience Manager填入時自動填入。

1. （可選）前往您連結至Experience Manager Assets的記錄型別，然後在連結的記錄欄位中按一下資產名稱。 資產的Experience Manager詳細資訊會顯示在快顯視窗中。 <!--update screen shot with hi-rez picture-->

   ![](assets/asset-pop-up-window-with-aem-details-and-thumbnail.png)

   影像檔案會顯示下列欄位：

   * 影像縮圖
   * 影像檔案名稱
   * 尺寸
   * 大小
   * 說明
   * Experience Manager的檔案路徑
   * 資產型別
   * 建立日期
   * 修改日期

1. （可選）若要在Maestro中開啟「Experience Manager Assets記錄詳細資訊」頁面，請執行下列動作：

   1. 前往 **Experience Manager Assets** Maestro記錄型別卡在您最初選取的工作區中，然後按一下以開啟記錄型別頁面。
Experience Manager Assets Maestro記錄型別頁面為唯讀。
   1. 從表格檢視中，按一下資產名稱

      或

      將游標停留在資產名稱上，按一下 **更多** 功能表 ![](assets/more-menu.png) 資產名稱右側，然後按一下 **檢視**.\
      如此將可開啟資產的大師 **詳細資料** 頁面。 這是唯讀頁面。
1. （可選）若要以Experience Manager開啟「Experience Manager資產記錄詳細資訊」頁面，請執行下列任一項作業：

   * 前往您連結之記錄的Maestro記錄型別頁面，在連結的記錄欄位中按一下資產名稱以開啟快顯視窗，然後按一下 **開啟** 圖示 ![](assets/open-asset-icon.png) 以開啟資產。
   * 前往 **Experience Manager Assets** Maestro記錄型別卡在您最初選取的同一個工作區中，並按一下以開啟記錄型別頁面，按一下資產名稱以開啟Maestro **詳細資料** 頁面，然後按一下 **移至來源** 在畫面的右上角。

     ![](assets/go-to-source-asset-maestro-details-page.png)
   * 前往 **Experience Manager Assets** Maestro記錄型別卡在您最初選取的相同工作區中，按一下卡片以開啟Experience Manager Assets記錄型別頁面，將游標停留在資產名稱上，然後按一下 **更多** 功能表，然後按一下 **移至來源**.

     ![](assets/go-to-source-option-on-table-view.png)

   資產會在Experience Manager Assets中開啟。

1. （可選）按一下 **新增欄位** 圖示 ![](assets/add-fields-icon.png) 「Experience Manager Assets記錄型別」頁面上「表格」檢視的右上角，新增或移除Experience Manager欄位。

   >[!NOTE]
   >
   >  您在Experience Manager Assets記錄型別頁面中新增或移除的欄位，不會從連結至Experience Manager資產的Maestro記錄型別中新增或移除。 這些欄位僅在唯讀的Experience Manager Assets記錄型別頁面上可見，因此您可以在Maestro中檢視它們。

1. （選擇性和條件性）如果您在Experience Manager連結資產中新增至少兩個日期欄位，請按一下 **檢視** 在Experience Manager Assets記錄型別頁面中的下拉式功能表，然後選取 **時間表** 檢視或 **建立檢視** 以建立時間表檢視。  如需詳細資訊，請參閱 [管理時間表檢視](/help/quicksilver/maestro/views/manage-the-timeline-view.md).
Experience Manager Assets連結的資產會顯示在時間軸檢視中。