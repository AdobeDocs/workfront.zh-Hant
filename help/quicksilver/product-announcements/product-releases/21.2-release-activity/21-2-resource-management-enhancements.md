---
content-type: release-notes
keywords: 備註，每季，更新，發行
navigation-topic: 2021-2-release-activity
title: 21.2資源管理增強功能
description: 此頁面說明21.2版對「預覽」環境所做的所有資源管理增強功能。 這些增強功能將在2021年5月10日當週的生產環境中提供。 如需21.2版所有可用變更的清單，請參閱21.2版總覽。
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 00133efe-f779-4217-87af-a223dcf043ee
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '564'
ht-degree: 0%

---

# 21.2資源管理增強功能

此頁面說明21.2版對「預覽」環境所做的所有資源管理增強功能。 這些增強功能將在2021年5月10日當週的生產環境中提供。 如需21.2版本可用的所有變更清單，請參閱[21.2版本概觀](../../../product-announcements/product-releases/21.2-release-activity/21-2-release-overview.md)。

## 工作負載平衡器中的月層級檢視

為協助您管理較長時間內的資源配置，我們現在為工作負載平衡器實作月層級檢視。 您一次最多可以檢視三個月，並更新每月資源配置。 在此變更之前，您只能按天或周檢視工作負載平衡器。

如需詳細資訊，請參閱[瀏覽工作負載平衡器](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md)。

## 情境規劃工具、工作負載平衡器和任務清單之間的連線

>[!NOTE]
>
>僅於新的Adobe Workfront體驗中提供。

為協助您進行專案的策略規劃，並確保其符合「情境規劃工具」的宏觀方案，我們在專案上建立了一個新區域，顯示方案中的工作角色需求以及在專案工作專案上估計的計畫時數。 此區域可用於專案層級的工作負載平衡器以及新Workfront體驗中的任務清單。 在傳統體驗中，這僅適用於專案工作負載平衡器。

如需詳細資訊，請參閱下列文章：

* [協調專案與行動方案之間的資源配置的概觀](../../../scenario-planner/overview-reconcile-allocations-between-projects-initiatives.md)。
* [瀏覽工作負載平衡器](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md)

>[!IMPORTANT]
>
>所有使用者皆可檢視這項新功能，無論是新版還是傳統Workfront體驗。 未購買Workfront Scenario Planner授權的客戶也可看到此專案。

## 在資源規劃工具中計算淨值時使用計畫時數

「資源規劃工具」中的新設定可讓您在計算淨值時使用計畫時數。

在此增強功能之前，Workfront僅使用預算時數計算淨值。 淨值會顯示可用與預算或計畫時數、FTE或成本之間的差異。 計算淨值時，預算時數仍是預設設定。

如需相關資訊，請參閱資源規劃工具](../../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md)的專案與角色檢視中的[時數概觀、約當全職人數與成本資訊。

## 在工作負載平衡器12週檢視

您現在可以在工作負載平衡器中檢視最多12週的資訊。 在此增強功能之前，您可以檢視2、4和6週的資訊。

如需有關檢視工作負載平衡器的資訊，請參閱[瀏覽工作負載平衡器](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md)瀏覽工作負載平衡器。

## 變更工作角色篩選器在工作負載平衡器未指派區域中的工作方式

為了改善工作角色篩選器在工作負載平衡器中工作的方式並符合使用者的期望，我們修改了篩選器在未指派區域中的功能。 您現在只能檢視配置給您在篩選條件中指定的工作角色的時數。

在此增強功能之前，當將工作角色篩選器套用至未指派區域時，工作負載平衡器顯示與指派給工作角色的工作專案相關的所有時數。

如需有關在工作負載平衡器中篩選資訊的資訊，請參閱在工作負載平衡器中管理篩選器[](../../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md)。
