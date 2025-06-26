---
content-type: reference
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: 計算自訂運算式中的條件運運算元
description: 使用文字模式在Adobe Workfront中建立計算的自訂資料時，您可以使用條件運運算元或修飾元。
author: Nolan
feature: Reports and Dashboards
exl-id: ce98ca39-cb86-4ef7-b75c-29ceb916e885
source-git-commit: e10fd7a3237d38ece8a5213990306ce511bd2412
workflow-type: tm+mt
source-wordcount: '731'
ht-degree: 1%

---

# 計算自訂欄位中的條件運運算元

<!-- Audited: 2/2024 -->

使用文字模式在Adobe Workfront中建立計算的自訂資料時，您可以使用條件運運算元或修飾元。 如需有關在Workfront中使用文字模式的資訊，請參閱[文字模式概觀](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md)。

條件運運算元或修飾元可連線陳述式中現有的Workfront欄位並產生新欄位，有助於建立條件陳述式。 條件運運算元最常見的用法是建置「IF」陳述式的條件。

您可以使用Workfront中的「IF」陳述式，將資料的欄位進行比較、格式化和字串在一起，以用於報表和自訂資料目的。

您可以為下列Workfront元素建立「IF」陳述式：

* 檢視
* 群組
* 已計算的自訂欄位
* 業務規則

如需有關建立「IF」陳述式的詳細資訊，請參閱[「IF」陳述式概述](../../../reports-and-dashboards/reports/calc-cstm-data-reports/if-statements-overview.md)。

本指南中的範例說明如何在計算的自訂欄位中使用條件運運算元。 當您在報告中遵循計算自訂欄位的正確語法時，也可在計算自訂欄或分組中使用它們。

如需有關報表中計算自訂欄位與計算自訂資料之間語法差異的資訊，請參閱[計算自訂欄位與計算欄](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-custom-fields-calculated-columns.md)。

如需商業規則的詳細資訊，請參閱[建立和編輯商業規則](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/business-rules.md)。

請參考API Explorer以尋找您要在計算的自訂運算式中參考的欄位。 如需API總管的相關資訊，請參閱[API總管](../../../wf-api/general/api-explorer.md)。

您可以在Workfront中使用下列條件修飾元：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>條件運運算元</th> 
   <th>條件運運算元語法</th> 
   <th>條件運運算元定義</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>等於</td> 
   <td>= </td> 
   <td> <p>使用此運運算元表示當對帳單的第一個欄位等於第二個欄位時，滿足條件。</p> <p>例如，在計算的自訂欄位中使用下列陳述式來建置「IF」陳述式，比較任務的計畫完成日期與預計完成日期： </p><p><code>IF({projectedCompletionDate}={plannedCompletionDate},"On Track","Off Track")</code></p> </td> 
  </tr> 
  <tr> 
   <td>大於 </td> 
   <td>&gt; </td> 
   <td>使用此運運算元指示當對帳單的第一個欄位大於第二個欄位時，符合條件。 <p>例如，在計算的自訂欄位中使用下列陳述式來建置「IF」陳述式，比較任務的計畫完成日期與預計完成日期： </p><p><code>IF({projectedCompletionDate}&gt;{plannedCompletionDate},"Late","")</code></p></td> 
  </tr> 
  <tr> 
   <td>大於或等於 </td> 
   <td>&gt;= </td> 
   <td>使用此運運算元指示當對帳單的第一個欄位大於或等於第二個欄位時，符合條件。 <p>例如，在計算的自訂欄位中使用下列陳述式來建置「IF」陳述式，比較任務的計畫完成日期與預計完成日期： </p><p><code>IF({projectedCompletionDate}&gt;={plannedCompletionDate},"Late","Early")</code></p></td> 
  </tr> 
  <tr> 
   <td>小於 </td> 
   <td>&lt; </td> 
   <td>使用此運運算元表示條件已符合  陳述式的第一個欄位小於第二個欄位。 <p>例如，在計算的自訂欄位中使用下列陳述式來建置「IF」陳述式，比較任務的計畫完成日期與預計完成日期： </p><p><code>IF({projectedCompletionDate}&lt;{plannedCompletionDate},"Early","")</code></p></td> 
  </tr> 
  <tr> 
   <td>小於或等於 </td> 
   <td>&lt;= </td> 
   <td>使用此運運算元表示條件已符合  陳述式的第一個欄位小於或等於第二個欄位。 <p>例如，在計算的自訂欄位中使用下列陳述式來建置「IF」陳述式，比較任務的計畫完成日期與預計完成日期： </p><p><code>IF({projectedCompletionDate}&lt;={plannedCompletionDate},"Early","Late")</code></p></td> 
  </tr> 
  <tr> 
   <td>不會 </td> 
   <td>！ </td> 
   <td> <p>在上述任何運運算元之前新增此運運算元，使運運算元無效。 </p> <p>例如： </p> 
    <ul> 
     <li>等於： = </li> 
     <li>不等於： ！= </li> 
    </ul> <p>在下列資料運算式前面新增此運運算元，會在運算式中新增負值陳述式： </p> 
    <ul> 
     <li>CONTAINS </li> 
     <li>在 </li> 
     <li>IFIN </li> 
     <li>ISBLANK </li> 
    </ul> <p>如需有關這些資料運算式的資訊，以及完整清單，請參閱<a href="../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md" class="MCXref xref">計算資料運算式概觀</a>。 </p> </td> 
  </tr> 
  <tr> 
   <td>或 </td> 
   <td>|| </td> 
   <td> <p>使用此運運算元指示當運算式時滿足條件  尋找陳述式的第一個或第二個值。 </p> <p>例如，在計算的自訂欄位中使用下列陳述式來建置「IF」陳述式，將「目前」或「計畫」狀態的專案標籤為「作用中」： </p><p><code>IF({status}="PLN"||{status}="CUR","Active","Not Active")</code></p> </td> 
  </tr> 
  <tr> 
   <td> 與 </td> 
   <td>&amp;&amp; </td> 
   <td> <p>使用此運運算元指示當運算式時滿足條件  尋找同時滿足兩個條件的專案。 </p> <p>例如，在計算自訂欄位中使用下列陳述式來建置「IF」陳述式，以尋找處於目前狀態且狀況為有風險的專案，並將它們標示為「需要中介」。 </p><p><code>IF({status}="CUR"&&{condition}="AR","Mediation Needed","")</code></p> </td> 
  </tr> 
 </tbody> 
</table>
