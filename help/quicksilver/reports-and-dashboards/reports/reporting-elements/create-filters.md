---
product-area: reporting
navigation-topic: reporting-elements
title: 在Adobe Workfront建立或編輯篩選器
description: 您可以限制在包含篩選器的項目清單中的螢幕上顯示的資訊量。 您可以根據對象的特定資訊定義某些條件，並只顯示符合這些條件的對象。
author: Nolan
feature: Reports and Dashboards
exl-id: 2e912e32-7924-418d-9d55-ce3c09f67d3e
source-git-commit: d6b483fd1f28012eb8df3e578a44187de6c3629d
workflow-type: tm+mt
source-wordcount: '2405'
ht-degree: 2%

---

# 在Adobe Workfront建立或編輯篩選器

您可以限制在包含篩選器的項目清單中的螢幕上顯示的資訊量。 您可以根據對象的特定資訊定義某些條件，並只顯示符合這些條件的對象。

可以在Adobe Workfront應用以下類型的篩選器：

* 在對象清單中快速篩選，以使用關鍵字查找項。 這些是暫時篩選器，您無法保存以備將來使用。

   有關快速篩選器的資訊，請參見 [將快速篩選器應用於清單](../../../workfront-basics/navigate-workfront/use-lists/apply-quick-filter-list.md)。

* 您可以保存和使用多個清單和報告上的大量時間的永久篩選器。 本文介紹如何建立永久篩選器或編輯清單或報告中的現有篩選器。

* 在Workfront其他地區，在清單和報告之外進行過濾。

   有關Workfront所有篩選器的清單以及可應用這些篩選器的區域，請參見 [篩選器概述Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)。

## 訪問要求

您必須具有以下訪問權限才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront計畫</strong></td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront許可證*</strong></td> 
   <td> <p>請求或更高</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>訪問級別配置*</strong></td> 
   <td> <p>編輯對篩選器、視圖和分組的訪問</p> <p>注：如果您仍然沒有訪問權限，請詢問您的Workfront管理員是否在您的訪問級別設定了其他限制。 有關Workfront管理員如何修改您的訪問級別的資訊，請參見 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自定義訪問級別</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>對象權限</strong></td> 
   <td> <p>管理對篩選器的權限</p> <p>有關請求附加訪問的資訊，請參見 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求訪問對象 </a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要瞭解您擁有的計畫、許可證類型或訪問權限，請與您的Workfront管理員聯繫。

## 構建篩選器介面的類型

可以使用下表中描述的過濾器構建器類型建立過濾器：

<table style="table-layout:auto">
<col>
<col>
<col>
<tbody>
<tr>
<td><strong>生成器類型</strong></td>
<td><strong>篩選對象</strong></td>
<td><strong>可用時</strong></td>
</tr>
<tr>
<td>標準生成器</td>
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
<li> <p>方案規劃器中的「項目」清單</p> <p>方案規劃器需要附加許可證。 有關Workfront方案規劃器的資訊，請參閱 <a href="../../../scenario-planner/scenario-planner-overview.md">方案計畫員概覽</a>。 </p> </li>
</ul>
<p>注：報表中不提供篩選器的標準構建器。
</td>
</tr>
<tr>
<td>舊式生成器</td>
<td>所有物件 </td>
<td>清單和報告</td>
</tr>
</tbody>
</table>

有關Workfront對象的資訊，請參見 [瞭解Adobe Workfront的對象](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md)。

使用不同的介面建立過濾器時，請考慮以下事項：

* 在找到上表所列區域的舊式過濾器介面的相同位置中，可以找到標準生成器。
* 標準生成器是所有可用區域的預設體驗。 要切換到舊式篩選器生成器，請按一下 **更多** 菜單 [!UICONTROL **篩選器**] 選擇 [!UICONTROL **返回舊式篩選器**]。

   ![返回舊版篩選器](assets/use-legacy-filters.png)

* 保存的濾鏡在兩個構建器中都可用，而不管您最初使用哪種經驗來構建它們。 例如，如果使用舊式生成器建立篩選器，則也可以在標準生成器介面中查找和修改篩選器。

   >[!TIP]
   >
   >標準生成器中不包含「全部」篩選器，因為未應用篩選器時將顯示所有清單項。 按一下 [!UICONTROL **全部清除**] 在生成器右上角，清除任何活動篩選器並顯示所有項目。 如果 [!UICONTROL **全部清除**] 灰顯，則不應用濾鏡。

