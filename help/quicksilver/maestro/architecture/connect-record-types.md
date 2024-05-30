---
title: 連線記錄型別
description: 指示個別記錄型別如何彼此關聯的一種方法是連線它們。 此外，您可以將Adobe Workfront Planning記錄型別與其他應用程式的物件型別連線起來，以增強您的使用者體驗，並將他們的焦點放在一個應用程式中。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: ae794ebe-4597-47a4-9ef3-3f4d31cb70c2
source-git-commit: 49335ec86057e4985477034558a271bf4efcab5e
workflow-type: tm+mt
source-wordcount: '2253'
ht-degree: 0%

---

<!-----
title: Connect record types
description: A way to indicate how individual record types relate to one another is to connect them. Also, you can connect Adobe Workfront Planning record types with object types from other applications to enhance your users' experience and keep their focus in one application.
hidefromtoc: yes
hide: yes
feature: Work management
role: User
author: Alina
--->

<!--update the metadata with real information when making this avilable in TOC and in the left nav-->
<!--************ THIS MIGHT NO LONGER BE A 'RELATIONSHIP' TYPE FIELD, BECAUSE THEY WILL SHOW IT IN THE CONNECTION TAB*****************************-->


# 連線記錄型別

{{planning-important-intro}}

您可以使用Adobe Workfront Planning來設計包含組織所需記錄型別的完全可自訂工作區。 指示個別記錄型別如何彼此關聯的一種方法是連線它們。 此外，您可以將Workfront Planning記錄型別與其他應用程式的物件型別連線起來，以增強您的使用者體驗，並將他們的焦點放在一個應用程式中。

您可以將記錄型別連結到其他應用程式，或使用其他應用程式的物件型別來記錄型別。

透過這樣做，您可以在Workfront Planning記錄上顯示連結記錄或物件型別的欄位。

本文說明如何在Workfront Planning中將兩種記錄型別或一種記錄型別與其他應用程式的物件連線。

在記錄或物件型別之間建立連線後，可以將個別記錄彼此連線。

如需有關將Workfront Planning記錄從另一個應用程式連線至物件的資訊，請參閱 [連線記錄](../records/connect-records.md).

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
   <p> 產品</p> </td>
   <td>
   <p> Adobe Workfront</p> <p>若要將Adobe Workfront Planning記錄型別與Experience Manager Assets連線，您必須擁有Adobe Experience Manager Assets授權，且貴組織的Workfront執行個體必須上線至Adobe統一體驗。 如需詳細資訊，請參閱 <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Workfront的AdobeUnified Experience</a>.</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront合約</p></td>
   <td>
<p>貴組織必須註冊Adobe Workfront Planning封閉測試版計畫。 請聯絡您的客戶代表以查詢此新產品/服務。 </p>
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
   <td> <p>Adobe Workfront Planning沒有存取層級控制</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>版面配置範本</p></td>
   <td> <p>您的Workfront或群組管理員必須在版面配置範本中新增Planning區域。 如需詳細資訊，請參閱 <a href="../access/access-overview.md">存取權總覽</a>. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>權限</p></td>
   <td> <p>管理工作區的許可權</a> </p>  
   <p>系統管理員擁有所有工作區的許可權，包括他們未建立的工作區。
</td>
  </tr>
 </tbody>
</table>

<!--Maybe enable this at GA - but planing is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->


## 有關連線記錄型別的考量事項

* 您可以在Adobe Workfront Planning中連線下列實體：

   * 兩種記錄型別

     記錄型別必須屬於相同的工作區。
   * 來自另一個應用程式的記錄型別和物件型別。

* 您可以使用以下應用程式中的以下物件型別與Workfront Planning記錄型別連線：

   * Adobe Workfront：

      * 專案
      * 專案組合
      * 計劃
      * 公司
      * 群組

   * Adobe Experience Manager Assets：

      * 影像
      * 資料夾

     >[!IMPORTANT]
     >
     >您必須擁有Adobe Experience Manager Assets授權，且貴組織的Workfront執行個體必須上線至Adobe商業平台或Adobe Admin Console，才能將Workfront Planning記錄連線至Adobe Experience Manager Assets。
     >
     >如果您對上線Adobe Admin Console有任何疑問，請參閱 [Adobe Unified Experience常見問題集](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/unified-experience-faq.md).

* 為記錄型別建立個別記錄後，您可以從連結的記錄型別欄位中選取連線的記錄。 如需詳細資訊，請參閱 [連線記錄](../records/connect-records.md).

