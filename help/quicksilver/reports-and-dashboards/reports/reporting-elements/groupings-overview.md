---
content-type: overview
product-area: reporting
navigation-topic: reporting-elements
title: Adobe Workfront中的群組概觀
description: 您可以新增群組，以管理報表和清單中資訊的配置。
author: Nolan
feature: Reports and Dashboards
exl-id: d050372e-c4a0-4c49-b220-5b35334ab8d0
source-git-commit: 302771f4d64b386149623f87a3436d0c40f421d5
workflow-type: tm+mt
source-wordcount: '848'
ht-degree: 0%

---

# Adobe Workfront中的群組概觀

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: This article was supposed to be replaced by "Groupings overview", but decided to keep this here because this is linked in too many places. "Create groupings" and "Edit existing groupings" have been added also (with videos) to replace portions of the old content here.) </p>
-->

您可以新增群組，以管理報表和清單中資訊的配置。

您可以透過下列方式將群組新增至報表：

* 您可以編輯現有群組，以建立群組。

   如需自訂現有分組的相關資訊，請參閱 [編輯現有群組](../../../reports-and-dashboards/reports/reporting-elements/edit-existing-groupings.md).

* 您可以從頭建立分組。

   如需從草稿開始建立分組的詳細資訊，請參閱 [在Adobe Workfront中建立群組](../../../reports-and-dashboards/reports/reporting-elements/create-groupings.md).

依預設，群組會以灰色或藍色醒目提示顯示在報表或清單中。 報表或清單的結果會列在其個別分組下，沒有醒目提示。

您最多可將三個群組新增至報表。 您可以建立矩陣報表，以最多四個群組來組織資訊。 如需矩陣報表的詳細資訊，請參閱 [建立矩陣報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md).

在標準分組報表中，第一個分組是較深的顏色，第二和第三分組則較淺。 不能為分組自定義突出顯示的顏色或分組名稱的字型。 分組名稱后面括弧中的數字表示該分組下的結果數。 如果報表跨越多個頁面，請確定您顯示 *全部* 報表或清單中的結果，可準確計算每個群組下的結果。

![分組範例](assets/grouping-example-blue.png)

使用群組時，請考量下列事項：

* 您可以按現有分組自訂資訊。 所有可檢視群組的使用者也可以查看您的變更。
* Workfront管理員必須授予您編輯篩選器、檢視和群組的存取權，才能建立群組。

   如需授與篩選器、檢視和群組存取權的相關資訊，請參閱 [授予篩選器、檢視和群組的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-fvg.md).

* 您對群組的權限層級會指定群組的儲存方式。 如果最初建立了分組，則可以保存更改，否則系統將提示您保存分組的版本。 如果您對已與他人共用的群組進行變更，也會影響這些群組。
* 只有在共用給您「管理」存取權的使用者授予您「管理」存取權時，您才可自訂已與您共用的群組。 如需共用群組的相關資訊，請參閱 [共用篩選、檢視或分組](../../../reports-and-dashboards/reports/reporting-elements/share-filter-view-grouping.md).
* 不能編輯內嵌分組。
* 不能按多選自定義欄位（例如，複選框）或可以有多個值的欄位（例如，資源管理器）進行分組。

## 分組的其他資訊

您可以在使用分組時，通過聚合分組行上每個列中的值來進一步管理報告資訊，並按分組欄位對資訊進行排序。 您也可以在不再需要分組時將其移除。

* [分組中的匯總值](#aggregate-values-in-groupings)
* [按分組排序](#sort-by-a-grouping)
* [移除分組](#remove-a-grouping)

### 分組中的匯總值 {#aggregate-values-in-groupings}

您可以匯總報表各欄的值，以匯總分組行中報表中顯示的資料。 如需匯總分組中欄資料的詳細資訊，請參閱 [Adobe Workfront中的檢視概觀](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

>[!NOTE]
>
>在按分組方式聚合以下欄位的值時，父對象（例如父任務）適用以下例外：
>
>* 除「實際小時數」（例如，「計畫/實際人工成本」、「計畫/實際費用成本」、「計畫/實際成本」、「計畫小時數」）之外，所有數字和幣種欄位僅匯總子任務和獨立任務的值。 它們不會匯總父任務或父項的父項的值。
>* 「實際小時數」匯總主要父任務和獨立任務的值；它們不會匯總父任務或子任務的父任務的數量。
>* 數字和貨幣值的自訂資料欄位會匯總所有任務：父母、子女、父母和獨立任務。


### 按分組排序 {#sort-by-a-grouping}

無法排序分組。 檢視可排序。 要按分組中捕獲的值對清單進行排序，必須在視圖的其中一列中包括相同的值，並在視圖中應用排序。 這樣，清單就會間接地按分組中的值排序（它按視圖中的值排序，視圖中的值也在分組中捕獲）。 如需建立檢視及依檢視內的值排序的詳細資訊，請參閱 [Adobe Workfront中的檢視概觀](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

### 移除分組 {#remove-a-grouping}

移除分組的方式取決於您最初是建立分組，還是與您共用分組。 無法刪除預設分組。

* **如果已建立分組，並將其刪除**，則會從Workfront系統中移除分組。 您先前已與之共用的任何使用者都無法再使用分組。
* **如果已與您共用分組，而您將其移除**，則僅會為您移除群組。 最初建立此群組的使用者以及已共用給的任何其他使用者，仍可存取群組。

如需移除分組的相關資訊，請參閱文章 [移除篩選器、檢視和群組](../../../reports-and-dashboards/reports/reporting-elements/remove-filters-views-groupings.md).
