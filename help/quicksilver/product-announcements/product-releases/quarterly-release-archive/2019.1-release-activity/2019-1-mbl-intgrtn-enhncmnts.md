---
content-type: release-notes
navigation-topic: 2019-1-release-activity
title: 2019.1行動裝置和整合增強功能
description: 此頁面說明2019.1版包含的所有資源管理增強功能。 此功能現在可在生產環境中使用。
author: Luke
feature: Product Announcements, Workfront Integrations and Apps
recommendations: noDisplay, noCatalog
exl-id: 6b86ba0d-977a-4c89-8832-e81bf28d9dad
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '961'
ht-degree: 0%

---

# 2019.1行動裝置和整合增強功能

此頁面說明2019.1版包含的所有資源管理增強功能。 此功能現在可在生產環境中使用。

如需2019.1年度所有變更的清單，請參閱 [2019.1版本活動概覽](../../../../product-announcements/product-releases/quarterly-release-archive/2019.1-release-activity/2019-1-release-activity-overview.md).

## 更新資源規劃工具中的預設篩選器

資源規劃工具中的預設篩選器不再依專案群組進行篩選。

現在檢視資源規劃工具時，您只能看見目前且預設對日期敏感的專案。 預設會包含下列專案的資訊：

* 計畫完成日期在當月的第一個日期之後。
* 計劃開始日期在今天起第四個月的最後日期之前。
* 狀態為「目前」或「計畫」。

預設篩選器先前會從下列其他專案擷取資訊：

* 計畫完成日期在當月的第一個日期之後。
* 計劃開始日期在今天起第四個月的最後日期之前。
* 狀態為「目前」或「計畫」。
* 使用與已登入使用者之主群組相符的群組。

如需將篩選器套用至資源規劃工具的相關資訊，請參閱 [在資源規劃工具中篩選資訊](../../../../resource-mgmt/resource-planning/filter-resource-planner.md).

## 使用萬用字元作為資源規劃工具篩選器

現在當您在資源規劃工具中建立篩選器時，可以使用萬用字元。 例如，您可以使用$$USER.ID來篩選已登入之使用者的相關資訊，或使用$$USER.companyID來篩選與已登入之使用者屬於同一公司之所有使用者的相關資訊。 如需使用者型變數的完整清單，請參閱 [使用者型萬用字元篩選器變數](../../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md#user-based-variables) 中的區段 [萬用字元篩選器變數](../../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

以前，資源規劃工具篩選器沒有萬用字元。

如需有關在資源規劃工具中篩選的資訊，請參閱 [在資源規劃工具中篩選資訊](../../../../resource-mgmt/resource-planning/filter-resource-planner.md)

視訊

## 支援資源規劃工具中以日期為基礎的萬用字元篩選變數

現在當您在資源規劃工具中建立篩選器時，可以使用任何版本的$$TODAY萬用字元篩選器變數。

在此增強功能之前，您只能使用以使用者為基礎的萬用字元篩選變數。

如需有關在資源規劃工具中篩選的資訊，請參閱 [在資源規劃工具中篩選資訊](../../../../resource-mgmt/resource-planning/filter-resource-planner.md).

如需萬用字元篩選變數的詳細資訊，請參閱 [萬用字元篩選器變數](../../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

視訊

## 資源規劃工具中角色檢視的匯出選項

您現在可以在「角色」檢視中，選取要從「資源規劃工具」匯出的資訊層次。

您可以匯出下列任一專案：

* 僅限角色
* 角色和專案
* 角色、專案和使用者

在此增強功能之前，所有層級的資訊都會匯出至角色檢視中。 這些選項已在先前版本的專案和使用者檢視中引入。

如需有關從資源規劃工具匯出資訊的資訊，請參閱 [從資源規劃工具匯出資訊](../../../../resource-mgmt/resource-planning/export-resource-planner.md).

視訊

## 匯出資源規劃工具的資料格式選項

您現在可以選取從資源規劃工具匯出時，要如何在Excel檔案中顯示資訊。

您可以透過下列方式顯示從「資源規劃工具」匯出的資訊之可用性與配置：

* 依其所屬物件名稱取消群組。 在這種情況下，其所屬的物件名稱會顯示在每一列資料上。 （這是預設選項）
* 依其所屬物件名稱分組。 在這種情況下，匯出的檔案中的資訊會顯示在Workfront中。

在此增強功能之前，匯出的檔案中的資訊會顯示在Workfront中。

如需有關從資源規劃工具匯出資訊的資訊，請參閱 [從資源規劃工具匯出資訊](../../../../resource-mgmt/resource-planning/export-resource-planner.md).

視訊

## 持續排程時間表

>[!NOTE]
>
>已棄用資源排程工具，並已從Workfront的23.1版本中移除。 如需有關使用工作負載平衡器排程資源的資訊，請參閱 [工作負載平衡器概覽](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

排程時間表現在會保留您重新整理時間表或離開頁面時選取的時間範圍。

在此增強功能之前，當您重新整理或離開頁面進行導覽時，排程時間表會傳回預設時間範圍。

此增強功能在以下區域提供：

* 「人員」區域中的「排程」標籤
* 團隊正在處理索引標籤
* 專案「人員配置」標籤上的「排程」子標籤

如需在「資源排程」區域使用時間表的相關資訊，請參閱「開始使用資源排程」。

視訊

## 資源規劃工具中的新匯出選項

您現在可以選取要從「資源規劃工具」匯出的資訊層級。

在「專案」檢視中，您可以匯出下列任一專案：

* 僅限專案
* 專案和角色
* 專案、角色和使用者

在「使用者檢視」中，您可以匯出下列任一專案：

* 僅限使用者
* 使用者和專案
* 使用者、專案、角色、任務和問題

在此增強功能之前，依預設會匯出資源規劃工具之所有檢視中的所有資訊層級。

如需有關從資源規劃工具匯出資訊的資訊，請參閱 [從資源規劃工具匯出資訊](../../../../resource-mgmt/resource-planning/export-resource-planner.md).

視訊

## 更新至資源規劃工具中的使用者檢視

系統中的所有使用者現在都會顯示在資源規劃工具的使用者檢視中，但只有與已篩選專案相關聯的使用者也會顯示時數資訊。

在此更新之前，只有指派到您篩選的專案上工作專案的使用者會顯示在資源規劃工具的使用者檢視中。

您可以使用以使用者為基礎的篩選器，將「使用者檢視」中顯示的使用者人數，減少至僅指派給您要顯示之專案的使用者人數。

如需資源規劃工具中篩選器的相關資訊，請參閱 [在資源規劃工具中篩選資訊](../../../../resource-mgmt/resource-planning/filter-resource-planner.md).
