---
content-type: overview;reference
product-area: reporting
navigation-topic: reporting-navigation-topic
title: 開始使用報告
description: 報表可讓您檢視使用者和工作的最新狀況。 使用報表，您可以在Adobe Workfront中顯示物件的相關資訊。
author: Nolan
feature: Reports and Dashboards
exl-id: 478512af-a47c-4488-878a-581e238e0064
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '3292'
ht-degree: 1%

---

# 開始使用報告

<!-- Audited: 12/2023 -->

報表可讓您檢視使用者和工作的最新狀況。 使用報表，您可以在Adobe Workfront中顯示物件的相關資訊。

如需瞭解物件以及如何在Workfront應用程式中報告物件的相關資訊，請參閱[Adobe Workfront物件概觀](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md)。

## 報表元素

報表是Workfront中下列三個元素的組合：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">檢視</td> 
   <td> <li>定義報表中的欄，以及可在每欄中加入的資訊。</li> <li>如需檢視的相關資訊，請參閱<a href="../../../reports-and-dashboards/reports/reporting-elements/views-overview.md" class="MCXref xref">Adobe Workfront中的檢視總覽</a>。</li> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">分組</td> 
   <td> <li>根據常見資訊對資訊進行分類，並在標題下列出報告結果。</li> <li>如需群組的相關資訊，請參閱Adobe Workfront中的<a href="../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md" class="MCXref xref">群組概觀</a>。</li> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">篩選器</td> 
   <td> <li>控制報表中顯示的資訊量。</li> <li>如需篩選的詳細資訊，請參閱<a href="../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md" class="MCXref xref">篩選總覽</a>。</li> <li>如需篩選修飾元的資訊，請參閱<a href="../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md" class="MCXref xref">篩選和條件修飾元</a>。</li> <li>您可以使用萬用字元進行篩選，讓您的篩選器更通用，並提供更靈活的使用方式。</li> <li>如需在篩選中使用萬用字元的詳細資訊，請參閱<a href="../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md" class="MCXref xref">萬用字元篩選變數</a>。</li> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>當您從清單中選取新的篩選器、檢視或群組時，即使您登出Workfront或關閉瀏覽器，該選取專案仍會保留。

如需有關報表元素的資訊，請參閱[報表元素：篩選器、檢視和群組](../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md)。

若要增強報表，您可以新增下列元素：

* 圖表：報表中結果的視覺化表示法。\
  如需關於圖表報表的資訊，請參閱[新增圖表至報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md)。

* 矩陣分組：以彙總表格格式彙總報表資訊。\
  如需矩陣報表的相關資訊，請參閱[建立矩陣報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md)。

* 提示：開啟的篩選器，您每次執行報表時，皆可透過不同方式自訂和套用。\
  如需提示的相關資訊，請參閱[新增提示至報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)。

建立報表時，您可以在Report Builder中個別修改這些元素。

增強報表中所包含資訊相關性的另一種方法，是將條件式格式套用至檢視。 如需使用條件式格式的資訊，請參閱[在檢視中使用條件式格式](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md)。

## 系統報表

Workfront提供數個系統報告，預設會載入您的系統。\
在系統中輸入資訊後，您可以使用這些報表以可視方式顯示資訊。

如需有關如何存取系統報表以及哪些系統報表可用的詳細資訊，請參閱[使用Adobe Workfront內建報表](../../../reports-and-dashboards/reports/using-built-in-reports/use-workfront-built-in-reports.md)。

## 建立報表

除了Workfront提供的系統報表之外，您也可以建立自己的自訂報表，以符合貴組織的需求。

若要建立報告，您可以執行下列任一項作業：

* 從頭開始建立報表。
* 複製現有報表。

  您必須至少具有「檢視」許可權，才能複製其他人建立的報表。 如需複製報告的詳細資訊，請參閱[建立報告復本](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md)。

如需建立報表的相關資訊，請參閱[建立自訂報表](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)。

### 建立報告的先決條件 {#prerequisites-for-creating-reports}

* 您必須擁有Standard或Plan授權才能建立您自己的報告。

  如需Workfront授權型別的相關資訊，請參閱目前授權的[授權總覽](../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md)，以及新授權的[新授權總覽](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/licenses-overview.md)。

* 您的Workfront管理員必須授予您存取層級中「編輯報表」的存取權。

  如需授與編輯報告存取權的相關資訊，請參閱[授與報告、儀表板和行事曆的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md)。

