---
content-type: reference
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: 計算的自訂運算式中的條件運算子
description: 使用文字模式時，在Adobe Workfront中建立計算的自訂資料時，可以使用條件運算子或修飾元。
author: Nolan
feature: Reports and Dashboards
exl-id: ce98ca39-cb86-4ef7-b75c-29ceb916e885
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '756'
ht-degree: 1%

---

# 計算自訂欄位中的條件運算子

使用文字模式時，在Adobe Workfront中建立計算的自訂資料時，可以使用條件運算子或修飾元。

如需在Workfront中使用文字模式的相關資訊，請參閱 [文字模式概觀](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

條件運算子或修飾元通過連接語句中的現有Workfront欄位並生成新欄位來幫助建立條件語句。 條件運算子最常見的用法是建立&quot;IF&quot;陳述式的條件。

您可以使用Workfront中的「IF」陳述式來比較、格式化資料欄位，以及將資料欄位串連在一起，以利報表和自訂資料之用。

您可以為下列Workfront元素建立「IF」陳述式：

* 檢視
* 群組
* 計算自訂欄位

如需有關建立「IF」陳述式的詳細資訊，請參閱 [&quot;IF&quot;陳述式概述](../../../reports-and-dashboards/reports/calc-cstm-data-reports/if-statements-overview.md).

本指南中的範例說明如何在計算的自訂欄位中使用條件運算子。 遵循報表中計算自訂欄位的正確語法時，您也可以在計算自訂欄位或群組中使用這些欄位。

如需報表中計算自訂欄位與計算自訂資料之間語法差異的相關資訊，請參閱 [計算自訂欄位與計算欄](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-custom-fields-calculated-columns.md).

請參考API總管，尋找您要在計算的自訂運算式中參考的欄位。 如需API總管的相關資訊，請參閱 [API Explorer](../../../wf-api/general/api-explorer.md).

您可以在Workfront中使用下列條件修飾元：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>條件運算子</th> 
   <th>條件運算子語法</th> 
   <th>條件運算子定義</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>等於 (區分大小寫)</td> 
   <td>= </td> 
   <td> <p>使用此運算子可指示當語句的第一個欄位等於第二個欄位時，條件已滿足。</p> <p>例如，在計算的自定義欄位中使用以下語句來生成「IF」語句，該語句將計畫完成日期與任務的預計完成日期進行比較： </p><pre>IF({projectedCompletionDate}={plannededCompletionDate},"On Track","Off Track")</pre> </td> 
  </tr> 
  <tr> 
   <td>大於 </td> 
   <td>&gt; </td> 
   <td>使用此運算子可指示當語句的第一個欄位大於第二個欄位時滿足條件。 <p>例如，在計算的自定義欄位中使用以下語句來生成「IF」語句，該語句將計畫完成日期與任務的預計完成日期進行比較： </p><pre>IF({projectedCompletionDate}&gt;{plannededCompletionDate},"Late","")</pre></td> 
  </tr> 
  <tr> 
   <td>大於或等於 </td> 
   <td>&gt;= </td> 
   <td>使用此運算子可指示當語句的第一個欄位大於或等於第二個欄位時，滿足條件。 <p>例如，在計算的自定義欄位中使用以下語句來生成「IF」語句，該語句將計畫完成日期與任務的預計完成日期進行比較： </p><pre>IF({projectedCompletionDate}&gt;={planededCompletionDate},"Late","Early")</pre></td> 
  </tr> 
  <tr> 
   <td>小於 </td> 
   <td>&lt; </td> 
   <td>使用此運算子可指示當語句的第一個欄位小於第二個欄位時滿足條件。 <p>例如，在計算的自定義欄位中使用以下語句來生成「IF」語句，該語句將計畫完成日期與任務的預計完成日期進行比較： </p><pre>IF({projectedCompletionDate}&lt;{planededCompletionDate},"Early","")</pre></td> 
  </tr> 
  <tr> 
   <td>小於或等於 </td> 
   <td>&lt;= </td> 
   <td>使用此運算子可指示當語句的第一個欄位小於或等於第二個欄位時，已滿足條件。 <p>例如，在計算的自定義欄位中使用以下語句來生成「IF」語句，該語句將計畫完成日期與任務的預計完成日期進行比較： </p><pre>IF({projectedCompletionDate}&lt;={planededCompletionDate},"Early","Late")</pre></td> 
  </tr> 
  <tr> 
   <td>不 </td> 
   <td>! </td> 
   <td> <p>在上述任何運算子前面新增此運算子，以否定運算子。 </p> <p>例如： </p> 
    <ul> 
     <li>等於: = </li> 
     <li>不等於: != </li> 
    </ul> <p>在下列資料運算式前面新增此運算子，會在運算式中新增負陳述式： </p> 
    <ul> 
     <li>包含 </li> 
     <li>在 </li> 
     <li>IFIN </li> 
     <li>ISBLANK </li> 
    </ul> <p>如需這些資料運算式的相關資訊和完整清單，請參閱 <a href="../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md" class="MCXref xref">計算資料運算式</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>或 </td> 
   <td>|| </td> 
   <td> <p>使用此運算子可指示當運算式找到語句的第一個值或第二個值時，條件已滿足。 </p> <p>例如，在計算的自定義欄位中使用以下語句來構建「IF」語句，該語句將當前或計畫狀態中的項目標籤為「活動」： </p><pre>IF({status}="PLN"|{status}="CUR","Active","Not Active")</pre> </td> 
  </tr> 
  <tr> 
   <td> 和 </td> 
   <td>&amp;&amp; </td> 
   <td> <p>使用此運算子可指示當表達式同時找到滿足兩個條件的項目時，條件已滿足。 </p> <p>例如，在計算的自定義欄位中使用以下語句來構建「IF」語句，該語句查找處於當前狀態且條件為「風險」的項目，並將它們標籤為「需要調解」。 </p><pre>IF（{status}="CUR"&amp;&amp;{condition}="AR","需要中介",""）)</pre> </td> 
  </tr> 
 </tbody> 
</table>
