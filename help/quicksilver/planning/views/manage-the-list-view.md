---
title: 在Adobe Workfront規劃中管理清單檢視
description: 在Adobe Workfront Planning中，存取記錄之「連線記錄」頁面中的物件時，您可以在清單檢視中顯示物件及其欄位。 本文說明如何在記錄的「連線記錄」頁面中建立或編輯清單檢視。
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 1c7e6973-6e9e-4c93-9d3b-89ed90df9d14
last-update: 2026-04-01T18:23:03Z
git-commit-file: c04fc32836179ccbd80a7de3978493caf8ba8670
source-git-commit: cbee9aabad7300c2a7ff7aa92bc68a6368a1efcd
workflow-type: tm+mt
source-wordcount: '1799'
ht-degree: 1%

---


# 在Adobe Workfront Planning中管理清單檢視

<!--
although list views in Planning are very similar to Workfront enhanced lists, keep this one separate with all the information, because of Planning standalone; some information here is also duplicated in this main Glist article: help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md
-->

<!--
<span class="preview">The information highlighted on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

{{planning-important-intro}}

您可以在Workfront Planning的下列區域中檢視清單檢視中的物件：

* 記錄的詳細資訊區域中專案的已連線記錄頁面

  在清單檢視中![連線記錄頁面上的專案](assets/projects-on-connected-records-page-list-view.png)

* 記錄型別層級的請求表單清單

  ![在清單檢視中要求表單](assets/request-forms-in-list-view.png)

本文說明如何在Workfront Planning中導覽、建立或編輯清單檢視。

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
   <td role="rowheader"><p>Adobe Workfront授權</p></td> 
   <td><p> 建立和刪除檢視的標準</p>
   <p>更新檢視元素的投稿人或更新者</p>
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

如需Workfront存取需求的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++ 

## 關於清單檢視的考量事項

* 對於連線的記錄頁面清單檢視，請考量下列事項：

   * 您只能在記錄的已連線記錄頁面中檢視清單檢視中的專案。 清單檢視不適用於已連線記錄頁面中的任何其他物件或記錄型別。

  如需有關建立連線記錄頁面的資訊，請參閱[新增連線記錄頁面至記錄](/help/quicksilver/planning/records/add-a-connected-records-page-to-a-record.md)。
   * 您必須先將Workfront專案與Planning記錄型別連線，才能在記錄的已連線記錄頁面中檢視清單檢視。 如需詳細資訊，請參閱[連線記錄型別](/help/quicksilver/planning/architecture/connect-record-types.md)。
   * 您可以在記錄的連線記錄頁面中建立專案的多個清單檢視。

* 對於請求表單清單檢視，請考慮下列事項：

   * 您無法為Planning請求表單建立或編輯其他清單檢視。 Workfront會為請求表單建立一個清單檢視。<!--this will change-->

     如需請求表單的相關資訊，請參閱[在Adobe Workfront Planning中建立和管理請求表單](/help/quicksilver/planning/requests/create-request-form.md)。
* 根據顯示的位置，並非每個清單檢視都有本文所述的所有元素。

## 管理清單檢視 {#manage-a-list-view}

Workfront Planning清單檢視類似於Workfront的增強型清單。 增強型檢視的大部分元素也存在於清單檢視的Workfront Planning中。

如需詳細資訊，請參閱[使用增強型清單](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md)。

<!--
Removed - more direct steps below: 
{{step1-to-planning}}

1. (Conditional) To access a projects connected page, do the following: 

    1. Click a workspace card, then click a record type card. 
    1. From any view, click the name of a record to open the record's preview or details page. 
    1. Add a **Connected records page** for connected projects as described in the article [Add a Connected records page to a record](/help/quicksilver/planning/records/add-a-connected-records-page-to-a-record.md).

    The Connected records page displays projects connected to the record in the list view. 

    ![Projects on connected records page in list view](assets/projects-on-connected-records-page-list-view.png)

1. (Conditional) To access a list of request forms, do the following: 

    1. {{step1-to-planning}}

    1. (Conditional) To access a projects connected page, do the following: 

    1. Click a workspace card, then click a record type card.
    1. Click the **More** menu ![More menu](assets/more-menu.png) to the right of the record name in the header, then click **Manage request forms**.

        A list of request forms displays.

-->

1. 移至下列其中一個區域的清單檢視：

   * 記錄的詳細資訊區域中專案的已連線記錄頁面
   * 記錄型別的「請求表單」頁面

