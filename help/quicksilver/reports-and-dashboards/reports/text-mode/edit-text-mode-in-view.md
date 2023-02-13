---
product-area: reporting
navigation-topic: text-mode-reporting
title: 使用文本模式編輯視圖
description: '注意：在本文新增章節：/Content/Reports and Dashboards/Reports/Reporting Elements/create-customize-views.html ***此外，在「文字模式」概觀文章中草稿此區域)'
author: Nolan
feature: Reports and Dashboards
exl-id: b99a2d14-a226-4075-9b1b-ac9426fd41b8
source-git-commit: 89a6d856f9f87a67b6a2ccfb4282f9f6200b977c
workflow-type: tm+mt
source-wordcount: '1636'
ht-degree: 1%

---

# 使用文本模式編輯視圖

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">NOTE: add a section in this article: /Content/Reports and Dashboards/Reports/Reporting Elements/create-customize-views.html *** Also, draft this area in the Text Mode overview article) </p>
-->

您可以使用文字模式編輯清單或報表中的檢視，以存取標準介面中無法使用的欄位，並建立更複雜的檢視。

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
   <td> <p>編輯對篩選器、檢視、群組的存取</p> <p>編輯對報表、控制面板、日曆的存取，以編輯報表中的報表元素</p> <p>注意：如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>管理報表權限以編輯報表中的檢視</p> <p>管理檢視的權限以進行編輯</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
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

## 在檢視中編輯文字模式

使用文字模式編輯檢視，對報表和清單是相同的。 從報表或清單存取檢視的方式有所不同。

>[!TIP]
>
>建議您在標準模式中盡可能多地建立檢視，然後轉換為文字模式以編輯它。

