---
product-area: reporting
navigation-topic: reporting-elements
title: 「報表元素：篩選器、檢視和群組」
description: Workfront中每個清單和報告都必須具備的主要元素是篩選器、檢視和群組。 每個元素在任何報表中都會提供不同資訊。
author: Nolan
feature: Reports and Dashboards
exl-id: 5697905e-42c0-403b-85d4-798a1a3a2e7f
source-git-commit: 3cee374b68b26f2a423d41101300ec8b6685fadd
workflow-type: tm+mt
source-wordcount: '838'
ht-degree: 0%

---

# 報表元素：篩選器、檢視和群組

<!-- Audited: 11/2024 -->

<!--AL: Add information here about all the different kinds of FVGs: in reports, in lists, beta, etc // OR: this article should be a high-level overview of reporting elements. Then, each type of element should have:</p>
<p>- overview for Filters</p>
<p>- create a filter</p>
<p>- share a filter</p>
<p>ALL in Reporting elements but the Shared ones should be linked to Basics> Sharing; some of the articles in the Basics> Navigation> Use lists might beed to link here as well-->

有數個元素可讓Adobe Workfront中的清單或報表變成可能。 每個清單和報表都必須具備的主要元素為篩選器、檢視和群組。 每個元素在任何報表中都會提供不同資訊。

## 報表元素的相關考量事項

使用篩選器、檢視和分組時，請考慮下列事項：

* 報表元素可作為報表的建置區塊。 它們定義報告或清單的外觀和風格，以及報告或清單中包含的資訊。
* Workfront中的報表只針對一個物件。 您必須先為報表定義主要物件，才能建置報表。 因此，所有報表元素都是物件專屬的。
* 您的Workfront管理員必須授予您存取層級中篩選器、檢視和群組的存取權，才能在清單和報告中檢視或編輯它們。

  如需授與篩選器、檢視和群組存取權的相關資訊，請參閱[授與篩選器、檢視和群組的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-fvg.md)。

* 您的Workfront管理員必須授予您存取層級中報告、儀表板和行事曆的存取權，才能檢視或編輯報告。

  如需授與報告、儀表板和行事曆存取權的相關資訊，請參閱[授與報告、儀表板和行事曆的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md)。

* 如果您在報表或清單上選取篩選、檢視或分組，即使您登出或關閉瀏覽器，Workfront仍會針對該物件的清單保留此選取範圍。 例如，如果您為任務報告選取特定檢視，則該選取項會出現在其他任務清單中，例如專案上的任務清單。

## 篩選器

此篩選器可控制報表中顯示的結果，通常會將結果從一般縮小為特定。 其運作方式就像篩選器，僅擷取您需要的資訊，並將該資訊帶回您的報表。

例如，如果您只想檢視指派給登入使用者的任務，您可以建立標題為「我的任務」的篩選器，定義篩選必須符合的條件，並執行報告以僅檢視指派給登入使用者的任務。

篩選器的部分屬性包括：

* Workfront預設為各種物件提供許多篩選器。
* 您可以自訂擁有或管理的篩選器。

  如需篩選的詳細資訊，請參閱文章[篩選概觀](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)。

## 檢視

透過定義報表的檢視，您可以定義報表中包含的資訊。 如同所有報告元素，檢視是以一個物件型別為基礎。

例如，任務報告的檢視可以顯示「到期日」、包含主要財務詳細資訊（如「成本」），或用來顯示「指派」與「交貨日期」詳細資訊。 檢視可用於提供報表中資料的各種詳細資訊。

檢視的某些屬性包括：

* 您可以使用預設的Workfront檢視，也可以建立您自己的檢視。
* 您可在執行報表後，從「檢視」下拉式欄位套用其他檢視。
* 其他檢視會暫時取代建立報告時定義的檢視；不過，下次您返回報告時會顯示預設檢視。

  如需檢視的詳細資訊，請參閱文章[ Adobe Workfront中的檢視總覽](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)。

## 群組

分組可控制您組織資料的方式，使其更易於閱讀和理解。 分組會在整個報表中建立水準條，以顯示按通用屬性一起列出的結果。 建立群組時，您可以定義條件來決定要將報表的結果分組。

例如，依專案名稱將跨多個專案的任務清單分組，會以該名稱組織屬於單一專案的所有個別任務。

分組的部分屬性包括：

* 如果您稍後想要將圖表新增至報表，分組是強制性的報表元素。
* 分組在結果中顯示彙總值&#x200B;。
* 分組決定圖表中的軸。
* 分組會決定矩陣報表中的標題識別。\
  如需矩陣報表的詳細資訊，請參閱文章[建立矩陣報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md)。

* 分組有助於建立報表的摘要標籤，提供報表的彙總值。
* Workfront預設為不同的物件提供許多分組。
* 您可以自訂擁有或管理的群組。

  如需群組的詳細資訊，請參閱Adobe Workfront中的[群組概觀](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)。

## 其他報表元素

除了篩選器、檢視和群組之外，您也可以將下列元素新增至報表：

* **提示**：開啟的篩選器，每次執行報表時都可以以不同方式自訂和套用。\
  如需有關提示的詳細資訊，請參閱文章[新增提示至報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)。

* **圖表**：您可以新增圖表並以視覺化方式顯示資訊，藉此增強報表。\
  如需有關報表中圖表的詳細資訊，請參閱文章[將圖表新增至報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md)。
