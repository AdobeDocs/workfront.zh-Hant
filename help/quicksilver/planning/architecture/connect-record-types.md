---
title: 連線記錄型別
description: 指示個別記錄型別如何彼此關聯的一種方法是連線它們。 此外，您可以將Adobe Workfront Planning記錄型別與其他應用程式的物件型別連線起來，以增強您的使用者體驗，並將他們的焦點放在一個應用程式中。
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: ae794ebe-4597-47a4-9ef3-3f4d31cb70c2
source-git-commit: f7ad56375c20e26b0d45ae0966e2e156b5a200f1
workflow-type: tm+mt
source-wordcount: '2248'
ht-degree: 1%

---


# 連線記錄型別

<!--<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview Sandbox environment.</span>-->

{{planning-important-intro}}

<!--
You can use Adobe Workfront Planning to design fully-customizable workspaces that contain record types needed in your organization. A way to indicate how individual record types relate to one another is to connect them. Also, you can connect Workfront Planning record types with object types from other applications to enhance your users' experience and keep their focus in one application. -->

您可以將記錄型別彼此連線，也可以將記錄型別與其他應用程式的物件型別連線。

本文說明如何將兩個Workfront Planning記錄型別或Workfront Planning記錄型別與其他應用程式的物件連線。

建立記錄或物件型別之間的連線後，您可以將個別記錄連線至彼此，並在Workfront Planning記錄上顯示連結記錄或物件型別的欄位。

如需連線型別的一般資訊，請參閱[連線記錄型別概觀](/help/quicksilver/planning/architecture/connect-record-types-overview.md)。

如需有關連線記錄或記錄與其他應用程式物件的資訊，請參閱[連線記錄](/help/quicksilver/planning/records/connect-records.md)。

如需連線記錄型別和記錄的範例，請參閱[連線記錄型別和記錄的範例](/help/quicksilver/planning/architecture/example-connect-record-types-and-records.md)。

<!--ensure this last linked article is right; the title and the link should have changed-->

## 存取需求

+++ 展開以檢視Workfront Planning的存取需求。

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
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront規劃<p></li>
   <li><p> Adobe Experience Manager Assets (如果要連線AEM資產與Planning記錄型別)<p>
   <p>您必須擁有Adobe Experience Manager Assets授權，以及AEM Assets與Workfront之間的整合。
    如需詳細資訊，請參閱<a href="/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/workfront-for-aem-asset-essentials.md">Experience Manager Assets與Assets Essentials的Adobe Workfront：文章索引</a>。 </p>
   </li>
   </ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront計畫*</p></td> 
   <td> 
<p>下列任一Workfront計畫：</p> 
<ul><li>選取</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>舊版Workfront計畫不提供Workfront計畫</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront規劃計畫*</p></td> 
   <td> 
<p>任何 </p> 
<p>如需每個Workfront計畫包含內容的詳細資訊，請聯絡您的Workfront客戶經理。 </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront平台</p></td> 
   <td> 
<p>貴組織的Workfront例項必須加入Adobe統一體驗，才能存取Workfront規劃的所有功能。</p> 
<p>如需詳細資訊，請參閱<a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Workfront的Adobe統一體驗</a>。 </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront授權*</p></td> 
   <td> <p>標準</p> 
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
   <td>   <p>管理工作區</a>的許可權 </p>  
   <p>系統管理員擁有所有工作區的許可權，包括他們未建立的工作區。</p></td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>版面配置範本</p></td> 
   <td> <p>必須為所有使用者(包括Workfront管理員)指派一個版面配置範本，該範本包含主功能表中的Planning區域 </p> </td> 
  </tr> 
</tbody> 
</table>

*如需Workfront存取需求的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

<!-- OLD: 

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Product</p> </td>
   <td>
   <p> Adobe Workfront</p> 
   <p> Adobe Workfront Planning</p>
   <p>To connect Adobe Workfront Planning record types with Experience Manager Assets, you must have an Adobe Experience Manager Assets license and your organization's instance of Workfront must be onboarded to the Adobe Unified Experience. For information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>.</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the early access stage for Workfront Planning </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license*</p></td>
   <td>
   <p>New: Standard</p> 
   <p>Current: Plan</p>
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level configurations</p></td>
   <td> <p>There are no access level controls for Adobe Workfront Planning</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your Workfront or group administrator must add the Planning area in your layout template. For information, see <a href="/help/quicksilver/planning/access/access-overview.md">Access overview</a>. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>Manage permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create.</p>
