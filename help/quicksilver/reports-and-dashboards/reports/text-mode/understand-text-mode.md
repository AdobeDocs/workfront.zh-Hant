---
product-area: reporting
navigation-topic: text-mode-reporting
title: 文字模式概觀
description: 建立構成報告或清單的元素時，您可以使用標準或文字模式介面，在Adobe Workfront中建立報告或清單。
author: Nolan
feature: Reports and Dashboards
exl-id: 8be8cbd0-da1b-4e90-a52e-dc352f646d18
source-git-commit: 9caac488522d2a12d3bdf4bf23ba7e44c6dbf7d2
workflow-type: tm+mt
source-wordcount: '798'
ht-degree: 0%

---

# 文字模式概觀

<!-- Audited: 1/2025 -->

<!--(NOTE: Linked to the UI (for the areas mentioned in the comments below and the new NWE filters as well))-->

<!--(NOTE: Alina: ***Linked to other articles. Do not move, rename or change url.Linked to the product, in the report builder, when using a field that is not recognized in standard mode.)-->

<!--(NOTE: This will be linked to the Ninja feature about adding a filter to the User typeahead field (which originally is open only for text mode filters). Update the Context Sensitive sheet at release time)-->

建立構成報告或清單的元素時，您可以使用標準或文字模式介面，在Adobe Workfront中建立報告或清單。

標準介面可讓您參照在Workfront介面中可立即使用的欄位及其屬性。

使用文字模式，您可以參考在標準模式下可能不可用，但在Workfront資料庫中可用的欄位和屬性。

如需使用文字模式建立報表的詳細資訊，包括類別、影片和教學課程，請參閱Adobe Experience League網站上的「瞭解」一節。

## 使用文字模式之前的考量事項

>[!TIP]
>
>您也可以使用自訂欄位的文字模式版本，以擴充計算自訂欄位的功能。 用於建立計算自訂欄位的語法和規則與您用於報表和清單中的語法和規則不同。 如需新增計算自訂欄位的資訊，請參閱[新增計算欄位至表單](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md)。

* 在報表中開始使用文字模式之前，強烈建議您先參加進階報表課程，以更深入地瞭解我們的文字模式語言。
* 建議您使用標準模式，以確保在Workfront軟體更新時，您建立的報表保持不變。 雖然文字模式可讓您建立更複雜的檢視、篩選器和群組，但維護起來也更為複雜，且不保證會在Workfront軟體更新時進行。
* 建議您一律嘗試在標準介面中建置所有報表元素，並僅在少數調整中切換至文字模式產生器。

  >[!TIP]
  >
  >使用標準產生器會為您提供重要的建置區塊和程式碼模式，讓您隨後在文字模式中修改程式碼時使用這些重要區塊和程式碼模式。

* 為了以文字模式成功建置報表和清單，您必須使用一組規則和唯一語法。 開始之前，請務必熟悉文字模式的Workfront語法。

  如需有關使用文字模式的語法和規則的資訊，請參閱[文字模式語法概述](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md)。

* 在文字模式下自訂報表元素後，您可能無法切換回標準模式（在檢視中），或是您建立之元素的程式碼可能會遭到刪除（在篩選器和群組中）。 這是因為並非所有文字模式支援的欄位都支援標準模式。

## 標準模式介面

「標準模式」介面會顯示欄位，以對應您要在報表或清單中顯示的應用程式元素。 標準模式介面是一組下拉式功能表，您可以從中選擇要在報表或清單中顯示的欄位。

如需有關標準模式介面的詳細資訊，以及瞭解如何建立報告或清單，請參閱：

* [建立自訂報告](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)。
* [報表元素：篩選器、檢視和群組](../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md)

## 文字模式介面

文字模式可讓您使用標準模式介面中無法使用的欄位，來建立更複雜的檢視、篩選器、群組和提示。 在Workfront文字模式中，是編碼陳述式的集合，指出您要在報表或清單中顯示的物件。

如需所有可報告欄位的完整清單，請參閱[API總管](../../../wf-api/general/api-explorer.md)。

>[!NOTE]
>
>並非所有透過API可用的欄位都可透過文字模式介面使用。 如果您在文字模式程式碼中使用正確的欄位，但未顯示預期的結果，則欄位可能只能透過API報告。

## 存取報表元素及編輯文字模式 {#access-reporting-elements-and-edit-text-mode}

從報表或清單存取檢視、群組和篩選器時，存取文字模式介面的方式會類似。

如需有關在檢視、篩選器和分組中使用文字模式的資訊，請參閱：

* [使用文字模式編輯檢視](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-view.md)
* [使用文字模式編輯篩選器](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md)
* [使用文字模式編輯群組](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-grouping.md)

自訂提示只能在文字模式中編輯。 您只能從報告存取提示。

如需有關存取自訂提示的文字模式介面的資訊，請參閱[新增提示至報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)。

## 使用文字模式的常見原因 {#common-reasons-to-use-text-mode}

除了建立只能使用文字模式設定的自訂提示外，我們建議您使用Report Builder來建置檢視、篩選器和群組。 不過，在某些情況下，您可以使用文字模式來增強報表和清單。

如需文字模式常見用法的詳細資訊，請參閱[文字模式常見用法概觀](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md)。
