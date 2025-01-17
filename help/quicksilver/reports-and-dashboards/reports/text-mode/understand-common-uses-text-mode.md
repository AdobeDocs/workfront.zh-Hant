---
product-area: reporting
navigation-topic: text-mode-reporting
title: 文字模式的常見用途概觀
description: 文字模式的常見用途概觀
author: Nolan
feature: Reports and Dashboards
exl-id: 81512837-1ec4-4dbc-ace4-bdf08fe667ce
source-git-commit: 9caac488522d2a12d3bdf4bf23ba7e44c6dbf7d2
workflow-type: tm+mt
source-wordcount: '762'
ht-degree: 0%

---

# 文字模式的常見用途概觀

<!-- Audited: 1/2025 -->

<!--(NOTE: Alina: ***This is linked to Understanding Text Mode (article), and the TOC article for examples of various reporting elements)</p>-->

您可以在報表與報表元素中使用文字模式，藉此擴展您的報表功能。 您也可以使用某個版本的文字模式，以建置更複雜的計算自訂欄位。 如需文字模式的詳細資訊，請參閱[文字模式概觀](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md)。

本文僅概述幾個常見範例，說明在Adobe Workfront中極可能需要使用文字模式來擴展報表或計算自訂欄位功能的位置。 如需更詳細的範例清單，請參閱：

* [自訂檢視、篩選和群組範例：發行項索引](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md)
* [報表中計算的自訂資料](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-custom-data-reports.md)

如需使用文字模式建立報表的詳細資訊，包括類別、影片和教學課程，請參閱Adobe Experience League網站上的「瞭解」一節。

## 您可能在清單和報告中使用文字模式的例項

建議您使用Report和List Builder來建置檢視、篩選器和群組。 不過，在某些情況下，您可以使用文字模式來增強報表和清單。

當您想要在Workfront中達成下列目標時，可以使用文字模式：

* 在自訂表單中建立自訂計算自訂欄位。\
  如需有關計算自訂欄位的詳細資訊，請參閱本文中的[在計算自訂欄位中使用文字模式](#use-text-mode-in-calculated-custom-fields)區段。
* 增強超出Report Builder可能的篩選器、檢視和群組。 如需有關使用文字模式進行篩選、檢視和分組的資訊，請參閱本文中的下列章節：

   * [在檢視中使用文字模式](#use-text-mode-in-views)
   * [在篩選中使用文字模式](#use-text-mode-in-filters)
   * [在分組中使用文字模式](#use-text-mode-in-groupings)

* 建立自訂提示。 您只能使用文字模式建立自訂提示。

  如需建立自訂提示的相關資訊，請參閱[新增提示至報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)。

## 在計算自訂欄位中使用文字模式 {#use-text-mode-in-calculated-custom-fields}

您可以使用文字模式將計算的自訂欄位新增到自訂表單。

如需將計算自訂欄位新增至自訂表單的詳細資訊，請參閱[建立自訂表單](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)。

如需以文字模式建立計算自訂欄位的詳細資訊，請參閱[將計算欄位新增至表單](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md)。

例如，您可以新增計算自訂欄位，顯示專案標示為進行中時的時間和日期戳記。 您可以將此計算用於其他狀態。

如需詳細資訊，請參閱[計算自訂欄位範例：在自訂表單中顯示[狀態]時間戳記](../../../reports-and-dashboards/reports/calc-cstm-data-reports/example-status-timestamp-in-calculated-field.md)。

## 在檢視中使用文字模式 {#use-text-mode-in-views}

您可以在檢視中使用文字模式，展開您可以在檢視中顯示的欄位和物件。

如需在檢視中使用文字模式的最常見原因範例，請參閱下列文章：

* [檢視：顯示未包含在標準介面中的物件](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-display-objects-not-in-standard-interface.md)
* [檢視：顯示資料行](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-calculation-between-two-fields.md)中兩個欄位之間的計算結果
* [檢視：永久編輯資料行的寬度](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-edit-column-width-permanently.md)
* [檢視：合併一個共用資料行中多個資料行的資訊](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-merge-columns.md)
* [檢視：移除資料行](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-remove-link-to-object.md)中物件的連結
* [報表中的參考集合](../../../reports-and-dashboards/reports/text-mode/reference-collections-report.md)
* [檢視：隱藏資料行的內容](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-hide-column-content.md)
* [檢視：在欄中顯示影像，而非字串](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-display-image-in-view.md)
* [檢視：在任務清單中顯示任務縮排](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-display-task-identations.md)
* [檢視：計算時間和日期差異](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-calculate-time-and-date-differences.md)

## 在篩選中使用文字模式 {#use-text-mode-in-filters}

當您建立篩選時，可以使用文字模式來展開可依其篩選的欄位和物件。

如需在篩選中使用文字模式的最常見原因範例，請參閱下列文章：

* [篩選器：建立參考相同欄位（「AND」陳述式）的多個篩選器規則](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/filter-refrence-the-same-field-multiple-times.md)
* [篩選器：僅顯示核准狀態的專案](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/filter-for-items-in-approval-status.md)
* [篩選器：當狀態與不同群組相關聯時，依相同名稱狀態顯示專案](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/filter-same-name-statuses-from-different-groups.md)
* [篩選器：比較兩個欄位來排除清單中的專案](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/filter-items-by-comparing-two-fields.md)
* 在發行項[使用EXISTS陳述式建立複雜文字模式篩選器](../../../reports-and-dashboards/reports/text-mode/create-complex-text-mode-filters-using-exists-statements.md)中，橫跨物件階層](../../../reports-and-dashboards/reports/text-mode/create-complex-text-mode-filters-using-exists-statements.md#examples)多個層級的文字模式篩選器範例[
* 區段[為發行項[使用EXISTS陳述式建立複雜文字模式篩選器](../../../reports-and-dashboards/reports/text-mode/create-complex-text-mode-filters-using-exists-statements.md)中的遺失物件建立複雜文字模式篩選器](../../../reports-and-dashboards/reports/text-mode/create-complex-text-mode-filters-using-exists-statements.md#missing-object-filters)

## 在分組中使用文字模式 {#use-text-mode-in-groupings}

建立群組時，您可以使用文字模式來展開您可在清單和報告中作為群組依據的欄位和物件。

如需在群組中使用文字模式最常見原因的範例，請參閱下列文章：

* [群組：依照群組中所有物件通用的計算值來組織清單結果](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/grouping-by-calculated-common-values.md)
* [群組：新增第四個群組至清單](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/grouping-add-fourth-grouping.md)
* [群組：編輯群組中的顯示名稱](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/grouping-rename-grouping.md)
* [群組：指出群組結果應使用文字模式收合或展開](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/grouping-collapsed-or-expanded-results.md)