</td>
  </tr>
 </tbody>
</table>

*For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). -->

+++


## 連線記錄型別

<!--when changes here, also update the article for "Connect records"-->

{{step1-to-planning}}

1. 按一下您要連線其記錄型別的工作區，

   或

   從工作區中，展開現有工作區名稱右側的向下箭頭，搜尋工作區，然後在工作區顯示在清單中時選取該工作區。
1. 按一下記錄型別的卡片以開啟記錄型別頁面。
1. 按一下表格檢視右上角的&#x200B;**+**&#x200B;圖示，然後按一下&#x200B;**新增連線**&#x200B;索引標籤。

   ![](assets/new-connection-tab-with-workfront-aem-options.png)

1. 在&#x200B;**記錄型別**&#x200B;欄位中，搜尋記錄型別，或選取下列其中一項：

   * 來自目前工作區的另一個記錄型別

     ![](assets/many-to-many-connection-picker.png)

     >[!TIP]
     >
     > 
     >如果您在選取的工作區中沒有其他記錄型別，工作區區段不會顯示。


   * 來自另一個工作區的記錄型別，該記錄型別被設定為從其他工作區連線。 如需詳細資訊，請參閱[編輯記錄型別](/help/quicksilver/planning/architecture/edit-record-types.md)。

     ![](assets/new-connection-allow-multiple-records-box.png)

     >[!TIP]
     >
     >如果沒有記錄型別被設定為從其他工作區連線，則工作區區段不會顯示。


   * 來自&#x200B;**Workfront物件型別**&#x200B;區段的&#x200B;**專案、Portfolio、方案、公司**&#x200B;或&#x200B;**群組**。

     ![](assets/workfront-project-connection-selection.png)

   * 來自&#x200B;**Adobe應用程式**&#x200B;區段的&#x200B;**Experience Manager Assets**。

     ![](assets/aem-assets-connection-selection.png)

1. 更新下列資訊：

   * **名稱**：已連線欄位的名稱，它會顯示在原始記錄型別的資料表檢視或記錄頁面中。 這會在原始記錄型別的表格檢視或原始記錄的連結記錄欄位中建立連結記錄欄。 依預設，欄位名稱是您連線的記錄或物件的名稱。

   >[!TIP]
   >
   >您可以有多個連線連線到相同的記錄或物件型別。 如果您不編輯已連線的欄位名稱，Workfront會在已連線記錄的名稱后新增一個數字，以表示相同名稱的已連線記錄型別數目。

   * **描述**：有關連線記錄欄位的額外資訊。 當您將滑鼠游標停留在表格中的欄位欄位上時，會顯示欄位說明。
   * **允許多筆記錄**：選取此選項以表示當連結的記錄型別欄位顯示在原始記錄上時，允許使用者新增多筆記錄。 依預設會選取此選項。

     只有在連線來自兩個不同工作區的記錄或記錄和Adobe Experience Manager資產物件時，才能使用此選項。

     ![](assets/new-connection-allow-multiple-records-box.png)

   * **連線型別**：選取下列其中一個選項，以指出它們可以連線到多少筆記錄，以及可從多少筆記錄連線：

      * 多對多
      * 一對多
      * 多對一
      * 一對一

     此選項僅在連線來自相同工作區的記錄或記錄和Workfront物件型別時可用。

     ![](assets/many-to-many-connection-picker.png)

     如需連線型別的詳細資訊，請參閱[連線記錄型別概觀](/help/quicksilver/planning/architecture/connect-record-types-overview.md)。

   * **選取查詢欄位**：選取此選項以從選取的記錄型別新增欄位。 查閱欄位是與您要連結的記錄或物件型別相關聯的欄位。 連結它們會顯示您連結的記錄或物件在您連結的記錄上的資訊。 依預設會選取此選項。

     >[!TIP]
     >
     > 您無法新增下列欄位型別做為查閱欄位：
     >
     >    * 人員
     >    * 建立者
     >    * 上次修改者
     >    * Workfront預先輸入欄位（包括專案所有者或專案贊助者等欄位）

1. （有條件且選擇性）如果您選取連線Workfront物件，請從&#x200B;**僅連結符合這些條件的物件**&#x200B;區段中選取&#x200B;**自訂表單**。 只有已附加所選自訂表單的物件才能連結至所選記錄型別。 您可以選取多個表單。

   >[!NOTE]
   >
   > 您必須先在Workfront中為選取的物件建立自訂表單，這些表單才會顯示在此清單中。

