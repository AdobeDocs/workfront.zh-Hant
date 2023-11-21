---
title: 連線記錄
description: 在記錄型別之間建立連線後，可以將個別記錄彼此連線。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 17796cdc-6de8-4209-a5af-b255dc64d70a
source-git-commit: d3c22c84a9b246d1a45853c5d2825241f58bebe9
workflow-type: tm+mt
source-wordcount: '1975'
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
<!--udpate the metadata with real information when making this available in TOC and in the left nav-->

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

  <!--when you add more objects, fix the Access Requirements below which right now refer only to projects-->

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
   <td><p>任何，若要建立Maestro記錄</p> 
<p>工作或更高以在Workfront中檢視專案</p>
  <p>如需詳細資訊，請參閱 <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md">Adobe Workfront授權總覽</a>.</p> 
  </td>
  </tr>
  <tr>
   <td role="rowheader">存取層級</td>
   <td> <p>任何，若要建立Maestro記錄</p>
<p>檢視專案、Portfolio、方案的或更高存取權</p> 
<p>檢視使用者不屬於的群組或公司時，對群組和公司的額外存取權</p>   
</td>
  </tr>
<tr>
   <td role="rowheader"><p>物件許可權</p></td>
   <td> <p>檢視您想要與Maestro記錄連結的物件或更高許可權  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>版面配置範本</p></td>
   <td> <p>您的系統管理員必須在您的版面配置範本中新增Maestro區域。 如需詳細資訊，請參閱 <a href="../access/grant-access.md">授與Adobe大師的存取權</a>. </p></td>
  </tr>
 </tbody>
</table>

<!--
After permssions - replace the table with: 

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Adobe product</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the Adobe Maestro closed beta program. Contact your account representative to inquire about this new offering. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license</p></td>
   <td>
   <p>Any</p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level</p></td>
   <td> <p>Any</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your Workfront or group administrator must add the Maestro area in your layout template. For information, see <a href="../access/grant-access.md">Grant access to Adobe Maestro</a>. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>Manage permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
</td>
  </tr>
 </tbody>
</table>

-->

<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->

## 連線記錄

### 有關連線記錄的考量事項

* 建立記錄型別之間的連線後，連線的記錄型別會在連結它們的記錄型別表格中顯示為連結的記錄欄位。
* 您可以從連結記錄欄位中瀏覽並新增連結記錄的記錄和物件以及物件型別。
* 您可以將連結的記錄型別的欄位新增至您正在連結的記錄型別的表格。
* 您無法手動更新連結來源記錄之連結欄位的值。

  連結記錄中連結欄位的值會自動填入您連結的Maestro記錄。

* 所有可以存取Maestro的人都可以看到您在Maestro記錄之間或Maestro記錄與Workfront物件之間的連線。 此外，您也可以檢視及編輯其他人的連線。 <!--add that this is based on your permissions in both Maestro and Workfront (or, later, any other application)-->
* 您可以將一個Maestro記錄連線到另一個應用程式的一個或多個物件。
* 您無法連線分類來記錄型別，或從其他應用程式連線物件。 <!-- this is temporary; there will be certain objects (teams, etc) that will be linked to taxonomies, per Lilit-->
* 若要將Maestro記錄與Workfront物件連結，您必須具備下列條件：

   * Workfront物件。 例如，您必須先在Workfront中建立專案、投資組合、方案、公司或群組。
   * Maestro工作區、記錄型別和記錄。 如需詳細資訊，請參閱下列文章：

      * [建立工作區](../architecture/create-workspaces.md)
      * [建立記錄型別](../architecture/create-record-types.md)
      * [建立記錄](../records/create-records.md)

   * 記錄型別之間的連線，或記錄型別與其他應用程式物件之間的連線。 如需詳細資訊，請參閱 [連線記錄型別](../architecture/connect-record-types.md)

### 連線大師記錄

1. 按一下 **主要功能表** 圖示 ![](assets/main-menu-workfront.png) 位於Workfront右上角，或 **主功能表** 圖示 ![](assets/main-menu-shell.png)  （如果有的話）按一下 **大師** ![](assets/maestro-icon.png).

   根據預設，上次存取的工作區應該會開啟。

