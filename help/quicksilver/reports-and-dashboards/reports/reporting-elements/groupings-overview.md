---
content-type: overview
product-area: reporting
navigation-topic: reporting-elements
title: Adobe Workfront中的群組概觀
description: 您可以新增群組來管理報告和清單中資訊的配置。
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

您可以新增群組來管理報告和清單中資訊的配置。

您可以透過下列方式將分組新增至報表：

* 您可以編輯現有群組來建立群組。

  如需自訂現有群組的相關資訊，請參閱[編輯現有群組](../../../reports-and-dashboards/reports/reporting-elements/edit-existing-groupings.md)。

* 您可以從頭開始建立群組。

  如需從頭開始建立群組的詳細資訊，請參閱[在Adobe Workfront中建立群組](../../../reports-and-dashboards/reports/reporting-elements/create-groupings.md)。

依預設，群組在報表或清單中以灰色或藍色反白顯示。 報告或清單的結果會列在其個別群組下，不會反白顯示。

您最多可以向一個報表新增三個群組。 您可以建立矩陣報表，將資訊組織成最多四個群組。 如需矩陣報表的詳細資訊，請參閱[建立矩陣報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md)。

在標準分組報表中，第一個分組的顏色較深，第二個和第三個分組則較淺。 您無法自訂群組反白顯示的顏色，或群組名稱的字型。 群組名稱后面括弧內的數字代表該群組下的結果數。 如果您的報告跨越多個頁面，請確定您在報告或清單中顯示&#x200B;*全部*&#x200B;個結果，以取得每個群組下結果的準確計數。

![範例群組](assets/grouping-example-blue.png)

使用分組時，請考慮下列事項：

* 您可以自訂現有群組中的資訊。 所有可檢視群組的使用者也可檢視您的變更。
* 您的Workfront管理員必須授予您編輯篩選器、檢視和群組的存取權，才能建立群組。

  如需授與篩選器、檢視和群組存取權的相關資訊，請參閱[授與篩選器、檢視和群組的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-fvg.md)。

* 您的群組許可權層級會指定儲存群組的方式。 如果您最初建立了分組，則可以儲存變更，否則系統會提示您儲存分組的版本。 如果您對已與其他人共用的群組進行變更，也會影響這些變更。
* 只有在共用群組的使用者授與您管理存取權時，您才能自訂與您共用的群組。 如需共用群組的相關資訊，請參閱[共用篩選器、檢視或群組](../../../reports-and-dashboards/reports/reporting-elements/share-filter-view-grouping.md)。
* 您無法編輯內嵌分組。
* 您不能依多選自訂欄位（例如核取方塊）或可有多個值的欄位（例如Resource Manager）來分組。

## 有關分組的其他資訊

在使用「群組」時，您可以進一步管理報表資訊，方法是彙總「群組」列上各欄的值，以及依「群組」欄位排序資訊。 您也可以在不再需要分組時將其移除。

* [群組中的彙總值](#aggregate-values-in-groupings)
* [依群組排序](#sort-by-a-grouping)
* [移除分組](#remove-a-grouping)

### 分組中的彙總值 {#aggregate-values-in-groupings}

您可以彙總報告每欄的值，彙總分組行中報告顯示的資料。 如需群組內彙總資料行資料的詳細資訊，請參閱Adobe Workfront中的[檢視總覽](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)。

>[!NOTE]
>
>當您彙總分組中下列欄位的值時，下列例外情況適用於父系物件（例如父系任務）：
>
>* 除「實際時數」（例如「計畫/實際勞力成本」、「計畫/實際費用成本」、「計畫/實際成本」、「計畫時數」）之外的所有數字與幣別欄位，只會彙總子任務與獨立任務的值。 它們不會彙總父系任務的值或父系父系的值。
>* 實際小時彙總主要父系和獨立任務的值；它們不會彙總父系任務的父系或子系任務的數量。
>* 數字和貨幣值的自訂資料欄位會彙總所有工作：父項、子項、父項的父項以及獨立工作。

### 依群組排序 {#sort-by-a-grouping}

無法排序群組。 檢視可以排序。 若要依群組中所擷取的值進行清單排序，您必須在檢視的其中一個欄中包含相同的值，並在檢視中套用排序。 如此一來，清單會間接地依分組中的值排序（它依檢視中的值排序，檢視也會在分組中擷取）。 如需有關建立檢視及依檢視內之值排序的詳細資訊，請參閱[Adobe Workfront中的檢視總覽](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)。

### 移除分組 {#remove-a-grouping}

移除分組的方式取決於您最初是建立分組，還是與您共用分組。 您無法移除預設群組。

* **如果您已建立群組並移除該群組**，則會從Workfront系統中移除該群組。 先前共用該群組的任何使用者都無法再使用該群組。
* **如果群組已與您共用，而您將其移除**，則僅會為您移除該群組。 原本建立該群組的使用者，以及與該群組共用的任何其他使用者，仍擁有該群組的存取權。

如需有關移除群組的資訊，請參閱文章[移除篩選器、檢視和群組](../../../reports-and-dashboards/reports/reporting-elements/remove-filters-views-groupings.md)。
