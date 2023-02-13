---
title: 22.2資源管理增強功能
description: 22.2資源管理增強功能
author: Luke
draft: Probably
feature: Product Announcements
exl-id: 5f11c43c-3aa8-4135-b6bf-07b9993e63d9
source-git-commit: be4904f0b37870c1bfc8ec345e468d5fc283aa36
workflow-type: tm+mt
source-wordcount: '367'
ht-degree: 0%

---

# 22.2資源管理增強功能

本頁介紹在「預覽」環境的22.2版中進行的所有資源管理增強。 這些增強功能將可在生產環境中使用

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in January 2022
</MadCap:conditionalText>
-->

2022年4月4日當周。

如需22.2版所有可用變更的清單，請參閱 [22.2版本概觀](../../../product-announcements/product-releases/22.2-release-activity/22-2-release-overview.md).

## 工作負載平衡器導覽的改善

為了改善您在使用工作負載平衡器時的體驗，我們引入了以下增強功能：

* 調整分配時的取消和儲存按鈕現在是固定的，即使任務超過螢幕上包含的時間範圍，或「摘要」面板顯示時也是如此。
* 顯示使用者和工作項目名稱的左側面板現在有黏性，可讓您水準捲動較長的時間範圍，而且仍可讀取面板中所列項目的名稱。
* 只要按一下，即可折疊和展開左側面板中列出的所有項目，而不是在使用者或專案層級。
* 左面板現在也可調整大小。
* 現在，工作負載平衡器有全螢幕模式。

有關導航工作負載平衡器的詳細資訊，請參見 [導航工作負載平衡器](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## 訪問工作負載平衡器中的高級分配

為了使分配工作項更簡單和更準確，您現在可以在工作負載平衡器中手動分配工作項時進行高級分配。 在此增強功能之前，您可以在編輯項目、項目標題或清單中存取「進階指派」。

如需詳細資訊，請參閱 [使用工作負載平衡器手動分配工作](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-manually.md).

## 新公式，用於在選擇「預設計畫」首選項時計算用戶可用性

為了在資源管理工具中提供更準確的資訊，我們更改了當Workfront管理員在「資源管理首選項」中選擇「預設計畫」時，Workfront用於計算用戶可用性的公式。 在新更新中，Workfront會使用下列公式來計算使用者可用性：

用戶可用小時數=（預設計畫小時數 — 例外） &#42; FTE — 休假時間

在此更新前，Workfront使用下列公式計算選取「預設排程」時的使用者可用性：

用戶可用小時數=(預設計畫小時數 — （計畫例外+超時）) &#42; 用戶FTE值

如需詳細資訊，請參閱 [配置資源管理首選項](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

