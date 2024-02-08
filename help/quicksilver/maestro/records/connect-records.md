---
title: 連線記錄
description: 在記錄型別之間建立連線後，可以將個別記錄彼此連線。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 17796cdc-6de8-4209-a5af-b255dc64d70a
source-git-commit: 24975c463c93de61672f1986d82d1d6500133baa
workflow-type: tm+mt
source-wordcount: '2379'
ht-degree: 1%

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

{{maestro-important-intro}}

您可以將AdobeMaestro記錄彼此連線，或連線到其他應用程式的物件。

您必須先將兩個記錄型別彼此連線，或將記錄型別從另一個應用程式連線到物件型別。 這會建立連結的記錄欄位。 然後，您可以使用連結的記錄欄位，將記錄彼此連線，或將記錄從其他應用程式連線到其他物件。

連線記錄類似於將記錄從另一個應用程式連線到物件。

如需有關將記錄型別相互連線或從其他應用程式連線到物件型別的資訊，請參閱 [連線記錄型別](../architecture/connect-record-types.md).

如需連線記錄型別的範例，請參閱 [連線記錄型別和記錄的範例](../architecture/example-connect-record-types-and-records.md).

您可以連線下列專案：

* Maestro作業記錄
* 使用分類法記錄的大型作業記錄
* 主要分類法
* 使用其他應用程式的物件來製作作業記錄或分類。

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
   <td> <p>管理工作區的許可權以連線記錄 </p>  
   <p>檢視工作區或更高許可權，可檢視與其他應用程式之物件和欄位的所有連線，無論您對其他應用程式的存取權為何。 </p>
   <p>系統管理員擁有所有工作區的許可權，包括他們未建立的工作區。</p>
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

* 在您連線記錄型別之後，連線的記錄型別會在它們所連結的記錄型別表格中，以及在它們所連結的記錄的「詳細資訊」頁面上，顯示為連結的記錄欄位。
* 您可以從連結記錄欄位中瀏覽並新增連結記錄的記錄和物件以及物件型別。
* 您可以將連結的記錄型別的欄位新增至您正在連結的記錄型別的表格。
* 您無法手動更新連結來源記錄之連結欄位的值。

  連結記錄的連結欄位值會填入您從原始記錄或物件自動連結的Maestro記錄。

* 擁有工作區之Maestro和「檢視」存取許可權或較高許可權的所有人，都可以看到您在Maestro記錄之間或Maestro記錄與其他應用程式物件之間的連線。 無論連線至應用程式的許可權為何，使用者都可以檢視連線的記錄和物件。
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
1. （視條件而定）將選取的記錄型別與其他記錄型別連結後，請移至連結的記錄欄，然後按兩下要與其他記錄連結之記錄對應的儲存格。

   ![](assets/connect-other-records-smaller-box-in-table-view.png)

1. 執行下列其中一項：

   * 從清單中按一下已連線的記錄名稱，將其新增至選取的記錄。 記錄會自動新增。
   * 開始輸入記錄的名稱，並在它顯示在清單中時按一下它。 記錄會自動新增。
   * 按一下 **檢視全部** 以顯示所有記錄。

1. （視條件而定）如果您按一下 **全選** 在上一步中， **連線物件** 方塊隨即顯示。

   ![](assets/connected-objects-table-for-records.png)

1. 開始在搜尋方塊中輸入記錄名稱，然後在清單中顯示記錄時選取記錄

   或

   在方塊中選取一或多個記錄的名稱，然後按一下 **連線物件** 在「連線物件」方塊的右上角。

   >[!TIP]
   >
   >    您可以開啟記錄的「詳細資訊」頁面，找到連結的記錄欄位，然後按一下 **+** 圖示來從連線的記錄或物件型別新增記錄。

   新增下列專案：

   * 連結的記錄會顯示在您在步驟6中選取之記錄的連結記錄欄位中。 <!--accurate?-->
   * 如果您在連線記錄型別時新增連結查閱欄位，則連結欄位會填入來自連結記錄的資訊。

   更新連結的記錄會自動更新連結的記錄之連結欄位。 您無法手動編輯連結的欄位。

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

<!--when we will have more applications to link to from Maestro, change the title to something like: Connect Maestro records to objects from other applications-->

在Maestro記錄型別和Workfront物件型別之間建立連線後，您可以將個別Maestro記錄連線到Workfront中的物件。 您連結的Workfront欄位會自動填入您連結物件的Maestro記錄中。

>[!NOTE]
>
>您無法將Workfront物件與Workfront的Maestro記錄連線。


{{step1-to-maestro}}

根據預設，上次存取的工作區應該會開啟。

1. （可選）展開現有工作區名稱右側的向下箭頭，並選取您要連線記錄的工作區。
1. 按一下記錄型別的卡片以開啟記錄型別頁面。
1. 選取 **表格** 從檢視 **檢視** 下拉式功能表。

1. 按一下 **新記錄**  將個別記錄新增至您選取的記錄型別。 如需詳細資訊，請參閱 [建立記錄](../../maestro/records/create-records.md).
1. （視條件而定）將選取的記錄型別與Workfront物件型別連線後，請移至連結物件欄，然後按兩下您要與Workfront物件連結之記錄對應的儲存格。

   ![](assets/connect-projects-smaller-box-in-table-view.png)

1. 執行下列其中一項：

   * 按一下清單中的物件，將其新增至選取的記錄。 物件按字母順序列出。 物件會自動新增。
   * 開始輸入物件的名稱，當物件顯示在清單中時，按一下該物件。 物件會自動新增。
   * 按一下 **檢視全部** 顯示您至少擁有檢視許可權的所有物件。

1. （視條件而定）如果您按一下 **檢視全部** 在上一步中， **連線物件** 方塊隨即顯示。

   ![](assets/connect-objects-box-to-select-projects.png)