1. （視條件而定）如果您選取連線至Experience Manager Assets，請從&#x200B;**從下列存放庫連結資產**&#x200B;區段的&#x200B;**Experience Manager存放庫**&#x200B;下拉式功能表中選取存放庫。 這是必填欄位。 此欄位只會顯示您在Experience Manager Assets中有權存取的存放庫。

   >[!NOTE]
   >
   >您的Workfront管理員可以透過Workfront中的中繼資料對應，將Workfront Planning欄位對應至Experience Manager Assets欄位。 如需詳細資訊，請參閱[設定Adobe Workfront與Experience Manager Assets之間的資產中繼資料對應](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/assets/integrations/configure-asset-metadata-mapping.html?lang=en)。

1. （視條件而定）如果您選取連線至Experience Manager Assets或Workfront Planning記錄型別，請在&#x200B;**記錄外觀**&#x200B;區域中選取下列其中一個選項：

   * **名稱和影像**：連線記錄的名稱和縮圖或圖示都會顯示在連線記錄欄位中。 這是預設選項。
   * **名稱**：連線的記錄欄位中只會顯示連線記錄的名稱。
   * **影像**：連線記錄欄位中只會顯示連線記錄的縮圖或圖示。

   沒有縮圖影像的記錄會改為顯示記錄型別圖示。 在&#x200B;**記錄外觀**&#x200B;區域顯示連線記錄的範例。

   >[!NOTE]
   >
   >* 當您允許連結多個記錄時，只顯示縮圖可能會節省較小區域（例如記錄檢視）的空間。
   >
   >* 記錄的名稱是記錄的主要欄位。 如需詳細資訊，請參閱[主要欄位概述](/help/quicksilver/planning/fields/primary-field-overview.md)。
   >
   >* 選取Workfront物件型別時，無法選取記錄外觀。
   >
   >* 您在「記錄」外觀區域中選取的內容會決定記錄在系統所有位置的連線中的顯示方式，包括所有檢視和詳細資訊頁面。

1. 按一下「**建立**」。

1. （視條件而定）若您選取&#x200B;**選取查閱欄位**&#x200B;設定，**新增查閱欄位**&#x200B;方塊就會開啟。

   按一下&#x200B;**+**&#x200B;圖示，從&#x200B;**未選取的欄位**&#x200B;區域新增欄位。

   或

   按一下&#x200B;**-**&#x200B;圖示以從&#x200B;**選取的欄位**&#x200B;區域移除欄位

   ![](assets/add-lookup-fields-for-another-maestro-record-type-box.png)

   連結記錄或物件後，所連線欄位的值會自動填入。

   >[!IMPORTANT]
   >
   >    擁有工作區檢視或更高許可權的所有人都可以檢視連結欄位中的資訊，無論其在連結物件型別應用程式中的許可權或存取層級為何。


1. （選擇性）按一下&#x200B;**跳過**&#x200B;以跳過從連結的記錄或物件型別新增欄位。 連結記錄的名稱或主要欄位是您連線之記錄型別的表格檢視中唯一可見的欄位。

