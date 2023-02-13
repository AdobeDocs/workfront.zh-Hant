---
product-area: projects;user-management
navigation-topic: assign-tasks
title: 管理任務上的用戶和角色分配時數
description: 為任務分配用戶或角色時，將分配這些用戶或角色以工作特定的小時數完成任務。 當任務「持續時間類型」為「簡單」時，您可以手動修改分配給任務的每個用戶或作業角色的小時數。
author: Alina
feature: Work Management
exl-id: 2c0cd6ef-8719-4680-aa63-5e229de0f819
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '580'
ht-degree: 0%

---

# 管理任務上的用戶和角色分配時數

為任務分配用戶或角色時，將分配這些用戶或角色以工作特定的小時數完成任務。 當任務「持續時間類型」為「簡單」時，您可以手動修改分配給任務的每個用戶或作業角色的小時數。

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>工作或更高</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>編輯對任務的訪問</p> <p>注意：如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>為任務貢獻或更高權限</p> <p>編輯權限以在「編輯任務」框中更新分配小時數</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 修改任務分配時數的考量事項

>[!IMPORTANT]
>
>手動修改任務上每個分配的分配後，任務的「計畫時數」可能會相應更新。 如需詳細資訊，請參閱 [在管理用戶分配時更新任務計畫小時數](../../../manage-work/tasks/task-information/planned-hours.md#update) 在文章中 [計畫小時數概觀](../../../manage-work/tasks/task-information/planned-hours.md).

* 分配給任務的各個資源的總小時數表示任務的計畫小時數。
* 如果任務分配了一個用戶或角色，則分配給用戶或角色的小時數與任務的「計畫小時數」匹配。
* 在多個分配的情況下，如果任務「持續時間類型」為「簡單」，則預設情況下，每個用戶或任務角色將分配等量的小時數以處理任務。 如需詳細資訊，請參閱下列文章：

   * [任務持續時間和持續時間類型概覽](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md)
   * [持續時間類型概觀：簡單](../../../manage-work/tasks/taskdurtn/simple-duration-type.md)

* 當任務具有「簡單持續時間類型」時，您可以手動更改每個用戶或作業角色分配的小時數，以指明某些任務分配者可能比其他任務分配者有更多時間處理任務。
* 不能修改分配給任務的團隊的小時數。
* 您無法手動修改問題的用戶或作業角色分配。
* 您還可以使用工作負載平衡器管理用戶對任務或問題的每日、每週或每月分配。 如需詳細資訊，請參閱 [在工作負載平衡器中管理用戶分配](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

## 修改任務的用戶或角色分配小時數

1. 轉到要更改分配小時數的分配的任務。
1. 按一下 **更多** 功能表 ![](assets/qs-more-icon-on-an-object.png) 在任務名稱旁，按一下 **編輯**，然後 **分配**.

   或

   按一下 **分配** 區域，然後按一下 **進階**.

1. 確保 **持續時間類型** 任務是 **簡單**.
1. 修改 **分配** 每個任務受託人。 這些是整個任務期間每個分配給此任務的總分配。 這也可能會更新任務的總計畫小時數。

   ![](assets/advanced-assignments-simple-duration-multiple-resources-nwe-350x198.png)

1. 按一下&#x200B;**儲存**。
