---
content-type: overview;how-to-procedural
product-area: projects;user-management
navigation-topic: assign-tasks
title: 修改任務分配概覽
description: 您可以將任務指派給使用者、團隊或工作角色，或取消指派任務。 您可以同時指派多個資源，或僅指派一個資源。 您可以一次指派一個任務，或大量指派多個任務。
author: Alina
feature: Work Management
exl-id: e774f2db-494d-4f93-8727-3c073e5f930b
source-git-commit: 7e77223595d3c9cf0d6592a09e893142439adb2c
workflow-type: tm+mt
source-wordcount: '873'
ht-degree: 0%

---

# 修改任務分配概覽

您可以將任務指派給使用者、團隊或工作角色，或取消指派任務。 您可以同時指派多個資源，或僅指派一個資源。 您可以一次指派一個任務，或大量指派多個任務。

>[!TIP]
>
>您可以指派多個使用者、工作角色或團隊。 您只能指派作用中的使用者、工作角色和團隊。
>
>如果在停用前已指派使用者、工作角色或團隊，則他們仍會指派給工作項目。 在此情況下，我們建議：
>
>* 將工作項重新分配給活動資源。
>* 將已停用團隊中的用戶與活動團隊關聯，並將工作項重新分配給活動團隊。
>


本文包含有關修改任務分配的影響的一般資訊。 如需如何指派工作的詳細資訊，請參閱下列文章：

* 有關分配任務的資訊，請參閱 [指派任務](../../../manage-work/tasks/assign-tasks/assign-tasks.md) 和 [修改任務清單中的多個用戶分配](../../../manage-work/tasks/assign-tasks/modify-multiple-assignments-in-task-list.md).

* 有關在「計畫」區域中修改多個任務的分配的資訊，請參閱 [修改調度區域中任務的多個用戶分配](../../../resource-mgmt/resource-scheduling/modify-multipl-assignments-scheduling-areas.md).
* 有關使用工作負載平衡器分配任務的資訊，請參見 [工作負載平衡器中分配工作的概述](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md).

本文中的某些資訊也適用於問題的分配。 如需指派問題的詳細資訊和其他考量事項，請參閱 [修改問題分配概覽](../../../manage-work/issues/manage-issues/modify-issue-assignments-overview.md).

## 何時修改任務上的用戶分配

您可能出於多種原因需要修改任務的用戶分配，包括：

* 使用者加入或離開您的團隊
* 使用者休假時間超過任務到期日

   >[!NOTE]
   >
   >在將用戶分配到工作時，根據其計畫的可用性會影響任務的計畫日期和預計日期。 如需排程的相關資訊，請參閱 [建立排程](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

* 特定角色或用戶被設定為多個任務的受託人，並且您想要快速修改要分配給不同用戶或角色的所有項目

## 指派給工作角色、團隊和使用者的多項考量事項

為工作項分配多個資源時，請考慮以下事項：

* 使用者可以有多個與其設定檔相關聯的工作角色。 有關將用戶與作業角色關聯的資訊，請參閱 [編輯使用者的設定檔](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* 通常會先將任務或問題指派給一個或多個作業角色或團隊。 當專案準備好開始時，也可能需要將其指派給使用者。\
   如果將任務或問題指派給一或多個角色，然後您又指派一個使用者，Adobe Workfront會根據下列規則決定要與其他使用者建立關聯的作業角色（如果有的話）:

   * 如果只分配了一個作業角色，並且該角色與用戶的主角色匹配，則該任務或問題僅分配給完成其主角色的用戶。
   * 如果分配了多個角色，且至少有一個角色與用戶的輔助角色匹配，則任務或問題將分配給履行其中一個「其他角色」(如果有多個匹配，則Workfront會隨機選擇)的用戶，以及已分配的任何其他角色。
   * 如果分配了一個或多個作業角色，並且沒有與用戶角色匹配的角色，則將任務或問題分配給該角色或角色以及該用戶。

* 如果將任務或問題分配給某個團隊，並且您也分配了某個用戶，則任務或問題將同時分配給該團隊和該用戶。

## 刪除受分配者如何影響任務小時數和分配百分比

移除使用者會影響工作小時數和分配百分比。 刪除用戶對任務的影響取決於為任務選擇的持續時間類型。 如需持續時間類型的相關資訊，請參閱 [任務持續時間和持續時間類型概覽](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

從具有以下持續時間類型的任務中刪除用戶時：

* **簡單：** 分配給該用戶的計畫小時數將從任務的總計畫小時數中扣除。

   >[!IMPORTANT]
   >
   >這可能對您的項目計畫產生負面影響，因為它會更改任務和項目的總計畫時數。

* **努力驅動：** 其他使用者的分配百分比不會變更。
* **計算分配：** 調整其他使用者的配置百分比，使得總計等於100%。
* **計算工作：** 其他使用者的分配百分比不會變更。

## 取消指派任務的考量事項

您可以一次從一個任務中刪除分配，也可以批量從多個任務中刪除分配。

有關從任務中大量刪除分配的詳細資訊，請參見 [修改任務清單中的多個用戶分配](../../../manage-work/tasks/assign-tasks/modify-multiple-assignments-in-task-list.md).

從任務中刪除分配時，請考慮以下事項：

* 從任務中取消分配用戶時，任務仍被分配給用戶在任務中履行的作業角色。
* 從任務中取消分配作業角色或團隊時，如果未將任務分配給任何其他資源，則該任務仍為未分配狀態。