如需建立檢視的詳細資訊，請參閱 [Adobe Workfront中的檢視概觀](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

如需建立報表的相關資訊，請參閱 [建立自訂報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. 執行下列任一項作業：

   1. 若要從報表存取檢視，請前往報表，然後按一下 **報表動作** > **編輯** > **欄（檢視）** 標籤。
   1. 要從清單訪問視圖，請轉至清單，然後從 **檢視** 下拉式選單中，將滑鼠移至您要修改的檢視上，然後按一下 **編輯** 圖示 ![](assets/edit-icon.png).

      檢視產生器隨即開啟。

1. 在檢視中選取欄。

   或

   選取 **欄（檢視）** ，然後選取欄。

   >[!TIP]
   >
   >要使用文本模式編輯視圖，必須一次編輯一列。

1. 按一下 **切換到文本模式** 建立器的右上角。

   >[!NOTE]
   >
   >以文字模式編輯欄時，Workfront會新增 `textmode=true` 行代碼到列。 這表示欄已在文字模式中修改。

   ![](assets/switch-to-text-mode-in-view-nwe-highlighted-350x447.png)

   下表概述文本模式視圖中的關鍵行：

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: make this a snippet and add it to the grouping article too)</p>
   -->

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>範例行</th> 
      <th>說明</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td> <p><strong>valuefield</strong>=</p> </td> 
      <td> <p>這是資料庫中顯示的對象或欄位的名稱。 有關對象和欄位在資料庫中如何顯示的詳細資訊，請參見 <a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">API Explorer</a>.</p> <p>存在下列情況：</p> 
       <ol> 
        <li value="1"> <p> 如果您顯示的欄位名稱是片語，而非單一名詞，您必須對 <code>valuefield</code>. 例如，對於任務的計畫起始日期，代碼為： </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>範例: </b></span></span><code>valuefield=plannedStartDate</code> </p> </li> 
        <li value="2"> <p>如果要顯示自訂欄位，請 <code>valuefield</code> 值是欄位的實際名稱，如您在介面中所見。 例如，對於名為「更多資訊」的自訂欄位，程式碼為：</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>範例: </b></span></span><code>valuefield=More information</code> </p> </li> 
        <li value="3"> <p>如果要顯示與視圖中的其他對象相關的對象，請使用 <code>valuefield</code> 代碼行的對象名稱和屬性以冒號分隔。 </p> <p>例如，在任務視圖中顯示Portfolio所有者名稱的列在值欄位行中具有以下值：</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>範例: </b></span></span><code>valuefield=project:portfolio:owner:name</code> </p> <p>這表示從報表（任務）的對象中，您可以從該處訪問下一個相關對象（項目），您可以從項目（項目組合）訪問以下相關對象，然後依次訪問項目組合所有者（所有者）及其名稱（名稱）。 </p> </li> 
       </ol> <p>有關對象如何彼此連接的資訊，請參見一節 <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-interdependency-and-hierarchy-of-objects" class="MCXref xref">對象的相互依存和層次</a> in <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">了解Adobe Workfront中的物件</a>.</p> <p>注意：如果您選擇在標準介面中無效的文本模式欄位，則無法切換回列內的標準介面。</p> </td> 
     </tr> 
     <tr> 
      <td><strong>valueformat=</strong> </td> 
      <td> <p>此行代表用來顯示 <code>valuefield</code>. 此 <code>valueformat</code> 識別物件或欄位是否顯示為文字、數字、百分比或日期。</p> <p>建議您使用 <code>HTML</code> 為 <code>valueformat</code>，尤其是使用 <code>valueexpression</code>，以確保資訊的顯示最準確。 </p> <p>如需此行的其他值的相關資訊，請參閱 <a href="../../../reports-and-dashboards/reports/text-mode/use-conditional-formatting-text-mode.md" class="MCXref xref">在文字模式中使用條件式格式</a>.</p> </td> 
     </tr> 
     <tr> 
      <td> <p><strong>valueexpression=</strong> </p> </td> 
      <td> <p>您可以新增此行以取代 <code>valuefield</code>，以便在欄中顯示計算欄位。</p> <p>您必須將 <code>valuefield</code> 在 <code>valueexpression</code>.</p> <p>存在下列情況： </p> 
       <ol> 
        <li value="1"> <p>如果您想以大寫顯示欄位，請使用：</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>範例: </b></span></span><code>valueexpression=UPPER({valuefield})</code> </p> <p>此 <code>valuefield</code> 的拼寫方式與API檔案總管中顯示的一樣。 </p> </li> 
        <li value="2">如果您想要新增多個 <code>valuefields</code> 把它們串在一起，就必須按時間分開。</li> 
        <li value="3"> <p>例如，如果要顯示任務的主要受託人的名稱，請使用 <code>valueexpression</code>，您會使用：</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>範例: </b></span></span><code>valueexpreesion={assignedTo}.{name}</code> </p> </li> 
        <li value="4"> <p>如果您想在 <code>valueexpression</code> 行，必須在欄位名稱前面 <code>DE:</code> 以指出這是自訂欄位。 欄位名稱的拼寫方式與介面中顯示的名稱相同。 </p> <p>重要：若您使用自訂欄位放在某些使用者具有限制權限的自訂表單區段中，當這些使用者在報表中檢視此計算時，值運算式的計算會空白。 如需調整自訂表單區段權限的相關資訊，請參閱 <span href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md"><a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">建立或編輯自訂表單</a></span>.</p> <p>例如，如果您有標示為「開發人員名稱」的自訂欄位，而您想要在欄中以大寫顯示此欄位，您可以使用下列項目 <code>valueexpression</code> 以指出：</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>範例: </b></span></span><code>valueexpression=UPPER({DE:Developer Name}</code>) </p> <p>參考Typeahead類型自訂欄位時，請使用下列運算式來參考在標示為「開發人員名稱」的欄位中選取之物件的名稱：</p> <p><code>valueexpression=UPPER({DE:Developer Name:name})</code> </p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td> <p><strong>descriptionkey= / description=</strong> </p> </td> 
      <td> <p>將滑鼠移到列的名稱上時，此行定義工具提示的文本。 在這種情況下，它使用鍵來翻譯說明文本中的名稱值。 如果要修改說明，請將此行更改為： </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>範例: </b></span></span><code>description=Your Value</code>.</p> </td> 
     </tr> 
     <tr> 
      <td><strong>namekey= / name=</strong> </td> 
      <td> <p>此行定義列標籤。 在此情況下，會根據索引鍵使用縮寫的值。</p> <p>如果要修改列名，可將此值更改為： </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>範例: </b></span></span><code>name=Your Value</code> </p> <p><code>Name</code> 可讓您為欄名稱輸入任何文字，而<code>namekey</code> 需要您輸入用於轉換列名稱的鍵。</p> <p>若要變更欄名稱，您也可以新增 <code>displayname </code>行，如果沒有。</p> </td> 
     </tr> 
     <tr> 
      <td><strong>displayname =</strong> </td> 
      <td> <p>您可以新增下列行以變更欄的名稱，這會暫停 <code>namekey/name</code> 值：</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>範例: </b></span></span><code>displayname=Your Value</code> </p> </td> 
     </tr> 
     <tr> 
      <td><strong>querysort=</strong> </td> 
      <td>此行定義按一下列標題時結果的排序方式。 如果不存在，則無法在報表執行後排序欄。</td> 
     </tr> 
     <tr> 
      <td><strong>width=</strong> </td> 
      <td> <p>此行表示用於列的像素數。 如果省略該行或將其設為0（零），則該列不會出現在視圖中。</p> <p>在文字模式中手動修改此欄位時，您也必須新增 <code>usewidths=true</code> 值。</p> </td> 
     </tr> 
     <tr> 
      <td><strong>usewidths=true</strong> </td> 
      <td> <p>除了 <code>width=</code> 行。 </p> </td> 
     </tr> 
     <tr> 
      <td><strong>makeFieldEditable=</strong> </td> 
      <td> <p>此行定義列中顯示的值是否內聯可編輯。 如果此行等於 <strong>true</strong>，欄中的值便可內嵌編輯。 如果此行等於 <code>false</code>，則欄中的值不會內嵌編輯。</p> </td> 
     </tr> 
     <tr> 
      <td><strong>link.valuefield=</strong> </td> 
      <td> <p>僅當您希望列中顯示的值連結到與其關聯的對象時，才插入此行。 連結會開啟物件的詳細資訊頁面。 此值應符合 <code>valuefield=</code> 行。 插入此項目時，您也必須新增 <code>link.valueformat=</code> 行。 </p> <p> 例如，您可以插入 <code>link.valuefield=priority</code> 在「問題」檢視中，問題的「優先順序」會顯示為連結。 按一下此連結會開啟「問題」頁面。</p> </td> 
     </tr> 
     <tr> 
      <td><strong>link.valueformat=</strong> </td> 
      <td> <p>只有在插入 <code>link.valuefield</code> 行，將連結新增至欄中的值。 連結會開啟物件的詳細資訊頁面。 此值應符合 <code>valueformat=</code> 行，並指示用於顯示 <code>valuefield</code>. </p> <p>重要：在內建欄中檢視文字模式（也包含連結）時，您會注意到引用連結的數行。 當您以文字模式建立自己的自訂欄並新增連結陳述式時，這些行中的某些可能已不受支援，或是沒有必要。 新增連結值時必須使用的行是<code> link.valuefield</code> 和 <code>link.valueformat</code>. </p> </td> 
     </tr> 
     <tr> 
      <td><strong>aggregator.function=</strong> </td> 
      <td> <p>這表示如何匯總各欄的值。 有多行開頭為 <code>aggregator.</code> 它們都指匯總欄結果的匯總器。 </p> <p>一般而言， <code>aggregator.</code> 行與列對象的行匹配。 </p> 
       <div class="example" data-mc-autonum="<b>Example: </b>">
        <span class="autonumber"><span><b>範例: </b></span></span> 
        <p>匯總的任務報表中的「計畫小時數」列可能如下所示： </p> 
        <div>
         <pre>textmode=true</pre>
         <pre>valuefield=workRequired</pre>
         <pre>valueformat=compound</pre>
         <pre>aggregator.function=SUM</pre>
         <pre>aggregator.valuefield=workRequired</pre>
         <pre>aggregator.displayformat=minutesAsHoursString</pre>
         <pre>aggregator.valueformat=compound</pre>
         <pre>namekey=workRequired</pre>
         <pre>shortview=false</pre> 
        </div> 
       </div> 
       <div>
        此 <code>aggregator. </code>行可以包含 <code>valuefield </code>或 <code>valueexpression</code>
       </div> </td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下 **套用** 如果要保存更改並繼續編輯視圖。
1. 按一下 **儲存+關閉** 儲存報表。

   或

   按一下 **保存視圖** 將視圖保存在清單中。