* 您的Workfront管理員必須授予您存取層級中編輯篩選器、檢視和群組的存取權。

  如需授與編輯篩選器、檢視和群組存取權的相關資訊，請參閱[授與篩選器、檢視和群組的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-fvg.md)。

* 您必須定義一個要報告的物件。 報表是Workfront中的特定物件，您必須先選取物件型別，才能開始建立報表。 您只能報告Workfront介面中可用的物件。

### 報告擁有權 {#report-ownership}

在Workfront中建立報表時，您會成為該報表的預設擁有者，且會顯示在「我的報表」區段中。 您無法變更報表的擁有者。

複製報表時，您會自動成為所複製報表的所有者。
如需複製報告的資訊，請參閱[建立報告復本](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md)。

您可以檢閱&#x200B;**輸入者**&#x200B;欄位，以檢視報表擁有者。

![輸入者欄位](assets/unshimmed-entered-by.png)

### 在產生器介面中建立報表 {#create-reports-in-the-builder-interface}

建議您先使用報告建置介面來建置新報告。 此介面提供了一組簡化的工具，可引導您逐步將元素放在一起，以建立您想要的報告。 您有物件和欄位，您可以從清單中選取並新增至所有報表元素。\
如需有關在報告建置介面中建立報告的詳細資訊，請參閱[建立自訂報告](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)。

