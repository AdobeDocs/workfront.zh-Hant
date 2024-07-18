---
title: 22.2資源管理增強功能
description: 22.2資源管理增強功能
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 5f11c43c-3aa8-4135-b6bf-07b9993e63d9
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '373'
ht-degree: 0%

---

# 22.2資源管理增強功能

此頁面說明22.2版對「預覽」環境所做的所有資源管理增強功能。 這些增強功能將在生產環境中提供

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in January 2022
</MadCap:conditionalText>
-->

2022年4月4日當週。

如需22.2版本可用的所有變更清單，請參閱[22.2版本概觀](../../../product-announcements/product-releases/22.2-release-activity/22-2-release-overview.md)。

## 工作負載平衡器導覽的改進

為了改善您使用工作負載平衡器的體驗，我們引進了以下增強功能：

* 調整配置時的取消和儲存按鈕現在有粘性，即使任務長於畫面上包含的時間範圍或顯示摘要面板時。
* 顯示使用者名稱和工作專案的左側面板現在是粘性面板，可讓您水準捲動較長的時間範圍，並且仍然能夠讀取面板中列出的專案名稱。
* 只要按一下滑鼠，即可摺疊和展開左側面板中列出的所有專案，而不是在使用者或專案層級。
* 左側面板現在也可以調整大小。
* 工作負載平衡器現在提供全熒幕模式。

如需有關瀏覽工作負載平衡器的詳細資訊，請參閱[瀏覽工作負載平衡器](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md)。

## 存取工作負載平衡器中的進階指派

為了使指派工作專案更容易、更準確，您現在可以在工作負載平衡器中手動指派工作專案時進行進階指派。 在此增強功能之前，您可以在編輯專案時、從專案的標題或清單中存取進階工作。

如需詳細資訊，請參閱[使用工作負載平衡器](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-manually.md)手動指派工作。

## 選取「預設排程」偏好設定時，計算使用者可用性的新公式

為了在資源管理工具中提供更準確的資訊，我們已變更Workfront管理員在資源管理偏好設定中選取預設排程時，Workfront用來計算使用者可用性的公式。 透過新的更新，Workfront會使用以下公式計算使用者可用性：

使用者可用時數= （預設排程時數 — 例外） &#42; FTE — 休假時數

在此更新之前，當選取「預設排程」時，Workfront使用下列公式計算使用者可用性：

使用者可用時數= (預設排程時數 — （排程例外+休假時數）) &#42;使用者FTE值

如需詳細資訊，請參閱[設定資源管理喜好設定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md)。