* 將記錄型別與另一個記錄型別或另一個應用程式的物件型別連線後，就會出現下列情況：

   * **當您連線兩種記錄型別時**：連結的記錄欄位會在您連線的記錄型別上建立。 類似的連結記錄欄位會在您連線的記錄型別上建立。

     例如，如果您將「促銷活動」記錄型別與「產品」記錄型別連結，您會為「促銷活動」記錄型別建立名為「連結的產品」的連結記錄欄位，並為「產品」記錄型別建立自動名為「促銷活動」的連結記錄型別。

   * **當您從另一個應用程式將記錄型別與物件型別連線時**：連結的記錄欄位會在您連線的記錄型別上建立。 不會在其他應用程式的物件型別上自動建立任何連結的記錄欄位。

     只有當實際物件連線至Workfront Planning記錄時，才會為其他應用程式的物件建立新的Workfront Planning唯讀記錄型別。

     如需詳細資訊，請參閱 [連線記錄](../records/connect-records.md).

   * **當您新增您所連線之記錄或物件的查閱欄位時**：您可以將其他應用程式物件的欄位連線至Workfront Planning記錄型別。 這些是連結或查詢欄位。 連結的欄位會在您連線記錄或物件時，自動顯示已連線記錄或物件的資訊。 連結的查閱欄位永遠是唯讀的，而且會自動填入連線記錄或物件的值。

     例如，如果您將「行銷活動」記錄型別與Workfront專案連線，並且選擇將專案的「計畫完成日期」欄位帶入Workfront計畫記錄，則系統會自動為行銷活動建立名為「計畫完成日期」（來自「專案」）的連結欄位。 您無法手動編輯此連結的欄位。 計畫完成日期（來自專案）欄位會顯示連結專案的計畫完成日期。

     >[!IMPORTANT]
     >
     >    擁有工作區檢視或更高許可權的所有人都可以檢視連結欄位中的資訊，無論其在連結物件型別應用程式中的許可權或存取層級為何。

* 連結的記錄欄位前面有關係圖示 ![](assets/relationship-field-icon.png).

  連結的欄位前面有識別欄位型別的圖示。 例如，指示欄位是數字、段落或日期的圖示。

## 連線記錄型別

<!--when changes here, also update the article for "Connect records"-->

{{step1-to-maestro}}

根據預設，上次存取的工作區應該會開啟。

1. （可選）展開現有工作區名稱右側的向下箭頭，並選取您要連線記錄型別的工作區。
1. 按一下記錄型別的卡片以開啟記錄型別頁面。
1. 按一下 **+** 圖示並按一下 **新連線** 標籤。

   ![](assets/new-connection-tab-with-workfront-aem-options.png)

1. 在 **記錄型別** 欄位，搜尋記錄型別，或選取下列其中一項：

   * 來自所選工作區區段的其他記錄型別

     >[!TIP]
     >
     >您選取的工作區中只有記錄型別可供連線。
     > 
     >如果您在選取的工作區中沒有其他記錄型別，工作區區段不會顯示。

   * A **專案、Portfolio、計畫、公司**，或 **群組** 從 **Workfront物件型別** 區段。
   * **Experience Manager Assets** 從 **Adobe應用程式** 區段。

   ![](assets/new-connection-tab-fields-with-another-record-selected.png)


1. 更新下列資訊：

   * **名稱**：已連線的欄位名稱，會顯示在原始記錄型別的表格檢視或記錄頁面中。 這會在原始記錄型別的表格檢視或原始記錄的連結記錄欄位中建立連結記錄欄。

   >[!TIP]
   >
   >我們建議您將要連結的記錄名稱包含在已連線記錄欄位的名稱中，以擷取新欄位來自的記錄型別。 新連結的記錄欄位或其連結的欄位中看不到連結的記錄的名稱。

   * **說明**：有關連線記錄欄位的其他資訊。 當您將滑鼠游標停留在表格中的欄位欄位上時，會顯示欄位說明。
   * **允許多筆記錄**：選取此選項以表示您允許使用者在原始記錄上顯示「連結的記錄型別」欄位時新增多個記錄。 依預設會選取此選項。
   * **選取查閱欄位**：選取此選項，從選取的記錄型別新增欄位。 查閱欄位是與您要連結的記錄或物件型別相關聯的欄位。 連結它們會顯示您連結的記錄或物件在您所連結的記錄上的資訊。 依預設會選取此選項。

1. （條件式與選擇性）如果您已選取連線Workfront物件，請選取 **自訂表格** 從 **僅連結符合這些條件的物件** 區段。 只有已附加所選自訂表單的物件才能連結至所選記錄型別。 您可以選取多個表單。

   ![](assets/workfront-project-connection-selection.png)

   >[!NOTE]
   >
   > 您必須先在Workfront中為選取的物件建立自訂表單，這些表單才會顯示在此清單中。

1. （視條件而定）如果您已選取連線至Experience Manager Assets，請從 **Experience Manager存放庫** 中的下拉式功能表 **從下列存放庫連結資產** 區段。 這是必填欄位。 此欄位只會顯示您在Experience Manager Assets中有權存取的存放庫。

   <!--replace the screen shot below when they fix the permissions info icon bug-->

   ![](assets/aem-assets-connection-selection.png)