如需您可以報告的物件清單，請參閱文章[Adobe Workfront物件概觀](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#report-on-objects)中的[物件報告](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md)區段。

如需您可以在報表中顯示的欄位詳細資訊，請參閱[Adobe Workfront術語辭彙表](../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md)。

### 以文字模式建立報表 {#create-reports-in-text-mode}

有時在產生器介面中可能找不到某些欄位，但這些欄位可能會在API中提供。\
如需API中有哪些欄位可用的資訊，請參閱文章[API Explorer](../../../wf-api/general/api-explorer.md)。

如需有關如何使用API Explorer的資訊，請參閱文章[使用API Explorer](../../../wf-api/general/using-api-explorer.md)。

>[!NOTE]
>
>您無法在Workfront介面中報告Report Builder中無法提供的物件。 不過，如果可透過API使用與Report Builder中物件相關聯的欄位，您便可以報告這些欄位。 若要這麼做，您必須使用「文字模式」介面。

「文字模式」可讓您使用標準模式介面中無法使用的欄位，來建立更複雜的檢視、篩選器、群組和提示。

#### 文字模式術語 {#text-mode-terminology}

您必須使用特定語法才能使用Workfront文字模式介面。

如需文字模式Workfront語法的詳細資訊，請參閱[文字模式語法概觀](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md)。

#### 計算欄、條件式格式及文字模式的其他用途 {#calculated-columns-conditional-formatting-and-other-uses-of-text-mode}

除了在產生器介面中無法使用的欄位報告之外，您可以使用文字模式來顯示計算或特定欄位之間的比較。

如需報表中最常使用的文字模式清單，請參閱[文字模式常見使用概述](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md)。

如需在報表中包含計算自訂資料的相關資訊，請參閱[報表中的計算自訂資料](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-custom-data-reports.md)。

如需比較條件式格式的欄位資訊，請參閱[比較條件式格式的欄位](../../../reports-and-dashboards/reports/text-mode/compare-fields-conditional-formatting.md)。

您也可以使用報告中的文字模式來參照集合欄位。\
如需有關使用文字模式在報表中顯示集合資訊的資訊，請參閱[報表中的參考集合](../../../reports-and-dashboards/reports/text-mode/reference-collections-report.md)。

#### 文字模式範例 {#text-mode-samples}

我們有一個範例庫，內含您可以透過「文字模式」建立的最常使用的檢視、篩選器和群組。

若要瀏覽此程式庫並使用我們提供的部分範例，請參閱文章[自訂檢視、篩選及分組範例：文章索引](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md)。

## 報告的標籤

在介面中執行報表時，報表可包含數個標籤。

如需有關執行報表的資訊，請參閱文章[執行報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/run-report.md)。

在每個標籤上，您包含在報表中的資訊會以稍微不同的格式顯示。 選擇最符合您組織需求的格式。

您可以將任何標籤設為報表的預設標籤。 預設標籤是按一下報告名稱以將其開啟時顯示的第一個標籤，也是將報告放置到儀表板時顯示的標籤。

### 詳細資訊標籤 {#details-tab}

報表的詳細資訊標籤會顯示報表的物件，以及您在清單表單中為物件選擇的屬性。 每個報表都有「詳細資訊」標籤。

>[!IMPORTANT]
>
>根據您的時區，「詳細資訊」標籤中的資訊可能會與「圖表」標籤顯示不同。\
>例如，加州的使用者於2月12日晚上9:30 PST完成工作。 當紐約的使用者檢視包含此任務完成的報告時，實際完成日期在2月13日詳細資訊標籤和圖表詳細資訊中都顯示為2月13日，因為它是在2月13日美國東部時間凌晨12:30完成的。 不過，在圖表中，它包含在2月12日分組中，直到您展開圖表元素為止。

### 摘要標籤 {#summary-tab}

包含分組的報表具有「摘要」標籤。

「詳細資訊」標籤上以清單格式顯示的相同資訊會根據「摘要」標籤上報告中的分組進行彙總和彙總。

如需群組的相關資訊，請參閱Adobe Workfront中的[群組概觀](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)。

### 矩陣索引標籤 {#matrix-tab}

包含矩陣群組的報表具有矩陣標籤。

「詳細資訊」標籤上以清單格式顯示的相同資訊會以表格格式顯示，並按「矩陣」標籤上報告中的群組分組。

當您將矩陣群組新增到報表中時，摘要標籤會由矩陣標籤取代。

如需有關建立矩陣群組的資訊，請參閱文章[建立矩陣報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md)。

### 圖表索引標籤 {#chart-tab}

包含圖表的報表會有「圖表」標籤。

請考慮在報表中加入圖表，讓您的高階主管瞭解控制面板的影響力。 圖表是在報表中顯示資訊的簡明方式。 您可以按一下圖表元素來展開該元素，以顯示該元素中包含的專案。

>[!IMPORTANT]
>
>當您按一下圖表元素時，展開的資訊可能會根據您的時區，與圖表顯示不同的資訊。\
>例如，加州的使用者於2月12日晚上9:30 PST完成工作。 當紐約的使用者檢視包含此任務完成的報告時，實際完成日期在2月13日詳細資訊標籤和圖表詳細資訊中都顯示為2月13日，因為它是在2月13日美國東部時間凌晨12:30完成的。 不過，在圖表中，它包含在2月12日分組中，直到您展開圖表元素為止。

如需有關使用圖表建置報表的資訊，請參閱文章[將圖表新增至報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md)。

### 提示索引標籤 {#prompts-tab}

包含提示的報告具有提示標籤。

每次執行報表時，系統都會提示您新增篩選器至報表。 當您將提示新增到報告時，提示索引標籤會自動成為報告的預設索引標籤。 無法變更為其他索引標籤。

如需有關建立報表提示的資訊，請參閱文章[新增提示至報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)。

## 共用報表

建立報表後，您可以與其他使用者共用。

### 授予報告共用許可權 {#give-sharing-permissions-to-a-report}

您可以將共用許可權授予其他使用者，以檢視或管理您建立的報表。 您可以授予其他使用者與您相同或以下的許可權層級。 您也可以使用共用許可權將報表設為公開。 如需共用報表的資訊，請參閱[在Adobe Workfront中共用報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/share-report.md)。

### 排程報表傳送 {#schedule-a-report-delivery}

您可以排程報表傳送。 您共用報告的使用者會收到一封包含報告結果附件的電子郵件。 附件可採用下列格式：

* HTML
* PDF
* Excel
* .TSV

如需排程報表傳送的相關資訊，請參閱[報表傳送概述](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md)。

### 匯出報告的結果 {#export-the-results-of-a-report}

您可以將報告結果匯出為下列檔案格式：

* PDF
* Excel （.xls和.xlsx格式）
* 頁籤分隔檔

如需有關匯出報告結果的資訊，請參閱[匯出資料](../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md)。

報告匯出為其中一種格式後，您可以透過電子郵件以附件形式傳送或列印報告來與其他使用者共用。

### 新增報告至儀表板 {#add-a-report-to-a-dashboard}

您可以將報表新增至控制面板，並與其他使用者共用控制面板。 如需有關將報表新增至儀表板的資訊，請參閱[將報表新增至儀表板](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/add-report-dashboard.md)。

## 建立行事曆

如果您想要以行事曆格式顯示資料，您可以建立行事曆而非報告。

如需有關建立及使用行事曆的資訊，請參閱[行事曆報告總覽](../../../reports-and-dashboards/reports/calendars/calendar-reports-overview.md)。

## 報告使用情況

建立報告並與其他使用者共用後，您可以追蹤其使用這些報告的頻率。
如需關於報告使用情況的資訊，包括檢影片率、檢視者是什麼使用者，以及檢視者在哪些控制面板上顯示，請參閱文章[報告使用概觀](../../../reports-and-dashboards/reports/report-usage/report-usage-overview.md)。

## 用於參考報表的常用辭彙

下列辭彙可作為Workfront報表的參考：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>字詞或片語</strong> </th> 
   <th><strong>定義</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>進階選項</td> 
   <td> <p>參考Report Builder欄（檢視）標籤上的連結，此連結提供下列功能：</p> 
    <ul> 
     <li>根據您選取的條件，設定文字和影像的欄條件式樣式格式。</li> 
     <li>為欄重新加上標籤。</li> 
     <li>格式化欄中的值。</li> 
    </ul> <p>例如，您可能想要以粗體顯示所有父系任務，或者如果任務延遲，您可能想要以紅色顯示「規劃完成日期」。</p> </td> 
  </tr> 
  <tr> 
   <td>屬性</td> 
   <td> 資料庫中定義的物件欄位。 它用於「文字模式」運算式。 <br>例如，在文字模式運算式中使用時，狀態列位會顯示為<em>狀態</em>。 </td> 
  </tr> 
  <tr> 
   <td>Bean或JavaBean</td> 
   <td>Bean代表可重複使用的程式設計元素。 Bean這個術語代表Workfront應用程式中不同物件之間的關係。 在嘗試顯示基本報告工具中無法提供的物件其他屬性時，請務必熟悉這些關係。</td> 
  </tr> 
  <tr> 
   <td>產生器介面或Report Builder</td> 
   <td>「產生器介面」是一系列下拉式功能表，其中包含「欄」 （檢視）、「篩選」和「群組」標籤中顯示的欄位。 它提供Bean關係的直覺對映，以協助識別檢視中的欄、篩選條件以及分組的共同屬性。</td> 
  </tr> 
  <tr> 
   <td>駝峰式大小寫</td> 
   <td> <p>駝峰式大小寫是指將程式設計元素寫入一起將多字屬性字串的特定方式。 以駝峰式拼寫屬性時，第一個字的第一個字母是小寫，兩個字之間沒有空格，任何後續字的第一個字母是大寫。</p> <p>例如，主群組將寫入為<em>homeGroup</em>，資源集區將為<em>resourcePool</em>，而實際開始日期將為<em>actualStartDate</em>。</p> </td> 
  </tr> 
  <tr> 
   <td>圖表</td> 
   <td> <p>Report Builder中的標籤，儲存報表後的報表標籤，以及報表的可選元素，可讓您將圖表新增至任何報表。 建立圖表之前，您必須在報告中定義分組。</p> <p>下列圖表型別可新增至任何報表：<br></p> 
    <ul> 
     <li>欄</li> 
     <li>長條圖</li> 
     <li>圓形</li> 
     <li>折線</li> 
     <li>量測計</li> 
     <li>泡泡</li> 
    </ul> <p>如需有關將圖表新增至報表的詳細資訊，請參閱文章<a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md" class="MCXref xref">將圖表新增至報表</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>詳細資料</td> 
   <td>這是您儲存報告後報告的其中一個標籤。 它會顯示報告的結果，顯示在您選擇的檢視和分組中。</td> 
  </tr> 
  <tr> 
   <td>運算式</td> 
   <td>運算式是文字模式中的書面公式，用於傳達使用「文字模式」介面時要搜尋或顯示的資訊。 它通常是較大的Text Mode陳述式中的一行。</td> 
  </tr> 
  <tr> 
   <td>欄位</td> 
   <td> <p>是指物件的屬性。 例如，「狀態」是專案、任務或問題的欄位。 「Portfolio Manager」是Portfolio物件的欄位。</p> <p>您也可以建立自訂欄位，並將其新增至自訂表格。<br>如需建立自訂表單的相關資訊，請參閱文章<a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md">建立自訂表單</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>欄位名稱 </td> 
   <td>顯示在檢視中的屬性值，或是用在篩選條件中，或是群組的一般元素之屬性值。 「欄位名稱」的選項取決於「欄位Source」選項。</td> 
  </tr> 
  <tr> 
   <td>欄位來源 </td> 
   <td>顯示在檢視中的物件值，或是用在篩選條件中，或是作為分組的通用元素。 Source欄位中的選項取決於所建立UI元素的物件型別。 欄位Source可讓您參照UI元素的物件型別以外的物件屬性。</td> 
  </tr> 
  <tr> 
   <td>篩選器</td> 
   <td>決定要在報表中顯示哪些結果的主要報表元素。</td> 
  </tr> 
  <tr> 
   <td>表單 </td> 
   <td>可與「自訂表格」互換使用。 欄位和區段會新增至表單，然後附加至物件，以擴大您可與物件關聯的欄位數量。</td> 
  </tr> 
  <tr> 
   <td>分組 </td> 
   <td>識別結果清單組織方式的主要報表元素。 群組會在整個報表中建立水準條，以便依據建立結果時定義的通用屬性將結果分組。 在矩陣報表中使用群組來彙總資料，在圖表中使用群組來決定圖表的座標軸。</td> 
  </tr> 
  <tr> 
   <td>物件或物件型別</td> 
   <td> 物件是Workfront應用程式元素（例如，專案、任務、群組、公司、篩選器）。 「物件型別」是用來建立新報表、檢視、篩選或群組，以識別哪個物件是報表的焦點。 報表只能有一個物件型別，這是報表的主要物件。<br>父物件可在相同報表中參照。<br>如需物件階層的詳細資訊，請參閱文章<a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">Adobe Workfront物件概觀</a>中的「瞭解物件的相互依存性和階層」一節。</td> 
  </tr> 
  <tr> 
   <td>提示</td> 
   <td> <p>可在每次執行報表需要使用不同篩選器時新增至報表的可選報表元素。</p> <p>如需提示的相關資訊，請參閱<a href="/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md" class="MCXref xref">新增提示至報表</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>適用對象或條件修飾元</td> 
   <td> <p>此欄位會顯示在報告的下列區域中：</p> 
    <ul> 
     <li>在篩選器索引標籤上</li> 
     <li>「欄（檢視）」標籤中欄的「進階選項」畫面。 藉由定義限定元，您可以將「欄位名稱」與其他欄位或值比較。</li> 
     <li> 在自訂提示中<br><p>如需提示的相關資訊，請參閱<a href="/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md" class="MCXref xref">新增提示至報表</a>。</p>。</li> 
    </ul> <p>例如，當為「計畫完成日期」為「今天」的任務建立篩選器時，您可在「辨識符號」欄位中選取<strong>等於</strong>，並在「日期」欄位中選取今天的日期：</p> <p><em>任務&gt;計畫完成日期&gt;等於&gt; （今天的日期）</em> </p> <p>在此案例中，限定詞是<strong>等於</strong>。<br>如需限定詞的詳細資訊，請參閱文章<a href="../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md" class="MCXref xref">篩選和條件修飾詞</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>報表 </td> 
   <td>檢視、篩選和（有時）分組的組合。 報告的目的是跨介面一致地顯示資料、分發資訊，並免除定期執行相同搜尋或查詢的需求。</td> 
  </tr> 
  <tr> 
   <td>陳述式</td> 
   <td>由數個運算式組成，這些運算式可一起定義使用文字模式時報表中顯示的資訊。 可為報表中的檢視、篩選、分組或自訂提示建立陳述式。</td> 
  </tr> 
  <tr> 
   <td>摘要</td> 
   <td>這是您儲存報告後報告的其中一個標籤。 只有當您為報表定義分組時，才會建立此標籤。 它會根據報告建立期間定義的群組摘要資訊，並提供報告彙總物件的快速概觀。 它不會顯示報表中的所有物件，只會顯示彙總的物件。</td> 
  </tr> 
  <tr> 
   <td>文字模式介面</td> 
   <td>提供建立或修改原始透過產生器介面建立之自訂檢視、篩選器、群組和提示的程式碼的功能。 建議一開始透過產生器介面建立報表元素，然後在儲存後轉換為文字模式，以簡化進階檢視、篩選器、群組或提示的編碼。</td> 
  </tr> 
  <tr> 
   <td>使用者介面(UI)</td> 
   <td>指在任何指定時間顯示在使用者熒幕上的元件或建置區塊。</td> 
  </tr> 
  <tr> 
   <td>檢視（或欄）</td> 
   <td>報表的主要元素之一。 它可識別將顯示在報告清單中的欄標題。</td> 
  </tr> 
 </tbody> 
</table>
