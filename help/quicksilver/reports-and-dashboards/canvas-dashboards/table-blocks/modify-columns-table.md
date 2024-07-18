---
title: 在報告畫布中設定表格欄
description: 在報告畫布中設定表格欄
hidefromtoc: true
hide: true
exl-id: ce33888f-344d-4f69-b527-9679340d134b
source-git-commit: 535e9c8481ce0781ee0d35636bb6d56de4d1e102
workflow-type: tm+mt
source-wordcount: '1043'
ht-degree: 2%

---

# 在報告畫布中設定表格欄

表格中的欄可以設定為顯示。 您可以修改欄的下列方面：

* 姓名
* 排序
* 編輯許可權
* 游標停留文字
* 彙總
* 條件式格式設定

## 先決條件

開始之前，您必須先註冊Reporting Canvas測試版。 如需詳細資訊，請參閱[報告畫布測試版：概觀](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/reporting-canvas-beta-overview.md)。

## 修改表格中的欄

1. 前往現有報表，按一下報表標題中的&#x200B;**更多功能表**&#x200B;圖示![](assets/more-icon.png)，然後選取&#x200B;**編輯**。
1. 在報告中的表格標題上，按一下&#x200B;**編輯**&#x200B;圖示![](assets/edit-icon.png)。

   ![](assets/edit-icon-table-header-350x71.png)

   >[!NOTE]
   >
   >如果您剛建立表格且尚未新增任何欄位，請改為按一下表格中央的「編輯」按鈕。

1. （選擇性）新增、重新定位或刪除表格中的欄。 如需編輯表格中欄位的詳細資訊，請參閱[在報告畫布中新增或編輯表格區塊](../../../reports-and-dashboards/reporting-canvas/table-blocks/add-or-edit-report-table.md)

   | 新增欄 | 若要新增欄位至表格，請按一下頁面右側&#x200B;**欄位**&#x200B;面板中的欄位並拖曳至您要放置它的表格上，或按兩下欄位以新增為最右邊的欄。 |
   |---|---|
   | 移動欄 | 若要重新排清單格中的欄順序，請按一下欄名稱並將其拖曳到新位置。 |
   | 刪除欄 | 若要從表格中刪除欄，請按一下要刪除的欄，然後按一下欄名稱右側的x。 |

   {style="table-layout:auto"}

