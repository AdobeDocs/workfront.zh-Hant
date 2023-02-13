---
content-type: release-notes
keywords: 附註，每季，更新，發行
navigation-topic: 2021-2-release-activity
title: 21.2資源管理增強功能
description: 本頁介紹在「預覽」環境的21.2版中進行的所有資源管理增強。 這些增強功能將於2021年5月10日當周在生產環境中提供。 如需21.2版所有可用變更的清單，請參閱21.2版本概觀。
author: Luke
feature: Product Announcements
exl-id: 00133efe-f779-4217-87af-a223dcf043ee
source-git-commit: 665732453b33b49421108791a560ab84d51280b9
workflow-type: tm+mt
source-wordcount: '556'
ht-degree: 0%

---

# 21.2資源管理增強功能

本頁介紹在「預覽」環境的21.2版中進行的所有資源管理增強。 這些增強功能將於2021年5月10日當周在生產環境中提供。 如需21.2版所有可用變更的清單，請參閱 [21.2版本概觀](../../../product-announcements/product-releases/21.2-release-activity/21-2-release-overview.md).

## 工作負載平衡器中的月級視圖

為了幫助您管理較長時間內的資源分配，我們現在為工作負載平衡器實施了月級視圖。 您一次最多可以檢視三個月，並更新每月的資源分配。 在此更改之前，您只能按日或周查看工作負載平衡器。

如需詳細資訊，請參閱 [導航工作負載平衡器](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## 方案規劃器、工作負載平衡器和任務清單之間的連接

>[!NOTE]
>
>僅適用於新的Adobe Workfront體驗。

為了幫助您進行項目的戰略規劃並確保這些計畫與方案規劃器的全局計劃一致，我們在項目上建立了一個新區域，顯示了方案中的任務職責要求以及項目工作項目上預計的計畫小時數。 此區域適用於項目級工作負載平衡器，以及新Workfront體驗中的任務清單。 在傳統體驗中，這僅適用於項目工作負載平衡器。

如需詳細資訊，請參閱下列文章：

* [協調項目和舉措之間資源分配的概覽](../../../scenario-planner/overview-reconcile-allocations-between-projects-initiatives.md).
* [導航工作負載平衡器](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md)

>[!IMPORTANT]
>
>這項新功能可供所有使用者檢視，在新版和傳統版Workfront體驗中皆可。 這也會顯示給尚未購買Workfront方案規劃器授權的客戶。

## 在資源計畫員中計算淨值時使用計畫小時數

資源計畫員中的新設定允許您在計算淨值時使用計畫小時數。

在此增強功能之前，Workfront僅使用「預算小時數」計算淨值。 淨值顯示「可用」與「預算」或「計畫小時數」、「FTE」或「成本」之間的差異。 計算淨值時，預算小時數仍為預設設定。

如需詳細資訊，請參閱 [資源計畫員的「項目」和「職責」視圖中的小時數、FTE和成本資訊概覽](../../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md).

## 工作負載平衡器中的12週視圖

您現在可以在工作負載平衡器中查看多達12週的資訊。 在此增強功能之前，您可以檢視2、4和6週的資訊。

有關查看工作負載平衡器的資訊，請參見 [導航工作負載平衡器](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md)導航工作負載平衡器。

## 更改「作業角色」篩選器在工作負載平衡器的「未分配」區域中的工作方式

為了改進工作角色篩選器在工作負載平衡器中的工作方式，並滿足用戶的期望，我們修改了「未分配」區域中篩選器的功能。 您現在只能查看分配給您在篩選器中指定的作業角色的小時數。

在此增強之前，在將「作業角色」篩選器應用到「未分配」區域時，工作負載平衡器將顯示與分配給作業角色的工作項目關聯的所有小時。

有關在工作負載平衡器中篩選資訊的資訊，請參見 [在工作負載平衡器中管理篩選器](../../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md).