1. （可選）展開現有工作區名稱右側的向下箭頭，並選取您要連線記錄的工作區。
1. 按一下記錄型別的卡片以開啟記錄型別頁面。
1. 選取 **表格** 從檢視 **檢視** 記錄型別頁面右上角的下拉式功能表。
1. 從選取的記錄型別新增連線至其他記錄或物件型別。 如需詳細資訊，請參閱 [連線記錄型別](../architecture/connect-record-types.md).

   表格中會新增一欄，以顯示連結的記錄型別。

1. 將記錄新增至表格中，以將記錄新增至您選取的記錄型別。 如需詳細資訊，請參閱 [建立記錄](../../maestro/records/create-records.md).
1. 從表格檢視中列出的記錄，移至連結的記錄欄，並將游標停留在您要與其他Maestro記錄連結之記錄的對應儲存格上，然後按一下 **+** 圖示。

   此 **連線物件** 方塊隨即顯示。

   ![](assets/connected-objects-table-for-records.png)

1. 開始在搜尋方塊中輸入記錄名稱，然後在清單中顯示記錄時選取記錄

   或

   在方塊中選取一或多個記錄的名稱，然後按一下 **連線物件** 在「連線物件」方塊的右上角。

   新增下列專案：

   * 連結的記錄會顯示在您在步驟3中所選記錄的連結記錄欄位中。 更新連結的記錄會自動更新您連結之記錄的連結記錄欄位。 <!--ensure the number of the step stays accurate-->
   * 屬於連結記錄的連結欄位會自動填入原始連結記錄的資訊。 您無法手動編輯連結的欄位。

     >[!TIP]
     >
     >* 我們會交替使用「連結欄位」和「查詢欄位」。
     >
     >* 如果在連線記錄型別時啟用了「允許多筆記錄」設定，則多個選定物件的欄位值會以逗號分隔顯示，或根據您選擇的彙總器彙總。

1. （可選）關閉Maestro記錄型別頁面，然後移至您選取的工作區。
1. 按一下您所連結之記錄型別的卡片。

   例如，如果您將Campaign記錄與產品記錄連線，請按一下 **產品** 卡片。

   記錄型別卡片應在「表格」檢視中開啟。

   請注意，「促銷活動連結記錄」欄位會顯示您在「產品記錄」型別頁面中連結至產品的促銷活動名稱。 更新行銷活動資訊會自動更新產品記錄型別的行銷活動連結記錄欄位。

### 將Maestro記錄連線到Workfront物件

<!--when we will have more applications to link to from Maestro, change the title to soemthing like: Connect Maestro records to objects from other applications-->

在Maestro記錄型別和Workfront物件型別之間建立連線後，您可以將個別Maestro記錄連線到Workfront中的物件。 您也可以將欄位從Workfront物件連線至Maestro記錄型別。

1. 按一下 **主要功能表** 圖示 ![](assets/main-menu-workfront.png) 位於Workfront右上角，或 **主功能表** 圖示 ![](assets/main-menu-shell.png)  （如果有的話）按一下 **大師** ![](assets/maestro-icon.png).

   根據預設，上次存取的工作區應該會開啟。

1. （可選）展開現有工作區名稱右側的向下箭頭，並選取您要連線記錄的工作區。
1. 按一下記錄型別的卡片以開啟記錄型別頁面。
1. 從「 」中選取「表格」檢視 **檢視** 記錄型別頁面右上角的下拉式功能表。
1. 從Workfront將新的連線新增至所選記錄型別的物件型別。 從Workfront區段下的下列物件中選取：

   * 專案
   * 專案組合
   * 方案
   * 公司
   * 群組

   如需詳細資訊，請參閱 [連線記錄型別](../architecture/connect-record-types.md).

   表格中會新增一欄，以顯示連結物件型別。

