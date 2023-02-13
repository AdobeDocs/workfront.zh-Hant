---
product-area: reporting
navigation-topic: create-and-manage-reports
title: 建立自訂報表
description: 了解如何建立報表，有助於您存取貴組織在Adobe Workfront中需要的資訊。 您可以使用Workfront中提供的任何內建報表，或從頭開始建立您自己的報表。
author: Nolan
feature: Reports and Dashboards
exl-id: 10c4df37-f09f-4b91-9cfd-3d0c3835bc7b
source-git-commit: 61fcb4c3646f60fa5f667d874af3320360d5d286
workflow-type: tm+mt
source-wordcount: '1821'
ht-degree: 1%

---


# 建立自訂報表

了解如何建立報表，有助於您存取貴組織在Adobe Workfront中需要的資訊。 您可以使用Workfront中提供的任何內建報表，或從頭開始建立您自己的報表。

如需內建報表的詳細資訊，請參閱 [使用Adobe Workfront內建報表](../../../reports-and-dashboards/reports/using-built-in-reports/use-workfront-built-in-reports.md). 如需複製報表以建立報表的相關資訊，請參閱 [建立報表副本](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>計劃 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>編輯對報表、控制面板、日曆的存取</p> <p>編輯對篩選器、檢視、群組的存取</p> <p>注意：如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>您將取得您所建立報表的管理權限</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 建立報表 {#create-a-report}

若要觀看如何建立報表的影片，請參閱此 [建立自訂報表](#Walk-thr) 下方。

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在右上角，按一下 **報表**.
1. 按一下 **新增報表**，然後選取您要用於報表的物件類型。

   報告建立工具會載入。

   如需可用物件報表的特定資訊，請參閱區段 [對象報告](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#reporting-on-objects) 在文章中 [了解Adobe Workfront中的物件](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

   ![](assets/nwe-select-new-report-350x666.png)

   >[!TIP]
   >
   >您也可以複製現有報表，以建立報表。 如需詳細資訊，請參閱 [建立報表副本](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).

1. 在報告建立工具中，將下列項目新增至您的報告：

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
      <td> <p>將欄新增至報表，可決定報表包含的資訊。</p> <p>若要了解如何新增欄，請參閱 <a href="#add-columns-view-to-a-report" class="MCXref xref">新增欄（檢視）至報表</a>.<br></p> </td> 
     </tr> 
     <tr> 
      <td>群組</td> 
      <td> <p>將群組新增至報表可決定報表的組織方式。</p> <p>若要了解如何新增群組，請參閱 <a href="#add-groupings-to-a-report" class="MCXref xref">新增分組至報表</a>.</p> </td> 
     </tr> 
     <tr> 
      <td>篩選器</td> 
      <td> <p>將篩選規則新增至報表，可決定您在報表中看到的資訊。</p> <p>若要了解如何新增篩選器，請參閱 <a href="#add-filters-to-a-report" class="MCXref xref">新增篩選器至報表</a>.</p> </td> 
     </tr> 
     <tr> 
      <td>圖表</td> 
      <td> <p>將圖表新增至報表，可決定以視覺化方式呈現報表中的資訊。</p> <p>若要了解如何新增圖表，請參閱 <a href="#add-a-chart-to-a-report" class="MCXref xref">新增圖表至報表</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 在報表建立程式期間的任何時間點，按一下 **套用** 來儲存變更。
1. 完成後，按一下 **儲存+關閉**.

### 新增欄（檢視）至報表 {#add-columns-view-to-a-report}

1. 如 [建立報表](#create-a-report) 一節。
1. 在報告建立工具中，選取 **欄（檢視）** 標籤，以識別要在報表中顯示的欄。
1. （選用）按一下 **應用現有視圖** 來使用現有視圖。

   如需建立新檢視的詳細資訊，請參閱 [Adobe Workfront中的檢視概觀](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. 若要新增欄，請按一下 **添加列**.

   或

   若要變更現有欄，請選取您要變更的欄，然後按一下目前名稱旁的(x)。

1. 開始輸入要添加的欄位。 如果欄位可用，則會填入每個物件的關聯位置。 按一下欄位名稱，將其新增至欄。

   如需您在欄中看到欄位的詳細資訊，請參閱 [Adobe Workfront術語表](../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

   ![](assets/nwe-add-column-typeahead-350x459.png)

1. （選用）在 **欄設定** 區域，選擇 **按此列排序** 要按降序字母順序遞增排序列中的值，請指明清單是否應將此列作為第一個排序。

   如果要先依一欄中的值排序，接著依第二欄中的值排序，報表檢視中可以有多個排序層級。

   如果多個結果根據第一個排序標準相同，則它們會按照第二個排序標準的順序排序。 如果多個結果根據第一和第二排序標準相同，則它們根據第三個排序等進行排序。

   >[!NOTE]
   >
   >如果添加的欄位引用的對象與要報告的對象相距太遠，則可能無法按此欄位排序。\
   >例如，問題報告無法按「項目所有者」欄位排序，因為它引用了3個附加對象：專案、擁有者和名稱。 不過，您仍可將此欄位新增至問題報表，並查看其相關資訊。\
   >若要進一步了解報表中的跨物件參考，請參閱 [報表和控制面板學習路徑](https://one.workfront.com/s/learningpath2/workfront-reporting-MC7MZT2BOL2ZC2LMJ4MA3EMHOCNY?tabset-dc70e=2).

1. （選用）如果您使用分組，且想要匯總（匯總）欄中的資訊，請按一下 **匯總此欄，依** 下拉式清單 **欄設定** 區域，然後選取要用來匯總列中資訊的選項。

   匯總的資訊顯示在分組行的列中。

   ![分組匯總摘要](assets/aggregate-summary-displays-on-groupings-2022-350x195.png)

   如需匯總欄中資料的詳細資訊，請參閱 [Adobe Workfront中的檢視概觀](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

   >[!NOTE]
   >
   >在按分組方式聚合以下欄位的值時，父對象（例如父任務）適用以下例外：
   >
   >* 除「實際小時數」（例如，「計畫/實際人工成本」、「計畫/實際費用成本」、「計畫/實際成本」、「計畫小時數」）之外，所有數字和幣種欄位僅匯總子任務和獨立任務的值。 它們不會匯總父任務或父項的父項的值。
   >* 「實際小時數」匯總主要父任務和獨立任務的值；它們不會匯總父任務或子任務的父任務的數量。
   >* 數字和貨幣值的自訂資料欄位會匯總所有任務：父母、子女、父母和獨立任務。


   如需在報表中使用分組的詳細資訊，請參閱 [Adobe Workfront中的群組概觀](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. （選用）按一下 **進階選項** 指定列的以下資訊：

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
      <td> <p>選擇您希望欄中欄位的值顯示的格式。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">在報告面板上顯示此欄</td> 
      <td> <p>選取此選項，當報告與其他報告並排顯示時，即可在控制面板上顯示此欄。 取消選取此選項時，在並排顯示報表的控制面板上檢視報表時，不會顯示此欄。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">欄規則</td> 
      <td> <p>按一下 <strong>為此欄新增規則</strong> 向列添加條件式格式。 新增規則後，您可以定義欄位和文字樣式，以顯示符合該規則的欄位。 按一下 <strong>新增規則</strong> 完成規則的定義後。 如需檢視中條件式格式的詳細資訊，請參閱 <a href="../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md" class="MCXref xref">在檢視中使用條件式格式</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下 **套用** 若要套用您目前所做的變更，並繼續編輯報表，請使用下列選項。

   按一下 **儲存+關閉** 如果您已完成編輯報表中的欄，且想要儲存報表。

### 新增分組至報表 {#add-groupings-to-a-report}

1. 如 [建立報表](#create-a-report) 一節。
1. 在報告建立工具中，選取 **分組** 標籤來識別要如何將報表中的項目分組。
1. 按一下 **添加分組** 來新增群組。

   或

   選擇 **應用現有分組** 要選擇現有分組
   ![](assets/nwe-add-grouping-350x230.png)

1. 開始鍵入要作為分組添加的欄位。 如果欄位可用，則會填入每個物件的關聯位置。 按一下欄位名稱，將其新增至該群組。
1. （選用）您可以按一下「 」，以文字模式選擇建立分組 **切換到文本模式**. 如需使用文字模式的詳細資訊，請參閱 [文字模式概觀](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

   如需建立新群組的詳細資訊，請參閱 [Adobe Workfront中的群組概觀](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. （選用）選取 **預設折疊此分組** 如果希望此分組中的結果顯示為已折疊而不是展開。

   預設會停用此設定，且群組的結果一律會顯示在展開清單中。

   >[!TIP]
   >
   >* 當您在檢視清單時手動調整分組時，Workfront會記住您的手動偏好設定，直到您登出為止。 當您重新登入時，清單會根據此設定顯示。
   >* 從圖表元素存取群組後，其結果一律會顯示為已展開。


1. （可選）您可以選擇建立矩陣分組，以網格格式顯示結果。

   如需建立矩陣報表的詳細資訊，請參閱 [建立矩陣報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md).

1. 按一下 **套用** 若要套用您目前所做的變更，並繼續編輯報表，請使用下列選項。

   按一下 **儲存+關閉** 如果您已完成編輯報表中的群組，且想要儲存報表。

### 新增篩選器至報表 {#add-filters-to-a-report}

1. 如 [建立報表](#create-a-report) 一節。
1. 在報告建立工具中，選取 **篩選器** 標籤，以識別您要報表包含的資訊量。
1. 按一下 **新增篩選規則** 新增自訂篩選器。\
   或\
   選擇 **套用現有篩選** 來使用現有篩選器。

   ![](assets/nwe-add-a-filter-350x93.png)

1. 如果您按一下 **新增篩選規則**，開始輸入您要新增為篩選器的欄位。 如果欄位可用，則會填入每個物件的關聯位置。 按一下欄位名稱，將其新增至該篩選器。\
   使用篩選修飾元來建置篩選器。 如需篩選修飾元的詳細資訊，請參閱 [篩選條件修飾元](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

   如需建立新篩選器的詳細資訊，請參閱 [Adobe Workfront中的篩選器概觀](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. （選用）您可以按一下「 」，選擇在文字模式中建立篩選器 **切換到文本模式**.

   如需使用文字模式的詳細資訊，請參閱 [文字模式概觀](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

1. 按一下 **套用** 完成編輯報表中的篩選器以套用目前為止的變更後，請使用下列選項繼續編輯報表。

   按一下 **儲存+關閉** 報表而您想儲存報表時，才會顯示此變數。

### 新增圖表至報表 {#add-a-chart-to-a-report}

1. 如 [建立報表](#create-a-report) 一節。
1. 在報告建立工具中，選取 **圖表** 頁簽，然後選擇要添加的圖表類型。

   ![](assets/nwe-add-a-chart-350x247.png)

   如需在報表中建立圖表的詳細資訊，請參閱 [新增圖表至報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

1. 按一下 **套用** 若要套用您目前所做的變更，並繼續編輯報表，請使用下列選項。

   按一下 **儲存+關閉** 如果您已完成報表的編輯，且想要儲存報表。
