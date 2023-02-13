---
product-area: reporting
navigation-topic: reporting-elements
title: 在Adobe Workfront中建立或編輯篩選器
description: 您可以透過篩選限制項目清單中畫面上顯示的資訊量。 您可以根據有關對象的特定資訊定義特定條件，並只顯示符合這些條件的對象。
author: Lisa
feature: Reports and Dashboards
exl-id: 2e912e32-7924-418d-9d55-ce3c09f67d3e
source-git-commit: fd2723eeb6a8323a8f2fcdb506991704777bdea8
workflow-type: tm+mt
source-wordcount: '2483'
ht-degree: 1%

---

# 在Adobe Workfront中建立或編輯篩選器

您可以透過篩選限制項目清單中畫面上顯示的資訊量。 您可以根據有關對象的特定資訊定義特定條件，並只顯示符合這些條件的對象。

您可以在Adobe Workfront中套用下列類型的篩選器：

* 對象清單中的快速篩選器，以使用關鍵字查找項目。 這些是暫時性篩選，您無法儲存以供日後使用。

   如需快速篩選的相關資訊，請參閱 [將快速篩選器應用於清單](../../../workfront-basics/navigate-workfront/use-lists/apply-quick-filter-list.md).

* 您可以儲存的永久篩選器，並在多個清單和報表上使用許多時間。 本文說明如何建立永久篩選器或編輯清單或報表中的現有篩選器。