1. （視條件而定）可用時，請執行下列任一項作業來修改清單檢視：

   1. 展開清單左上角的下拉式檢視功能表，以選取其他檢視，或按一下&#x200B;**新增檢視**&#x200B;並建立另一個檢視。

      >[!TIP]
      >
      >檢視會在整個系統中共用。 如果您為一個記錄型別建立「專案」檢視，則可以在顯示已連線專案的其他記錄型別上檢視它。

   1. 將滑鼠停留在現有檢視的名稱上，然後按一下&#x200B;**更多**&#x200B;功能表![更多](assets/more-menu.png)，然後按一下下列其中一項：
      * **重新命名**，為檢視提供新名稱
      * **共用**，與其他人共用檢視
      * **刪除**，以刪除檢視。

      >[!NOTE]
      >
      >* 您必須擁有檢視的管理許可權才能編輯、共用或刪除檢視。
      >
      >* 您無法修改系統檢視。
      >
      >* 在修改檢視以恢復其原始偏好設定後，您可以重設與您共用的檢視（您只有「檢視」的許可權），也可以複製檢視並共用其副本。 如需詳細資訊，請參閱[使用增強型清單](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md)。

   1. 按一下&#x200B;**篩選器**&#x200B;圖示![篩選器圖示](assets/filter-icon.png)將篩選器新增至檢視。 結果會立即在清單中篩選。 您無法儲存並命名篩選器。 日後存取頁面時會記住篩選器，這些篩選器也是共用檢視的一部分。

      >[!TIP]
      >
      >若要套用個人化篩選，請為欄位值選取下列其中一個選項：
      >
      >* **我（已登入的使用者）**&#x200B;在引用使用者的欄位中引用已登入的使用者。
      >
      >* **我的團隊**&#x200B;或&#x200B;**我的主團隊**&#x200B;在引用團隊的欄位中引用您的團隊。
      >
      >* **我的群組**&#x200B;或&#x200B;**我的主群組**&#x200B;在引用群組的欄位中引用您的群組。
      >
      >* **我的公司**&#x200B;在引用公司的欄位中引用您的公司。
      > 
      >* **我的角色**&#x200B;或&#x200B;**我的主要角色**，在引用角色的欄位中引用您的工作角色。

   1. 按一下&#x200B;**欄**&#x200B;圖示![欄圖示](assets/columns-icon.png)以選取要在檢視中顯示或隱藏的欄。
   1. 暫留在欄名稱上，然後按一下欄名稱左側的向下箭頭，然後按一下下列其中一項：
      * **重新命名**，為資料行新增&#x200B;**自訂標籤**。 Workfront中原始欄位的名稱不會變更。
      * **排序**，依選取的欄位排序清單。 表示排序方向的排序圖示會新增至欄標題。
   1. 按一下清單右上角的&#x200B;**+**&#x200B;圖示，新增或移除清單中的欄，然後按一下&#x200B;**儲存**。

      **資料行管理員**&#x200B;開啟。

      您只能將現有欄位新增到清單檢視。
您不能移除在第一欄顯示的清單檢視中的主要欄位。

      <!-- 
        update indent here: 
        1. <span class="preview">Click the **Grouping** icon ![Grouping icon](assets/grouping-icon.png) to choose fields to group items by, then sort them in an ascending or descending order. </span>
        -->

   1. 按一下&#x200B;**格式化儲存格**&#x200B;圖示![格式化儲存格圖示](assets/format-cells-icon.png)。 **格式**&#x200B;方塊開啟。 <!--change the name of the box when they update it-->
