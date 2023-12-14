---
title: 連線記錄型別
description: 指示個別記錄型別如何彼此關聯的一種方法是連線它們。 此外，您也可以將Maestro記錄型別與其他應用程式的物件型別連線起來，以強化使用者的體驗，並將他們的焦點放在一個應用程式中。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: ae794ebe-4597-47a4-9ef3-3f4d31cb70c2
source-git-commit: a74f9f8940a170d8e1347fd99ff2a6c816b12eca
workflow-type: tm+mt
source-wordcount: '1941'
ht-degree: 0%

---

<!-----
title: Connect record types
description: A way to indicate how individual record types relate to one another is to connect them. Also, you can connect Maestro record types with object types from other applications to enhance your users' experience and keep their focus in one application.
hidefromtoc: yes
hide: yes
feature: Work management
role: User
author: Alina
--->

<!--update the metadata with real information when making this avilable in TOC and in the left nav-->
<!--************ THIS MIGHT NO LONGER BE A 'RELATIONSHIP' TYPE FIELD, BECAUSE THEY WILL SHOW IT IN THE CONNECTION TAB*****************************-->


# 連線記錄型別

>[!IMPORTANT]
>
>本文資訊是指Adobe Maestro，這是Adobe Workfront的新產品。
>
>目前，Adobe大師是測試版計畫的一部分，向有限數量的客戶開放。 您必須是Workfront客戶才能使用Maestro功能。
>
>如需加入Maestro測試版計畫的詳細資訊，請聯絡您的客戶代表。
>
>如需詳細資訊，請參閱 [Adobe大師概觀](../maestro-overview.md).

您可以使用Adobe Maestro來設計包含貴組織所需記錄型別的完全可自訂工作區。 指示個別記錄型別如何彼此關聯的一種方法是連線它們。 此外，您也可以將Maestro記錄型別與其他應用程式的物件型別連線起來，以強化使用者的體驗，並將他們的焦點放在一個應用程式中。

您可以連線下列專案：

* Maestro作業記錄型別
* 將主要作業記錄型別轉換為分類記錄型別
* 作業記錄型別的主要分類型別
* 來自其他應用程式的大型作業記錄型別和物件型別。

這樣，您就可以在另一個Maestro記錄上顯示連結記錄或物件型別的欄位。

本文說明如何將兩個Maestro記錄型別或Maestro記錄型別與另一個應用程式的物件連線。

建立記錄或物件型別之間的連線後，您就可以將個別記錄彼此連線。

如需有關將Maestro記錄從另一個應用程式連線到物件的資訊，請參閱 [連線記錄](../records/connect-records.md).

如需連線記錄型別的範例，請參閱 [連線記錄型別和記錄的範例](../architecture/example-connect-record-types-and-records.md).

<!--ensure this last linked article is right; the title and the link should have changed-->

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
   <p> Adobe產品</p> </td>
   <td>
   <p> Adobe Workfront</p> 
   <p>若要將Maestro記錄型別與Experience Manager Assets連線，您必須擁有Adobe Experience Manager Assets</p>
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
   <p> Adobe Workfront</p> <p>To connect Maestro record types with Experience Manager Assets, you must have an Adobe Experience Manager Assets</p> </td>
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
   <p>System Administrators have permissions to all workspaces, including the ones they did not create
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


## 有關連線記錄型別的考量事項

請考量下列事項：

* 您可以在Maestro中連線下列實體：

   * 兩種作業記錄型別
   * 兩種分類
   * 作業記錄型別和分類法
   * 來自其他應用程式的作業記錄型別和物件型別。

     >[!TIP]
     >
     >    您無法將分類記錄型別連線到作業記錄型別，或從另一個應用程式連線到物件型別。

* 您可以連線下列具有Maestro記錄型別的應用程式的物件：

   * Adobe Workfront：

      * 專案
      * 專案組合
      * 計劃
      * 公司
      * 群組

   * Adobe Experience Manager Assets：

      * 資產
      * 資料夾
      * 集合

