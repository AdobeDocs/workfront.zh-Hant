---
title: 連線記錄型別
description: 指示個別記錄型別如何彼此關聯的一種方法是連線它們。 此外，您可以將Adobe Workfront Planning記錄型別與其他應用程式的物件型別連線起來，以增強您的使用者體驗，並將他們的焦點放在一個應用程式中。
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: ae794ebe-4597-47a4-9ef3-3f4d31cb70c2
source-git-commit: e26a3d0e283182e08902c263252c8d067838c23a
workflow-type: tm+mt
source-wordcount: '2764'
ht-degree: 0%

---


<!--keep the 30 fields limit in yellow till Jan 2026; also the global record type cross-workspace capability information-->

# 連線記錄型別

<span class="preview">本頁醒目提示的資訊指出尚未普遍可用的功能。 它僅在預覽環境中可供所有客戶使用。 每月發行至生產環境後，生產環境中為啟用快速發行的客戶也提供相同的功能。</span>

<span class="preview">如需快速發行資訊，請參閱[為您的組織啟用或停用快速發行](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>


{{planning-important-intro}}

<!--
You can use Adobe Workfront Planning to design fully-customizable workspaces that contain record types needed in your organization. A way to indicate how individual record types relate to one another is to connect them. Also, you can connect Workfront Planning record types with object types from other applications to enhance your users' experience and keep their focus in one application. -->

您可以將記錄型別彼此連線，也可以將記錄型別與其他應用程式的物件型別連線。

當有數種工作物件型別影響彼此時，連線記錄型別會很有幫助。 例如，您可以使用行銷活動，而每個行銷活動可能會迎合多個品牌。 若要指出此關係，您可以將行銷活動連結至品牌。 這會為Campaign記錄上的Brands建立連線欄位。

此外，每個行銷活動的工作可能會在Workfront的多個專案中進行規劃。 若要指出此問題，您可以將行銷活動連結至相關專案。 這會為行銷活動記錄上的專案建立一個連線欄位。

建立連線欄位後，您可以在兩個記錄或物件型別之間連線個別記錄。

>[!NOTE]
>
><span class="preview">一個記錄型別最多可以有30個連線欄位。</span>

本文說明如何將兩個Workfront Planning記錄型別或Workfront Planning記錄型別與其他應用程式的物件連線。

建立記錄或物件型別之間的連線後，連線欄位會新增至Planning記錄型別。 在連線欄位中，您可以將個別記錄連線至彼此，並在Workfront Planning記錄上顯示連結記錄或物件型別的欄位。

如需連線型別的一般資訊，請參閱[連線記錄型別概觀](/help/quicksilver/planning/architecture/connect-record-types-overview.md)。

如需有關連線記錄或記錄與其他應用程式物件的資訊，請參閱[連線記錄](/help/quicksilver/planning/records/connect-records.md)。

如需連線記錄型別和記錄的範例，請參閱[連線記錄型別和記錄的範例](/help/quicksilver/planning/architecture/example-connect-record-types-and-records.md)。

<!--ensure this last linked article is right; the title and the link should have changed-->


## 存取需求

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
   <td role="rowheader"><p>Adobe Workfront套件</p></td> 
   <td> 
<p>若要從相同工作區連線記錄型別： </p>
<ul> 
<li><p>任何Workfront和任何Planning套件</p></li>
<li><p>任何工作流程與任何Planning套件</li></ul>

<p>若要從不同的工作區連線記錄型別：</p>

<ul> 
<li><p>任何Workfront和任何Planning套件</p></li>
<li><p>任何工作流程和Planning Prime或Ultimate套件</p></li></ul>
<p>如需每個Workfront Planning套件所含內容的詳細資訊，請聯絡您的Workfront客戶代表。 </p> 
   </td> 
<tr> 
<td> 
   <p> 其他產品</p> </td> 
   <td> 
   <p> 除了Adobe Workfront，您必須擁有Adobe Experience Manager Assets授權以及AEM Assets與Workfront之間的整合，才能將AEM資產與Planning記錄型別連線。<p>
    如需詳細資訊，請參閱<a href="/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/workfront-for-aem-asset-essentials.md">適用於Experience Manager Assets和Assets Essentials的Adobe Workfront：文章索引</a>。 </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront授權</p></td> 
   <td><p>標準</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>物件許可權</p></td> 
   <td>   <p>管理工作區的許可權</p>  
   <p>系統管理員擁有所有工作區的許可權，包括他們未建立的工作區</p>  </td> 
  </tr>  
</tbody> 
</table>

如需Workfront存取需求的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++


<!--Old:
<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Products</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront Planning<p></li>
   <li><p> Adobe Experience Manager Assets, if you want to connect AEM assets with Planning record types<p>
   <p>You must have an Adobe Experience Manager Assets license and an integration between AEM Assets and Workfront.
    For information, see <a href="/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/workfront-for-aem-asset-essentials.md">Adobe Workfront for Experience Manager Assets and Assets Essentials: article index</a>. </p>
   </li>
   </ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront plan*</p></td> 
   <td> 
<p>Any of the following Workfront plans:</p> 
<ul><li>Select</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning is not available for legacy Workfront plans</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront Planning package*</p></td> 
   <td> 
<p>Any </p> 
<p>For more information about what is included in each Workfront Planning plan, contact your Workfront account manager. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront platform</p></td> 
   <td> 
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access Workfront Planning.</p> 
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license*</p></td> 
   <td> <p>Standard</p> 
   <p>Workfront Planning is not available for legacy Workfront licenses</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Access level configuration</p></td> 
   <td> <p>There are no access level controls for Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>   <p>Manage permissions to a workspace</p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create.</p></td> 
  </tr> 
 
</tbody> 
</table> -->

## 連線記錄型別

<!--when changes here, also update the article for "Connect records"-->

{{step1-to-planning}}

1. 按一下您要連線其記錄型別的工作區，

   或

   從工作區中，展開現有工作區名稱右側的向下箭頭，搜尋工作區，然後在工作區顯示在清單中時選取該工作區。
1. 按一下記錄型別的卡片以開啟記錄型別頁面。
1. 按一下表格檢視右上角的&#x200B;**+**&#x200B;圖示，然後按一下&#x200B;**新增連線**&#x200B;索引標籤。

   ![使用Workfront AEM選項的新連線標籤](assets/new-connection-tab-with-workfront-aem-options-no-buttons.png)

1. 搜尋記錄型別，或選取下列其中一項：

   * 來自目前工作區的記錄型別

     ![相同工作區記錄型別的多重選取連線選擇器](assets/multi-select-connection-picker-record-type.png)

     >[!TIP]
     >
     > 
     >如果您在選取的工作區中沒有其他記錄型別，工作區區段不會顯示。

   * 來自另一個工作區的記錄型別，該記錄型別被設定為從其他工作區連線。

     >[!TIP]
     >
     >必須針對&#x200B;**進階設定** **或**&#x200B;編輯記錄型別<span class="preview">方塊的&#x200B;**跨工作區設定**</span>&#x200B;索引標籤中的記錄型別，啟用&#x200B;**允許連線至其他工作區中的此記錄型別**&#x200B;設定，才能從其他工作區存取記錄型別。 如果沒有記錄型別被設定為從其他工作區連線，則工作區區段不會顯示。
     >
     >如需詳細資訊，請參閱[設定記錄型別的跨工作區功能](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md)。<!--update screen shot at production-->
     >
     >![編輯記錄型別方塊進階設定索引標籤](assets/edit-record-type-box-advanced-settings-tab.png)

     <!--Old:
        [!TIP]
        The **Allow connecting to this record type in other workspaces** setting must be enabled for a record type in the **Advanced settings** tab of the **Edit record type** box, for a record type to be accessible from other workspaces. If there are no record types that are configured to connect from other workspaces, the workspace section does not display.
        ![Edit record type box advanced settings tab](assets/edit-record-type-box-advanced-settings-tab.png)
        -->

   如需詳細資訊，請參閱[編輯記錄型別](/help/quicksilver/planning/architecture/edit-record-types.md)。

   * 來自&#x200B;**Workfront物件型別**&#x200B;區段的&#x200B;**專案、Portfolio、方案、公司**&#x200B;或&#x200B;**群組**。

     ![Workfront專案連線選擇](assets/multi-select-connection-picker-project.png)

   * 來自&#x200B;**Experience Manager Assets應用程式**&#x200B;區段的&#x200B;**Adobe**。

     ![AEM Assets連線選擇](assets/aem-assets-connection-selection.png)

     針對您選取的記錄或物件型別，會開啟「新連線」標籤。

1. 以新的連線欄位名稱更新&#x200B;**Name**&#x200B;欄位，因為它會出現在原始記錄型別的資料表檢視或記錄頁面中。 這會在原始記錄型別的表格檢視中建立連線的記錄欄（或欄位）。 依預設，欄位名稱是您連線的記錄或物件的名稱。

   >[!TIP]
   >
   >您可以有多個連線連線到相同的記錄或物件型別。 如果您不編輯已連線的欄位名稱，Workfront會在已連線記錄的名稱后新增一個數字，以表示相同名稱的已連線記錄型別數目。

1. 新增連線記錄欄位的相關資訊，以更新&#x200B;**描述**&#x200B;欄位。 當您將滑鼠游標停留在表格中的欄位欄位上時，會顯示欄位說明。
1. （視條件而定）當您從兩個不同的工作區或記錄和Adobe Experience Manager資產物件連線記錄型別時，請選取&#x200B;**允許多筆記錄**。 透過選取它，您表示當連線的記錄型別欄位顯示在原始記錄上時，您可以允許使用者新增多個記錄。 依預設會選取此選項。

   ![從另一個工作區新增記錄型別的連線](assets/new-connection-allow-multiple-records-box.png)

1. （視條件而定）當您從相同工作區連線記錄型別，或使用Workfront物件型別的Planning記錄型別時，請選取下列其中一項：

   * **多重選取**：選取此專案以允許目前記錄型別中的一個記錄與連線記錄型別中的多個記錄連線。
   * **Single-select**：選取此專案可允許來自目前記錄型別的一個記錄與來自連線記錄型別的一個記錄連線。

1. 選取&#x200B;**在連結的記錄型別**&#x200B;上建立對應的欄位。 選取後，除了新增到目前記錄型別的連線欄位外，還會為您連線的記錄型別建立連線欄位。 預設為停用。

   >[!TIP]
   >
   >除了<span class="preview">一個記錄型別</span>有30個連線欄位的限制外，一個記錄型別有500個欄位的限制。 建議將此設定設為關閉（尤其是分類記錄型別），以避免達到此限制。
   >

1. （視條件而定）如果您已啟用&#x200B;**在連結的記錄型別**&#x200B;上建立對應的欄位，請從下列選項中選擇，以指出使用者可連線到多少筆記錄，以及可從多少筆記錄連線：

   * 多對多
   * 一對多
   * 多對一
   * 一對一

   如需連線型別的詳細資訊，請參閱[連線記錄型別概觀](/help/quicksilver/planning/architecture/connect-record-types-overview.md)。

   >[!NOTE]
   >
   >如果您為「連線」型別選取「一對多」或「一對一」，而您稍後想要連線記錄或已在其他地方連線的物件，您將會收到警告，指出再次連線會將它從原始連線中移除。 您可以允許移除或選取其他記錄。

1. （有條件且選擇性）當您選取連線Workfront物件時，請從&#x200B;**僅連結符合這些條件的物件**&#x200B;區段中選擇&#x200B;**自訂表單**。 只有已附加所選自訂表單的物件才能連結至所選記錄型別。 您可以選取多個表單。

   >[!NOTE]
   >
   > 您必須先在Workfront中為選取的物件建立自訂表單，這些表單才會顯示在此清單中。

1. （視條件而定）當您選取連線至Experience Manager Assets時，請從&#x200B;**從下列存放庫連結資產**&#x200B;區段的&#x200B;**Experience Manager存放庫**&#x200B;下拉式功能表中選擇存放庫。 這是必填欄位。 此欄位只會顯示您在Experience Manager Assets中有權存取的存放庫。

   >[!NOTE]
   >
   >您的Workfront管理員可以透過Workfront中的中繼資料對應，將Workfront Planning欄位對應至Experience Manager Assets欄位。 如需詳細資訊，請參閱[設定Adobe Workfront與Experience Manager Assets之間的資產中繼資料對應](https://experienceleague.adobe.com/zh-hant/docs/experience-manager-cloud-service/content/assets/integrations/configure-asset-metadata-mapping)。


1. （視條件而定）當您選取連線至Experience Manager Assets或Workfront Planning記錄型別時，請在&#x200B;**記錄外觀**&#x200B;區域中選擇下列其中一個選項：

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

1. 選取&#x200B;**選取查閱欄位**&#x200B;以從您連線的記錄型別新增欄位。 查閱欄位是與您要連結的記錄或物件型別相關聯的欄位。 連結它們會顯示您連結的記錄或物件在您連結的記錄上的資訊。 依預設會選取此選項。

   >[!TIP]
   >
   >* 您無法將Workfront預先輸入欄位（包括專案所有者或專案贊助者之類的欄位）新增為查詢欄位。
   >
   >* Workfront物件的日期欄位資訊在Workfront Planning中會以24小時格式顯示，無論其在Workfront中的顯示方式為何。
   >
   >   例如，如果專案的計劃開始日期在Workfront中顯示為3:00下午，則在匯入的查詢欄位中，它將在Workfront Planning中顯示為15:00。

1. 按一下「**建立**」。

1. （視條件而定）若您選取&#x200B;**選取查閱欄位**&#x200B;設定，**新增查閱欄位**&#x200B;方塊就會開啟。

   按一下&#x200B;**+**&#x200B;圖示，從&#x200B;**未選取的欄位**&#x200B;區域新增欄位。

   或

   按一下&#x200B;**-**&#x200B;圖示以從&#x200B;**選取的欄位**&#x200B;區域移除欄位

   ![新增其他記錄型別方塊的查閱欄位](assets/add-lookup-fields-for-another-maestro-record-type-box.png)

   連結記錄或物件後，所連線欄位的值會自動填入。

   >[!IMPORTANT]
   >
   >    擁有工作區檢視或更高許可權的所有人都可以檢視連結欄位中的資訊，無論其在連結物件型別應用程式中的許可權或存取層級為何。

1. （選擇性）按一下&#x200B;**跳過**&#x200B;以跳過從連結的記錄或物件型別新增欄位。 連結記錄的名稱或主要欄位是您連線之記錄型別的表格檢視中唯一可見的欄位。

1. 為您新增的查閱欄位選擇彙總器。

   >[!NOTE]
   >
   >您無法新增下列欄位型別的彙總：
   >
   >    * 段落
   >    * 核取方塊

   當使用者在連結的記錄欄位中選取多個連結的記錄時，連結欄位的值會根據您選擇的彙總器，以逗號分隔或顯示為摘要值。

   如果查閱欄位包含多個未彙總的值，請在檢視中排序或分組時考慮以下事項：

   * 排序由第一個值完成

   * 記錄會依每個欄位值的唯一組合分組

   * 時間軸檢視會根據所連線記錄型別的第一個日期值（當它顯示在檢視中時）建置

   >[!IMPORTANT]
   >
   > 如果您希望欄位能新增為時間軸和行事曆檢視的開始和結束日期，新增查閱日期欄位時必須選取彙總值。 例如，您可以選取MAX或查閱日期欄位的MIN彙總。

   連結的編號欄位![的](assets/aggregator-drop-down-for-number-linked-field.png)彙總下拉式清單

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

1. （選擇性）使用&#x200B;**搜尋**&#x200B;圖示![搜尋圖示](assets/search-icon.png)來搜尋欄位。

1. 按一下&#x200B;**新增欄位**&#x200B;以儲存變更。

   已新增下列專案：

   * 您正在連結的記錄型別上的連結記錄欄位。 在您手動新增連結的記錄型別後，連結的記錄欄位將顯示連結的記錄型別的個別記錄。 如需新增記錄的資訊，請參閱[連線記錄](/help/quicksilver/planning/records/connect-records.md)。 連結的記錄欄位名稱是您在步驟6中選取的名稱。<!--accurate-->

   * 一個連結（或查詢）欄位（或數個欄位），在您手動新增連結記錄欄位中的記錄或物件後，顯示連結記錄或物件型別的相關資訊。 只有在建立連線時選取&#x200B;**選取查閱欄位**&#x200B;設定時，才會建立查閱欄位。 查閱欄位會自動根據以下模式命名：

     `<Name of the original field on the linked record> (from <Name of your linked field>)`

     例如，如果您連結的行銷活動記錄型別具有方案記錄型別，並將方案連結記錄欄位命名為「方案資訊」，然後選取此選項以在行銷活動表格檢視中同時顯示方案的預算欄位，則連結的欄位在行銷活動表格檢視中會自動命名為`Budget (from Program information)`。

   * 當您連結記錄型別到彼此時，連結的記錄欄位也會新增到您連結的記錄型別上，但只有當您啟用&#x200B;**在連結的記錄型別**&#x200B;上建立對應的欄位設定時。 連結的記錄型別上連結的記錄欄位名稱是您連結的記錄型別名稱。

     例如，如果您從「促銷活動」記錄型別連結「產品」記錄型別，並命名促銷活動「連結的產品」的已連線欄位，則會為「產品」記錄型別建立「促銷活動」連結記錄欄位。

     >[!TIP]
     >
     > 連結的記錄欄位不會為來自另一個應用程式的物件在其各自的應用程式中建立。
     >我們建議您不要建立分類記錄型別的連結，因為每個記錄型別有500個欄位的限制，<span class="preview">加上連線欄位30個的限制</span>。

   <!--see the span preview text in the TIP above; it might not show up in green-->

1. （選擇性和條件性）在原始記錄型別或連結記錄型別表格檢視中，按一下連結記錄欄位標題中的向下箭頭，然後按一下下列其中一項：

   * **編輯欄位**：更新欄位的&#x200B;**名稱**&#x200B;和&#x200B;**描述**&#x200B;資訊。
   * **編輯查閱欄位**：新增或移除任何連結記錄的欄位。

   ![編輯資料表資料行](assets/edit-field-and-lookup-fields-drop-down-menu-in-table-column.png)中的欄位和查閱欄位下拉式功能表

   若要新增或移除查詢欄位，請遵循上述步驟16至17中的指示。<!--ensure these step numbers stay accurate-->

   >[!NOTE]
   >
   > 您無法從其他應用程式新增屬於您正在連結至物件型別的記錄型別的查閱欄位。
   >
   > 例如，您無法將「促銷活動狀態」的查詢欄位新增至您正從促銷活動連結至的Workfront專案。

1. （選擇性）從連結的記錄型別中，按一下連結的記錄欄位標題或查閱欄位標題中的向下箭頭，然後按一下&#x200B;**刪除**。

   記錄欄位或查詢欄位將會刪除。 如果您刪除記錄欄位，則與連結記錄關聯的任何查閱欄位也會被刪除。
