---
product-area: reporting
navigation-topic: reporting-elements
title: '''報表元素：篩選、檢視和群組'
description: Workfront中每個清單和報表必須具備的主要元素包括篩選、檢視和群組。 每個元素在任何報表中都提供不同的資訊。
author: Lisa
feature: Reports and Dashboards
exl-id: 5697905e-42c0-403b-85d4-798a1a3a2e7f
source-git-commit: 442e0b8fde9e4acaa2686ccd292fb003f72be623
workflow-type: tm+mt
source-wordcount: '843'
ht-degree: 0%

---

# 報表元素：篩選器、檢視和群組

<!--
<div style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>AL: Add information here about all the different kinds of FVGs: in reports, in lists, beta, etc // OR: this article should be a high-level overview of reporting elements. Then, each type of element should have:</p>
<p>- overview for Filters</p>
<p>- create a filter</p>
<p>- share a filter</p>
<p>ALL in Reporting elements but the Shared ones should be linked to Basics> Sharing; some of the articles in the Basics> Navigation> Use lists might beed to link here as well</p>
</div>
-->

有數個元素可讓清單或報表在Adobe Workfront中運作。 每個清單和報表必須具備的主要元素包括篩選、檢視和群組。 每個元素在任何報表中都提供不同的資訊。

## 報表元素的考量事項

使用篩選器、檢視和群組時，請考量下列事項：

* 報表元素可作為報表的基礎要素。 它們定義報表或清單的外觀和風格，以及報表或清單中包含的資訊。
* Workfront中的報表是一個物件專屬的。 您必須先定義報表的主要物件，才能建立報表。 因此，所有報表元素都是物件專屬的。
* Workfront管理員必須授予您存取層級中的篩選器、檢視和群組的存取權，才能在清單和報表中檢視或編輯這些項目。

   如需授與篩選器、檢視和群組存取權的相關資訊，請參閱 [授予篩選器、檢視和群組的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-fvg.md).

* Workfront管理員必須授予您存取層級中報表、控制面板和日曆的存取權，才能檢視或編輯報表。

   有關授予對報表、控制面板和日曆的訪問權限的資訊，請參閱 [授予對報表、控制面板和日曆的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).

* 如果您在報表或清單上選取篩選、檢視或分組，即使您登出或關閉瀏覽器，Workfront仍會保留該物件清單的篩選、檢視或分組選項。 例如，如果為任務報告選擇了特定視圖，則會為其他任務清單（如項目上的任務清單）顯示該選擇。

## 篩選器

篩選器會控制報表中顯示的結果，通常會將結果從一般縮小到特定。 它就像一個篩子，只會擷取您需要的資訊，並將該資訊傳回您的報表。

例如，如果您只想查看指派給登入使用者的任務，您可以建立標題為「我的任務」的篩選器，定義篩選器必須符合的條件，並執行報表，以僅檢視指派給登入使用者的任務。

篩選器的某些屬性為：

* Workfront預設會為各種物件提供數個篩選器。
* 您可以自訂擁有或管理的篩選器。

   如需篩選器的詳細資訊，請參閱文章 [Adobe Workfront中的篩選器概觀](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

![篩選器圖示](assets/projects-list-with-filter-drop-down-highlighted-nwe.png)

## 檢視

定義報表檢視後，您可以定義報表中包含的資訊。 與所有報表元素一樣，檢視也是以一個物件類型為基礎。\
例如，任務報表的視圖可以顯示到期日，包括關鍵財務詳細資訊（如成本），或用於顯示分配和交貨日期詳細資訊。 檢視可用來傳送報表中資料的各種詳細資料。

檢視的某些屬性為：

* 您可以使用預設的Workfront檢視，或建立自己的檢視。
* 您可以在執行報表後，從「檢視」下拉式欄位套用其他檢視。
* 其他檢視會暫時取代建立報表時所定義的檢視；不過，下次您返回報表時，會顯示預設檢視。

   如需檢視的詳細資訊，請參閱文章 [Adobe Workfront中的檢視概觀](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

## 群組

分組控制您整理資料的方式，讓您更容易閱讀和理解。 分組會在報表中建立橫條，顯示依共同屬性一起列出的結果。 在建立分組時，您可以定義要如何對報表結果進行分組的條件。

例如，將跨多個項目的任務清單按項目名稱分組，以該名稱組織屬於單個項目的所有相應任務。

分組的某些屬性包括：

* 如果您稍後想要將圖表新增至報表，群組會是強制報表元素。
* 分組會在結果中顯示匯總值&#x200B;。
* 分組決定圖表中的軸。
* 群組會決定矩陣報表中的標題識別。\
   如需矩陣報表的詳細資訊，請參閱文章 [建立矩陣報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md).

* 分組有助於建立報表的「摘要」標籤，提供報表的匯總值。
* Workfront依預設會為不同物件提供許多群組。
* 您可以自訂您擁有或管理的群組。

   如需分組的詳細資訊，請參閱 [Adobe Workfront中的群組概觀](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

## 其他報表元素

除了篩選、檢視和群組之外，您也可以將下列元素新增至報表：

* **提示**:一種開啟的篩選器，每次執行報表時，可以以不同方式自訂和套用。\
   有關提示的詳細資訊，請參閱文章 [新增提示至報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

* **圖表**:您可以新增圖表以及以視覺化方式顯示資訊，借此增強報表。\
   如需報表中圖表的詳細資訊，請參閱文章 [新增圖表至報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).