1. 按一下「**建立**」。

1. （視條件而定）如果您已選取 **選取查閱欄位** 設定， **新增查詢欄位** 方塊開啟。

   按一下 **+** 圖示以從新增欄位 **未選取的欄位** 區域。

   或

   按一下 **-** 圖示可移除中的欄位 **選取的欄位** 區域

   ![](assets/add-lookup-fields-for-another-maestro-record-type-box.png)

   連結記錄或物件後，所連線欄位的值會自動填入。

   >[!IMPORTANT]
   >
   >    擁有工作區檢視或更高許可權的所有人都可以檢視連結欄位中的資訊，無論其在連結物件型別應用程式中的許可權或存取層級為何。


1. （選用）按一下 **略過** 並且不要從連結的記錄或物件新增任何欄位。 此 **名稱** 是原始記錄表格檢視中唯一可見的欄位。

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
   * **獨特**：從查詢欄位值中移除重複專案，並僅顯示唯一值。 下列欄位型別無法使用此選項：
      * 段落
      * 核取方塊
      * 人員

   >[!NOTE]
   >
   >例如，您可以從Campaign記錄（原始記錄）連結產品記錄（連結記錄），並將其命名為「產品欄位」。 您也可以選擇從行銷活動記錄連結產品記錄的「預算」欄位，並將其稱為「產品預算」。 如果您允許在「產品欄位」中選取多個記錄，您可以選取預算為$100,000的產品1和預算為$110,000的產品2，以及預算為$100,000的產品3。 您可以在連結欄位中檢視原始記錄的下列「預算」資訊（視您選擇的彙總而定）：
   >
   >* **無**： $100,000， $110,000， $100,000
   >* **MAX**： $110,000
   >* **MIN**： $100,000
   >* **SUM**： $310,000
   >* **平均**：$103,000.33
   >* **獨特**： $100,000
   >

1. （選用）使用 **搜尋** 圖示 ![](assets/search-icon.png) 以搜尋欄位。

1. 按一下 **新增欄位** 以儲存變更。

   已新增下列專案：

   * 您正在連結的記錄型別上的連結記錄欄位。 在您手動新增連結的記錄型別後，連結的記錄欄位將顯示連結的記錄型別的個別記錄。 如需新增記錄的資訊，請參閱 [連線記錄](/help/quicksilver/maestro/records/connect-records.md). 連結的記錄欄位名稱是您在步驟6中選取的名稱。 <!--accurate-->

   * 在連結記錄欄位中手動新增記錄或物件之後，顯示連結記錄或物件型別欄位資訊的連結欄位。 連結的欄位僅在 **選取查閱欄位** 建立連線時會選取「設定」。 連結的欄位會自動根據以下模式命名：

     `<Name of the original field on the linked record> (from <Name of your linked field>)`

     例如，如果您連結的「行銷活動」記錄型別具有「方案」記錄型別，且將「方案」連結的記錄欄位命名為「方案資訊」，然後選取以在「行銷活動」表格檢視中同時顯示「方案」的「預算」欄位，則連結的欄位會自動命名為 `Budget (from Program information)` 在行銷活動的表格檢視中。

   * 當您將記錄型別連結到彼此時，連結的記錄欄位也會新增到您連結到的記錄型別上。 連結的記錄型別上連結的記錄欄位名稱是您連結的記錄型別名稱。

     例如，如果您從「行銷活動」記錄型別連結「產品」記錄型別，並將行銷活動的已連線欄位命名為「連結的產品」，則會為「產品」記錄型別建立「行銷活動」連結記錄欄位。

     >[!TIP]
     >
     > 系統不會為其他應用程式的物件建立連結記錄欄位，以連結至您在Workfront Planning中連結的記錄型別。

1. （選擇性和條件性）在原始記錄型別或連結記錄型別表格檢視中，按一下連結記錄欄位標題中的向下箭頭，然後按一下下列其中一項：

   * **編輯欄位**：您只能更新 **名稱** 和 **說明** 欄位資訊。
   * **編輯查閱欄位**：新增或移除任何連結記錄的欄位。

   ![](assets/edit-field-and-lookup-fields-drop-down-menu-in-table-column.png)

   若要新增或移除查詢欄位，請遵循上述步驟10至14中的指示。 <!--ensure these step numbers stay accurate-->

   >[!NOTE]
   >
   > 您無法從其他應用程式新增屬於您正在連結至物件型別的記錄型別的查閱欄位。
   >
   > 例如，您無法將「促銷活動狀態」的查詢欄位新增至您正從促銷活動連結至的Workfront專案。

1. （可選）從連結的記錄型別中，按一下連結的記錄欄位標題或查閱欄位標題中的向下箭頭，然後按一下 **刪除**.

   記錄欄位或查詢欄位將會刪除。 如果您刪除記錄欄位，則與連結記錄關聯的任何查閱欄位也會被刪除。
