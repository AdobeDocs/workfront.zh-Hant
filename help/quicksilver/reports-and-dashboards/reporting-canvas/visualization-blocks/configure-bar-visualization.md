---
title: 在報表畫布中設定橫條圖視覺效果
description: 在報表畫布中設定橫條圖視覺效果
author: Nolan
feature: Reports and Dashboards
exl-id: 7dc4f156-d262-482f-aa82-c905f0d1b20f
source-git-commit: ca70952bf0acd71f748b042852d434b560727a83
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 2%

---


# 在報表畫布中設定橫條圖視覺效果

橫條圖視覺效果可協助您使用水準橫條來強調重要資訊，以快速訴說您的資料故事。

## 必要條件

開始之前，您必須先註冊報表畫布Beta版。 如需詳細資訊，請參閱 [報告畫布測試版：概觀](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/reporting-canvas-beta-overview.md).

## 設定長條圖視覺效果

>[!NOTE]
>
>當您建立和編輯報表中的區塊時，所有變更都會自動儲存。

1. 首先，使用新增視覺效果區塊 **長條圖** 報表的視覺效果型別，如中所述 [在報告畫布中新增或編輯視覺效果區塊](../../../reports-and-dashboards/reporting-canvas/visualization-blocks/add-or-edit-report-visualization.md).

1. 按一下「編輯視覺效果」圖示 ![](assets/edit-icon.png) 然後執行下列任一項作業。

   1. 於 **設定** 標籤：

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">視覺效果類型</td>
         <td><p>切換至不同的視覺效果型別。 若您這麼做，選單上的後續選項可能會變更。</p></td>
        </tr>
        <tr>
         <td role="rowheader">垂直軸</td>
         <td><p>選取您要沿著垂直左邊緣描繪的資料，或是橫條圖視覺效果的Y軸。 視覺效果會根據水平軸上的每個專案比較此軸上的專案。</p></td>
        </tr>
        <tr>
         <td role="rowheader">水平軸</td>
         <td><p>在左側下拉式選單中，選取您要沿著水準或X軸描繪的資料。 此軸上的專案會根據其值顯示為比較長條。</p><p>在右側的下拉式功能表中，選取您希望視覺效果如何沿著水平軸計算和顯示值：</p>
          <ul>
           <li><p><b>計數</b>：值的數量</p></li>
           <li><p><b>總和</b>：所有值的總數 </p></li>
           <li><p><b>平均</b>：所有值的平均值</p></li>
           <li><p><b>最小值</b>：僅最低值</p></li>
           <li><p><b>最大值</b>：僅最高值</p></li>
          </ul></td>
        </tr>
        <tr>
         <td role="rowheader">+ 新增值</td>
         <td>新增另一個要沿水平軸追蹤的欄位。</td>
        </tr>
       </tbody>
      </table>

   1. 於 **資料** 標籤：

      | 資料來源（下拉式功能表） | 將視覺效果的資料來源變更為報表畫布上的另一個表格。 |
      |---|---|
      | 顯示資料來源 | 啟用此選項以在報告畫布上顯示視覺效果的來源表格，或停用隱藏它的選項。 |

      {style="table-layout:auto"}

      <!--   
      NOLAN-FLAG: convert table to html. 
      -->

1. 按一下視覺效果設定功能表以外的任何位置，將其關閉。
