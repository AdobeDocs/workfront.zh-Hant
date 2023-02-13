---
content-type: release-notes
navigation-topic: 2020-3-release-activity
title: 20.3資源管理增強功能
description: 本頁介紹在生產環境的20.3版中進行的所有資源管理增強。 這些增強功能已於2020年8月10日當周在生產環境中推出。
author: Luke
feature: Product Announcements
exl-id: a2c34117-e03c-4394-9b81-7c18433531d1
source-git-commit: 665732453b33b49421108791a560ab84d51280b9
workflow-type: tm+mt
source-wordcount: '829'
ht-degree: 0%

---

# 20.3資源管理增強功能

本頁介紹在生產環境的20.3版中進行的所有資源管理增強。 這些增強功能已於2020年8月10日當周在生產環境中推出。

如需20.3版所有可用變更的清單，請參閱 [20.3版本概觀](../../../product-announcements/product-releases/20.3-release-activity/20.3-release-overview.md).

## 在工作負載平衡器的「已分配工作」區域中包括來自問題的小時數

為了讓您查看所有人員工作負載的完整圖景，我們引入了一種設定，允許您在工作負載平衡器的「已分配工作」區域中包括從問題到問題的數小時。

有關在工作負載平衡器中工作的資訊，請參見 [導航工作負載平衡器](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## 調整工作負載平衡器中非工作日的分配

您可以使用工作負載平衡器調整非工作日的資源分配。

有關在工作負載平衡器中管理分配的資訊，請參見 [在工作負載平衡器中管理用戶分配](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

## 工作負載平衡器中可用的變數篩選器

為了改進您的體驗並在共用資訊時為您提供更大的靈活性，我們現在已為工作負載平衡器實施了變數篩選器。 已將以下篩選器添加到工作負載平衡器：

* &quot;Me&quot;（依使用者篩選時）
* &quot;My Primary Role&quot;（按角色篩選時）
* 「我的主團隊」或「我的所有團隊」（依團隊篩選時）。

這些篩選器會取代$$USER.ID、$$USER.roleID、$$USER.homeTeamID和$$USER.teamID的萬用字元篩選變數

如果應用其中一個篩選器，然後共用工作負載平衡器，或將其放在控制面板上，則所有其他用戶將看到自己的資訊。

有關將篩選器應用到工作負載平衡器的資訊，請參見 [篩選工作負載平衡器中的資訊](../../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md).

## 工作負載平衡器中項目的新排序

現在，工作負載平衡器會根據項目中任務的最早計畫起始日期和最近計畫完成日期（在用戶顯示在螢幕上的時間範圍內）對項目進行排序。 這可讓您以類似樹狀結構的階層來組織工作，以便您更輕鬆地識別一天的工作。

有關在工作負載平衡器中查看項目和工作項的資訊，請參見 [導航工作負載平衡器](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## 在工作負載平衡器中顯示實際工作進度

為了讓您準確了解工作負載的進度，我們在工作負載平衡器中引入了新的設定，該設定根據任務和問題的預計日期顯示任務和問題的時間表。 您可以啟用「顯示預計日期」設定，以查看除計畫時間表外工作項的預計時間表。

另外，通過這項改進，如果任務或問題在其計畫完成日期之前完成，則從剩餘天數開始分配的小時數將被刪除，以表明這些小時數不計入用戶的總體分配。

有關如何導航工作負載平衡器和啟用設定的資訊，請參見 [導航工作負載平衡器](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## 先前與20.2版通訊的工作負載平衡器功能

* [在工作負載平衡器中調整每日和每週分配](#adjust-daily-and-weekly-allocation-in-the-workload-balancer)
* [更新工作負載平衡器中的任務計畫小時數](#update-task-planned-hours-in-the-workload-balancer)
* [更方便地更新工作負載平衡器中的分配](#a-more-convenient-way-to-update-allocations-in-the-workload-balancer)

### 在工作負載平衡器中調整每日和每週分配 {#adjust-daily-and-weekly-allocation-in-the-workload-balancer}

為避免資源耗盡，您現在可以使用工作負載平衡器調整用戶的每日和每週分配。

在此增強之前，只有使用資源調度工具才能實現此功能。

有關在工作負載平衡器中管理分配的資訊，請參見 [在工作負載平衡器中管理用戶分配](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

**適用於下列環境：**

* Adobe Workfront Classic
* 全新Adobe Workfront體驗

### 更新工作負載平衡器中的任務計畫小時數 {#update-task-planned-hours-in-the-workload-balancer}

>[!NOTE]
>
>2020.2版後不久，此增強功能即將推出生產環境。

訪問級別的「資源管理」區域中的新選項現在允許具有此訪問權限的用戶從工作負載平衡器編輯計畫小時。 在工作負載平衡器中調整分配時，每日分配總數不需要與任務的「計畫小時數」匹配。 保存分配後，分配小時的合計將成為任務的「計畫小時」。 這隻適用於具有簡單持續時間類型的任務。

有關在工作負載平衡器中管理分配的資訊，請參見 [在工作負載平衡器中管理用戶分配](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

有關授予對資源管理的訪問權限的資訊，請參見 [授予資源管理的訪問權限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md).

### 更方便地更新工作負載平衡器中的分配 {#a-more-convenient-way-to-update-allocations-in-the-workload-balancer}

為了更方便地管理用戶對工作負載平衡器中工作項的分配，您現在可以按兩下該工作項。 您還可以使用現有的「編輯分配」菜單選項。 此外，您不再需要啟用顯示分配以便能夠更新它們。

有關在工作負載平衡器中管理分配的資訊，請參見 [在工作負載平衡器中管理用戶分配](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).
