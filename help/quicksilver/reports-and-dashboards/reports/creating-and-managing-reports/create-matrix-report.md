---
product-area: reporting
navigation-topic: create-and-manage-reports
title: 建立矩陣報告
description: 矩陣報表會以彙總表格格式呈現摘要資訊，因此相較於傳統報表中的清單，更容易檢視。
author: Nolan
feature: Reports and Dashboards
exl-id: 714f2802-089f-4a41-8205-f397cf474a24
source-git-commit: 12e8bc389c42510b5adbb0190eb71c9f6a9f52a7
workflow-type: tm+mt
source-wordcount: '1075'
ht-degree: 0%

---

# 建立矩陣報告

矩陣報表會以彙總表格格式呈現摘要資訊，因此相較於傳統報表中的清單，更容易檢視。

## 何時使用矩陣報表

您可以為包含2個或多個群組的任何報表建立矩陣報表。 傳統報表最多可包含3個群組，而矩陣報表最多可包含4個群組。

例如，您想要建立顯示3個月期間所記錄時數的小時報告，且想要根據輸入時數的人以及按月和按周來組織報告。

![](assets/report-matrix-overview-350x123.png)

## 資料在矩陣報表中的顯示方式

矩陣報表中的資訊一律會顯示為數值。 在大多數情況下，包含數值的欄最適合在矩陣報表中顯示（例如記錄時數與實際成本）。

不過，其他欄（例如「狀態」）仍可顯示在矩陣報表中，如下圖所示：\
![](assets/report-matrix-status-350x73.png)

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具有下列存取權才能執行本文中的步驟：

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
      <td> 
      <p>新增：</p>
         <ul>
         <li><p>標準</p></li>
         </ul>
      <p>目前：</p>
         <ul>
         <li><p>規劃</p></li>
         </ul>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td><p>編輯報告、儀表板、行事曆的存取權</p> <p>編輯對篩選器、檢視、群組的存取權</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>管理報表的許可權</p></td> 
  </tr> 
 </tbody> 
</table>

*如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 設定矩陣報表

1. 建立傳統報表，在報表輸出中包含數值資料。\
   如需有關如何建立報告的資訊，請參閱[建立自訂報告](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)。

1. 移至您在步驟1建立的報表，按一下&#x200B;**報表動作**，然後選取&#x200B;**編輯**。

1. （視條件而定）如果您已建立檢視，且要將其套用至此報表，請按一下&#x200B;**套用現有檢視**，然後從下拉式清單中選取檢視。
1. （視條件而定）如果要為報表建立新的檢視，請完成下列步驟：

   1. 按一下&#x200B;**欄（檢視）**&#x200B;標籤，然後選取要在矩陣報表中摘要的欄。
   1. 在&#x200B;**資料行設定**&#x200B;區域中，按一下&#x200B;**摘要此資料行**&#x200B;下拉式清單，然後選取其中一個可用選項來摘要資訊。

      >[!IMPORTANT]
      >
      >如果未選取此選項，則矩陣報表中無法正確顯示欄中的資訊。

      ![](assets/qs-report-matrix-summarized-350x392.png)

   1. 對[欄（檢視）]索引標籤中的每個欄重複此程式，然後按一下[完成]。****

1. 按一下&#x200B;**群組**&#x200B;標籤。
1. （視條件而定）如果您已建立群組，且想要將其套用至此報表，請按一下&#x200B;**套用現有群組**，然後從下拉式清單中選取群組。
1. （視條件而定）如果要為報表建立新的矩陣群組，請完成下列步驟：

   1. 選取產生器介面右上角的&#x200B;**切換至矩陣群組**。
   1. 在&#x200B;**列群組**&#x200B;區段中，識別建立表格水準群組的列群組。
   1. （選擇性）若要新增其他列群組，請按一下[新增次要列群組]。****
   1. 在&#x200B;**欄群組**&#x200B;區段中，識別建立資料表垂直群組的欄群組。
   1. （選擇性）若要新增其他欄群組，請按一下&#x200B;**新增次要欄群組**。
   1. （視條件而定）如果您依日期新增分組，也請指定結果是否依日、周、月、季或年分組。\
      ![](assets/qs-grouping-by-date-options-for-matrix-report-350x450.png)

   1. （視條件而定）如果您選取依日期分組及依季度顯示結果，例如，請選取&#x200B;**顯示沒有結果的季度**&#x200B;核取方塊，以指定是否要顯示沒有資料的季度。\
      ![](assets/qs-show-quarters-with-no-results-on-matrix-report-350x175.png)

      >[!NOTE]
      >
      >**沒有結果的顯示季度**&#x200B;欄位僅適用於矩陣群組，不適用於標準群組。\
      >只有位於具有有效資料的兩個季度之間的季度沒有資料，才會在Matrix標籤中的資料值顯示零。 位於篩選器選取之時間範圍開始和結束且沒有資料的季度，完全不會出現在矩陣群組中。 沒有結果的季度將不會顯示在報告之詳細資訊索引標籤上的分組中。

1. （選擇性和條件性）按一下&#x200B;**矩陣設定**，然後從下列選項中選取：\
   **顯示記錄計數：**&#x200B;選取此選項可顯示包含指定欄位之專案總數的列。\
   **顯示值資料行：**&#x200B;選取此選項可在矩陣中顯示下列資訊：

   * 記錄計數
   * 值欄

     >[!NOTE]
     >
     >此欄包含說明每一列資料代表的資訊。\
     >當您彙總分組中下列欄位的值時，下列例外情況適用於父系物件（例如父系任務）：
     >
     >   
     >   
     >   * 除「實際時數」（例如「計畫/實際勞力成本」、「計畫/實際費用成本」、「計畫/實際成本」、「計畫時數」）之外的所有數字與幣別欄位，只會彙總子任務與獨立任務的值。 它們不會彙總父系任務的值或父系父系的值。
     >   * 實際小時彙總主要父系和獨立任務的值；它們不會彙總父系任務的父系或子系任務的數量。
     >   * 數字和貨幣值的自訂資料欄位會彙總所有工作：父項、子項、父項的父項以及獨立工作。 如果您建立了矩陣報表，以在&#x200B;**值**&#x200B;欄中顯示計畫時數或實際時數，請注意，任何父物件（例如父系工作）的時數或成本資訊都不會顯示在矩陣報表中。 若要檢視父物件的時數，您必須檢視&#x200B;**詳細資料**&#x200B;標籤。
     >   
     >   
     >

   **條件規則：**&#x200B;請為彙總的值設定任何格式規則。\
   新增規則後，您可以定義欄位和文字樣式，以顯示符合該規則的欄位。 完成規則定義後，按一下&#x200B;**[新增規則]**，然後按一下&#x200B;**[完成]**&#x200B;以儲存規則。

1. 按一下&#x200B;**篩選器**&#x200B;索引標籤，以定義將在報告中顯示的資訊。
1. （視條件而定）如果您已建立篩選器，且想要將其套用至此報表，請按一下&#x200B;**套用現有篩選器**，然後從下拉式清單中選取篩選器。
1. （視條件而定）如果要為此報告建立新的篩選器，請參閱[篩選和條件修飾元](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md)

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   and
   <a href="../../../reports-and-dashboards/reports/reporting-elements/advanced-filter-condition-qualifiers.md" class="MCXref xref">Advanced Filter and condition qualifiers </a>
   </MadCap:conditionalText>
   -->

   瞭解建立篩選器時可使用的各種限定詞的相關資訊。

1. 按一下&#x200B;**儲存+關閉**&#x200B;以儲存並檢視矩陣報告。
