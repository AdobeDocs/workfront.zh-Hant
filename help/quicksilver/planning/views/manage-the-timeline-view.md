---
title: 管理時間表檢視
description: 在Adobe Workfront Planning記錄型別頁面的時間軸檢視中，存取及編輯記錄。 本文說明如何建立時間表檢視，以及如何編輯或刪除現有的時間表檢視。 使用篩選器、群組和設定自訂時間軸。 使用「劃分」功能來顯示連線的記錄。
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: f348af7f-5bb9-4d88-9bcb-3bef7e8892dd
source-git-commit: 4e295b4fdbbde7439567ef2a4f4383ad8dea738c
workflow-type: tm+mt
source-wordcount: '3872'
ht-degree: 2%

---

# 管理時間表檢視

<span class="preview">本頁醒目提示的資訊指出尚未普遍可用的功能。 它僅在預覽環境中可供所有客戶使用。 每月發行至生產環境後，生產環境中為啟用快速發行的客戶也提供相同的功能。</span>

<span class="preview">如需快速發行資訊，請參閱[為您的組織啟用或停用快速發行](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>

{{planning-important-intro}}

存取Adobe Workfront Planning中的記錄型別頁面時，您可以在時間軸檢視中顯示記錄。

如需有關記錄檢視的資訊，請參閱[管理記錄檢視](/help/quicksilver/planning/views/manage-record-views.md)。

## 存取需求

+++ 展開以檢視存取需求。 

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
<ul><li>選擇</li> 
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
<p>貴組織的Workfront例項必須上線至Adobe Unified Experience，才能存取Workfront Planning。</p> 
<p>如需詳細資訊，請參閱<a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">適用於Workfront的Adobe Unified Experience</a>。 </p> 
   </td> 
   </tr> 
  </tr> 
    <td role="rowheader"><p>Adobe Workfront授權*</p></td> 
   <td><p> 建立和刪除檢視的標準</p>
   <p>更新檢視元素的投稿人或更新者</p>
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
   <p>檢視許可權以暫時變更檢視設定或複製檢視</p> </td> 
  </tr> 
<tr>
   <td role="rowheader"><p>版面配置範本</p></td>
   <td> 必須為具有輕度或貢獻者授權的使用者指派包含Planning的版面配置範本。
   <p>標準使用者和系統管理員預設會啟用Planning區域。</p></div></li></ul>
</td>
  </tr>
</tbody> 
</table>

*如需Workfront存取需求的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++     

## 管理時間表檢視 {#manage-a-timeline-view}

建立時間表檢視時，所選記錄型別的所有記錄都會以時間順序時間表顯示。

請考量下列事項：

* 您至少有兩個日期欄位與記錄型別相關聯時，才能建立時間表檢視。 當您有一個或沒有與記錄型別相關聯的日期欄位時，時間軸檢視選項會變暗。

  建立時間表檢視時，您可以從下列日期欄位中選取：

   * 記錄日期
   * 記錄系統產生的欄位：建立日期、上次修改日期
   * 來自已連線的記錄或物件型別的查詢日期（只有在您連線記錄或物件型別時為其新增彙總器時）
* 根據與記錄關聯的日期，在下列情況下，某些記錄可能不會顯示在時間軸檢視中：

   * 當開始和結束日期沒有值時
   * 當「開始」或「結束」日期沒有值時
   * 當開始日期在結束日期之後時

<div class="preview">

* 您可以在時間表檢視中建立和編輯記錄。 如需詳細資訊，請參閱[建立記錄](/help/quicksilver/planning/records/create-records.md)。

</div>

<!--move this bullet under the same div as above OR add a span or another div tag?? ??

* You can resize the records' bars in the timeline view by clicking, then dragging and dropping their margins in a new position. Resizing the records' bars updates their start and end dates immediately. For information, see [Edit records](/help/quicksilver/planning/records/edit-records.md).

-->

若要管理時間表檢視：

1. 移至您要檢視其時間軸的記錄型別頁面。
1. 建立時間表檢視，如文章[管理記錄檢視](/help/quicksilver/planning/views/manage-record-views.md)中所述。

   ![時間表檢視範例](assets/timeline-view-example.png)

   與您選取的記錄型別相關聯的記錄會在時間軸中顯示為長條，並依其開始日期的時間順序依預設排序。

   >[!TIP]
   >
   >    時間軸中記錄的排序在壓縮檢視中不可見。

1. （視條件而定）如果管理員已啟用自訂季度，而Workfront偵測到自訂季度設定方式發生問題，則開啟時間表檢視時，您可能會收到警告。

   存在下列情況：

   * 如果偵測到季度日期之間有間隔或重疊，您可能會收到通知，告知您現在可以設定自訂季度，且這些季度可能需要編輯。

     ![自訂季度通知遺失或季度之間有間隔](assets/custom-quarter-notification-missing-or-gaps.png)

     >[!TIP]
     >
     >只有在貴組織購買後，才應立即顯示此訊息。購買前，已啟用Planning和自訂季度。 為您的組織啟用Workfront規劃後，不允許季度之間的重疊和間隙。

   * 如果季度已部分設定，而同一年內有某些月份遺失，當您捲動以顯示一年其餘時間需要使用遺失季度設定的遺失季度時，可能會收到通知。

   ![時間軸檢視上遺失自訂季度原始訊息](assets/missing-custom-quarters-original-message-on-timeline-view.png)

   關於自訂季度的警告訊息為每位使用者顯示一次。

   >[!NOTE]
   >
   >若未正確儲存自訂季度，則時間軸檢視會顯示傳統季度。
   >在「設定」區域中設定自訂季度後，時間軸檢視會顯示自訂季度，而非傳統季度。
   >如需詳細資訊，請參閱[啟用自訂季度](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-custom-quarters-projects.md)。

1. （視條件而定）如果您是Workfront管理員，請按一下&#x200B;**前往設定**&#x200B;設定您的季度。 如果沒有，請按一下[確定] **&#x200B;**，並要求Workfront管理員設定自訂季度。

   >[!TIP]
   >
   >僅會針對Workfront管理員顯示「前往設定」按鈕。

1. （選擇性和條件性）當記錄名稱被截斷時，將滑鼠懸停在記錄列上以顯示記錄的完整名稱和其他資訊。 如需有關在時間軸中設定記錄列截斷的資訊，請參閱本文中的[編輯時間軸檢視設定](#edit-the-timeline-view-settings)小節。

1. 執行下列任一項作業來瀏覽時間軸：

   * 按一下左上角的左右圖示，或使用水準捲動在時間軸中前後移動。 重新整理頁面會保留選取的時間範圍。
   * 按一下右上角的&#x200B;**今日**，將時間軸置中到今天的日期。
   * 從時間範圍下拉式選單中選取下列其中一個選項，以更新時間增量並更新檢視：

      * **年**：顯示有年指標的季和月。
      * **季**：顯示有季指示的月和周。
      * **月**：顯示周和日。
1. （選擇性）按一下&#x200B;**切換至精簡檢視**&#x200B;以顯示日期在同一行上不相交的記錄。<!--check to see if they updated the name of the setting here-->
1. （視條件而定）如果您將模式變更為&#x200B;**緊密**，請按一下&#x200B;**切換至標準**&#x200B;檢視，以個別行顯示記錄。 **標準**&#x200B;選項是預設值。 <!--check to see if they updated the name of the setting here-->

1. 執行下列動作以快速尋找符合關鍵字的記錄：

   1. 按一下&#x200B;**搜尋**&#x200B;圖示![搜尋圖示](assets/search-icon.png)，然後開始輸入與熒幕上顯示之記錄的任何欄位相關聯的關鍵字。 正確相符的數目會顯示在搜尋專案旁邊，而具有正確相符專案的記錄會反白顯示。

      ![搜尋方塊和結果時間表檢視](assets/search-box-and-results-timeline-view.png)

      您可以使用熒幕上可見的任何文字或特殊字元。

      您無法使用與未顯示在時間表檢視中的欄位關聯的關鍵字。

   1. 在鍵盤上按Enter鍵以移至下一個找到的欄位。
   1. （選擇性）如果有多個相符專案，請按一下搜尋關鍵字右邊的向上和向下箭頭，以尋找表格中的所有相符專案。
   1. 按一下搜尋方塊中的&#x200B;**x**&#x200B;圖示以清除搜尋關鍵字。

   1. <span class="preview">（選擇性）按一下&#x200B;**全熒幕**&#x200B;圖示![開啟全熒幕圖示](assets/open-full-screen-icon.png)以全熒幕開啟檢視，然後按一下&#x200B;**退出全熒幕**&#x200B;圖示![退出全熒幕圖示](assets/exit-full-screen-icon.png)或鍵盤上的Escape以退出全熒幕。 </span>

1. 更新下列檢視元素，如下列子區段所述：
   * [篩選器](#add-filters)
   * [分組](#add-grouping)
   * [設定](#edit-the-timeline-view-settings)
     <!--* [Sort](#add-sort) not yet in timeline; also check the anchor and make sure it's correct-->

1. （選擇性）按一下&#x200B;**劃分**，在時間軸上顯示連線的記錄。

   如需相關資訊，請參閱本文章的[使用劃分功能在時間軸檢視](#break-down-connected-records-in-the-timeline-view)中顯示連線記錄。

### 新增篩選器

您可以使用篩選器來減少熒幕上顯示的資訊量。

在時間軸檢視中使用篩選器時，請考量下列事項：

<!-- this list is almost identical to the one for the table view - update both-->

* 您為時間軸檢視建立的篩選器與套用至相同記錄型別之任何其他檢視中的篩選器是獨立運作的。

* 這些篩選器對於您選取的檢視而言是唯一的。 相同記錄型別的兩個時間軸檢視可以套用不同的篩選器。

* 檢視相同時間表檢視的兩個使用者會看到目前套用的相同篩選器。

* 您無法為您為時間表檢視建置的篩選器命名。

* 移除篩選器會將篩選器從存取與您相同記錄型別以及顯示與您相同檢視的任何人移除。

* 您可以依已連線的記錄欄位或查詢欄位進行篩選。
* 您可以依顯示多個值的查閱欄位進行篩選。

若要將篩選器新增至時間表檢視：

1. 如文章[管理記錄檢視](/help/quicksilver/planning/views/manage-record-views.md)中所述，建立記錄型別頁面的時間軸檢視。
1. 選取時間表檢視，然後按一下表格右上角的&#x200B;**篩選器**。
1. 按一下&#x200B;**新增條件**&#x200B;並新增下列資訊：

   * **選取您要依**&#x200B;篩選的欄位<!-- the tip below might change-->

   * **選取選項** （或篩選修飾元）以定義欄位必須符合何種條件

     下表顯示每種欄位型別的可用修飾元。

     <table>
        <thead>
        <tr>
            <th><b>欄位類型</b></th>
            <th><b>修飾元</b></th>
        </tr>
        </thead>
        <tbody>
        <tr>
            <td>單行，段落，公式 </td>
            <td><p>包含</p>
            <p>不包含</p>
            <p>是</p>
            <p>不是</p>
            <p>是空的</p>
            <p>不是空的</p></td>
        </tr>
        <tr><td>單選</td>
            <td><p>是</p>
            <p>不是</p>
            <p>屬於任一</p>
            <p>不屬於</p>
            <p>是空的</p>
            <p>不是空的</p></td>
        </tr>
        <tr>
            <td>多選，人員</td>
            <td><p>具有任一</p>
            <p>具有所有</p>
            <p>完全符合</p>
            <p>不具有</p>
            <p>是空的</p>
            <p>不是空的</p></td>
        </tr>
        <tr>
            <td>數字、百分比、貨幣</td>
            <td><p>=</p>
            <p>≠</p>
            <p> &lt; </p>
            <p>&gt;</p>
            <p>≤</p>
            <p>≥</p>
            <p>是空的</p>
            <p>不是空的</p></td>
        </tr>
        <tr>
            <td>日期</td>
            <td><p>是</p>
            <p>不是</p>
            <p>晚於</p>
            <p>早於</p>
            <p>介於</p><p>不介於</p>
            <p>是空的</p><p>不是空的</p></td>
        </tr>

     <tr>
            <td>核取方塊</td>
            <td><p>是</p>
        </tr>
        </tbody>
        </table>

   * 選取所選欄位的值。

   ![篩選器UI資料表檢視](assets/filter-ui-table-view.png)

   您可以新增的篩選條件數量沒有限制。

1. （選擇性）按一下&#x200B;**新增條件**&#x200B;以新增另一個篩選選項，並重複上述步驟。 套用的篩選器數會顯示在&#x200B;**篩選器**&#x200B;圖示的左側。
1. 按一下左側的下列運運算元，指示如何連結及套用篩選條件：

   * **AND**：必須符合所有指定的條件。
   * **OR**：必須符合任何指定的條件。
這是預設選項。

   1. （選擇性）新增其他篩選器群組，並由&#x200B;**AND**&#x200B;或&#x200B;**OR**&#x200B;運運算元加入。

      ![檢視中的多重層級篩選器](assets/multi-tiered-filters-in-views.png)

   系統會根據您的篩選條件自動篩選記錄清單。 <!--at this time, you can't name and save the filter - but will this change?!-->
   <!-- asked on the task for the simple filters whether there is a limitation for how many statements a filter can have?!-->

1. （選擇性）按一下&#x200B;**x**&#x200B;圖示以移除篩選條件。
1. （選擇性）按一下&#x200B;**篩選器**&#x200B;或頁面上的任何其他位置，以關閉篩選器方塊。<!--right now you cannot "clear all" for filters, but this might come later-->


### 新增分組

<!-- groupings are almost identical between this view and table  but they display a little differently, so I kept the steps for both; update in both places if they make changes to groupings-->

將群組套用至檢視時，您可以依照類似的資訊來群組記錄。

在時間軸檢視中使用群組時，請考量下列事項：

* 您可以在表格和時間軸檢視中套用群組。 表格檢視的分組與相同記錄型別之時間軸檢視中的群組是獨立的。
* 您可以在檢視中套用3個群組層級。 記錄會依照您選取的群組順序進行分組。
&lt;!—*使用API時，您最多可以套用4個層級的群組。  — 現在正在檢查此專案 — >
* 群組對於您選取的檢視而言是唯一的。 相同記錄型別的兩個表格檢視可以套用不同的群組。 檢視相同表格檢視的兩個使用者會看到目前套用的相同分組。
* 您無法為表格檢視建立的分組命名。
* 移除群組會將群組從存取與您相同記錄型別以及顯示與您相同檢視的任何人中移除。
* 您可以編輯列在群組下的記錄。
* 您可以依連線的記錄欄位或查詢欄位來分組。
* 當您依具有多個值（尚未由彙總器彙總）的查閱欄位來分組時，記錄會依每個唯一的欄位值組合來分組。
* 您可以參考與目前記錄型別相距最多4個層級的欄位。 例如，如果您正在建立「活動」記錄型別的群組，且「活動」已連線至「產品」記錄型別，而該記錄型別已連線至「行銷活動」記錄型別，而該記錄型別已連線至「Workfront專案」，則您可在您為「活動」記錄型別所建立的分組中參考專案的「狀態」。
* 群組會按其值的字母順序列出。
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
1. 按一下左側面板中的&#x200B;**日期和時間**，然後選取要在時間軸上顯示的&#x200B;**開始日期**&#x200B;和&#x200B;**結束日期**。 您可以選擇預設的「開始」和「結束」日期，也可以選擇任何可用的日期欄位。

   代表記錄的長條圖，其開始日期為您為「開始」日期指定的日期，結束日期為您與「結束」日期對應的日期。

   >[!NOTE]
   >
   >* 沒有開始或結束日期值或開始日期晚於結束日期的記錄不會顯示在時間軸檢視中。
   >
   >* 如果您使用「劃分」選項顯示其他記錄，則「開始」與「結束」日期為主要記錄的日期。 您無法在此區域選擇連線記錄的「開始」和「結束」日期。

1. （條件式與選擇性）如果您是Workfront管理員，請在&#x200B;**使用自訂季度**&#x200B;方塊中按一下&#x200B;**前往設定**，前往設定區域並設定自訂季度。 設定自訂季度後，您可以在時間軸檢視中顯示它們，而非傳統季度。 如果您不是Workfront管理員，可以向管理員要求為您的組織啟用自訂季度。

   如需詳細資訊，請參閱[啟用自訂季度](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-custom-quarters-projects.md)。

   ![在時間表檢視設定內使用自訂季度警告](assets/use-custom-quarters-warning-inside-timelive-view-settings.png)

   >[!TIP]
   >
   >僅會針對Workfront管理員顯示「前往設定」按鈕。

1. 按一下左側面板中的&#x200B;**長條樣式**，以指示您要在記錄長條上顯示的資訊。

   使用「標準」檢視中的「劃分」選項時，您可以定義主要記錄以及連線記錄的長條樣式。

   預設會選取記錄的主要欄位（或標題），如記錄的表格檢視中所定義。
   <!--adjust this when the primary field is released??-->

1. （選擇性和條件性）如果您在記錄中新增縮圖，請選取&#x200B;**縮圖**&#x200B;選項，以顯示與其記錄列中的記錄相關聯的影像。

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

1. （選擇性和條件性）如果您以標準模式顯示時間軸，請選取&#x200B;**截斷列詳細資料**&#x200B;設定。 選取時，記錄列上的資訊會被截斷，而且只有在您將滑鼠懸停在記錄列上時，才會完全顯示資訊。 預設會取消選取此設定，且記錄資訊會完全顯示在長條上。

   ![時間軸設定方塊上啟用截斷設定](assets/truncate-setting-enabled-on-timeline-settings-highlighted.png)

   >[!TIP]
   >
   >以精簡模式顯示時間軸檢視時，無法使用截斷列詳細資料設定。
   >

1. 按一下左側面板中的&#x200B;**色彩**，以自訂時間軸中記錄和群組的色彩。

   ![色彩標籤時間表檢視](assets/color-tab-timeline-view.png)

   使用「標準」檢視中的「劃分」選項時，您可以定義主要記錄以及連線記錄的色彩。

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

1. （選擇性）如果您使用&#x200B;**劃分**&#x200B;選項，請對時間軸中顯示的每個已連線記錄，重複從步驟4開始的步驟。

1. 按一下「**儲存**」。

   記錄會以您所選取的規格顯示在時間軸檢視中。

### 在時間軸檢視中劃分連線記錄

您可以使用「劃分」功能，在記錄的時間軸檢視中顯示連線的記錄。 按連線劃分記錄可讓您檢視其他連線記錄的時間表，並瞭解這些記錄可能會如何影響記錄的效能和截止日期。

#### 使用劃分功能時的注意事項

* 您可以在時間軸檢視中選取的記錄型別記錄下顯示連線的記錄或物件。
* 只有在以「標準」模式檢視記錄時，才可以在時間軸檢視中顯示連線的記錄。 您無法在時間軸檢視的「精簡」模式中使用「劃分」選項。
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
1. 從&#x200B;**標準**&#x200B;或&#x200B;**緊密**&#x200B;模式，按一下時間軸檢視右上角的&#x200B;**劃分**。
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
1. 按一下向右箭號以展開記錄型別並顯示其連線。

   ![依時間表檢視中的方案劃分的行銷活動](assets/campaigns-broken-down-by-programs-in-timeline-highlighted.png)

   >[!IMPORTANT]
   >
   >    當您在劃分中顯示多個連線的記錄時，它們並非以階層順序。
   >
   >例如，如果您檢視行銷活動的時間表，並將產品接著將方案新增至劃分，則方案不一定先連線至產品。
   >
   >產品和方案都必須連線至行銷活動，才能顯示為劃分選項的選項，而且您可以依任何順序將其新增至劃分。

1. （視條件而定）如果您正在以精簡模式檢視時間軸，請按一下&#x200B;**切換檢視**。 劃分在&#x200B;**壓縮**&#x200B;模式中不可見。

   >[!TIP]
   >
   >在&#x200B;**切換到標準檢視中選取**&#x200B;不要再顯示此專案&#x200B;**？**&#x200B;方塊，然後再切換檢視。
   >
   >只有目前的瀏覽器才會記住此喜好設定。 如果您變更瀏覽器或電腦，則必須再次選取此喜好設定。
   >
   >將檢視切換為「標準」後，您無法恢復為「緊密」模式，並在檢視中顯示已連線的記錄。
1. （選用）重複上述步驟以新增更多連線記錄。