1. 將個別記錄新增至表格中，以將個別記錄新增至您選取的記錄型別。 如需詳細資訊，請參閱 [建立記錄](../../maestro/records/create-records.md).
1. 從表格檢視中列出的記錄，移至連結物件欄，將游標停留在您要與Workfront中其他物件連結之記錄對應的儲存格上，然後按一下 **+** 圖示。 <!--change Workfront to other applications, when this will be possible-->

   此 **連線物件** 方塊隨即顯示。

   ![](assets/connect-objects-box-to-select-projects.png)

1. 開始在搜尋方塊中輸入Workfront物件的名稱，然後在其顯示在清單中時選取它

   或

   在方塊中選取一或多個物件的名稱，然後按一下 **連線物件** 在「連線物件」方塊的右上角。

   下列專案已新增至Maestro：

   * 選取的Workfront物件會新增至連結的記錄欄位。
   * 將連結欄位新增至連結記錄時，會針對您選取的每個連結欄位建立新的連結欄位（或查詢欄位）。
   * 名為「Workfront物件」的新記錄型別會建立在與您連結的Maestro記錄相同的工作區中。 物件的名稱是此記錄型別名稱的一部分。 例如，連結至Workfront專案會在Maestro中建立Workfront專案記錄型別。

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
     >* 連結的Workfront物件不會建立連結至Maestro連結記錄的連結記錄欄位。


1. （可選）關閉Maestro記錄型別頁面，然後移至您選取的工作區。
1. 按一下Workfront物件記錄型別的卡片。 例如，按一下 **Workfront專案** 卡片，如果您連結至Workfront專案。 唯讀Workfront記錄型別卡片應在表格檢視中開啟。

   >[!NOTE]
   >
   >    * Workfront記錄型別頁面中列出的記錄是唯讀的Workfront物件。 從Workfront記錄型別連結的欄位也會顯示為唯讀欄，且在Workfront中填入欄位時自動填入。
   >    * 您無法在Maestro中手動更新Workfront欄位。 Workfront物件欄位必須填入Workfront，且欄位值會自動顯示在Maestro的Workfront記錄中。
   >
   >    * 若要在「時間軸」檢視中顯示Workfront物件記錄型別，唯讀Workfront記錄型別頁面的「表格」檢視中必須至少顯示兩個日期欄位。

1. （可選）若要在Maestro中開啟Workfront物件記錄「詳細資訊」頁面，請執行下列任一項作業：

   * 從您連結的記錄型別中，前往Workfront物件連結的記錄欄位，然後按一下Workfront物件的名稱。
   * 從 **表格** 檢視Workfront記錄型別頁面，按一下Workfront物件的名稱

     或

     按一下 **更多** Workfront物件名稱右側的功能表，然後按一下 **檢視**.

     ![](assets/workfront-object-more-menu-in-table-with-go-to-source-link.png)

   這會開啟連結Workfront物件的「Maestro詳細資訊」頁面。 這是唯讀頁面。

1. （可選）若要在Workfront中開啟連結的Workfront物件，請執行下列任一項作業：

   * 從 **表格** 檢視Workfront記錄型別頁面，按一下Workfront物件的名稱，

   或

   按一下 **更多** Workfront物件名稱右側的功能表，然後按一下 **移至來源**.

   ![](assets/workfront-project-maestro-details-page-with-go-to-source-link.png)

   這會開啟Workfront物件頁面。 如果您有許可權，可以編輯Workfront物件的相關資訊。

1. （可選）按一下 **新增欄位** 圖示 ![](assets/add-fields-icon.png) 在「Workfront記錄型別」頁面的「表格檢視」右上角，新增或移除Workfront記錄型別中的Workfront欄位。

   >[!NOTE]
   >
   >  您在Workfront物件記錄型別頁面中新增或移除的欄位，不會從連結至Workfront物件型別的Maestro記錄型別中新增或移除。 這些欄位僅在唯讀的Workfront記錄型別頁面上可見，因此您可以在Maestro中檢視它們。

1. （選擇性和條件性）如果您將至少兩個日期欄位新增至Workfront物件，請按一下 **檢視** Workfront物件記錄型別頁面中的下拉式功能表，然後選取 **時間表** 檢視。 Workfront連結物件會顯示在時間軸檢視中。