執行下列動作：

      1. 按一下&#x200B;**新增條件**。
      1. 在&#x200B;**If**&#x200B;行中，選取欄位並選擇欄位值並新增修飾元。 修正因子會根據您選擇的欄位型別而變更。

         >[!TIP]
         >
         >只有清單檢視中顯示的欄位才適用於條件式格式。

      1. （選擇性）按一下&#x200B;**與另一個欄位比較**&#x200B;圖示![與另一個欄位比較](assets/compare-to-another-field-icon.png)並選擇您要與所選欄位值進行比較的欄位，而不新增欄位值。 例如，您可以比較專案所有者和專案贊助者欄位。

         >[!TIP]
         >
         >只有清單檢視中顯示的欄位才適用於條件式格式。 您比較的欄位必須屬於相同型別。

      1. （選擇性）按一下&#x200B;**If**&#x200B;行中的「**新增條件**」，將更多條件新增至相同規則。

         >[!TIP]
         >
         >您可以在條件規則中新增最多10個條件，而且一個欄位最多可以有20個規則。

      1. 按一下條件之間的&#x200B;**Or**&#x200B;聯結器，變更為&#x200B;**和**，並指示必須同時符合多個條件。 **或**&#x200B;是預設聯結器。
      1. 在&#x200B;**格式**&#x200B;行中，選取欄位以指示要格式化的欄。<!--edit this area, if it changes names??-->
      1. （選擇性）按一下所選欄位旁的&#x200B;**顏色圓形**&#x200B;圖示![顏色圓形圖示](assets/color-circle.png)，展開該欄位並在&#x200B;**儲存格填滿**&#x200B;區域中選擇另一種顏色，以變更儲存格中的背景顏色，或是從&#x200B;**文字顏色**&#x200B;區域挑選一種顏色，以變更儲存格中的文字顏色。
      1. 按一下&#x200B;**文字格式**&#x200B;圖示![文字格式圖示](assets/text-format-icon.png)並從下列選項中選取，以格式化儲存格中的文字：
         * 粗體
         * 斜體

      1. 開啟&#x200B;**套用至列**&#x200B;設定，將格式套用至符合條件的欄位整列。
      1. （選擇性）在&#x200B;**格式**&#x200B;方塊中按一下&#x200B;**新增條件**，為其他欄位新增另一個規則，並重複上述步驟。
      1. （選擇性）按一下「全部清除&#x200B;**」**&#x200B;以移除所有格式設定。
      1. 按一下&#x200B;**格式**&#x200B;方塊外部以關閉它。

         這會將您帶回清單檢視。
格式會立即套用至清單檢視。
**格式化儲存格**&#x200B;圖示旁有一個藍點，表示檢視已套用特殊格式。

   1. （選擇性）按一下&#x200B;**群組**&#x200B;圖示![群組圖示](assets/grouping-icon.png) <!--have they updated this to "Grouping"??-->，以使用通用欄位將清單中的專案群組。 選取其中一個選項，或使用搜尋列來尋找欄位。

      該欄位必須是清單中的欄，然後才能按它分組。 並非所有欄位型別都可用於分組。

   1. 按一下&#x200B;**列高**&#x200B;圖示![列高圖示](assets/row-height-icon.png)以更新列的垂直長度。 從下列選項中選擇:

      * 短
      * 標準。 這是預設選擇。
      * 媒體
      * 高

   <!--leave these here, although they duplicate for Enhanced lists in Workfront-->

1. （可選）在清單右上角的搜尋方塊中新增關鍵字，以搜尋專案。

   符合搜尋字詞的專案會在清單中反白顯示。

1. （選擇性和條件性）在專案<!--change projects to items here when more items will display in the Glist-->已連線的頁面中，若要新增更多專案至清單並自動將它們連線至選取的記錄，請執行下列其中一個動作：

   * 按一下清單右上角的&#x200B;**連線記錄**&#x200B;以新增現有專案。
   * 按一下清單底部的&#x200B;**新列**&#x200B;以新增專案。
1. 按一下清單中連線專案的名稱，以在其他瀏覽器標籤中開啟它。
1. 在清單的儲存格內按兩下以編輯欄位的資訊，然後按下Enter以儲存變更。

   有些欄位是唯讀的。 例如，專案的完成百分比是由系統計算的欄位，您無法手動進行編輯。

1. 將滑鼠懸停在清單中專案的名稱上，然後按一下&#x200B;**更多**&#x200B;功能表[更多](assets/more-menu.png)，然後按一下&#x200B;**檢視**&#x200B;以在另一個索引標籤中開啟專案

   或

   選取一或多個專案，並注意清單底部的動作列，然後按一下下列其中一項（如果可用）。 根據您從哪個區域存取清單檢視，按一下下列其中一個選項：

   * **刪除**&#x200B;以刪除專案。 刪除專案會中斷專案與記錄的連線，並將其移至Workfront的「資源回收筒」。 Workfront管理員可在刪除已刪除的專案後30天內復原這些專案。 刪除表單不會刪除提交表單時建立的請求或記錄。
   * **中斷連線**&#x200B;以中斷專案與記錄的連線。 中斷專案的連線會從目前記錄中移除該專案及其查閱欄位的所有值。

     連線記錄頁面清單檢視中的![動作列](assets/actions-bar-connected-records-page-list-view.png)

   * **編輯表單**：開啟Planning要求表單並允許您編輯它。
   * **取消發佈**：取消發佈要求表單。 這會從請求區域移除表單，並且使用者無法再將請求新增到此記錄型別。
   * **共用**：開啟申請表的[共用]方塊，您可以在此與其他人共用。
   * **複製連結**：複製Planning要求表單的連結，以便與其他使用者共用。 如果表單已公開共用，您可以與Workfront Planning以外的人員共用連結。

     Planning要求清單中的![動作列](assets/actions-bar-in-inake-forms-list.png)



