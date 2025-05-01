---
product-area: reporting
navigation-topic: reporting-elements
title: 篩選和條件修飾元
description: 篩選和條件修飾元可讓您建立篩選器，並建立格式化報表結果的條件。
author: Nolan
feature: Reports and Dashboards
exl-id: 13e9d926-8a89-490e-aa7a-e6e8baf2a36b
source-git-commit: 6bd9dc626befc4dfa4054760e7ec7d677f6da6e5
workflow-type: tm+mt
source-wordcount: '1593'
ht-degree: 0%

---

# 篩選和條件修飾元

<!-- Audited: 11/2024 -->

<!--(NOTE: Alina: This is temporary - Lilit is fixing this in a future story: NOTE If the field you are filtering for has multiple options, this filters out the results that contain only the choice you specify. If the field contains additional options including the one specified, those results are not filtered from the report. See this document and search for "not equal" for the link to the req doc: https://docs.google.com/document/d/1WA0zZ_wws-2qb908i53BFQ8zDwL3nPJHyIybtJvvnqU/edit)-->

篩選和條件修飾元可讓您建立篩選器，並建立格式化報表結果的條件。

如需建立篩選的詳細資訊，請參閱文章[篩選概觀](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)。

如需有關在檢視中使用條件格式的詳細資訊，請參閱文章[在檢視中使用條件格式](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md)。

## 篩選和條件修飾元

有些修飾元是內建的，您可以從篩選器或條件式格式陳述式內的下拉式選單中進行選擇。 其他修飾元只能用於文字模式篩選中。

如需瞭解文字模式的詳細資訊，請參閱[文字模式概觀](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md)。

如需內建時間範圍修飾元的清單，請參閱文章[依時間範圍篩選報表](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/filter-reports-time-frames.md)。

您可以在篩選和條件式格式陳述式中使用下列條件修飾元：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>內建修飾元</strong> </p> </th> 
   <th> <p><strong>文字模式修飾元</strong> </p> </th> 
   <th> <p><strong>說明</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr valign="top"> 
   <td> <p><strong>為空白</strong> </p> </td> 
   <td> <p><strong>空白</strong> </p> </td> 
   <td> <p>物件的欄位存在，但該欄位目前沒有值。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>不是空白的</strong> </p> </td> 
   <td> <p><strong>notblank</strong> </p> </td> 
   <td> <p>您正在篩選的欄位已存在，且已被指定值。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>null</strong> </p> </td> 
   <td> <p>欄位為空白或不存在。 例如，您要尋找沒有父系任務ID的專案。 這表示您只想看到獨立的工作。 「父系任務ID」的限定詞是<strong>null</strong>，因為沒有ID的任務（在此例中為父系）不存在。 </p> <p>此修飾元只能用於文字模式篩選中。 如需篩選器中文字模式的詳細資訊，請參閱<a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">使用文字模式編輯篩選</a>。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>notnull</strong> </p> </td> 
   <td> <p>您正在篩選的欄位存在，且包含null以外的值。</p> <p>此修飾元只能用於文字模式篩選中。 如需篩選器中文字模式的詳細資訊，請參閱<a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">使用文字模式編輯篩選</a>。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>包含</strong> </p> </td> 
   <td> <p><strong>cicontains</strong> </p> </td> 
   <td> <p>這是<strong>包含</strong>的<i>不區分大小寫</i>版本。 例如： <code>cicontains inf</code>擷取任何包含<code>Inf</code>或<code>inf</code>的值。</p> <p> <p>注意：Adobe Workfront會搜尋您為每個篩選陳述式指定的確切字詞或片語。 例如，如果您要搜尋名稱中包含詞語<code>new project</code>的任何專案，Workfront不會顯示名稱中只有<code>new</code>或只有<code>project</code>或<code>new main project</code>的專案。 此篩選只會尋找名稱中有精確字詞<code>new project</code>的專案。</p> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>不包含</strong> </p> </td> 
   <td> <p><strong>cinotcontains</strong> </p> </td> 
   <td> <p>這是<strong>notcontains</strong>的<i>不區分大小寫</i>版本。</p><p>此修飾元會篩選缺少指定值的專案。</p> <p>例如，<code>does not contain inf</code>擷取名稱中沒有<code>Inf</code>或<code>inf</code>的任何專案。</p> <p>附註：套用至包含多個值的欄位時（例如專案中的附註集合），篩選器會依照下列方式決定排除專案：
<ul>
    <li>如果集合中的所有專案都包含指定文字，則從結果中排除整個記錄。</li>
    <li>如果集合中至少有一個專案不包含指定的文字，則記錄會保留在結果中。</li>
</ul>
 </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> </td> 
   <td> <p><strong>包含</strong> </p> </td> 
   <td> <p> 在整個文字字串中搜尋指定的<i>區分大小寫</i>文字。</p> <p>例如，使用<code>contains Inf</code>會擷取任何含有<code>Inf</code>的內容，例如單字 <code>Infinity.</code></p> <p>此修飾元只能用於文字模式篩選。如需有關篩選中文字模式的詳細資訊，請參閱<a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">使用文字模式編輯篩選</a>。</p> </td> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>notcontains</strong> </p> </td> 
   <td> <p>它會篩選缺少指定<i>區分大小寫</i>值的專案。</p> <p>例如，<code>notcontains inf</code>擷取任何不含<code>inf</code>的值，但會顯示包含<code>Inf</code>的值。</p> <p>此修飾元只能用於文字模式篩選中。 如需篩選器中文字模式的詳細資訊，請參閱<a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">使用文字模式編輯篩選</a>。</p> </td> 
  </tr> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>cieq</strong> </p> </td> 
   <td> <p>這是<strong>eq</strong>的<i>不區分大小寫</i>選項。 它只會傳回與搜尋值完全相符的值。</p> <p>例如，當搜尋具有特定名稱的任務時，<code>task name cieq test</code>會尋找名稱是<code>Test</code>、<code>TEST</code>或<code>Test</code>的任務，但找不到具有名稱的任務 <code>test 123.</code></p> <p>搜尋狀態時，不支援<strong>cieq</strong>修飾元。 您應該使用區分大小寫的修飾詞<strong>eq</strong>來搜尋狀態。</p> <p>此修飾元只能用於文字模式篩選中。 如需篩選器中文字模式的詳細資訊，請參閱<a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">使用文字模式編輯篩選</a>。</p> </td>
  </tr> 
  <tr valign="top"> 
   <td> </td> 
   <td><strong>電影</strong> </td> 
   <td> <p>這是<strong>ne</strong>的<i>不區分大小寫</i>選項，它與<b>cieq</b>修飾元相反。 它只會傳回與搜尋值不完全相符的結果，不會考慮值的大小寫。</p> <p>例如，<b>cine</b>會傳回不等於「current」或「Current」的任何值。 </p> <p>此修飾元只能用於文字模式篩選中。 如需篩選器中文字模式的詳細資訊，請參閱<a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">使用文字模式編輯篩選</a>。</p> </td> 
  </tr>   <tr valign="top"> 
   <td> </td> 
   <td> <p><strong>eq</strong> </p> </td> 
   <td> <p>此修飾元只會傳回搜尋值完全相符的<i>區分大小寫</i>。</p> <p>例如，在搜尋完成的專案時，<code>eq CPL</code>會傳回所有處於完成狀態的專案。 <code>eq CPL, CUR</code>未傳回結果，因為專案無法同時完成且為目前專案。</p> <p>此修飾元只能用於文字模式篩選中。 如需篩選器中文字模式的詳細資訊，請參閱<a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">使用文字模式編輯篩選</a>。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> </td> 
   <td><strong>ne</strong> </td> 
   <td> <p>這是<strong>eq</strong>相對的<i>區分大小寫</i>。 它只會傳回與搜尋值不完全相符的結果，也會符合值的大小寫。</p> <p>例如，<b>ne</b>會傳回不等於「Current」的值，但不會傳回不等於「current」的值。 </p> <p>此修飾元只能用於文字模式篩選中。 如需篩選器中文字模式的詳細資訊，請參閱<a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">使用文字模式編輯篩選</a>。<br></p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>ciin</strong> </p> </td> 
   <td> <p> 這是</strong>中<strong>的<i>不區分大小寫</i>版本。</p> <p>此修飾元只能用於文字模式篩選中。 如需篩選器中文字模式的詳細資訊，請參閱<a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">使用文字模式編輯篩選</a>。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>西諾丁</strong> </p> </td> 
   <td> <p>這是<strong>notin</strong>的<i>不區分大小寫</i>版本。</p> <p>此修飾元只能用於文字模式篩選中。 如需篩選器中文字模式的詳細資訊，請參閱<a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">使用文字模式編輯篩選</a>。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> <p> </p> <p> </p> <p><strong>等於</strong> </p> </td> 
   <td> <p><strong>在</strong> </p> </td> 
   <td> <p>此修飾元可讓您建立逗號分隔的<i>區分大小寫</i>變數清單，以與篩選器中評估的單一屬性進行比較。 系統會將整個清單視為OR陳述式，並傳回符合一或多個變數條件的任何結果。</p> <p>例如，在搜尋專案時，使用<code>in CUR, PLN, CPL</code>會傳回所有處於「目前」、「OR規劃」或「完成」狀態的專案。</p> <p>內建修飾元<strong>Equal</strong>對應至<strong>in</strong>的文字模式修飾元。 這表示您可以為該欄位選擇等於多個值。</p> <p>例如，您可在專案報表中選擇「狀態等於目前、計畫、廢棄」，並可檢視任何這些狀態的專案。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>不等於</strong> </p> </td> 
   <td> <p><strong>notin</strong> </p> </td> 
   <td> <p>這是<i>區分大小寫</i>，與<strong>in</strong>相反。 它只傳回指定清單以外的結果。</p> <p>此修飾元只能用於文字模式篩選中。 如需篩選器中文字模式的詳細資訊，請參閱<a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">使用文字模式編輯篩選</a>。</p> <p>注意： <span>如果您要篩選的欄位有多個選項，這會篩選出包含您所指定之選項、您所指定之選項以及任何其他選項的結果。</span> </p> </td> 
  </tr>
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>贊</strong> </p> </td> 
   <td> <p>這個修飾元會以類似於<strong>contains</strong>的方式，搜尋<i>區分大小寫</i>文字字串的部分。 但是，<strong>like</strong>提供插入萬用字元以分隔文字的功能。</p> <p>例如，在搜尋備註時，使用<code>like %Current% %Dead%</code>會傳回任何包含片語「Current to Dead」的備註。 其中不包含任何包含「無效至目前」的備註。 每個值都會依照其列出的順序進行搜尋。 %代表萬用字元取代文字的字元或區段。 底線也可用於單一萬用字元，例如傳回「專案」和「專案」的<code>like Project_</code>。 如果您打算在篩選中使用<strong>like</strong>或<strong>clike</strong>修飾元，建議避免在自訂資料欄位名稱、引數選項值或其他物件名稱中使用%或_字元。</p><p>此修飾元只能用於文字模式篩選中。 如需篩選器中文字模式的詳細資訊，請參閱<a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">使用文字模式編輯篩選</a>。</p> </td> 
  </tr>  
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>cilike</strong> </p> </td> 
   <td> <p>這是<strong>like</strong>的<i>不區分大小寫</i>版本。 例如： <code>cilike %Current% %Dead%</code>會傳回任何包含<code>Current to Dead</code>或<code>current to dead</code>的備註。</p> <p>此修飾元只能用於文字模式篩選中。 如需篩選器中文字模式的詳細資訊，請參閱<a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">使用文字模式編輯篩選</a>。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td><strong>不存在</strong> </td> 
   <td><strong>NOTEXISTS</strong> </td> 
   <td> <p>此修飾詞僅能與EXISTS陳述式中的複雜篩選器搭配使用。 這些篩選條件僅參考下列物件： </p> 
    <ul> 
     <li>物件階層中跨多個層級的物件 </li> 
     <li>遺失的物件 </li> 
    </ul> <p>如需有關使用EXISTS陳述式建立複雜篩選器的資訊，請參閱文章<a href="../../../reports-and-dashboards/reports/text-mode/create-complex-text-mode-filters-using-exists-statements.md">使用EXISTS陳述式建立複雜文字模式篩選器</a>。 這是EXISTS陳述式中使用的唯一修飾元。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>大於</strong> </p> </td> 
   <td> <p><strong>gt</strong> </p> </td> 
   <td> <p>這會搜尋值大於輸入值的所有結果，不包括輸入的值。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>小於</strong> </p> </td> 
   <td> <p><strong>lt</strong> </p> </td> 
   <td> <p>這會搜尋值小於輸入值的所有結果，不包括輸入的值。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>大於或等於</strong> </p> </td> 
   <td> <p><strong>gte</strong> </p> </td> 
   <td> <p>這會搜尋值大於或等於輸入值的所有結果。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>小於或等於</strong> </p> </td> 
   <td> <p><strong>lte</strong> </p> </td> 
   <td> <p>這會搜尋值小於或等於輸入值的所有結果。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>介於</strong>之間 </p> </td> 
   <td> <p><strong>介於</strong>之間 </p> </td> 
   <td> <p>提供兩個必要欄位值，並搜尋兩個欄位範圍內的所有結果，包括輸入的值。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>notbetween</strong> </p> </td> 
   <td> <p>這與<strong>介於</strong>之間的數字相反。 它提供兩個必填值欄位，並搜尋兩個欄位範圍以外的所有結果，包括輸入的值。</p> <p>此修飾元只能用於文字模式篩選中。 如需篩選器中文字模式的詳細資訊，請參閱<a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">使用文字模式編輯篩選</a>。</p> </td> 
  </tr>

</tbody> 
</table>
