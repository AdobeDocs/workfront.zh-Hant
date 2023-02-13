---
title: 在報表畫布中設定表格欄
description: 在報表畫布中設定表格欄
author: Nolan
feature: Reports and Dashboards
exl-id: ce33888f-344d-4f69-b527-9679340d134b
source-git-commit: 61fcb4c3646f60fa5f667d874af3320360d5d286
workflow-type: tm+mt
source-wordcount: '1042'
ht-degree: 2%

---


# 在報表畫布中設定表格欄

表格中的列可配置為顯示。 可以修改列的以下方面：

* 名稱
* 排序
* 編輯權限
* 游標停留文字
* 匯總
* 條件式格式設定

## 必要條件

開始之前，您必須註冊「報表畫布測試版」。 如需詳細資訊，請參閱 [報表畫布測試版：概述](/help/quicksilver/product-announcements/betas/reporting-canvas-beta/reporting-canvas-beta-overview.md).

## 修改表中的列

1. 前往現有報表，按一下 **更多功能表** 圖示 ![](assets/more-icon.png) 在報表標題中，然後選取 **編輯**.
1. 在報表的表格標題上，按一下 **編輯** 圖示 ![](assets/edit-icon.png).

   ![](assets/edit-icon-table-header-350x71.png)

   >[!NOTE]
   >
   >如果您剛建立表格，但尚未新增任何欄位，請改為按一下表格中央的「編輯」按鈕。

1. （可選）新增、重新定位或刪除表格中的欄。 如需編輯表格中欄位的詳細資訊，請參閱 [在報表畫布中新增或編輯表格區塊](../../../reports-and-dashboards/reporting-canvas/table-blocks/add-or-edit-report-table.md)

   | 新增欄 | 若要將欄新增至表格，請按一下並拖曳欄位， **欄位** 面板，將其放置至您要放置的表格上，或按兩下欄位以將其新增為最右側的欄。 |
   |---|---|
   | 移動列 | 要重新排清單中列的順序，請按一下列名並將其拖到新位置。 |
   | 刪除欄 | 若要從表格中刪除欄，請按一下您要刪除的欄，然後按一下欄名稱右側的x。 |

   {style=&quot;table-layout:auto&quot;}

1. 要配置列，請在表的標題行中按一下要修改的列的名稱，然後在右側面板上按一下以下其中一個頁簽：

   <table style="table-layout:auto"> 
    <col> class="TableStyle-TableStyle-List-options-in-steps-Column-Column1" /&gt;
    <tbody>
     <tr data-mc-conditions="">
      <th role="rowheader" colspan="2">資料標籤</th>
     </tr>
     <tr data-mc-conditions="">
      <td role="rowheader">彙總依據</td>
      <td><p> 要匯總（在標題中匯總）列中的資訊，請從 <strong>根據</strong> 下拉式功能表。 可用的選項取決於欄中包含的資料類型。</p><p>如果您在表格中使用群組，匯總值會顯示在欄名稱上方的群組列中，而非欄名稱旁。</p></td>
     </tr>
     <tr data-mc-conditions="">
      <td role="rowheader">欄位格式</td>
      <td><p>（僅當欄包含日期、百分比、貨幣或時間資料，而非文字時才可用。） 在 <b>欄位格式</b> 下拉式清單。 例如，您可以在欄的數字後面顯示百分比符號，或變更日期的顯示方式。</p></td>
     </tr>
     <tr data-mc-conditions="">
      <td role="rowheader">欄位可供編輯</td>
      <td><span>啟用 <strong>欄位可編輯</strong> 如果要允許查看表的用戶編輯列的名稱。</span></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>排序</strong></td>
      <td><p>依預設，表格會根據其最左側欄中的資料以升序排序。 若要改為依選取的欄排序，請按一下旁邊的向下箭頭 <strong>排序</strong>，然後按一下核取方塊 <b>按此列排序</b>. 然後，您可以選取 <strong>排序</strong> 方向（遞增或遞減值）和 <strong>排序順序</strong> （此列的相對排序優先順序與表格中的其他排序列相比）。</p><p>您可以重複此程式，最多依5個不同欄來排序表格。 請確定每欄的 <strong>排序順序</strong> 相對於您為排序選取的任何新欄。</p><p>注意：如果刪除選定要對表進行排序的列，並且還選擇另一列進行排序，則該列用於按降序對表進行排序。 如果沒有選擇其他列進行排序，則表將返回預設值：依其第一欄排序。</p><p>當您指定列來排序表格時，列名旁邊將顯示一個小框，其中的數字指示該列在排序表格時的相對優先順序（表格先按1排序，然後按2排序，依此類推），並顯示一個箭頭來指示排序方向是升序還是降序。 </p><p><img src="assets/sorting-indicator-350x170.png" style="width: 350;height: 170;"></p></td>
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
      <td role="rowheader"><strong>自訂欄標籤</strong> </td> 
      <td>輸入列的新顯示名稱（最多100個字元）。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">顯示游標停留文字</td> 
      <td> <p>確定當某人將游標暫留在欄名稱上時是否要顯示解釋性文字。</p> <p>預設會停用此選項。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">游標停留文字</td> 
      <td>(僅適用於 <strong>顯示暫留文字</strong> 已啟用。) 自訂當有人將游標停留在欄名稱上時顯示的解釋性文字。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>條件式格式設定</strong> </td> 
      <td> 
       <ol data-mc-continue="false"> 
        <li value="1"> <p>新增 <img src="assets/add-rule.png">，編輯 <img src="assets/edit-icon.png">，或刪除 <img src="assets/delete.png"> 當儲存格的值符合您指定的准則時，用來格式化欄中儲存格的規則。</p> <p>例如，您可以建立規則，當「專案狀態」欄位的值等於「建置」時，將該欄位中的字型變更為粗體紫色。</p> <p>或者，您可以使用 <b>顯示表徵圖</b> 向列中狀態為「當前」的每個項添加綠色標誌表徵圖。</p> <p> <img src="assets/conditional-formatting-options.png"> </p> <p>注意：如果您使用 <strong>顯示表徵圖</strong>，則其他格式選項將不可用。</p> <p>您可以選取 <strong>套用至整列</strong> 如果您希望格式能夠影響符合規則條件的儲存格的整列。 例如，您可以將黃色背景顏色套用至「到期日」欄中的日期儲存格，並套用至發生這些日期的整個列，以反白標示特定日期後到期的專案。</p> <p>提示：將格式選項新增至規則時，產生的儲存格格式會顯示在 <strong>預覽</strong> 在面板底部。</p> </li> 
        <li value="2">完成新增規則後，按一下 <strong>儲存</strong>.</li> 
        <li value="3"> <p>（選用）按一下 <b>+新增規則</b> 新增其他規則至相同欄。</p> <p>表格中的多個條件式格式規則會依下列順序套用：</p> 
         <ul> 
          <li> <p>系統會先評估套用至整列的規則，從左到右依序評估各欄的規則，然後從上到下依序評估一欄的規則。</p> <p>注意：行格式將覆蓋該行中單元格的其他條件格式，即使這些格式滿足其他列規則的條件。</p> </li> 
          <li> <p>其他規則會隨後從上到下評估，因為它們會列在欄的右側面板中。 您可以拖曳 <img src="assets/drag-object-icon.png"> 儲存的規則以變更其順序。</p> <p>注意：儲存格會根據符合的第一個條件進行格式化，即使符合其他條件，也不會進一步格式化。</p> </li> 
         </ul> </li> 
       </ol> </td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下 **回去** 畫面左上角的箭頭，返回您的報表。
