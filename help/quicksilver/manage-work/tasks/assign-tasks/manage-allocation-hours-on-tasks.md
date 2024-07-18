---
product-area: projects;user-management
navigation-topic: assign-tasks
title: 管理任務的使用者和角色分配時數
description: 將使用者或角色指派給任務時，會為其分配特定時數的工作以完成任務。 當任務「期間型別」為「簡單」時，您可以手動修改指派給任務的每個使用者或工作角色的時數。
author: Alina
feature: Work Management
exl-id: 2c0cd6ef-8719-4680-aa63-5e229de0f819
source-git-commit: 0d525df9beacc989ec3c1c695a7757dff0ad77b3
workflow-type: tm+mt
source-wordcount: '655'
ht-degree: 0%

---

# 管理任務的使用者和角色分配時數

<span class="preview">本頁醒目提示的資訊指出尚未普遍可用的功能。 它只能在「預覽」環境中供所有客戶使用，或在「生產」環境中供啟用快速發行的客戶使用。</span>

<span class="preview">如需快速發行資訊，請參閱[為您的組織啟用或停用快速發行](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>

<span class="preview">如需目前版本的相關資訊，請參閱[2024年第三季版本總覽](/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-release-overview.md)。</span>

將使用者或角色指派給任務時，會為其分配特定時數的工作以完成任務。 當任務「期間型別」為「簡單」時，您可以手動修改指派給任務的每個使用者或工作角色的時數。

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

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
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>編輯任務的存取權</p> <p>注意：如果您還是沒有存取權，請詢問您的Workfront管理員，他們是否在您的存取層級中設定其他限制。 如需Workfront管理員如何修改存取層級的詳細資訊，請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>Contribute或更高的任務許可權</p> <p>編輯許可權以在編輯任務方塊中更新分配時數</p> <p>如需請求其他存取權的資訊，請參閱<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求物件</a>的存取權。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的Workfront管理員。

## 修改任務分配時數的考量事項

>[!IMPORTANT]
>
>在您手動修改任務上每個指派的分配後，任務的計畫時數可能會相應地更新。 如需詳細資訊，請參閱文章[計畫時數概觀](../../../manage-work/tasks/task-information/planned-hours.md)中的[管理使用者配置時更新任務計畫時數](../../../manage-work/tasks/task-information/planned-hours.md#update)一節。

* 分配給指派給任務的個別資源的時數總計代表任務的計畫時數。
* 如果任務有一個使用者或角色指派，則分配給使用者或角色的時數與任務的計畫時數相符。
* 在多重指派的情況下，如果任務「期間型別」為「簡單」，則預設會為每個使用者或工作角色指派相等的時數，以處理任務。 如需詳細資訊，請參閱下列文章：

   * [任務期間與期間型別概觀](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md)
   * [期間型別概觀：簡單](../../../manage-work/tasks/taskdurtn/simple-duration-type.md)

* 當任務具有「簡單期間型別」時，您可以手動變更每個使用者或職務角色的分配時數金額，以表示某些任務受指派人可能比其他任務受指派人有更多時間處理任務。
* 您無法修改分配給指派給任務的團隊的時數。
* 您無法手動修改問題的使用者或工作角色分配。
* 您還可以使用工作負載平衡器管理每日、每週或每月使用者對任務或問題的分配。 如需詳細資訊，請參閱[在工作負載平衡器](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md)中管理使用者配置。

## 修改任務的使用者或角色配置時數

1. 移至您要變更其指派時數的任務。
1. 按一下工作名稱旁的&#x200B;**更多**&#x200B;功能表![](assets/qs-more-icon-on-an-object.png)，然後按一下&#x200B;**編輯**，再按一下&#x200B;**工作分派**。

   或

   按一下工作標題中的&#x200B;**工作總攬**&#x200B;區域，然後按一下&#x200B;**進階**。

1. 確定任務的&#x200B;**期間型別**&#x200B;是&#x200B;**簡單**。
1. 修改每個任務受指派人的&#x200B;**配置**。 這些是整個任務期間此任務的每個工作分派的整體配置。 這也可能更新任務的整體計畫時數。

   生產環境中的影像範例：
   ![](assets/advanced-assignments-simple-duration-multiple-resources-nwe-350x198.png)

   <span class="preview">預覽環境中的範例影像：</span>
   ![修改配置](assets/advanced-assignments-duration-type-allocations.png)

1. 按一下「**儲存**」。
