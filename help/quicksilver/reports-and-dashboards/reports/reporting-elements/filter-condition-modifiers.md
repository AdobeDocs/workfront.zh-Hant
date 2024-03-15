---
product-area: reporting
navigation-topic: reporting-elements
title: 篩選和條件修飾元
description: 篩選和條件修飾元可讓您建立篩選器，並建立格式化報表結果的條件。
author: Nolan
feature: Reports and Dashboards
exl-id: 13e9d926-8a89-490e-aa7a-e6e8baf2a36b
source-git-commit: d2268e50080ddbe306731d034d88fd29b712b86d
workflow-type: tm+mt
source-wordcount: '1516'
ht-degree: 0%

---

# 篩選和條件修飾元

<!-- Audited: 1/2024 -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: This is temporary - Lilit is fixing this in a future story: NOTE If the field you are filtering for has multiple options, this filters out the results that contain only the choice you specify. If the field contains additional options including the one specified, those results are not filtered from the report. See this document and search for "not equal" for the link to the req doc: https://docs.google.com/document/d/1WA0zZ_wws-2qb908i53BFQ8zDwL3nPJHyIybtJvvnqU/edit) </p>
-->

篩選和條件修飾元可讓您建立篩選器，並建立格式化報表結果的條件。

如需建立篩選器的詳細資訊，請參閱文章 [篩選器概觀](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

如需在檢視中使用條件式格式的詳細資訊，請參閱文章 [在檢視中使用條件式格式](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md).

## 篩選和條件修飾元

有些修飾元是內建的，您可以從篩選器或條件式格式陳述式內的下拉式選單中進行選擇。 其他修飾元只能用於文字模式篩選中。

如需瞭解文字模式的詳細資訊，請參閱 [文字模式概觀](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

如需內建時間範圍修飾元的清單，請參閱文章 [依時間範圍篩選報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/filter-reports-time-frames.md).

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
   <td> <p><strong>不為空白</strong> </p> </td> 
   <td> <p><strong>非空白</strong> </p> </td> 
   <td> <p>您正在篩選的欄位已存在，且已被指定值。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>null</strong> </p> </td> 
   <td> <p>欄位為空白或不存在。 例如，您要尋找沒有父系任務ID的專案。 這表示您只想看到獨立的工作。 「父系任務ID」的限定詞是 <strong>null</strong>，因為沒有ID的工作（在此為父系）並不存在。 </p> <p>此修飾元只能用於文字模式篩選中。 如需有關篩選器中文字模式的詳細資訊，請參閱 <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">使用文字模式編輯篩選器</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>notnull</strong> </p> </td> 
   <td> <p>您正在篩選的欄位存在，且包含null以外的值。</p> <p>此修飾元只能用於文字模式篩選中。 如需有關篩選器中文字模式的詳細資訊，請參閱 <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">使用文字模式編輯篩選器</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>包含</strong> </p> </td> 
   <td> <p><strong>芝麻菜</strong> </p> </td> 
   <td> <p>這是 <i>區分大小寫</i> 版本 <strong>包含</strong>. 例如： <code>cicontains inf</code> 擷取任何包含下列專案的值： <code>Inf</code> 或 <code>inf</code>.</p> <p> <p>注意：Adobe Workfront會搜尋您為每個篩選陳述式指定的確切字詞或片語。 例如，如果您要搜尋包含片語的任何專案 <code>new project</code> 在名稱中，Workfront不會顯示只有 <code>new</code> 或只是 <code>project</code>，或 <code>new main project</code> 在名稱中。 此篩選器只會尋找包含精確片語的專案 <code>new project</code> 在名稱中。</p> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>不包含</strong> </p> </td> 
   <td> <p><strong>香芹菜包含</strong> </p> </td> 
   <td> <p>這是 <i>區分大小寫</i> 版本 <strong>notcontains</strong>.</p><p>此修飾元會篩選缺少指定值的專案。</p> <p>例如， <code>does not contain inf</code> 擷取任何內容，而不 <code>Inf</code> 或 <code>inf</code> 在名稱中。</p> <p>注意： <span>如果您要篩選的欄位有多個選項，這會篩選出包含您指定之選擇、您指定之選擇以及任何其他選擇的結果。</span> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> </td> 
   <td> <p><strong>包含</strong> </p> </td> 
   <td> <p> 搜尋指定的 <i>區分大小寫</i> 整個文字字串中的文字。</p> <p>例如，使用 <code>contains Inf</code> 擷取任何內容 <code>Inf</code> 在其中，例如單字 <code>Infinity.</code></p> <p>此修飾元只能用於文字模式篩選。如需有關篩選中文字模式的詳細資訊，請參閱 <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">使用文字模式編輯篩選器</a>.</p> </td> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>notcontains</strong> </p> </td> 
   <td> <p>它會篩選缺少 <i>區分大小寫</i> 指定的值。</p> <p>例如， <code>notcontains inf</code> 擷取任何內容，而不 <code>inf</code>，但會顯示包含 <code>Inf</code>.</p> <p>此修飾元只能用於文字模式篩選中。 如需有關篩選器中文字模式的詳細資訊，請參閱 <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">使用文字模式編輯篩選器</a>.</p> </td> 
  </tr> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>cieq</strong> </p> </td> 
   <td> <p>這是 <i>區分大小寫</i> 選項 <strong>eq</strong>. 它只會傳回與搜尋值完全相符的值。</p> <p>例如，當搜尋具有特定名稱的任務時， <code>task name cieq test</code> 尋找名稱為的任務 <code>Test</code>， <code>TEST</code>，或 <code>Test</code>，但找不到名稱為的任務 <code>test 123.</code></p> <p>搜尋狀態時， <strong>cieq</strong> 不支援修飾元。 您應使用區分大小寫的修飾詞， <strong>eq</strong>，以搜尋狀態。</p> <p>此修飾元只能用於文字模式篩選中。 如需有關篩選器中文字模式的詳細資訊，請參閱 <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">使用文字模式編輯篩選器</a>.</p> </td>
  </tr> 
  <tr valign="top"> 
   <td> </td> 
   <td><strong>電影</strong> </td> 
   <td> <p>這是 <i>區分大小寫</i> 選項 <strong>新</strong>，而此函式與 <b>cieq</b> 修飾元。 它只會傳回與搜尋值不完全相符的結果，不會考慮值的大小寫。</p> <p>例如， <b>電影</b> 傳回不等於「current」或「Current」的任何值。 </p> <p>此修飾元只能用於文字模式篩選中。 如需有關篩選器中文字模式的詳細資訊，請參閱 <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">使用文字模式編輯篩選器</a>.</p> </td> 
  </tr>   <tr valign="top"> 
   <td> </td> 
   <td> <p><strong>eq</strong> </p> </td> 
   <td> <p>此修飾詞只會傳回精確的、 <i>區分大小寫</i> 搜尋值的相符項。</p> <p>例如，當搜尋完整的專案時， <code>eq CPL</code> 傳回所有處於完成狀態的專案。 <code>eq CPL, CUR</code> 不會傳回結果，因為專案無法同時完成和目前專案。</p> <p>此修飾元只能用於文字模式篩選中。 如需有關篩選器中文字模式的詳細資訊，請參閱 <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">使用文字模式編輯篩選器</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> </td> 
   <td><strong>新</strong> </td> 
   <td> <p>這是 <i>區分大小寫</i> 反向 <strong>eq</strong>. 它只會傳回與搜尋值不完全相符的結果，也會符合值的大小寫。</p> <p>例如， <b>新</b> 傳回不等於「Current」的值，但不會傳回不等於「current」的值。 </p> <p>此修飾元只能用於文字模式篩選中。 如需有關篩選器中文字模式的詳細資訊，請參閱 <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">使用文字模式編輯篩選器</a>.<br></p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>ciin</strong> </p> </td> 
   <td> <p> 這是 <i>區分大小寫</i> 版本 <strong>在</strong>.</p> <p>此修飾元只能用於文字模式篩選中。 如需有關篩選器中文字模式的詳細資訊，請參閱 <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">使用文字模式編輯篩選器</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>香茅素</strong> </p> </td> 
   <td> <p>這是 <i>區分大小寫</i> 版本 <strong>notin</strong>.</p> <p>此修飾元只能用於文字模式篩選中。 如需有關篩選器中文字模式的詳細資訊，請參閱 <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">使用文字模式編輯篩選器</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> <p> </p> <p> </p> <p><strong>等於</strong> </p> </td> 
   <td> <p><strong>在</strong> </p> </td> 
   <td> <p>此修飾詞可讓您建立以下專案以逗號分隔的清單： <i>區分大小寫</i> 要與篩選器中評估的單一屬性進行比較的變數。 系統會將整個清單視為OR陳述式，並傳回符合一或多個變數條件的任何結果。</p> <p>例如，在搜尋專案時，使用 <code>in CUR, PLN, CPL</code> 傳回所有處於「目前」、「OR計畫」或「完成」狀態的專案。</p> <p>內建修飾元 <strong>等於</strong> 對應至的文字模式修飾元 <strong>在</strong>. 這表示您可以為該欄位選擇等於多個值。</p> <p>例如，您可在專案報表中選擇「狀態等於目前、計畫、廢棄」，並可檢視任何這些狀態的專案。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>不等於</strong> </p> </td> 
   <td> <p><strong>notin</strong> </p> </td> 
   <td> <p>這是 <i>區分大小寫</i> 反向 <strong>在</strong>. 它只傳回指定清單以外的結果。</p> <p>此修飾元只能用於文字模式篩選中。 如需有關篩選器中文字模式的詳細資訊，請參閱 <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">使用文字模式編輯篩選器</a>.</p> <p>注意： <span>如果您要篩選的欄位有多個選項，這會篩選出包含您指定之選擇、您指定之選擇以及任何其他選擇的結果。</span> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>cilike</strong> </p> </td> 
   <td> <p>這是 <i>區分大小寫</i> 版本 <strong>按讚</strong>. 例如： <code>cilike %Current% %Dead%</code> 傳回任何包含 <code>Current to Dead</code> 或 <code>current to dead</code>.</p> <p>此修飾元只能用於文字模式篩選中。 如需有關篩選器中文字模式的詳細資訊，請參閱 <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">使用文字模式編輯篩選器</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>按讚</strong> </p> </td> 
   <td> <p>此修飾元會搜尋 <i>區分大小寫</i> 文字字串與 <strong>包含</strong>. 不過， <strong>按讚</strong> 提供插入萬用字元來分隔文字的功能。</p> <p>例如，搜尋備註時，使用 <code>like %Current% %Dead%</code> 傳回任何包含片語「Current to Dead」的備註。 其中不包含任何包含「無效至目前」的備註。 每個值都會依照其列出的順序進行搜尋。 %代表萬用字元取代文字的字元或區段。</p> <p>此修飾元只能用於文字模式篩選中。 如需有關篩選器中文字模式的詳細資訊，請參閱 <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">使用文字模式編輯篩選器</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td><strong>不存在</strong> </td> 
   <td><strong>NOTEXIST</strong> </td> 
   <td> <p>此修飾詞僅能與EXISTS陳述式中的複雜篩選器搭配使用。 這些篩選條件僅參考下列物件： </p> 
    <ul> 
     <li>物件階層中跨多個層級的物件 </li> 
     <li>遺失的物件 </li> 
    </ul> <p>如需有關使用EXISTS陳述式建立複雜篩選器的資訊，請參閱本文 <a href="../../../reports-and-dashboards/reports/text-mode/create-complex-text-mode-filters-using-exists-statements.md">使用EXISTS陳述式建立複雜的文字模式篩選器</a>. 這是EXISTS陳述式中使用的唯一修飾元。</p> </td> 
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
   <td> <p><strong>介於</strong> </p> </td> 
   <td> <p><strong>介於</strong> </p> </td> 
   <td> <p>提供兩個必要欄位值，並搜尋兩個欄位範圍內的所有結果，包括輸入的值。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>notbetween</strong> </p> </td> 
   <td> <p>這與 <strong>介於</strong>. 它提供兩個必填值欄位，並搜尋兩個欄位範圍以外的所有結果，包括輸入的值。</p> <p>此修飾元只能用於文字模式篩選中。 如需有關篩選器中文字模式的詳細資訊，請參閱 <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">使用文字模式編輯篩選器</a>.</p> </td> 
  </tr>

</tbody> 
</table>