* 在構建組合AND和OR運算子的多語句篩選器時，標準構建器和舊式構建器的語法稍有不同。 因此，當您從一個生成器切換到另一個生成器時，這些篩選器的顯示方式可能會有所不同。

   >[!INFO]
   >
   >存在以下方案：
   >
   >1. 使用標準生成器建立具有以下語法的篩選器：
   >
   >   `(A OR B) AND C`
   >
   >1. 切換到舊式生成器，並使用舊式生成器的語法編輯過濾器，如 [在舊式生成器中建立或編輯篩選器](#create-filter-in-legacy-builder) 的下界。 舊式生成器的語法按如下方式顯示篩選器語句：
   >
   >   `A AND C`
   >   `OR`
   >   `B AND C`
   >
   >1. 更改舊式介面中的篩選器。
   >1. 切換回標準生成器。 過濾器語句根據舊式生成器中支援的邏輯顯示，如上所述。

   >
   >   篩選器在標準生成器介面中顯示如下：
   >  
   >   `A AND C`
   >   `OR`
   >   `B AND C`
   > 
   >   這是因為在舊式介面中修改了篩選器。

## 在標準生成器中建立或編輯篩選器

可以使用標準生成器介面按以下方式建立篩選器：

* 從頭開始
* 編輯現有篩選器
* 複製現有篩選器
* 複製現有篩選器，編輯它並將其另存為新篩選器

使用標準生成器介面建立篩選器：

1. 轉到要建立篩選器或包含要自定義的篩選器的清單。
1. 按一下 **篩選** 表徵圖 ![「篩選器」表徵圖](assets/filter-nwepng.png) 開啟生成器介面。

   ![標準篩選器生成器](assets/new-filters-all-filter-types.png)

1. 查看以下篩選器清單：

   <table style="table-layout:auto">
   <col>
   <col>
   <tbody>
   <tr>
   <td role="rowheader"><strong>已新增至最愛</strong></td>
   <td>標籤為收藏夾的篩選器。 當您收藏濾鏡時，其原始位置顯示在濾鏡名稱下方，除非您將其作為收藏夾刪除，否則它將隱藏在原始清單中。</td>
   </tr>
   <tr>
   <td role="rowheader"><strong>已儲存</strong></td>
   <td>您自己構建並保存的篩選器。 預設情況下，此清單按最近保存的順序顯示已保存的篩選器，但可以拖動篩選器名稱以手動重新排序清單。</td>
   </tr>
   <tr>
   <td role="rowheader"><strong>系統預設值</strong></td>
   <td>Workfront系統預設篩選器，以及Workfront管理員在系統級別或佈局模板中添加到篩選器清單的篩選器。</td>
   </tr>
   <tr>
   <td role="rowheader"><strong>與我共用</strong></td>
   <td>其他人建立並與您共用的或在系統範圍內共用的篩選器。</td>
   </tr>
   </tbody>
   </table>

1. 執行下列任一項作業：

   * 按一下 **新建篩選器** 建立從頭開始的篩選器。
   * 將滑鼠懸停在您具有管理權限的現有篩選器上，然後按一下 **編輯** 表徵圖 ![編輯表徵圖](assets/edit-icon.png) 編輯。

      或

      將滑鼠懸停在您有權查看的現有篩選器上，按一下 **更多** 菜單 ![「更多」菜單](assets/more-icon-spectrum.png)，然後按一下 **重複** 複製現有篩選器並編輯副本。
   ![更多菜單選項](assets/new-filters-more-menu-options-with-delete.png)

1. （條件）根據是否要查找與篩選器組中所有語句或任何語句相匹配的對象，從以下選項中進行選擇：

   <table style="table-layout:auto">
   <col>
   <col>
   <tbody>
   <tr>
   <td role="rowheader"><strong>全部為 True 時包含</strong></td>
   <td>篩選器找到的對象必須與篩選器組中的所有篩選條件相匹配。 在這種情況下，篩選器語句由AND運算子連接。 這是預設選擇。</td>
   </tr>
   <tr>
   <td role="rowheader"><strong>任一項為 True 時包含</strong></td>
   <td>篩選器找到的對象必須與篩選器組中的任何篩選條件匹配。 在這種情況下，篩選器語句由OR運算子連接。</td>
   </tr>
   </tbody>
   </table>

   ![包含（如果全部或任意）或「真」下拉菜單](assets/new-filters-all-or-any-are-true-drop-down-menu-nwe.png)

   有關篩選器運算子的詳細資訊，請參見 [篩選器概述Adobe Workfront](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/filters-overview.md)。

1. 按一下欄位下拉菜單可查看最近使用的欄位和建議的要篩選的欄位的清單。 建議的欄位當前顯示在您正在篩選的清單中。

   也可以選擇 **瀏覽欄位** 查看可按篩選的所有欄位的清單。 高級搜索中的欄位按對象類別分組。

   ![查找要篩選的欄位](assets/new-filter-search-for-field.png)

1. 按一下修改量下拉菜單以選擇修改量。 預設修飾符為「等於」。

   有關詳細資訊，請參見 [篩選器和條件修飾符](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md)。

   >[!TIP]
   >
   >生成過濾器時，結果會立即顯示在清單中。 如果篩選器面板覆蓋清單，則可以關閉它以查看顯示。 當您再次開啟面板時，輸入的資訊將保留在生成器中。

1. 開始鍵入要篩選依據的欄位的值。 例如，如果要按以下方式篩選，請開始鍵入問題名稱 `Issue:Name`。 當值顯示在清單中時，選擇它。

   >[!TIP]
   >
   >根據您選擇的修改量，您可以選擇多個值。

1. 按一下 **添加篩選器** 框中，選擇「 CSV文本」。
1. （可選）按一下 **刪除** 表徵圖 ![刪除表徵圖](assets/delete.png) 刪除現有篩選器語句。

   或

   按一下 **全部清除** 以清除所有篩選條件。

1. （可選）按一下 **添加篩選器組** 添加另一組篩選條件。 集之間的預設運算子為AND。 按一下運算子將其更改為「或」。

   >[!TIP]
   >
   >當希望組通過與篩選器語句中的運算子不同的運算子連接時，您可能希望使用另一個篩選器組。

   >[!INFO]
   >
   >在篩選名稱中包含「市場營銷」的項目時，您可以使用以下多個篩選器組：
   >`(Project: Name Contains Marketing AND Project: Percent Complete Does not equal 100)`
   >`OR`
   >`(Project: Name Contains Marketing AND Project: Status Does not equal On Hold)`
   >在這種情況下，每個過濾器語句通過AND連接，而過濾器組通過OR連接。

1. （可選）按一下 **文本模式** 以繼續使用文本模式構建篩選器。

   ![選擇文本模式](assets/new-filter-select-text-mode.png)

   文本模式介面開啟。

   ![文本模式介面](assets/text-mode-interface-for-beta-filters-nwe.png)

   >[!TIP]
   >
   >我們建議盡可能使用標準構建器介面構建過濾器，並且在必須修改僅在文本模式下支援的過濾器時，僅使用文本模式。

   有關使用文本模式介面建立篩選器的詳細資訊，請參見 [使用文本模式編輯篩選器](/help/quicksilver/reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md)。

1. 按一下 **退出文本模式** 返回標準生成器介面。

   >[!WARNING]
   >
   >標準生成器或舊式介面不支援某些文本模式語句。 建立這些類型的語句後退出文本模式可能會生成警告消息。

1. （可選）按一下 **應用** 將篩選器應用到清單並查看結果。

   如果篩選器未產生任何結果，則清單將為空。

1. 按一下 **另存為新** 以保存篩選器以供將來使用。

   ![命名並保存篩選器](assets/save-as-untitled-filter-ui-nwe.png)

1. 選擇 **無標題篩選器** 鍵入新篩選器的名稱。

   >[!TIP]
   >
   >請務必命名篩選器，以便稍後找到它。 如果未命名過濾器，它將在系統中稱為「無標題過濾器」。

1. 從 **表徵圖** 的下界。

   ![選擇篩選器的表徵圖](assets/new-filter-select-icon.png)

1. （可選）添加篩選器的說明，以指明其唯一性。 說明顯示在篩選器清單的篩選器名稱下。

   >[!TIP]
   >
   >按一下 **取消** 隨時帶你回到過濾器建築區。

1. 按一下 **保存**。 篩選器將保存在「已保存」清單中，並應用於項清單。
1. （可選）要將濾鏡移到「收藏」清單，請將滑鼠懸停在濾鏡抽屜中的任何濾鏡上，然後按一下「收藏」表徵圖 ![收藏夾表徵圖](assets/favorites-icon-small.png)。

   或

   將滑鼠懸停在濾鏡抽屜中的任何濾鏡上，按一下「更多」菜單 ![「更多」菜單](assets/more-icon-spectrum.png)，然後按一下 **收藏夾**。

1. （可選）按一下 **堆棧篩選器** 按鈕。 此選項允許您應用多個保存的篩選器。 篩選規則按您選擇的順序應用。

   >[!TIP]
   >
   >可以選擇的篩選器數量沒有限制。
   >
   >選擇多個濾鏡時，必須同時滿足其所有條件才能顯示匹配結果。

   ![堆疊篩選器](assets/new-filter-stack-filters.png)

   選定的篩選器數顯示在項目清單頂部的篩選器表徵圖旁邊。

   ![選定的篩選器數](assets/number-of-filters-selected.png)

1. （可選）執行下列操作之一：

   * 與其他人共用過濾器，或使其在系統範圍內可用。 有關詳細資訊，請參見 [共用篩選器、視圖或分組](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/share-filter-view-grouping.md)。

   * 如果篩選器不再有效或重複，請刪除它。 您只能刪除自己擁有的篩選器。 您可以刪除與您共用的篩選器。 有關資訊，請參見 [刪除篩選器、視圖和分組](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/remove-filters-views-groupings.md)。

## 在舊式生成器中建立或編輯篩選器 {#create-filter-in-legacy-builder}

您可以通過以下方式在清單和報告中建立舊篩選器：

* 從頭開始
* 編輯現有篩選器並將其另存為新篩選器

無論您使用何種方法建立篩選器，從頭建立篩選器或從現有篩選器建立篩選器都是相似的。

1. 轉到包含要自定義的篩選器的清單或報表。
1. 按一下 **篩選** 表徵圖 ![「篩選器」表徵圖](assets/filter-nwepng.png)。

   >[!TIP]
   >
   >報表建立者必須允許編輯篩選器，以便查看報表上的「篩選器」下拉清單。 預設情況下，「報告預設」篩選器將應用於報告。 只有編輯報告時，才能自定義報告預設篩選器。

   ![篩選器下拉清單](assets/filter-drop-down-expanded-nwe.png)

1. 按一下 **新建篩選器** 清單中的「 」。

   或

   懸停在要修改的篩選器上，然後按一下 **編輯** 表徵圖 ![](assets/edit-icon.png)。

   啟動用於自定義篩選器的生成器。

1. 執行下列任一操作：

   * 通過按一下現有規則並選擇新選項來修改現有篩選器規則。
   * 通過按一下 **添加另一個篩選器規則**，開始鍵入要在 **開始鍵入欄位名稱** 框中，然後在下拉清單中顯示時按一下。

      與篩選器對象關聯的欄位列在 **開始鍵入欄位名稱** 框。

   * 按一下 **和** 或 **或** 添加新篩選器規則時。\
      添加篩選器規則時，使用篩選器修飾符來建立篩選器的條件。 有關篩選器修飾符的詳細資訊，請參閱 [篩選器和條件修飾符](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md)。

      >[!NOTE]
      >
      >通過多個OR語句連接一組AND語句時，必須重複在每組語句的OR語句之間不更改的欄位。
      >
      >![連接的篩選器語句](assets/filters-and-statements-connected-by-or-statements-builder-ui-old-filters-2022.png)
      >
      >在為包含「市場營銷」一詞且處於「當前」或「計畫」狀態的項目中的任務構建篩選器時，必須具備以下篩選器規則：
      >
      >`Task: Name Contains Marketing`
      >`AND`
      >`Project: Status Equals Current`
      >`OR`
      >`Task: Name Contains Marketing`
      >`AND`
      >`Project: Status Equals Planning`
      >
      >儘管任務：名稱包含「市場營銷」在兩個AND篩選器組之間不會更改，必須在第二個組中重複它。

   * 按一下「X」表徵圖刪除現有篩選器規則。

1. （可選）按一下 **切換到文本模式** 以使用「文本模式」介面添加篩選器。

   有關使用文本模式介面建立篩選器的詳細資訊，請參見 [使用文本模式編輯篩選器](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md)。

1. 按一下 **保存篩選器** 建立新篩選器或用更改替換選定的篩選器。

   或

   按一下 **另存為新篩選器** 中各屬性的附加資訊。

   新篩選器將顯示在篩選器清單中，並會自動應用於您選擇的清單或報告。

1. （可選）執行下列操作之一：

   * 與其他用戶共用您建立的篩選器，或使其在系統範圍內可用。 有關資訊，請參見 [共用篩選器、視圖或分組](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/share-filter-view-grouping.md)。
   * 刪除不再希望顯示在清單中的篩選器。 有關資訊，請參見 [刪除篩選器、視圖和分組](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/remove-filters-views-groupings.md)。