1. 開始在搜尋方塊中輸入Workfront物件的名稱，然後在其顯示在清單中時選取它

   或

   在方塊中選取一或多個物件的名稱，然後按一下 **連線物件** 在「連線物件」方塊的右上角。

   >[!IMPORTANT]
   >
   >* 您只能新增您有權檢視的Workfront物件。
   >
   >* 新增Workfront物件後，所有具有工作區檢視或更高許可權的人都可以檢視Workfront物件及其欄位資訊，無論他們在Workfront中的許可權或存取權為何。

   新增下列專案：

   * 選取的Workfront物件會新增至連結的記錄欄位。
   * 如果您在使用Workfront連線記錄型別時新增這些欄位，Workfront物件的連結欄位（或查詢欄位）會自動填入Workfront的資訊。

   >[!TIP]
   >
   >您可以開啟記錄的「詳細資訊」頁面，找到連結的記錄欄位，然後按一下 **+** 圖示來從連線的物件型別新增物件。

   如需有關將記錄型別與來自其他應用程式的物件連線的詳細資訊，請參閱 [連線記錄型別](../architecture/connect-record-types.md).

1. （選擇性）在表格檢視的連結欄位中，或從表格檢視的連結欄位中，按一下與Maestro記錄連線的Workfront物件名稱。 **詳細資料** Maestro記錄的頁面。

   這會開啟唯讀的Maestro **詳細資料** 連結的Workfront物件頁面。 將記錄型別與Workfront物件連線時，您選取作為查詢欄位的欄位會顯示在Workfront Maestro記錄的「詳細資料」頁面中。

   >[!TIP]
   >
   >* 當您啟用「允許多筆記錄」設定時，查閱欄位的值會以逗號分隔顯示，或根據您選擇的彙總器進行彙總。
   >
   >* Workfront中的連結Workfront物件不會建立連結記錄欄位。

1. （選用）若要在Workfront中開啟連結的Workfront物件，請按一下 **移至來源** 在Workfront物件的「詳細資訊」頁面的右上角。

   ![](assets/workfront-project-maestro-details-page-with-go-to-source-link.png)

   如果您至少有檢視物件的檢視許可權，此動作會開啟Workfront物件頁面。 如果您有許可權，可以編輯Workfront物件的相關資訊。

1. （可選）從Maestro記錄型別的表格檢視中，暫留在連結Workfront物件的欄標題上，然後按一下下拉式功能表，然後按一下 **編輯查閱欄位**.

1. 從新增Workfront物件欄位 **未選取的欄位** 區域

   或

   從移除Workfront物件欄位 **選取的欄位** 區域。

   這會從Maestro記錄中新增或移除連結欄位。 與已移除欄位相關聯的資訊仍保留在Workfront中。


### 將Maestro記錄連線到Adobe Experience Manager物件

<!--when we will have more applications to link to from Maestro, change the title to something like: Connect Maestro records to objects from other applications-->

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

1. （選用）按一下 **新記錄** 以將新記錄新增至您選取的記錄型別。 如需詳細資訊，請參閱 [建立記錄](../../maestro/records/create-records.md).
1. （視條件而定）將選取的記錄型別與Experience Manager Assets連線後，請移至連結物件欄，將游標停留在您要與Experience Manager中其他物件連結之記錄對應的儲存格上，然後按一下 **+** 圖示。

   >[!TIP]
   >
   >  您可以新增，按一下 **+** 圖示加以存取（在Maestro記錄的「詳細資訊」頁面中，位於連結物件欄位中），以將資產連結至記錄。

   此 **選取資產** 方塊隨即顯示。 <!--we might change this to Connect assets-->

   ![](assets/select-assets-box-for-aem-record-connections.png)

1. 按一下以選取下列部分資產型別：

   * 影像
   * 資料夾

   您可以選取多個資產。

   >[!IMPORTANT]
   >
   > 您只能連線您有權在Experience Manager中檢視的資產。 連線之後，所有Maestro使用者都可以在Maestro中檢視資產，無論他們在Experience Manager Assets中是否具備存取權。

1. 按一下 **選取**. <!-- we might change this to Connect-->

   新增下列專案：

   * 選取的Experience Manager資產會新增至連結的記錄欄位。
   * 連結欄位（或查詢欄位）會填入Experience Manager連線資產的資訊。

     Experience Manager資產欄位中的任何現有資訊都會自動顯示在連結或查詢欄位中。

     >[!TIP]
     >
     >* 如果您啟用「允許多筆記錄」設定，則多個物件的值會以逗號區隔，或根據您選擇的彙總器彙總。
     >
     >* 在Experience Manager Assets應用程式中，不會針對連結的Experience Manager資產建立連結至Maestro連結記錄的連結記錄欄位。

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

1. （可選）若要以Experience Manager開啟Experience Manager資產記錄「詳細資訊」頁面，請移至您要連結之記錄的「Maestro記錄型別」頁面，按一下連結記錄欄位中的資產名稱以開啟快顯視窗，然後按一下 **開啟** 圖示 ![](assets/open-asset-icon.png) 以開啟資產。

   如此即會在Adobe Experience Manager Assets中開啟Experience Manager資產。

1. （可選）從Maestro記錄型別的表格檢視中，暫留在連結Experience Manager資產的欄標題上，然後按一下下拉式功能表，然後按一下 **編輯查閱欄位**.

1. 從新增Experience Manager Assets物件欄位 **未選取的欄位** 區域

   或

   從移除Workfront物件欄位 **選取的欄位** 區域。

   這會從Maestro記錄中新增或移除連結欄位。 與已移除欄位相關的資訊仍保留在Adobe Experience Assets中。
