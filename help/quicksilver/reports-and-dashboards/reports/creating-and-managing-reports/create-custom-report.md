---
product-area: reporting
navigation-topic: create-and-manage-reports
title: 建立自訂報表
description: 您可以透過建立報告，提供貴組織在Adobe Workfront中所需資訊的存取權。 您可以使用Workfront中提供的任何內建報表，或從頭開始建立自訂報表。
author: Nolan
feature: Reports and Dashboards
exl-id: 10c4df37-f09f-4b91-9cfd-3d0c3835bc7b
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '1816'
ht-degree: 1%

---


# 建立自訂報表

<!--Audited: 10/2024-->

您可以透過建立報告，提供貴組織在Adobe Workfront中所需資訊的存取權。 您可以使用Workfront中提供的任何內建報表，或從頭開始建立自訂報表。

如需內建報表的詳細資訊，請參閱[使用Adobe Workfront內建報表](../../../reports-and-dashboards/reports/using-built-in-reports/use-workfront-built-in-reports.md)。

如需有關複製報表以建立報表的資訊，請參閱[建立報表復本](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md)。

如需建立和管理報告的詳細資訊，包括課程、影片和教學課程，請參閱Adobe Experience League網站上的「學習」一節。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront套件</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td> 
      <p>標準</p>
      <p>規劃</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>編輯報告、儀表板、行事曆的存取權</p> <p>編輯對篩選器、檢視、群組的存取權</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>您取得所建立報表的管理許可權</p>  </td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 建立報告 {#create-a-report}

{{step1-to-reports}}

1. 按一下&#x200B;**新增報表**，然後選取您要用於報表的物件型別。

   Report Builder隨即載入。

   如需有關可用物件報表的特定資訊，請參閱文章[瞭解Adobe Workfront中的物件](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#reporting-on-objects)中的[物件報表](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md)一節。

   ![選取新報告](assets/nwe-select-new-report-350x666.png)

   >[!TIP]
   >
   >您也可以製作現有報表的副本，以建立報表。 如需詳細資訊，請參閱[建立報告復本](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md)。

1. （可選）若要編輯新報告的標題，請在Report Builder左上角的文字欄位中輸入所需的報告標題。 我們建議僅使用UTF-8字元以避免相容性問題。

1. 在Report Builder中，將下列專案新增至報表：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>功能</th> 
      <th>說明</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td>欄（檢視）</td> 
      <td> <p>在報表中新增欄可決定報表所包含的資訊。</p> <p>若要瞭解如何新增欄，請參閱<a href="#add-columns-view-to-a-report" class="MCXref xref">新增欄（檢視）至報表</a>。<br></p> </td> 
     </tr> 
     <tr> 
      <td>群組</td> 
      <td> <p>在報表中新增群組，會決定報表的整理方式。</p> <p>若要瞭解如何新增群組，請參閱<a href="#add-groupings-to-a-report" class="MCXref xref">新增群組至報表</a>。</p> </td> 
     </tr> 
     <tr> 
      <td>篩選器</td> 
      <td> <p>將篩選規則新增至報表可決定您在報表中看到的資訊。</p> <p>若要瞭解如何新增篩選器，請參閱<a href="#add-filters-to-a-report" class="MCXref xref">新增篩選器至報表</a>。</p> </td> 
     </tr> 
     <tr> 
      <td>圖表</td> 
      <td> <p>將圖表新增至報表，可決定如何以視覺化方式呈現報表中的資訊。</p> <p>若要瞭解如何新增圖表，請參閱<a href="#add-a-chart-to-a-report" class="MCXref xref">新增圖表至報表</a>。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 在建立報告過程中，隨時按一下&#x200B;**套用**&#x200B;以儲存變更。
1. 完成之後，按一下&#x200B;**儲存+關閉**。

### 新增欄（檢視）至報表 {#add-columns-view-to-a-report}

1. 開始建立報告，如本文的[建立報告](#create-a-report)一節中所述。
1. 在Report Builder中，選取&#x200B;**欄（檢視）**&#x200B;索引標籤以識別要顯示在報表中的欄。
1. （選擇性）按一下&#x200B;**套用現有檢視**，然後在下拉式功能表中按一下檢視名稱，以使用現有檢視。

   如需建立檢視的詳細資訊，請參閱[在Adobe Workfront中的檢視總覽](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)。

1. （選擇性）若要移除現有的欄，請按一下您要移除的欄，然後按一下欄標題中目前名稱旁的&#x200B;**x**。

1. 若要新增欄，請按一下[新增欄]。****

   或

   若要變更現有欄，請按一下該欄，在Report Builder左上角的&#x200B;**顯示在此欄位欄位**&#x200B;區域中，按一下目前欄位右側的![移除](assets/remove-column-icon.png)圖示&#x200B;**移除欄點陣圖示**，然後開始輸入新欄位，然後在欄位顯示在清單中時按一下它。

   如需有關您在欄中看到的欄位詳細資訊，請參閱[Adobe Workfront術語辭彙表](../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md)。

   ![新增欄自動提示](assets/nwe-add-column-typeahead-350x459.png)

1. （選擇性）在&#x200B;**資料行設定**&#x200B;區域中，選取&#x200B;**依此資料行排序**&#x200B;以遞增字母順序來排序資料行中的值，然後指示清單是否應使用此資料行作為第一個排序。

   如果您想要先依一欄中的值排序，接著依第二欄中的值排序，則可以在報表檢視中進行多個層級的排序，依此類推。

   如果根據第一個排序標準有多個結果相同，則會依第二個排序標準的順序排序。 如果根據第一和第二排序標準有多個結果相同，則會根據第三排序標準排序等。

   >[!NOTE]
   >
   >如果您新增的欄位所參照的物件與您報告的物件距離太遠，您可能無法依此欄位排序。\
   >例如，問題報告無法依專案所有者欄位排序，因為它參考了3個額外的物件：專案、所有者和名稱。 不過，您仍可將此欄位新增至問題報告，並檢視相關資訊。

   <!--outdated: To learn more about cross-object references in reports, see the section "Advanced Reporting Part 1 of 3" in the [Reports and Dashboards Learning Path](https://one.workfront.com/s/learningpath2/workfront-reporting-MC7MZT2BOL2ZC2LMJ4MA3EMHOCNY?tabset-dc70e=2).-->

1. （選擇性）如果您使用群組，而且想要彙總（彙總）欄中的資訊，請按一下&#x200B;**欄設定**&#x200B;區域中的&#x200B;**彙總此欄**&#x200B;下拉式清單，然後選取您要用來彙總欄中資訊的選項。

   彙總資訊會顯示在群組列的欄中。

   ![群組的彙總摘要](assets/aggregate-summary-displays-on-groupings-2022-350x195.png)

   如需彙總資料行資料的詳細資訊，請參閱Adobe Workfront中的[檢視總覽](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)。

   >[!NOTE]
   >
   >當您彙總分組中下列欄位的值時，下列例外情況適用於父系物件（例如父系任務）：
   >
   >* 除「實際時數」（例如「計畫或實際勞力成本」、「計畫或實際費用成本」、「計畫或實際成本」、「計畫時數」）之外的所有數字與幣別欄位，只會彙總子任務與獨立任務的值。 它們不會彙總父系任務的值或父系父系的值。
   >* 實際小時彙總主要父系和獨立任務的值；它們不會彙總父系任務的父系或子系任務的數量。
   >* 數字和貨幣值的自訂資料欄位會彙總所有工作：父項、子項、父項的父項以及獨立工作。

   如需在報表中使用群組的詳細資訊，請參閱Adobe Workfront中的[群組概觀](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)。

1. （選擇性）按一下&#x200B;**進階選項**，為資料行指定下列資訊：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">自訂欄標籤</td> 
      <td> <p>指定欄的自訂標籤。 此標籤會取代預設標籤。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">欄位格式</td> 
      <td> <p>選取您要為欄中的欄位顯示值的格式。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">在報告面板上顯示此欄</td> 
      <td> <p>當報告與其他報告並排顯示時，選取此選項可在控制面板上顯示此欄。 取消選取此選項時，在報告並排顯示的儀表板上檢視報告時不會顯示此欄。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">欄規則</td> 
      <td> <p>按一下<strong>新增此資料行的規則</strong>以新增條件式格式至資料行。 新增規則後，您可以定義欄位和文字樣式，以顯示符合該規則的欄位。 完成規則定義後，按一下<strong>新增規則</strong>。 如需檢視中條件式格式的詳細資訊，請參閱<a href="../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md" class="MCXref xref">在檢視中使用條件式格式</a>。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下&#x200B;**套用**&#x200B;以套用您目前的變更，並使用下列選項繼續編輯報告。

   如果您已完成編輯報表中的欄，而且想要儲存報表，請按一下[儲存+關閉]。****

### 新增群組至報表 {#add-groupings-to-a-report}

1. 開始建立報告，如本文的[建立報告](#create-a-report)一節中所述。
1. 在Report Builder中，選取&#x200B;**群組**&#x200B;索引標籤以識別您要將報表中的專案群組化的方式。
1. 按一下&#x200B;**新增群組**&#x200B;以新增群組。

   或

   選擇&#x200B;**套用現有群組**&#x200B;以選取清單中顯示的現有群組。

   ![新增群組](assets/nwe-add-grouping-350x230.png)

1. 開始輸入您要新增為群組的欄位。 如果欄位可供使用，則會針對可與其關聯的每個物件填入欄位。 按一下欄位名稱以將其新增到該群組。
1. （選擇性）您可以按一下&#x200B;**切換至文字模式**，選擇在文字模式中建立群組。 如需有關使用文字模式的詳細資訊，請參閱[文字模式概觀](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md)。

   如需建立新群組的詳細資訊，請參閱Adobe Workfront中的[群組概觀](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)。

1. （選擇性）如果您想要此群組中的結果顯示摺疊而非展開，請依預設選取&#x200B;**摺疊此群組**。

   此設定預設為停用，群組結果一律顯示在展開清單中。

   >[!TIP]
   >
   >* 當您在檢視清單時手動調整群組，Workfront會記住您的手動偏好設定，直到您登出為止。 當您重新登入時，清單會根據此設定顯示。
   >* 從圖表元素存取群組結果後，群組結果一律展開顯示。

1. （選擇性）按一下&#x200B;**切換至矩陣群組**，以建立矩陣群組並以格線格式顯示您的結果。

   如需建立矩陣報表的詳細資訊，請參閱[建立矩陣報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md)。

1. 按一下&#x200B;**套用**&#x200B;以套用您目前的變更，並使用下列選項繼續編輯報告。

   如果您已完成編輯報表中的群組且想要儲存報表，請按一下&#x200B;**儲存+關閉**。

### 新增篩選器至報表 {#add-filters-to-a-report}

1. 開始建立報告，如本文的[建立報告](#create-a-report)一節中所述。
1. 在Report Builder中，選取&#x200B;**篩選器**&#x200B;索引標籤，以識別您要納入報表的資訊量。
1. 按一下&#x200B;**新增篩選器規則**&#x200B;以新增自訂篩選器。\
   或\
   選擇&#x200B;**套用現有的篩選器**&#x200B;以使用現有的篩選器。

   ![新增篩選器](assets/nwe-add-a-filter-350x93.png)

1. 如果您按一下&#x200B;**新增篩選規則**，請開始輸入您要新增為篩選的欄位。 如果欄位可供使用，則會針對可與其關聯的每個物件填入欄位。 按一下欄位名稱以將其新增至該篩選器。\
   使用篩選器修飾元來建置您的篩選器。 如需篩選修飾元的詳細資訊，請參閱[篩選和條件修飾元](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md)。

   如需建立新篩選的詳細資訊，請參閱[篩選總覽](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)。

1. （選擇性）您可以按一下&#x200B;**切換至文字模式**，選擇在文字模式中建立篩選器。

   如需有關使用文字模式的詳細資訊，請參閱[文字模式概觀](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md)。

1. 當您完成編輯報表中的篩選器時，請按一下&#x200B;**套用**&#x200B;以套用您到目前為止的變更，並使用下列選項繼續編輯報表。

   如果報表且您想要儲存報表，請按一下&#x200B;**儲存+關閉**。

### 新增圖表至報表 {#add-a-chart-to-a-report}

1. 開始建立報告，如本文的[建立報告](#create-a-report)一節中所述。
1. 在Report Builder中，選取&#x200B;**圖表**&#x200B;標籤，然後選取您要新增的圖表型別。

   ![新增圖表](assets/nwe-add-a-chart-350x247.png)

   如需在報告中建立圖表的詳細資訊，請參閱[將圖表新增至報告](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md)。

1. 按一下&#x200B;**套用**&#x200B;以套用您目前的變更，並使用下列選項繼續編輯報告。

   如果您已完成編輯報告並想要儲存報告，請按一下[儲存+關閉]。****