* 將記錄型別與另一個記錄型別或另一個應用程式的物件型別連線後，就會出現下列情況：

   * 當您連線兩種記錄型別時：「已連結」記錄欄位會在您連線的記錄型別上建立。 類似的連結記錄欄位會在您連線的記錄型別上建立。

     例如，如果您將「促銷活動」記錄型別與「產品」記錄型別連結，您會為「促銷活動」記錄型別建立名為「連結的產品」的連結記錄欄位，並為「產品」記錄型別建立自動名為「促銷活動」的連結記錄型別。

   * 使用分類法連線記錄型別欄位時：連結的記錄欄位會在您連線的記錄型別上建立。 您連線的分類法上不會建立任何連結的記錄欄位。

     例如，如果您將「行銷活動」記錄型別與「對象」分類記錄型別連結，您命名為「連結的對象」的連結記錄欄位就會建立在行銷活動記錄型別上。 在對象分類記錄型別上不會建立自動命名為「Campaign」的連結記錄欄位。 <!--this might be temporary-->

   * 當您用另一個應用程式的物件型別連線記錄型別欄位時：連結的記錄欄位會在您連線的記錄型別上建立。 Workfront中的Workfront專案不會自動建立任何連結的記錄欄位。 只有當實際物件連線到Maestro記錄時，才會在Workfront物件記錄型別上建立連結記錄欄位。

     如需詳細資訊，請參閱 [連線記錄](../records/connect-records.md).

* 連線記錄型別之後，您可以將一個記錄型別的多個欄位連線到另一個記錄型別。 我們將這些欄位稱為「連結欄位」或「查詢欄位」。
* 連結的記錄欄位前面有關係圖示 ![](assets/relationship-field-icon.png).
* 為記錄型別建立個別記錄後，您可以從連結的記錄型別欄位中選取連線的記錄。 如需詳細資訊，請參閱 [連線記錄](../records/connect-records.md).
* 您無法從連結的記錄型別編輯連結欄位的資訊，因為當您選取連結的記錄時，連結欄位就會自動從原始記錄型別填入。

## 連線記錄型別

<!--when changes here, also update the article for "Connect records"-->

1. 按一下 **[!UICONTROL 主要功能表]** 圖示 ![主要功能表](assets/dots-main-menu.png) 在Adobe Workfront的右上角，或（如果有的話）按一下 **[!UICONTROL 主要功能表]** 圖示 ![主要功能表](assets/lines-main-menu.png) 然後按一下「 」 **[!UICONTROL 大師]**.

   根據預設，上次存取的工作區應該會開啟。

1. （可選）展開現有工作區名稱右側的向下箭頭，並選取您要連線記錄型別的工作區。
1. 按一下記錄型別的卡片以開啟記錄型別頁面。
1. 按一下 **+** 圖示並按一下 **新連線** 標籤。

   ![](assets/new-connection-tab-with-workfront-aem-options.png)

1. 在 **記錄型別** 欄位中，選取下列其中一項： <!--is the field name spelled right? lowercase "t"?-->

   * 您選取之工作區的另一個作業記錄型別
   * 來自所選工作區的分類法
   * Workfront物件型別區段中的專案、Portfolio、方案、公司或群組。
   * Adobe應用程式區段中的Experience Manager Assets 。

   ![](assets/new-connection-tab-fields-with-another-record-selected.png)

   >[!TIP]
   >
   > 只有所選工作區的記錄型別和分類可供選取。

1. 更新下列資訊：

   * **名稱**：連線的欄位名稱，會顯示在原始記錄型別的表格檢視或「詳細資訊」頁面中。 這會在原始記錄型別的表格檢視或原始記錄的連結記錄欄位中建立連結記錄欄。 <!--ensure they updated this; and update the screen shot: it used to be "Label"-->

   >[!TIP]
   >
   >我們建議您將要連結的記錄名稱包含在已連線記錄欄位的名稱中，以擷取新欄位來自的記錄型別。 新連結的記錄欄位或其連結的欄位中看不到連結的記錄的名稱。

   * **說明**：有關連線記錄欄位的其他資訊。 當您將滑鼠游標停留在表格中的欄位欄位上時，會顯示欄位說明。
   * **允許多筆記錄**：選取此選項以表示您允許使用者在原始記錄上顯示「連結的記錄型別」欄位時新增多個記錄。 依預設會選取此選項。
   * **選取查閱欄位**：選取此選項，從選取的記錄型別新增欄位。 依預設會選取此選項。

1. （條件式與選擇性）如果您已選取連線Workfront物件，請選取 **自訂表格** 從 **僅連結符合這些條件的專案** 區段。 <!--this needs to be updated for each object when they fix this UI.--> 只有已附加所選自訂表單的物件才能連結至所選的Maestro記錄型別。 您可以選取多個表單。

   ![](assets/workfront-project-connection-selection.png)

1. （視條件而定）如果您已選取連線至Experience Manager Assets，請從 **Experience Manager存放庫** 中的下拉式功能表 **從下列存放庫連結資產** 區段。 這是必填欄位。 此欄位只會顯示您在Experience Manager Assets中有權存取的存放庫。

   ![](assets/aem-assets-connection-selection.png)

