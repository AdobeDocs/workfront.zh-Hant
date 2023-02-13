---
product-area: reporting
navigation-topic: reporting-elements
title: 篩選條件修飾元
description: 篩選條件修飾元可讓您建立篩選條件，並建立格式化報表結果的條件。
author: Lisa
feature: Reports and Dashboards
exl-id: 13e9d926-8a89-490e-aa7a-e6e8baf2a36b
source-git-commit: 442e0b8fde9e4acaa2686ccd292fb003f72be623
workflow-type: tm+mt
source-wordcount: '1556'
ht-degree: 1%

---

# 篩選條件修飾元

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: This is temporary - Lilit is fixing this in a future story: NOTE If the field you are filtering for has multiple options, this filters out the results that contain only the choice you specify. If the field contains additional options including the one specified, those results are not filtered from the report. See this document and search for "not equal" for the link to the req doc: https://docs.google.com/document/d/1WA0zZ_wws-2qb908i53BFQ8zDwL3nPJHyIybtJvvnqU/edit) </p>
-->

篩選條件修飾元可讓您建立篩選條件，並建立格式化報表結果的條件。

如需建立篩選器的詳細資訊，請參閱文章 [Adobe Workfront中的篩選器概觀](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

如需在檢視中使用條件式格式的詳細資訊，請參閱文章 [在檢視中使用條件式格式](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md).

## 篩選條件修飾元

如需內建時間格修飾元的清單，請參閱文章 [依時間範圍篩選報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/filter-reports-time-frames.md).

有些修飾元是內建的，您可以從篩選器或條件式格式陳述式內的下拉式選單中選擇這些修飾元。 其他修飾元只能用於文字模式篩選器。 如需了解文字模式的詳細資訊，請參閱 [文字模式概觀](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

您可以在篩選器和條件式格式陳述式中使用下列條件修飾元：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>內建修飾詞</strong> </p> </th> 
   <th> <p><strong>文本模式修飾符</strong> </p> </th> 
   <th> <p><strong>說明</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr valign="top"> 
   <td> <p><strong>空白</strong> </p> </td> 
   <td> <p><strong>空白</strong> </p> </td> 
   <td> <p>物件的欄位存在，但欄位尚未獲得值。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>不為空白</strong> </p> </td> 
   <td> <p><strong>空白</strong> </p> </td> 
   <td> <p>您要篩選的欄位存在且已指定值。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>null</strong> </p> </td> 
   <td> <p>欄位為空白或不存在。 例如，您要查找沒有父任務ID的項。 這表示您只想查看獨立任務。 「父任務ID」的限定符為 <strong>null</strong>，因為沒有ID的任務（在此例中為父項）不存在。 </p> <p>此修飾符只能用於文本模式篩選器。 如需篩選器中文字模式的詳細資訊，請參閱 <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">使用文字模式編輯篩選器</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>notnull</strong> </p> </td> 
   <td> <p>您要篩選的欄位存在，且包含null以外的值。</p> <p>此修飾符只能用於文本模式篩選器。 如需篩選器中文字模式的詳細資訊，請參閱 <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">使用文字模式編輯篩選器</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>包含</strong> </p> </td> 
   <td> <p><strong>環帶</strong> </p> </td> 
   <td> <p>（不區分大小寫）此版本不區分大小寫 <strong>包含</strong>. 例如："cicontains inf"可捕獲包含"Inf"或"inf"的任何值。</p> <p> <p>注意：Adobe Workfront會搜尋您為每個篩選陳述式指定的確切字詞或片語。 例如，如果您搜尋的專案名稱中包含「new project」一詞，Workfront不會顯示名稱中只有「new」或「project」或「new main project」的專案。 篩選器只會尋找名稱中具有確切字句「新專案」的專案。</p> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>cieq</strong> </p> </td> 
   <td> <p>（不區分大小寫）此選項不區分大小寫， <strong>eq</strong>. 它只會傳回與所搜尋值完全相符的值。</p> <p>例如，在搜索具有特定名稱的任務時，「任務名稱cieq test」會查找名稱為「Test」、「TEST」或「Test」的任務，但它找不到名稱為「test 123」的任務。</p> <p>此修飾符只能用於文本模式篩選器。 如需篩選器中文字模式的詳細資訊，請參閱 <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">使用文字模式編輯篩選器</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>cin</strong> </p> </td> 
   <td> <p>（不區分大小寫）此版本不區分大小寫 <strong>in</strong>.</p> <p>此修飾符只能用於文本模式篩選器。 如需篩選器中文字模式的詳細資訊，請參閱 <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">使用文字模式編輯篩選器</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>奇利克</strong> </p> </td> 
   <td> <p>此版本不區分大小寫 <strong>like</strong>. 例如："cilike %Current% %Dead%"返回包含"Current to Dead"或"current to dead"的任何注釋。</p> <p>此修飾符只能用於文本模式篩選器。 如需篩選器中文字模式的詳細資訊，請參閱 <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">使用文字模式編輯篩選器</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>金黃素</strong> </p> </td> 
   <td> <p>（不區分大小寫）此版本不區分大小寫 <strong>諾丁</strong>.</p> <p>此修飾符只能用於文本模式篩選器。 如需使用文字模式建立篩選器的詳細資訊，請參閱 <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">使用文字模式編輯篩選器</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> </td> 
   <td> <p><strong>包含</strong> </p> </td> 
   <td> <p>（區分大小寫）在整個文本字串中搜索指定的文本。</p> <p>例如，使用「包含Inf」可擷取其中包含「Inf」的任何項目，例如單字「Infinity」。</p> <p>此修飾符只能用於文本模式篩選器。有關篩選器中文本模式的詳細資訊，請參閱 <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">使用文字模式編輯篩選器</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>不包含</strong> </p> </td> 
   <td> <p><strong>cinothan</strong> </p> </td> 
   <td> <p>（不區分大小寫）它會篩選缺少指定值的項目。</p> <p>例如，「不包含inf」會擷取名稱中沒有「Inf」或「inf」的任何項目。</p> <p>注意： <span>如果您要篩選的欄位有多個選項，則此選項會篩選出包含您指定的選項、您指定的選項以及任何其他選項的結果。</span> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td><strong>不存在</strong> </td> 
   <td><strong>附註</strong> </td> 
   <td> <p>此修飾符僅用於EXISTS語句中的複雜篩選器。 這些篩選器只參考下列物件： </p> 
    <ul> 
     <li>在對象層次結構中跨越多個級別的對象 </li> 
     <li>缺少的對象 </li> 
    </ul> <p>有關使用EXISTS陳述式建立複雜篩選器的資訊，請參閱文章 <a href="../../../reports-and-dashboards/reports/text-mode/create-complex-text-mode-filters-using-exists-statements.md">使用EXISTS語句建立複雜的文本模式篩選器</a>. 這是EXISTS語句中唯一使用的修飾符。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> <p> </p> <p> </p> <p><strong>等於 (區分大小寫)</strong> </p> </td> 
   <td> <p><strong>in</strong> </p> </td> 
   <td> <p>（區分大小寫）此修飾詞可讓您建立以逗號分隔的變數清單，以與篩選器中評估的單一屬性進行比較。 整個清單會視為OR陳述式，並傳回符合一或多個變數之條件的任何結果。</p> <p>例如，在搜索項目時，使用「在CUR中」、「PLN」、「CPL」將返回處於「當前」、「或」「計畫」或「或」「完成」狀態的所有項目。</p> <p>內建修飾元 <strong>等於</strong> 對應於 <strong>in</strong>. 這表示您可以為欄位選擇等於多個值。</p> <p>例如，您可以在項目報表中選擇「狀態等於當前、計畫、無效」，並且可以查看任何這些狀態的項目。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> </td> 
   <td> <p><strong>eq</strong> </p> </td> 
   <td> <p>（區分大小寫）這只會傳回與所搜尋值完全相符的值。</p> <p>例如，在搜尋完成的專案時，"eq CPL"會傳回所有處於完成狀態的專案。 "eq CPL, CUR"不會傳回結果，因為專案無法同時完成和更新。</p> <p>此修飾符只能用於文本模式篩選器。 如需使用文字模式建立篩選器的詳細資訊，請參閱 <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">使用文字模式編輯篩選器</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>大於</strong> </p> </td> 
   <td> <p><strong>gt</strong> </p> </td> 
   <td> <p>這會搜尋值大於輸入值的所有結果，不包括輸入值。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>like</strong> </p> </td> 
   <td> <p>（區分大小寫）以類似於 <strong>包含</strong>. 不過， <strong>like</strong> 提供插入萬用字元以分解文字的功能。</p> <p>例如，在搜索附註時，使用"like %Current% %Dead%"返回任何包含短語"Current to Dead"的附註。 不包含任何包含「死到最新」的附註。 系統會依列出順序搜尋每個值。 %代表萬用字元或文字區段。</p> <p>此修飾符只能用於文本模式篩選器。 如需篩選器中文字模式的詳細資訊，請參閱 <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">使用文字模式編輯篩選器</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>小於</strong> </p> </td> 
   <td> <p><strong>lt</strong> </p> </td> 
   <td> <p>這會搜尋值小於輸入值的所有結果，不包括輸入值。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>大於或等於</strong> </p> </td> 
   <td> <p><strong>get</strong> </p> </td> 
   <td> <p>這會搜尋值大於或等於輸入值的所有結果。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>小於和等於</strong> </p> </td> 
   <td> <p><strong>lte</strong> </p> </td> 
   <td> <p>這會搜尋值小於或等於輸入值的所有結果。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>介於</strong> </p> </td> 
   <td> <p><strong>介於</strong> </p> </td> 
   <td> <p>提供兩個必填欄位值，並搜尋兩個欄位範圍內的所有結果，包括輸入的值。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>notcontains</strong> </p> </td> 
   <td> <p>（區分大小寫）會篩選缺少指定值的項目。</p> <p>例如，"notcontains inf"會擷取任何不含"inf"的項目，但會顯示包含"Inf"的值。</p> <p>此修飾符只能用於文本模式篩選器。 如需篩選器中文字模式的詳細資訊，請參閱 <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">使用文字模式編輯篩選器</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>之間</strong> </p> </td> 
   <td> <p>這是 <strong>介於</strong>. 它提供兩個必填值欄位，並搜索兩個欄位範圍之外的所有結果，包括輸入的值。</p> <p>此修飾符只能用於文本模式篩選器。 如需篩選器中文字模式的詳細資訊，請參閱 <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">使用文字模式編輯篩選器</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>不等於</strong> </p> </td> 
   <td> <p><strong>諾丁</strong> </p> </td> 
   <td> <p>（區分大小寫）這與 <strong>in</strong>. 它只返回指定清單中不返回的結果。</p> <p>此修飾符只能用於文本模式篩選器。 如需篩選器中文字模式的詳細資訊，請參閱 <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">使用文字模式編輯篩選器</a>.</p> <p>注意： <span>如果您要篩選的欄位有多個選項，則此選項會篩選出包含您指定的選項、您指定的選項以及任何其他選項的結果。</span> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> </td> 
   <td><strong>ne</strong> </td> 
   <td> <p>（區分大小寫）這與 <strong>eq</strong>. 它只會傳回與所搜尋值不完全相符的結果，也會比對值的大小寫。</p> <p>例如， <b>ne</b> 會傳回不等於「目前」的任何值，但不會傳回不等於「目前」的任何值。 </p> <p>此修飾符只能用於文本模式篩選器。 如需篩選器中文字模式的詳細資訊，請參閱 <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">使用文字模式編輯篩選器</a>.<br></p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> </td> 
   <td><strong>cine</strong> </td> 
   <td> <p>（不區分大小寫）此選項不區分大小寫， <strong>ne</strong> 而且是相反的 <b>cieq</b> 修飾詞。 它只會傳回與所搜尋值不完全相符的結果，而不會考慮值的大小寫。</p> <p>例如， <b>cine</b> 傳回不等於「current」或「Current」的任何值。 </p> <p>此修飾符只能用於文本模式篩選器。 如需篩選器中文字模式的詳細資訊，請參閱 <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">使用文字模式編輯篩選器</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
