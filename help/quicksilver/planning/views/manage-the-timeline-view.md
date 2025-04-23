---
title: 管理時間表檢視
description: 在Adobe Workfront Planning記錄型別頁面的時間軸檢視中，存取及編輯記錄。 本文說明如何建立時間表檢視，以及如何編輯或刪除現有的時間表檢視。 使用篩選器、群組和設定自訂時間軸。 使用「劃分」功能來顯示連線的記錄。
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: f348af7f-5bb9-4d88-9bcb-3bef7e8892dd
source-git-commit: 1dc2791bed0dfada109ee102e09c25ae9a52e6b0
workflow-type: tm+mt
source-wordcount: '2863'
ht-degree: 0%

---

# 管理時間表檢視

<span class="preview">本頁醒目提示的資訊指出尚未普遍可用的功能。 它僅在預覽環境中可供所有客戶使用。 每月發行至生產環境後，生產環境中為啟用快速發行的客戶也提供相同的功能。</span>

<span class="preview">如需快速發行資訊，請參閱[為您的組織啟用或停用快速發行](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>

{{planning-important-intro}}

存取Adobe Workfront Planning中的記錄型別頁面時，您可以在時間軸檢視中顯示記錄。

如需有關記錄檢視的資訊，請參閱[管理記錄檢視](/help/quicksilver/planning/views/manage-record-views.md)。

## 存取需求

+++ 展開以檢視存取需求。

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
   <li><p> Adobe Workfront規劃<p></li></ul></td> 
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
   <td role="rowheader"><p>Adobe Workfront規劃套件*</p></td> 
   <td> 
<p>任何 </p> 
<p>如需每個Workfront計畫包含內容的詳細資訊，請聯絡您的Workfront客戶經理。 </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront平台</p></td> 
   <td> 
<p>貴組織的Workfront例項必須上線至Adobe Unified Experience，才能存取Workfront Planning的所有功能。</p> 
<p>如需詳細資訊，請參閱<a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">適用於Workfront的Adobe Unified Experience</a>。 </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront授權*</p></td> 
   <td><p> 標準 </p>
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
   <td>   <p>管理檢視的許可權</p>  
   <p>檢視許可權以暫時變更檢視設定</p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>版面配置範本</p></td> 
   <td> <p>必須為所有使用者(包括Workfront管理員)指派一個版面配置範本，該範本包含主功能表中的Planning區域。 </p> </td> 
  </tr> 
</tbody> 
</table>

*如需Workfront存取需求的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 管理時間表檢視 {#manage-a-timeline-view}

<!--insert screen shot of timeline view-->

建立時間表檢視時，所選記錄型別的所有記錄都會以時間順序時間表顯示。

請考量下列事項：

* 您至少有兩個日期欄位與記錄型別相關聯時，才能建立時間表檢視。 當您有一個或沒有與記錄型別相關聯的日期欄位時，時間軸檢視選項會變暗。

  建立時間表檢視時，您可以從下列日期欄位中選取：

   * 記錄日期
   * 記錄系統產生的欄位：建立日期、上次修改日期
   * 來自已連線記錄或物件型別的查詢日期。
* 根據與記錄關聯的日期，在下列情況下，某些記錄可能不會顯示在時間軸檢視中：

   * 當開始和結束日期沒有值時
   * 當「開始」或「結束」日期沒有值時
   * 當開始日期在結束日期之後時

若要管理時間表檢視：

1. 移至您要檢視其時間軸的記錄型別頁面。
1. 建立時間表檢視，如文章[管理記錄檢視](/help/quicksilver/planning/views/manage-record-views.md)中所述。

   ![時間表檢視範例](assets/timeline-view-example.png)

   與您選取的記錄型別相關聯的記錄會在時間軸中顯示為長條，並依其開始日期的時間順序依預設排序。

   >[!TIP]
   >
   >    時間軸中記錄的排序在壓縮檢視中不可見。

1. （選擇性和條件性）當記錄名稱被截斷時，將滑鼠懸停在記錄列上以顯示記錄的完整名稱和其他資訊。

1. 執行下列任一項作業來瀏覽時間軸：

   * 按一下左右圖示，或使用水準捲動在時間軸中前後移動。 重新整理頁面會保留選取的時間範圍。
   * 按一下&#x200B;**今天**，將時間表置中到今天的日期。
   * 從時間範圍下拉式選單中選取下列其中一個選項，以更新時間增量：

      * 年
      * 季度
      * 月
1. 按一下&#x200B;**切換至標準**&#x200B;檢視，以個別行<!--check to see if they updated the name of the setting here-->顯示記錄

   或

   按一下&#x200B;**切換到壓縮檢視**&#x200B;以顯示日期在同一行上不相交的記錄。<!--check to see if they updated the name of the setting here-->

   預設情況下，記錄會顯示在「壓縮」檢視中。

1. 執行下列動作以快速尋找符合關鍵字的記錄：

   1. 按一下&#x200B;**搜尋**&#x200B;圖示![搜尋圖示](assets/search-icon.png)，然後開始輸入與熒幕上顯示之記錄的任何欄位相關聯的關鍵字。 正確相符的數目會顯示在搜尋專案旁邊，而具有正確相符專案的記錄會反白顯示。

      ![搜尋方塊和結果時間表檢視](assets/search-box-and-results-timeline-view.png)

      您可以使用熒幕上可見的任何文字或特殊字元。

      您無法使用與未顯示在時間表檢視中的欄位關聯的關鍵字。

   1. 在鍵盤上按Enter鍵以移至下一個找到的欄位。
   1. （選擇性）如果有多個相符專案，請按一下搜尋關鍵字右邊的向上和向下箭頭，以尋找表格中的所有相符專案。
   1. 按一下搜尋方塊中的&#x200B;**x**&#x200B;圖示以清除搜尋關鍵字。

1. 更新下列檢視元素，如下列子區段所述：
   * [篩選器](#add-filters)
   * [分組](#add-grouping)
   * [設定](#edit-the-timeline-view-settings)
     <!--* [Sort](#add-sort) not yet in timeline; also check the anchor and make sure it's correct-->

1. （選擇性）按一下&#x200B;**劃分**，在時間軸上顯示連線的記錄。

   如需詳細資訊，請參閱[使用劃分功能在時間軸檢視中顯示連線記錄](#break-down-connected-records-in-the-timeline-view)一節

### 新增篩選器

您可以使用篩選器來減少熒幕上顯示的資訊量。

在時間軸檢視中使用篩選器時，請考量下列事項：

<!-- this list is almost identical to the one for the table view - update both-->

* 您為時間軸檢視建立的篩選器與套用至相同記錄型別之任何其他檢視中的篩選器是獨立運作的。

* 這些篩選器對於您選取的檢視而言是唯一的。 相同記錄型別的兩個時間軸檢視可以套用不同的篩選器。

* 檢視相同時間表檢視的兩個使用者會看到目前套用的相同篩選器。

* 您無法為您為時間表檢視建置的篩選器命名。

* 移除篩選器會將篩選器從存取與您相同記錄型別以及顯示與您相同檢視的任何人移除。

* 在時間軸檢視中新增濾鏡，與在表格檢視中新增濾鏡相同。

  如需詳細資訊，請參閱文章[管理資料表檢視](/help/quicksilver/planning/views/manage-the-table-view.md)中的「新增篩選器」一節。

* 您可以依已連線的記錄欄位或查詢欄位進行篩選。
* 您可以依顯示多個值的查閱欄位進行篩選。


### 新增分組

<!-- groupings are almost identical between this view and table  but they display a little differently, so I kept the steps for both; update in both places if they make changes to groupings-->

將群組套用至檢視時，您可以依照類似的資訊來群組記錄。

在時間軸檢視中新增群組，類似於在表格檢視中新增群組。

在時間軸檢視中使用群組時，請考量下列事項：

* 您可以在表格和時間軸檢視中套用群組。 表格檢視的分組與相同記錄型別之時間軸檢視中的群組是獨立的。
* 您可以在檢視中套用3個群組層級。 記錄會依照您選取的群組順序進行分組。
&lt;！—*使用API時，您最多可以套用4個層級的群組。  — 現在正在檢查此專案 — >
* 群組對於您選取的檢視而言是唯一的。 相同記錄型別的兩個表格檢視可以套用不同的群組。 檢視相同表格檢視的兩個使用者會看到目前套用的相同分組。
* 您無法為表格檢視建立的分組命名。
* 移除群組會將群組從存取與您相同記錄型別以及顯示與您相同檢視的任何人中移除。
* 您可以編輯列在群組下的記錄。
* 您可以依連線的記錄欄位或查詢欄位來分組。
* 當您依具有多個值（尚未由彙總器彙總）的查閱欄位來分組時，記錄會依每個唯一的欄位值組合來分組。
* 您可以參考與目前記錄型別相距最多4個層級的欄位。 例如，如果您正在建立「活動」記錄型別的群組，且「活動」已連線至「產品」記錄型別，而該記錄型別已連線至「行銷活動」記錄型別，而該記錄型別已連線至「Workfront專案」，則您可在您為「活動」記錄型別所建立的分組中參考專案的「狀態」。
<!--checking into this: * You can apply up to 4 levels of grouping when using the API. -->
<!-- checking also into this: * You cannot group by a Paragraph-type field.-->

若要在時間表檢視中新增群組：

1. 如文章[管理記錄檢視](/help/quicksilver/planning/views/manage-record-views.md)中所述，建立記錄型別的時間表檢視。
1. 按一下時間軸檢視右上角的&#x200B;**群組**。

   ![使用連結欄位將UI時間表檢視分組](assets/grouping-ui-timeline-view-with-linked-fields.png)

1. 按一下其中一個建議的欄位，或按一下&#x200B;**選擇其他欄位**，搜尋其他欄位，然後在欄位顯示在清單中時按一下它。

   分組會自動套用至時間軸，且記錄會顯示在分組方塊內。

   <!-- add a step that you can rearrange the groupings here, when this will be possible-->

1. （可選）重複上述步驟以新增最多3個群組。

   為分組選取的欄位數會顯示在「分組」圖示旁。

   <!-- update screen shot with view redesign-->

   ![分組套用至時間表檢視](assets/grouping-applied-in-timeline-view.png)

1. （選擇性）在&#x200B;**群組記錄依據**&#x200B;方塊中，按一下選取要移除分組的欄位右邊的&#x200B;**x**&#x200B;圖示

   或

   按一下&#x200B;**全部清除**&#x200B;以移除所有欄位。

1. 按一下「**依**&#x200B;分組記錄」方塊外部以關閉它。
1. （選擇性）按一下&#x200B;**設定**，然後按一下&#x200B;**色彩**&#x200B;以使用色彩代碼分組。 如需詳細資訊，請參閱本文中的[編輯時間表檢視設定](#edit-the-timeline-view-settings)一節。

<!-- 

### Add sort

this is not possible right now; if this is the same functionality as the table view, document it there and link from here. 

-->

### 編輯時間軸檢視設定 {#edit-the-timeline-view-settings}

更新時間軸檢視設定，以指示要在檢視的時間軸區段中顯示哪些資訊及顯示方式。

1. 如文章[管理記錄檢視](/help/quicksilver/planning/views/manage-record-views.md)中所述，建立記錄型別的時間表檢視。
1. 按一下&#x200B;**設定**。
1. 按一下左側面板中的&#x200B;**日期和時間**，然後選取要在時間軸上顯示的&#x200B;**開始日期**&#x200B;和&#x200B;**結束日期**。 您可以選擇預設的「開始」和「結束」日期，也可以選擇任何可用的日期欄位。 代表記錄的長條圖，其開始日期為您為「開始」日期指定的日期，結束日期為您與「結束」日期對應的日期。

   >[!NOTE]
   >
   >沒有開始或結束日期值或開始日期晚於結束日期的記錄不會顯示在時間軸檢視中。

1. 按一下左側面板中的&#x200B;**長條樣式**，以指示您要在記錄長條上顯示的資訊。

   預設會選取記錄的主要欄位（或標題），如記錄的表格檢視中所定義。<!--adjust this when the primary field is released??-->

1. （選擇性和條件性）如果您將縮圖新增至記錄，請選取「縮圖」選項，以顯示與其記錄列中的記錄相關聯的影像。

   >[!NOTE]
   >
   >    您必須先在表格檢視中新增縮圖，才能在時間軸檢視中顯示它們。 如需詳細資訊，請參閱[新增縮圖至記錄](/help/quicksilver/planning/records/add-thumbnails-to-records.md)。

1. 按一下&#x200B;**新增欄位**，然後按一下&#x200B;**搜尋欄位**&#x200B;方塊內部，再按一下您要新增的欄位。

   >[!TIP]
   >
   >   * 您必須先建立欄位，才能將其新增到記錄列。
   > 
   >   * 您必須至少選取一個欄位。 預設會選取&#x200B;**名稱**。
   >
   >   * 您最多可以新增5個欄位。

   右側會顯示時間軸上長條圖的外觀。

   ![預覽的記錄詳細資料面板時間軸設定](assets/record-details-panel-timeline-settings-with-preview.png)

1. <span class="preview"> （選擇性和條件性）如果您以標準模式顯示時間軸，請啟用&#x200B;**截斷列詳細資料**&#x200B;設定。 啟用時，記錄列上的資訊將會被截斷，而且只有在您將滑鼠懸停在記錄列上時才會完全顯示。 此設定預設為停用，資訊會完全顯示在長條上。</span>

   ![時間軸設定方塊上啟用截斷設定](assets/truncate-setting-enabled-on-timeline-settings-highlighted.png)

   >[!TIP]
   >
   >* <span class="preview">以精簡模式顯示時間軸檢視時，無法使用截斷列詳細資料設定，且無法在行事曆檢視中使用。</span>
   >
   >* <span class="preview">如果您劃分時間軸檢視，以在時間軸中顯示連線的物件，則「截斷列詳細資料」設定只會套用至主要記錄型別。 它不適用於連線的記錄列。</span>


1. 按一下左側面板中的&#x200B;**色彩**，以自訂時間軸中記錄和群組的色彩。

   ![色彩標籤時間表檢視](assets/color-tab-timeline-view.png)

1. （條件式與選擇性）如果您將群組新增至時間軸檢視，請從下列選項中選取，以在&#x200B;**設定群組顏色**&#x200B;區段中設定群組的顏色：

   * **預設（灰色）**：群組的顏色設定為灰色。 這是預設值。
   * **欄位值**：群組的顏色符合您群組依據之欄位的顏色。

     >[!NOTE]
     >
     >    * 您只能將顏色與具有顏色編碼選項的欄位比對。 例如，您可以將顏色與「狀態」欄位配對，或與顏色關聯的選項欄位。
     >    
     >    * 您無法從連結的記錄或物件型別中尋找符合顏色的欄位。


   例如，多選或單選欄位可以有顏色編碼的選項。

   如果您依據沒有顏色編碼選項的欄位分組，則分組顏色保持灰色。

   >[!TIP]
   >
   >如果您未將群組新增至時間軸檢視，則不會顯示此區段。

1. 在&#x200B;**設定記錄色彩**&#x200B;區段中，從下列選項中選取，以設定記錄的色彩：

   * **記錄型別**：記錄的顏色符合您選取的記錄型別顏色。 這是預設選項。
   * **欄位值**：記錄的顏色符合您指定的欄位顏色。 繼續步驟10。<!--ensure this stays accurate-->
   * **群組**：記錄的顏色符合您為群組指定的顏色。 當您未將群組套用到時間軸檢視時，此選項會變暗。
   * **無**：記錄以白色列顯示。

1. （視條件而定）如果您為記錄顏色選取&#x200B;**欄位值**，請從&#x200B;**將記錄顏色與**&#x200B;下拉式功能表中選取欄位。

   ![時間軸檢視中的欄位選擇器下拉式功能表](assets/field-selector-drop-down-menu-timeline-view.png)

   下拉式選單中只會顯示具有色彩編碼選項的欄位。

   例如，多選或單選欄位可以有顏色編碼的選項。

   如果選取的記錄型別沒有包含顏色編碼選項的欄位，則此選項會變暗。

1. 按一下「**儲存**」。

   記錄會以您所選取的規格顯示在時間軸檢視中。

### 在時間軸檢視中劃分連線記錄

您可以使用「劃分」功能，在記錄的時間軸檢視中顯示連線的記錄。 按連線劃分記錄可讓您檢視其他連線記錄的時間表，並瞭解這些記錄可能會如何影響記錄的效能和截止日期。

#### 使用劃分功能時的注意事項

* 您可以在時間軸檢視中選取的記錄型別記錄下顯示連線的記錄或物件。
* 您可以使用「劃分」功能，在時間軸檢視中顯示下列專案：
   * Workfront Planning記錄已連線至選取的記錄型別。
   * Workfront物件型別或連線到所選記錄型別的Experience Manager資產。
   * Workfront Planning記錄或其他應用程式的物件，這些記錄或其他應用程式已連線至連線至所選記錄型別的記錄。

     例如，您可以將行銷活動連結至產品組合。 此外，您可以連線其他記錄型別、產品、專案以及行銷活動。 建立行銷活動時間表檢視時，您可以依產品組合、產品和專案劃分行銷活動。

* 您無法顯示僅連線到Workfront中的Workfront物件，但未連線到Workfront Planning記錄型別的物件型別。 您只能顯示在Workfront Planning中連線的物件或記錄型別。

  例如，任務會連線至Workfront中的專案。 使用劃分功能，您可以在Planning中顯示連結至行銷活動的專案，但不能顯示連結至Workfront中專案的任務。

  如果您想要在Workfront Planning記錄型別的時程檢視中同時顯示產品組合和專案，產品組合和專案都必須連線至Planning記錄，或連線至您正在管理其時程檢視之Planning記錄的記錄。
* 您只能顯示與至少兩個日期欄位關聯的記錄型別。
* 您要在時間軸檢視中顯示的記錄型別日期欄位，必須在所選記錄型別的表格檢視中顯示，以作為查詢欄位。
* 您要在時間軸檢視中顯示的記錄型別的「開始」和「結束」日期必須依時間順序排列。 例如，如果記錄的開始日期為1月31日，結束日期為1月1日，則它不會顯示在時間軸檢視中。 如需詳細資訊，請參閱本文中的[管理時間表檢視](#manage-a-timeline-view)一節。
* 您可以在記錄的劃分中加入5種記錄型別的限制。

#### 劃分連線記錄

1. 如文章[管理記錄檢視](/help/quicksilver/planning/views/manage-record-views.md)中所述，建立記錄型別的時間表檢視。
1. （視條件而定）如果您正在以標準模式檢視時間軸檢視，請按一下&#x200B;**劃分**。
1. 展開&#x200B;**選取連結的記錄型別**&#x200B;方塊並選取連線的記錄型別。<!--add a new screen shot - submitted a bug to remove the "the"-->

   時間軸檢視上的![劃分選擇器和按鈕](assets/breakdown-picker-and-button-on-timeline.png)

   >[!TIP]
   >
   >    如果您沒有任何連線的記錄，或連線的記錄至少沒有兩個日期欄位，**選取連結的記錄型別**&#x200B;方塊將無法使用。

1. 選擇&#x200B;**開始日期**&#x200B;和&#x200B;**結束日期欄位**。

   >[!TIP]
   >
   >    開始和結束日期必須是循序的。 如果「結束日期」早於「開始日期」，則時間軸中不會顯示任何記錄。

   如果選取的記錄與其他記錄連線，則時間軸中的列會顯示一個向右的箭頭。
1. 按一下向右箭號以展開記錄型別，顯示為「連線」。

   ![依時間表檢視中的方案劃分的行銷活動](assets/campaigns-broken-down-by-programs-in-timeline-highlighted.png)

1. （選用）重複上述步驟以新增更多連線記錄。