1. 按一下「**建立**」。

1. （視條件而定）如果您已選取 **選取查閱欄位** 在上一步中設定， **新增查詢欄位** 方塊開啟。

   按一下 **+** 圖示以從新增欄位 **未選取的欄位** 區域。

   或

   按一下 **-** 圖示可移除中的欄位 **選取的欄位** 區域

   ![](assets/add-lookup-fields-for-another-maestro-record-type-box.png)

   >[!NOTE]
   >
   >如果您未選取任何欄位，則 **名稱** 是原始記錄表格檢視中唯一可見的欄位。 此 **名稱** 欄位無法移除。

1. （選擇性和條件性）如果您選取連結數字、貨幣、百分比或日期型別欄位，請同時選取彙總值。 當使用者在連結的記錄欄位中選取多個連結的記錄時，連結欄位的值會根據您選擇的彙總器，以逗號分隔或顯示為彙總值。

   ![](assets/aggregator-drop-down-for-number-linked-field.png)

   >[!NOTE]
   >
   > 將記錄型別連線至Experience Manager Assets時，無法使用彙總器。

   從下列選項中選取：

   * **無**：顯示來自多筆記錄的值，並以逗號分隔。 這是預設選取範圍。
   * **MAX**：顯示連結記錄欄位中，來自多筆記錄之所有值的最高值。
   * **MIN**：顯示在連結的記錄欄位中，從多個記錄中選取之所有值的最低值。
   * **SUM**：顯示在連結的記錄欄位中，來自多個記錄的所有值總計。
   * **平均**：顯示連結記錄欄位中，來自多筆記錄之所有值的平均值。

   >[!NOTE]
   >
   >例如，您可以從Campaign記錄（原始記錄）連結產品記錄（連結記錄），並將其命名為「產品欄位」。 您也可以選擇從行銷活動記錄連結產品記錄的「預算」欄位，並將其稱為「產品預算」。 如果您允許在「產品欄位」中選取多個記錄，則可以選取預算為$120,000的產品1和預算為$100,000的產品2。 您可以在連結欄位中檢視原始記錄的下列「預算」資訊（視您選擇的彙總而定）：
   >
   >* **無**： $120,000， $100,000
   >* **MAX**： $120,000
   >* **MIN**： $100,000
   >* **SUM**：$220,000
   >* **平均**： $110,000
   >

1. （選用）使用 **搜尋** 圖示 ![](assets/search-icon.png) 以搜尋欄位。

1. （選用）按一下 **略過** 如果您不想從連線的記錄型別新增任何欄位。

1. 按一下 **新增欄位** 以儲存變更。

   已新增下列專案：

   * 在您手動新增連結的記錄型別後，將顯示連結的記錄欄位。 連結的記錄欄位名稱是您在步驟6中選取的名稱。 <!-- ensure this is still accurate-->

   * 在您手動新增連結記錄欄位中的記錄後，將顯示連結記錄型別欄位資訊的連結欄位。 連結的欄位僅在 **選取查閱欄位** 建立連線時會選取「設定」。 連結的欄位會根據以下模式命名：

     `<Name of the original field on the linked record> (from <Name of your linked field>)`

   * 您要連結的記錄型別上的連結記錄欄位。 連結的記錄型別上連結的記錄欄位名稱是您連結的記錄型別名稱。

     例如，如果您從「行銷活動」記錄型別連結「產品」記錄型別，並將行銷活動的已連線欄位命名為「連結的產品」，則會為「產品」記錄型別建立「行銷活動」連結記錄欄位。

1. （選擇性）從原始記錄型別或連結記錄型別表格檢視中，按一下連結記錄欄位標題中的向下箭頭，然後按一下下列其中一項：

   * **編輯欄位**：您只能更新 **名稱** 和 **說明** 欄位資訊。
   * **編輯查閱欄位**：新增或移除任何連結記錄的欄位。

   ![](assets/edit-field-and-lookup-fields-drop-down-menu-in-table-column.png)

   若要新增或移除查詢欄位，請遵循上述步驟7-12中的指示。 <!--ensure these step numbers stay accurate-->

1. （可選）從您要連結的記錄型別中，按一下連結的記錄欄位標題中的向下箭頭，然後按一下 **刪除**.

   記錄欄位和任何其他連結的查閱欄位都會刪除，而且欄位及其資訊無法復原。

   >[!TIP]
   >
   >    您連結的記錄型別上的連結記錄欄位不會刪除。 <!-- is this still accurate?! -->