1. （選擇性和條件性）如果您選取連結數字、貨幣、百分比或日期型別欄位，請同時選取彙總值以彙總多個值。 當使用者在連結的記錄欄位中選取多個連結的記錄時，連結欄位的值會根據您選擇的彙總器，以逗號分隔或顯示為摘要值。

   如果查閱欄位包含多個未彙總的值，請在檢視中排序或分組時考慮以下事項：

   * 排序由第一個值完成

   * 記錄會依每個欄位值的唯一組合分組

   * 時間表檢視是根據第一個日期值建置

   >[!IMPORTANT]
   >
   >    如果您希望欄位能新增為時間軸和行事曆檢視的開始和結束日期，新增查閱日期欄位時必須選取彙總值。 例如，您可以選取MAX或查閱日期欄位的MIN彙總。

   ![](assets/aggregator-drop-down-for-number-linked-field.png)

   >[!NOTE]
   >
   > 將記錄型別連線至Experience Manager Assets時，無法使用彙總器。

   從下列選項中選取：

   * **無**：顯示來自多個記錄的值（以逗號分隔）。 這是預設選取範圍。
   * **MAX**：顯示在連結的記錄欄位中選取之多個記錄的所有值中的最高值。
   * **MIN**：顯示在連結記錄欄位中選取之多個記錄的所有值中最低的值。
   * **SUM**：顯示在連結記錄欄位中選取之多個記錄的所有值總計。
   * **AVG**：顯示在連結記錄欄位中選取之多個記錄的所有值的平均值。
   * **唯一**：從查閱欄位值中移除重複專案，並且只顯示唯一值。 下列欄位型別無法使用此選項：
      * 段落
      * 核取方塊
      * 人員

   >[!NOTE]
   >
   >例如，您可以從Campaign記錄（原始記錄）連結產品記錄（連結記錄），並將其命名為「產品欄位」。 您也可以選擇從行銷活動記錄連結產品記錄的「預算」欄位，並將其稱為「產品預算」。 如果您允許在「產品欄位」中選取多個記錄，您可以選取預算為$100,000的產品1和預算為$110,000的產品2，以及預算為$100,000的產品3。 您可以在連結欄位中檢視原始記錄的下列「預算」資訊（視您選擇的彙總而定）：
   >
   >* **無**： $100,000， $110,000， $100,000
   >* **MAX**： $110,000
   >* **分鐘**： $100,000
   >* **總計**： $310,000
   >* **平均**： $103,000.33
   >* **唯一**： $100,000
   >

1. （選擇性）使用&#x200B;**搜尋**&#x200B;圖示![](assets/search-icon.png)來搜尋欄位。

1. 按一下&#x200B;**新增欄位**&#x200B;以儲存變更。

   已新增下列專案：

   * 您正在連結的記錄型別上的連結記錄欄位。 在您手動新增連結的記錄型別後，連結的記錄欄位將顯示連結的記錄型別的個別記錄。 如需新增記錄的資訊，請參閱[連線記錄](/help/quicksilver/planning/records/connect-records.md)。 連結的記錄欄位名稱是您在步驟6中選取的名稱。<!--accurate-->

   * 一個連結（或查詢）欄位（或數個欄位），在您手動新增連結記錄欄位中的記錄或物件後，顯示連結記錄或物件型別的相關資訊。 只有在建立連線時選取&#x200B;**選取查閱欄位**&#x200B;設定時，才會建立查閱欄位。 查閱欄位會自動根據以下模式命名：

     `<Name of the original field on the linked record> (from <Name of your linked field>)`

     例如，如果您連結的行銷活動記錄型別具有方案記錄型別，並將方案連結記錄欄位命名為「方案資訊」，然後選取此選項以在行銷活動表格檢視中同時顯示方案的預算欄位，則連結的欄位在行銷活動表格檢視中會自動命名為`Budget (from Program information)`。

   * 當您將記錄型別連結到彼此時，連結的記錄欄位也會新增到您連結到的記錄型別上。 連結的記錄型別上連結的記錄欄位名稱是您連結的記錄型別名稱。

     例如，如果您從「促銷活動」記錄型別連結「產品」記錄型別，並命名促銷活動「連結的產品」的已連線欄位，則會為「產品」記錄型別建立「促銷活動」連結記錄欄位。

     >[!TIP]
     >
     > 系統不會為其他應用程式的物件建立連結記錄欄位，以連結至您在Workfront Planning中連結的記錄型別。

1. （選擇性和條件性）在原始記錄型別或連結記錄型別表格檢視中，按一下連結記錄欄位標題中的向下箭頭，然後按一下下列其中一項：

   * **編輯欄位**：更新欄位的&#x200B;**名稱**&#x200B;和&#x200B;**描述**&#x200B;資訊。
   * **編輯查閱欄位**：新增或移除任何連結記錄的欄位。

   ![](assets/edit-field-and-lookup-fields-drop-down-menu-in-table-column.png)

   若要新增或移除查詢欄位，請遵循上述步驟16至17中的指示。<!--ensure these step numbers stay accurate-->

   >[!NOTE]
   >
   > 您無法從其他應用程式新增屬於您正在連結至物件型別的記錄型別的查閱欄位。
   >
   > 例如，您無法將「促銷活動狀態」的查詢欄位新增至您正從促銷活動連結至的Workfront專案。

1. （選擇性）從連結的記錄型別中，按一下連結的記錄欄位標題或查閱欄位標題中的向下箭頭，然後按一下&#x200B;**刪除**。

   記錄欄位或查詢欄位將會刪除。 如果您刪除記錄欄位，則與連結記錄關聯的任何查閱欄位也會被刪除。