* Workfront其他區域、清單與報表之外的篩選器。

   如需Workfront中所有篩選器的清單，以及可套用篩選器的區域，請參閱 [Adobe Workfront中的篩選器概觀](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront計畫*</strong></td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront授權*</strong></td> 
   <td> <p>要求或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>訪問級別配置*</strong></td> 
   <td> <p>編輯對篩選器、檢視和群組的存取權</p> <p>注意：如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>物件權限</strong></td> 
   <td> <p>管理篩選器的權限</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 篩選器建立介面的類型

您可以使用下表所述的篩選產生器類型來建立篩選器：

<table style="table-layout:auto">
<col>
<col>
<col>
<tbody>
<tr>
<td><strong>產生器類型</strong></td>
<td><strong>篩選物件</strong></td>
<td><strong>可用位置</strong></td>
</tr>
<tr>
<td>標準產生器</td>
<td>所有物件 </td>
<td>清單與報表</td>
</tr>
<tr>
<td>測試版產生器</td>
<td>
<ul>
<li> <p>專案</p> </li>
<li> <p>任務 </p> </li>
<li> <p>問題</p> </li>
<li> <p>專案組合</p> </li>
<li> <p>計劃</p> </li>
<li> <p>使用者</p> </li>
<li> <p>範本</p> </li>
<li> <p>群組</p> </li>
</ul>
</td>
<td>
<ul>
<li> <p>清單 </p> </li>
</ul>
<ul>
<li> <p>方案計畫員中的項目清單</p> <p>方案規劃器需要附加許可證。 有關Workfront方案計畫器的資訊，請參閱 <a href="../../../scenario-planner/scenario-planner-overview.md">方案計畫員概覽</a>. </p> </li>
</ul>
<p>注意：報表中無法使用篩選器的測試版產生器。
</td>
</tr>
</tbody>
</table>

如需Workfront物件的相關資訊，請參閱 [了解Adobe Workfront中的物件](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

## 在標準產生器中建立或編輯篩選器 {#create-filter-in-standard-builder}

您可以透過下列方式，在清單和報表中建立篩選器：

* 從頭開始
* 編輯現有篩選器並將其儲存為新篩選器

無論您使用何種方法建立篩選器，從草稿開始或從現有篩選器建立篩選器都很類似。

1. 前往包含您要自訂篩選器的清單或報表。
1. 按一下 **篩選** 圖示 ![篩選圖示](assets/filter-nwepng.png).

   >[!TIP]
   >
   >報表建立者必須允許編輯篩選器，才能檢視報表上的「篩選器」下拉式清單。 依預設，「報表預設」篩選器會套用至報表。 「報表預設」篩選條件僅可在您編輯報表時自訂。

   ![篩選下拉式清單](assets/filter-drop-down-expanded-nwe.png)

1. 按一下 **新增篩選** 在篩選器清單的頂端

   或

   暫留在您要修改的篩選器上，然後按一下 **編輯** 圖示 ![](assets/edit-icon.png).

   自訂篩選啟動的產生器。

1. 執行下列任一操作：

   * 按一下現有規則並選取新選項，以修改現有篩選規則。
   * 按一下 **新增其他篩選規則**，開始輸入要在 **開始鍵入欄位名稱** 框中，然後在下拉清單中出現時按一下它。

      與篩選器物件相關聯的欄位會列在 **開始鍵入欄位名稱** 框。

   * 按一下 **和** 或 **或** 新增篩選規則時。\
      新增篩選規則時，請使用篩選修飾元來建立篩選的條件。 如需篩選修飾元的詳細資訊，請參閱 [篩選條件修飾元](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

      >[!NOTE]
      >
      >通過多個OR語句連接一組AND語句時，必須對每組語句重複在OR語句之間不更改的欄位。
      >
      >![連接的篩選語句](assets/filters-and-statements-connected-by-or-statements-builder-ui-old-filters-2022.png)
      >
      >當您為包含「行銷」一詞且位於狀態為「目前」或「規劃」的專案中的任務建立篩選器時，您必須具備下列篩選規則：
      >
      >`Task: Name Contains Marketing`
      >`AND`
      >`Project: Status Equals Current`
      >`OR`
      >`Task: Name Contains Marketing`
      >`AND`
      >`Project: Status Equals Planning`
      >
      >雖然任務：名稱包含「行銷」不會在兩個「和」篩選群組之間變更，必須在第二個群組中重複。

   * 按一下「X」圖示以刪除現有的篩選規則。

1. （選用）按一下 **切換到文本模式** 使用「文本模式」介面添加篩選器。

   如需使用文字模式介面建立篩選器的詳細資訊，請參閱 [使用文字模式編輯篩選器](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md).

1. 按一下 **儲存篩選** 建立新篩選器，或將選取的篩選器取代為變更。

   或

   按一下 **另存為新篩選器** ，從所選篩選器建立新篩選器。

   新篩選器會顯示在篩選器清單中，並自動套用至您選取的清單或報表。

1. （選用）執行下列其中一項作業：

   * 將您建立的篩選器共用給其他使用者，或在全系統提供。 如需詳細資訊，請參閱 [共用篩選、檢視或分組](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/share-filter-view-grouping.md).
   * 移除您不想再顯示在清單中的篩選器。 如需詳細資訊，請參閱 [移除篩選器、檢視和群組](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/remove-filters-views-groupings.md).

## 在測試版產生器中建立或編輯篩選器

使用不同介面建立篩選器時，請考量下列事項：

* 您可以在相同位置找到測試版產生器，找到上表所列區域的標準篩選介面。
* 您可以在標準與測試版產生器介面之間來回切換，此介面提供測試版選項。
* 在單一區域中啟用測試版產生器後，就會是所有可用區域的預設體驗。 例如，如果您在專案清單中啟用測試版產生器，這也是您在清單中建立任務和問題篩選器的預設體驗。
* 您可以使用測試版產生器介面，透過下列方式建立篩選：

   * 從頭開始
   * 編輯現有篩選器
   * 複製現有篩選器
   * 複製現有篩選器、編輯該篩選器，然後儲存為新篩選器

* 儲存的篩選器可供兩個產生器使用，無論您原本用來建立篩選器的體驗為何。 例如，如果您使用標準產生器建立篩選器，也可以在測試版產生器介面中尋找和修改篩選器。

   >[!TIP]
   >
   >測試版產生器不包含「全部」篩選，因為所有清單項目都會在未套用篩選時顯示。 按一下 **全部清除** 在產生器的右上角，以清除任何作用中的篩選器並顯示所有項目。 若 **全部清除** 灰顯，則不會套用篩選。

* 建立結合AND和OR運算子的多陳述式篩選器時，標準和測試版產生器的語法稍有不同。 因此，當您從一個產生器切換至另一個產生器時，這些篩選器的顯示可能會不同。

   >[!INFO]
   >
   >存在以下情形：
   >
   >1. 使用測試版產生器來建立具有下列語法的篩選器：
   >
   >   `(A OR B) AND C`
   >
   >1. 切換回標準產生器，並使用標準產生器的語法編輯篩選器，如 [在標準產生器中建立或編輯篩選器](#create-filter-in-standard-builder) 一節。 標準產生器的語法會依照下列方式顯示篩選陳述式：
   >
   >   `A AND C`
   >   `OR`
   >   `B AND C`
   >
   >1. 變更標準介面中的篩選器。
   >1. 切換回測試版產生器。 篩選陳述式會根據標準產生器支援的邏輯顯示，如上所述。

   >
   >   篩選器會顯示在測試版產生器介面中，如下所示：
   >  
   >   `A AND C`
   >   `OR`
   >   `B AND C`
   > 
   >   之所以發生此情況，是因為篩選器是在標準介面中修改的。

使用測試版產生器介面建立篩選器：

1. 移至您要建立篩選器或包含要自訂篩選器的清單。
1. 按一下 **篩選** 圖示 ![篩選圖示](assets/filter-nwepng.png)，然後啟用 **測試版設定** ![測試版設定](assets/beta-toggle-white-on-existing-filters.png) 存取測試版產生器。 預設為停用。

   接下來，視需要同意測試版協定。 您只需同意一次，測試版產生器就會保持啟用。

   這會開啟測試版篩選產生器介面。

   >[!TIP]
   >
   >啟用測試版產生器時，篩選產生器介面的標題會變為藍色。 啟用測試版產生器介面後，Workfront會在所有可用區域中持續啟用它。

   ![測試版篩選產生器](assets/new-filters-all-filter-types.png)

1. 檢閱下列篩選器清單：

   <table style="table-layout:auto">
   <col>
   <col>
   <tbody>
   <tr>
   <td role="rowheader"><strong>已新增至最愛</strong></td>
   <td>您標示為我的最愛的篩選器。 當您收藏某個篩選器時，其原始位置顯示在篩選器名稱下方，並且它將從原始清單中隱藏，除非您將其作為收藏刪除。</td>
   </tr>
   <tr>
   <td role="rowheader"><strong>已儲存</strong></td>
   <td>您建立並儲存自己的篩選器。</td>
   </tr>
   <tr>
   <td role="rowheader"><strong>系統預設值</strong></td>
   <td>Workfront系統預設篩選器，以及Workfront管理員新增至篩選器清單的篩選器（在系統層級或您的配置範本中）。</td>
   </tr>
   <tr>
   <td role="rowheader"><strong>與我共用</strong></td>
   <td>其他人建立並與您共用的篩選器，或是在全系統內共用的篩選器。</td>
   </tr>
   </tbody>
   </table>

1. 執行下列任一項作業：

   * 按一下 **新篩選器** 從頭建立篩選。
   * 將滑鼠指標暫留在您可管理的現有篩選器上，然後按一下 **編輯** 圖示 ![編輯圖示](assets/edit-icon.png) 來編輯。

      或

      將滑鼠指標暫留在您可檢視的現有篩選器上，按一下 **更多** 功能表 ![更多功能表](assets/more-icon-spectrum.png)，然後按一下 **複製** 複製現有篩選器並編輯復本。
   ![更多功能表選項](assets/new-filters-more-menu-options-with-delete.png)

1. （條件性）根據您是否要查找匹配篩選器組中所有或任何語句的對象，從以下選項中選擇：

   <table style="table-layout:auto">
   <col>
   <col>
   <tbody>
   <tr>
   <td role="rowheader"><strong>全部為 True 時包含</strong></td>
   <td>篩選器找到的對象必須符合篩選器組中的所有篩選條件。 在此情況下，篩選語句由AND運算子連接。 這是預設選取項目。</td>
   </tr>
   <tr>
   <td role="rowheader"><strong>任一項為 True 時包含</strong></td>
   <td>篩選器找到的對象必須符合篩選器組中的任何篩選條件。 在此情況下，篩選語句由OR運算子連接。</td>
   </tr>
   </tbody>
   </table>

   ![包含全部或任何或true下拉式功能表](assets/new-filters-all-or-any-are-true-drop-down-menu-nwe.png)

   如需篩選運算子的詳細資訊，請參閱 [Adobe Workfront中的篩選器概觀](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. 按一下欄位下拉式功能表，即可檢視最近使用欄位的清單，以及要篩選的建議欄位。 建議欄位目前顯示在您篩選的清單中。

   您也可以選取 **瀏覽欄位** 要查看可篩選的所有欄位的清單。 高級搜索中的欄位按對象類別分組。

   ![找出要篩選的欄位](assets/new-filter-search-for-field.png)

1. 按一下修飾詞下拉式功能表以選取修飾詞。 預設修飾詞為「等於」。

   如需詳細資訊，請參閱 [篩選條件修飾元](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

   >[!TIP]
   >
   >建置篩選器時，結果會立即出現在清單中。 如果篩選面板覆蓋清單，您可以關閉它以看到顯示。 當您再次開啟面板時，輸入的資訊會保留在測試版產生器中。

1. 開始鍵入要篩選的欄位的值。 例如，如果要依篩選條件，請開始輸入問題名稱 `Issue:Name`. 在值顯示在清單中時選取它。

   >[!TIP]
   >
   >您可以選取多個值，視您選取的修飾詞而定。

1. 按一下 **新增篩選** 選擇其他欄位，並將新的篩選條件添加到filter語句中。
1. （選用）按一下 **刪除** 圖示 ![刪除圖示](assets/delete.png) 刪除現有篩選器語句。

   或

   按一下 **全部清除** 來清除所有篩選條件。

1. （選用）按一下 **新增篩選器群組** 新增另一組篩選條件。 集之間的預設運算子為AND。 按一下運算子，將其變更為OR。

   >[!TIP]
   >
   >當希望組由與篩選器語句中的運算子不同的運算子連接時，您可能希望使用另一個篩選器組。

   >[!INFO]
   >
   >當您篩選名稱中包含「行銷」且名稱未完成且非「暫掛」的專案時，可以使用下列多個篩選群組：
   >`(Project: Name Contains Marketing AND Project: Percent Complete Does not equal 100)`
   >`OR`
   >`(Project: Name Contains Marketing AND Project: Status Does not equal On Hold)`
   >在這種情況下，每個篩選語句都通過AND連接，而篩選組通過OR連接。

1. （選用）按一下 **文字模式** 繼續使用文字模式建立篩選器。

   ![選擇文本模式](assets/new-filter-select-text-mode.png)

   文本模式介面開啟。

   ![文本模式介面](assets/text-mode-interface-for-beta-filters-nwe.png)

   >[!TIP]
   >
   >建議您使用測試版產生器介面，並僅使用文字模式，盡可能多地建立篩選器，當您必須修改僅支援文字模式的篩選器時。

   如需使用文字模式介面建立篩選器的詳細資訊，請參閱 [使用文字模式編輯篩選器](/help/quicksilver/reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md).

1. 按一下 **退出文本模式** 返回測試版產生器介面。

   >[!WARNING]
   >
   >測試版產生器或標準介面不支援某些文字模式陳述式。 當您建立這些類型的陳述式時退出文字模式可能會產生警告訊息。

1. （選用）按一下 **套用** 將篩選器套用至清單並查看結果。

   如果篩選器未產生任何結果，則清單將為空。

1. 按一下 **另存為新** 儲存篩選器以供日後使用。

   ![命名並儲存篩選器](assets/save-as-untitled-filter-ui-nwe.png)

1. 選擇 **無標題篩選** 並輸入新篩選器的名稱。

   >[!TIP]
   >
   >請務必為篩選器命名，以便稍後找到篩選器。 如果您未為篩選器命名，系統會將其命名為「未命名篩選器」。

1. 從 **圖示** 下拉式功能表。

   ![選取篩選的圖示](assets/new-filter-select-icon.png)

1. （選用）新增篩選器的說明，以指出篩選器的獨特之處。 說明會顯示在篩選器清單的篩選器名稱下。

   >[!TIP]
   >
   >按一下 **取消** 隨時帶您返回篩選器建置區。

1. 按一下 **儲存**. 篩選器會儲存在「儲存」清單中，並套用至項目清單。
1. （可選）若要將篩選器移至「我的最愛」清單，請將滑鼠指標暫留在篩選器抽屜中的任何篩選器上，然後按一下「我的最愛」圖示 ![最喜愛的圖示](assets/favorites-icon-small.png).

   或

   將滑鼠指標暫留在篩選器抽屜中的任何篩選器上，按一下「更多」功能表 ![更多功能表](assets/more-icon-spectrum.png)，然後按一下 **最愛**.

1. （選用）按一下 **堆疊篩選器** 按鈕來啟用堆疊篩選器。 此選項可讓您套用多個儲存的篩選。 篩選規則會依您選取的順序套用。

   >[!TIP]
   >
   >可選取的篩選器數量沒有限制。
   >
   >選取多個篩選器時，必須同時符合其所有條件才會顯示相符的結果。

   ![堆疊篩選器](assets/new-filter-stack-filters.png)

   您選取的篩選器數目會顯示在項目清單頂端的篩選圖示旁。

   ![已選取的篩選器數](assets/number-of-filters-selected.png)

1. （選用）執行下列其中一項作業：

   * 與他人共用篩選器，或在全系統提供篩選器。 如需詳細資訊，請參閱 [共用篩選、檢視或分組](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/share-filter-view-grouping.md).

   * 如果篩選器不再有效或重複，請刪除該篩選器。 您只能刪除自己擁有的篩選器。 您可以移除已共用給您的篩選器。 如需詳細資訊，請參閱 [移除篩選器、檢視和群組](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/remove-filters-views-groupings.md).

