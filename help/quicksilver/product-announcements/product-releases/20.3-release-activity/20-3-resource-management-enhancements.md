---
content-type: release-notes
navigation-topic: 2020-3-release-activity
title: 20.3資源管理增強功能
description: 本頁說明20.3版中針對「生產」環境所做的所有資源管理增強功能。 這些增強功能已在2020年8月10日當週的生產環境中推出。
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: a2c34117-e03c-4394-9b81-7c18433531d1
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '837'
ht-degree: 0%

---

# 20.3資源管理增強功能

本頁說明20.3版中針對「生產」環境所做的所有資源管理增強功能。 這些增強功能已在2020年8月10日當週的生產環境中推出。

如需20.3版本可用的所有變更清單，請參閱[20.3版本總覽](../../../product-announcements/product-releases/20.3-release-activity/20-3-release-overview.md)。

## 包括問題時數在指派的工作區域工作負載平衡器

為了讓您全面瞭解您的所有人員的工作負載，我們引進了設定，可讓您在工作負載平衡器的已指派工作區域中包含問題的時數。

如需有關使用工作負載平衡器的資訊，請參閱[瀏覽工作負載平衡器](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md)。

## 在工作負載平衡器中調整非工作日的分配

您可以使用工作負載平衡器調整非工作日的資源配置。

如需有關在工作負載平衡器中管理配置的資訊，請參閱在工作負載平衡器中管理[使用者配置](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md)。

## 工作負載平衡器中可用的變數篩選器

為了改善您的體驗以及讓您在共用資訊時擁有更多彈性，我們現在為工作負載平衡器實作變數篩選器。 下列篩選器已新增到工作負載平衡器：

* 「我」（依使用者篩選時）
* 「我的主要角色」（依角色篩選時）
* 「我的主團隊」或「我的所有團隊」（依團隊篩選時）。

這些篩選器會取代$$USER.ID、$$USER.roleID、$$USER.homeTeamID和$$USER.teamIDs的萬用字元篩選器變數

當您套用這些篩選器之一，然後共用工作負載平衡器或將其放在儀表板上，所有其他使用者將看到他們自己的資訊。

如需有關將篩選器套用至工作負載平衡器的資訊，請參閱工作負載平衡器](../../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md)中的[篩選器資訊。

## 工作負載平衡器中專案的新排序

工作負載平衡器現在會根據使用者在畫面上顯示的時間範圍內發生之專案中任務的最早規劃開始日期，其次是最新規劃完成日期，來排序專案。 這可讓您以樹狀階層來組織工作，協助您更輕鬆地識別一天的工作。

如需有關在工作負載平衡器中檢視專案和工作專案的資訊，請參閱[瀏覽工作負載平衡器](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md)。

## 在工作負載平衡器中顯示實際工作進度

為了讓您準確看到工作負荷的進度，我們在工作負載平衡器中引入新設定，根據任務的預計日期顯示任務和問題的時間表。 您可以啟用「顯示預計日期」設定，以檢視工作專案的預計時間表以及計畫時間表。

此外，透過這項改善，如果任務或問題在計畫完成日期之前完成，則會刪除剩餘天數的分配時數，以表示這些時數不會計入使用者的整體分配中。

如需有關瀏覽工作負載平衡器及啟用設定的資訊，請參閱[瀏覽工作負載平衡器](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md)。

## 工作負載平衡器功能先前在20.2版本中宣佈發行

* [在工作負載平衡器](#adjust-daily-and-weekly-allocation-in-the-workload-balancer)中調整每日和每週配置
* [在工作負載平衡器](#update-task-planned-hours-in-the-workload-balancer)更新任務計畫時數
* [更新工作負載平衡器中分配的一種更方便的方法](#a-more-convenient-way-to-update-allocations-in-the-workload-balancer)

### 在工作負載平衡器中調整每日和每週分配 {#adjust-daily-and-weekly-allocation-in-the-workload-balancer}

為避免資源倦怠，您現在可以使用工作負載平衡器調整使用者的每日和每週分配以工作。

在此增強功能之前，這只能使用「資源排程」工具。

如需有關在工作負載平衡器中管理配置的資訊，請參閱在工作負載平衡器中管理[使用者配置](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md)。

**在以下環境中可用：**

* Adobe Workfront Classic
* 全新Adobe Workfront體驗

### 在工作負載平衡器中更新任務計畫時數 {#update-task-planned-hours-in-the-workload-balancer}

>[!NOTE]
>
>此增強功能將在2020.2版發佈後不久在生產環境中可用。

存取層級的「資源管理」區域中的新選項現在可讓具有此存取許可權的使用者從工作負載平衡器編輯規劃時數。 當您在工作負載平衡器中調整分配時，每日分配的總數不需要匹配任務的計畫時數。 儲存配置後，配置時數總計將成為任務的計畫時數。 這僅適用於具有簡單期間型別的任務。

如需有關在工作負載平衡器中管理配置的資訊，請參閱在工作負載平衡器中管理[使用者配置](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md)。

如需授與資源管理的存取許可權的相關資訊，請參閱[授與資源管理的存取許可權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md)。

### 更新工作負載平衡器中分配的一種更方便的方法 {#a-more-convenient-way-to-update-allocations-in-the-workload-balancer}

為了更便於管理工作負載平衡器中工作專案的使用者配置，您現在可以按兩下工作專案。 您仍然可以使用現有的「編輯配置」功能表選項。 此外，您不再需要啟用顯示配置才能更新它們。

如需有關在工作負載平衡器中管理配置的資訊，請參閱在工作負載平衡器中管理[使用者配置](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md)。
