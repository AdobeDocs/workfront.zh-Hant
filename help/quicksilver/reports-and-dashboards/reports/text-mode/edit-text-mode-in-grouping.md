---
product-area: reporting
navigation-topic: text-mode-reporting
title: 編輯分組中的文本模式
description: '''注意：使所有FVG文章都相同，以便在文字模式中編輯)`'
author: Nolan
feature: Reports and Dashboards
exl-id: 2eeecc16-ea6d-4a56-8ea3-e213706e89bf
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '1559'
ht-degree: 1%

---

# 編輯分組中的文本模式

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">NOTE: make all FVG articles the same for editing in text mode)</p>
-->

您可以使用文字模式，在清單或報表中編輯分組，以存取標準介面中無法使用的欄位，並建立更複雜的分組。

>[!TIP]
>
>建議您在標準模式中盡可能多地建立群組，然後將其轉換為文字模式以進行編輯。

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>計劃 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>編輯對篩選器、檢視、群組的存取</p> <p>編輯對報表、控制面板、日曆的存取，以編輯報表中的群組</p> <p>注意：如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>管理報表的權限，以編輯報表中的群組</p> <p>管理群組的權限以進行編輯</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 必要條件

開始在報表或清單中使用文字模式之前，請務必熟悉Workfront文字模式語法。

如需詳細資訊，請參閱：

* [文字模式概觀](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md)
* [文字模式語法概觀](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md)
* [自訂檢視、篩選和分組範例](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md)

## 編輯分組中的文本模式

使用文字模式編輯分組對於報表和清單是相同的。 從報表或清單存取分組的方式有所差異。

>[!NOTE]
>
>分組是在報表中建立圖表時的強制報表元素。 圖表不支援文本模式分組。 有關向報表添加圖表的資訊，請參見 [新增圖表至報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

如需建立群組的詳細資訊，請參閱 [在Adobe Workfront中建立群組](../../../reports-and-dashboards/reports/reporting-elements/create-groupings.md).

如需建立報表的相關資訊，請參閱 [建立自訂報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. 執行下列任一項作業：

   1. 若要從報表存取分組，請前往報表，然後按一下 **報表動作** > **編輯** > **分組** 標籤。
   1. 要從清單訪問分組，請轉至清單，然後從 **分組** 下拉式選單中，將滑鼠移至您要修改的群組上方，然後按一下 **編輯** 圖示 ![](assets/edit-icon.png).

      分組產生器隨即開啟。

1. 按一下 **添加分組** 若要新增分組，請按一下 **切換到文本模式** 建立器的右上角。

   >[!TIP]
   在標準介面中，最多可以新增3個群組。 您只能使用文字模式來新增第4個分組，而且Workfront中的分組層級不能超過4個。

1. 開始鍵入要分組依據的欄位名稱。

   在清單中看到欄位時，請選取該欄位的名稱。

1. 按一下 **切換到文本模式** 建立器的右上角。

   然後，分組將以文本模式顯示。

   以文字模式編輯群組時，Workfront會新增

   ```
   textmode=true
   ```

   代碼行到分組。 這表示在文本模式下修改了分組。

   **範例：** 要按項目名稱然後按主要受託人的名稱對任務清單進行分組，您的分組應在文本模式下如下所示。

   ```
   textmode=true<br>group.0.linkedname=project<br>group.0.namekey=view.relatedcolumn<br><strong>group.0.valuefield=project:name</strong><br>group.0.namekeyargkey.0=project<br>group.0.namekeyargkey.1=name<br><strong>group.0.valueformat=string</strong><br>group.1.linkedname=assignedTo<br>group.1.namekey=view.relatedcolumn<br><strong>group.1.valuefield=assignedTo:name</strong><br>group.1.namekeyargkey.0=assignedTo<br>group.1.namekeyargkey.1=name<br><strong>group.1.valueformat=string</strong>
   ```

   >[!IMPORTANT]
   粗體行是必填行。

   <!--
   <div class="example" data-mc-autonum="<b>Example: </b>" data-mc-conditions="QuicksilverOrClassic.Draft mode"> <span class="autonumber"><span><b>Example: </b></span></span>
   <p>To group a list of tasks by the Project Name and then by the name of the Primary Assignee, your grouping should look like the following, in text mode:</p>
   <p><code>textmode=true</code> </p>
   <p><code>group.0.linkedname=project</code> </p>
   <p><code>group.0.namekey=view.relatedcolumn</code> </p>
   <p><code style="font-weight: bold;">group.0.valuefield=project:name</code> </p>
   <p><code>group.0.namekeyargkey.0=project</code> </p>
   <p><code>group.0.namekeyargkey.1=name</code> </p>
   <p><code style="font-weight: bold;">group.0.valueformat=string</code> </p>
   <p><code>group.1.linkedname=assignedTo</code> </p>
   <p><code>group.1.namekey=view.relatedcolumn</code> </p>
   <p><code style="font-weight: bold;">group.1.valuefield=assignedTo:name</code> </p>
   <p><code>group.1.namekeyargkey.0=assignedTo</code> </p>
   <p><code>group.1.namekeyargkey.1=nam</code>e</p>
   <p><code style="font-weight: bold;">group.1.valueformat=string</code> </p> <note type="important">
   The lines in bold are mandatory.
   </note>
   </div>
   -->

   分組中的每個欄位都有參考該欄位的數行程式碼。

   下表概述了文本模式分組中的關鍵行。

   <!--
   <div data-mc-conditions="QuicksilverOrClassic.Draft mode">
   <p>(NOTE: Should I add the group.1. information to this table and break the snippet? If yes, delete the snippet)</p>
   <p>(NOTE: this is a snippet, same as view >> same fields >>> see the steps in creating a view and add the same steps here for making a grouping)</p>
   </div>
   -->

   >[!TIP]
   文本模式分組中的關鍵行類似於構建文本模式視圖所需的行。

   <!--
   <note type="tip">  
   <p>The key lines in a text mode grouping are similar to the lines required to build text-mode views.</p>
   </note>
   -->

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th><strong>範例行</strong> </th> 
      <th><strong>說明</strong> </th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td><strong>群組.&lt;number&gt;.</strong> </td> 
      <td> <p>每行程式碼前面都有此文字。 參考在分組中選取之相同欄位的程式碼行會以相同的數字編號，如下所示：</p> 
       <ul> 
        <li>報表的第一個分組的組號為0。 引用第一個分組的所有行開頭為 <code>group.0</code>.</li> 
        <li>報告的第二個分組的組號為1。 引用第二個分組的所有行開頭為 <em><code>group.1</code></em>.</li> 
        <li>報告的第三個分組的組號為2。 引用第三個分組的所有行的開頭為 <em><code>group.2</code></em>.</li> 
        <li>只有在文本模式下，您才可以為第四個分組添加組編號3。 引用第四個分組的所有行開頭為 <em><code>group.3</code></em>.</li> 
       </ul> <p>注意：產生器不支援4個群組。 只有使用文字模式時才支援。 Workfront不支援超過4個層級的群組。</p> </td> 
     </tr> 
     <tr> 
      <td> <p><strong>valuefield</strong>=</p> </td> 
      <td> <p>這是資料庫中顯示的對象或欄位的名稱。 有關對象和欄位在資料庫中如何顯示的詳細資訊，請參見 <a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">API Explorer</a>.</p> <p>存在下列情況：</p> 
       <ol> 
        <li value="1"> <p> 如果您顯示的欄位名稱是片語，而非單一名詞，您必須對 <code>valuefield</code>. 例如，對於任務的計畫起始日期，代碼為：</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>範例: </b></span></span><code>group.0.valuefield=plannedStartDate</code> </p> </li> 
        <li value="2"> <p>如果要顯示自訂欄位，請 <code>valuefield</code> 值是欄位的實際名稱，如您在介面中所見。 例如，對於名為「更多資訊」的自訂欄位，程式碼為：</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>範例: </b></span></span><code>group.0.valuefield=More information</code> </p> </li> 
        <li value="3"> <p>如果要按與其他對象相關的對象分組，請使用 <code>valuefield</code> 代碼行的對象名稱和屬性以冒號分隔。</p> <p>例如，按Portfolio名稱分組的任務清單的值欄位行具有以下值：</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>範例: </b></span></span><code>group.0.valuefield=project:portfolio:name</code> </p> <p>這表示您可以從報表（任務）的物件存取下一個相關物件（專案）;從那裡，您可以從項目（產品組合）訪問以下相關對象；然後是產品組合名稱（名稱）。</p> </li> 
       </ol> <p>有關對象如何彼此連接的資訊，請參見一節 <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-interdependency-and-hierarchy-of-objects" class="MCXref xref">對象的相互依存和層次</a> in <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">了解Adobe Workfront中的物件</a>.</p> <p>注意：如果在文本模式中選擇在標準介面中無效的欄位，並切換到標準介面，則會刪除分組。</p> </td> 
     </tr> 
     <tr> 
      <td><strong>valueformat=</strong> </td> 
      <td> <p>此行代表用來顯示 <code>valuefield</code>. 此 <code>valueformat</code> 識別物件或欄位是否顯示為文字、數字、百分比或日期。</p> <p>建議您使用 <code>HTML</code> 為 <code>valueformat</code>，尤其是使用 <code>valueexpression</code>，以確保資訊的顯示最準確。</p> <p>如需此行的其他值的相關資訊，請參閱 <a href="../../../reports-and-dashboards/reports/text-mode/use-conditional-formatting-text-mode.md" class="MCXref xref">在文字模式中使用條件式格式</a>.</p> </td> 
     </tr> 
     <tr> 
      <td> <p><strong>valueexpression=</strong> </p> </td> 
      <td> <p>您可以新增此行以取代 <code>valuefield</code>，如果您想要依據多個欄位之間的計算將清單分組。</p> <p>您必須將 <code>valuefield</code> 在 <code>valueexpression</code>.</p> <p>存在下列情況：</p> 
       <ol> 
        <li value="1"> <p>如果您想以大寫顯示分組名稱，請使用：</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>範例: </b></span></span><code>group.0.valueexpression=UPPER({valuefield})</code> </p> <p>此 <code>valuefield</code> 的拼寫方式與API檔案總管中顯示的一樣。</p> </li> 
        <li value="2">如果您想要新增多個 <code>valuefields</code> 把他們綁在一起 <code>valueexpression </code>行，您必須以句點分隔。<p>例如，如果要在任務清單中以大寫顯示產品組合的名稱，請在 <code>valueexpression</code> 行：</p><p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>範例: </b></span></span><code>group.0.valueexpression=UPPER({project}.{portfolio}.{name})</code></p><p>如果您想在 <code>valueexpression</code> 行，必須在欄位名稱前面 <code>DE:</code> 以指出這是自訂欄位。 欄位名稱的拼寫方式與介面中顯示的名稱相同。</p><p>重要： <span>若您使用放置在自訂表單區段（該區段對某些使用者具有限制權限）的自訂欄位時，會計算 <code>valueexpression </code>當這些使用者在報表中檢視此計算時，為空白。 如需調整自訂表單區段權限的相關資訊，請參閱</span> <span href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md"><a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">建立或編輯自訂表單</a></span>.</p><p>例如，如果您有標示為「開發人員名稱」的自訂欄位，而您想依此欄位分組，並以大寫顯示，則可使用下列項目 <code>valueexpression</code> 以指出：</p><p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>範例: </b></span></span><code>group.0.valueexpression=UPPER({DE:Developer Name}</code>)</p><p>參考Typeahead類型自訂欄位時，請使用下列運算式來參考在標示為「開發人員名稱」的欄位中選取之物件的名稱：</p><p><code>valueexpression=UPPER({DE:Developer Name:name})</code></p></li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td><strong>namekey= / name=</strong> </td> 
      <td> <p>此行定義分組標籤。 在此情況下，會根據索引鍵使用縮寫的值。</p> <p>如果要修改分組名稱，可將此值更改為：</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>範例: </b></span></span><code>group.0.name=Your Value</code> </p> <p><code>Name</code> 可讓您輸入分組名稱的任何文字，而 <code>namekey</code> 需要您輸入用於轉換分組名稱的鍵。</p> <p>若要變更分組名稱，您也可以新增 <code>displayname </code>行，如果沒有。</p> </td> 
     </tr> 
     <tr> 
      <td><strong>displayname =</strong> </td> 
      <td> <p>您可以新增下列行以變更欄的名稱，這會覆寫 <code>namekey/name</code> 值：</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>範例: </b></span></span><code>group.0.displayname=Your Value</code> </p> <p>建議移除包含 <code>name </code>重新命名群組時。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. （選用）將下列其中一行程式碼新增至任何分組，以指出分組中的結果是否應顯示在展開或收合的清單中。 依預設，群組會展開：


   ```
   group.0.iscollapsed=true
   ```

   如果要顯示分組並收合結果

   ```
   group.0.iscollapsed=false
   ```

   如果希望分組顯示結果展開

   <!--   
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: the tips repeat in the Create groupings to organize results article, Common uses of text mode, Edit groupings to organize reports, Create a Custom Report) </p>   
     -->

   >[!TIP]
   * 當您在檢視清單時手動調整分組時，Workfront會記住您的手動偏好設定，直到您登出為止。 當您重新登入時，清單會根據此設定顯示。
   * 從圖表元素存取群組後，其結果一律會顯示為已展開。


1. 按一下 **完成** 如果您想要儲存變更並繼續編輯群組或報表。
1. 按一下 **儲存分組** 或 **儲存+關閉** 儲存報表。