1. 若要設定欄，請在表格的標頭列按一下您要修改的欄名稱，然後在右側面板上按一下下列其中一個索引標籤：

   <table style="table-layout:auto"> 
    <col> class="TableStyle-TableStyle-List-options-in-steps-Column-Column1" /&gt;
    <tbody>
     <tr data-mc-conditions="">
      <th role="rowheader" colspan="2">資料標籤</th>
     </tr>
     <tr data-mc-conditions="">
      <td role="rowheader">彙總依據</td>
      <td><p> 若要彙總（在標題中彙總）欄中的資訊，請從<strong>根據</strong>的彙總下拉式功能表中選取您想要的彙總型別。 可用的選項取決於欄中包含的資料型別。</p><p>如果您在表格中使用群組，則聚總值會顯示在欄名稱上方的群組列中，而非欄名稱旁邊。</p></td>
     </tr>
     <tr data-mc-conditions="">
      <td role="rowheader">欄位格式</td>
      <td><p>（只有當欄包含日期、百分比、貨幣或時間資料，而非文字時，才可使用。） 在<b>欄位格式</b>下拉式清單中，選取您要的資料格式。 例如，您可以在欄中的數字後面顯示百分比符號，或變更日期的顯示方式。</p></td>
     </tr>
     <tr data-mc-conditions="">
      <td role="rowheader">欄位可供編輯</td>
      <td><span>若要允許檢視表格的使用者編輯資料行的名稱，請啟用<strong>欄位可編輯</strong>。</span></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>排序</strong></td>
      <td><p>依預設，表格會根據其最左欄中的資料以遞增順序排序。 若要改為依選取的欄排序，請按一下<strong>排序</strong>旁的向下箭頭，然後按一下核取方塊<b>依此欄排序</b>。 然後，您可以選取<strong>排序</strong>方向（遞增或遞減值）和<strong>排序順序</strong> （此資料行相對於表格中其他排序資料行的相對排序優先順序）。</p><p>您可以重複此程式，最多可依5個不同的欄來排序表格。 請確定每個資料行相對於您選取要排序的任何新資料行，都有正確的<strong>排序順序</strong>。</p><p>附註：如果您刪除選取用來排序表格的欄，而同時選取另一個欄來排序，則會使用該欄來以遞減順序來排序表格。 如果沒有選取要排序的其他欄，表格會傳回預設值：依第一欄排序。</p><p>當您指定資料欄來排序表格時，資料欄名稱旁會顯示一個小方塊，其數字表示該資料欄在排序表格時的相對優先順序（表格會先依1、2等排序），箭頭表示排序方向是遞增還是遞減。 </p><p><img src="assets/sorting-indicator-350x170.png" style="width: 350;height: 170;"></p></td>
     </tr>
    </tbody>
   </table>

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <th role="rowheader" colspan="2">樣式標籤</th> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>自訂資料行標籤</strong> </td> 
      <td>輸入欄的新顯示名稱（限制100個字元）。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">顯示游標停留文字</td> 
      <td> <p>決定當有人將游標停留在欄名稱上時，是否要顯示說明文字。</p> <p>此選項預設為停用。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">游標停留文字</td> 
      <td>（只有啟用<strong>顯示暫留文字</strong>時才能使用。） 自訂當有人將游標停留在欄名稱上時顯示的說明文字。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>條件式格式</strong> </td> 
      <td> 
       <ol data-mc-continue="false"> 
        <li value="1"> <p>新增<img src="assets/add-rule.png">、編輯<img src="assets/edit-icon.png">或刪除<img src="assets/delete.png">當資料行的儲存格值符合您指定的准則時，會格式化資料行中的儲存格的規則。</p> <p>例如，您可以建立一個規則，當「專案狀態」欄位的值等於「建置」時，將該欄位的字型變更為粗體紫色。</p> <p>或者，您可以使用<b>顯示圖示</b>，將綠色旗標圖示新增至欄中狀態為「目前」的每個專案。</p> <p> <img src="assets/conditional-formatting-options.png"> </p> <p>注意：如果您使用<strong>顯示圖示</strong>，則無法使用其他格式選項。</p> <p>若要讓格式設定影響符合規則條件的儲存格之整列，可以選取<strong>套用至整列</strong>。 例如，您可以不僅對「到期日」欄中的日期儲存格套用黃色背景顏色，而且對這些日期出現的整列套用黃色，藉此反白特定日期後到期的專案。</p> <p>提示：當您新增格式選項至規則時，產生的儲存格格式會顯示在面板底部的<strong>預覽</strong>下方。</p> </li> 
        <li value="2">新增完規則後，請按一下[儲存]。<strong></strong></li> 
        <li value="3"> <p>（選擇性）按一下「<b>+新增規則</b>」，將其他規則新增至相同欄。</p> <p>表格中的多個條件式格式規則會依下列順序套用：</p> 
         <ul> 
          <li> <p>系統會先評估套用至整個列的規則，從左至右評估每個欄，然後在欄中從上至下。</p> <p>附註：資料列格式會覆寫該資料列中儲存格的其他條件式格式，即使這些儲存格在其他方面符合其他資料欄規則的條件亦然。</p> </li> 
          <li> <p>系統會從上到下評估列於欄右側面板中的其他規則。 您可以拖曳該面板中的<img src="assets/drag-object-icon.png">個已儲存規則來變更其順序。</p> <p>注意：儲存格會根據儲存格符合的第一個條件進行格式化，即使儲存格符合其他條件，也不會進一步進行格式化。</p> </li> 
         </ul> </li> 
       </ol> </td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下畫面左上角的&#x200B;**返回**&#x200B;箭頭以返回您的報告。
